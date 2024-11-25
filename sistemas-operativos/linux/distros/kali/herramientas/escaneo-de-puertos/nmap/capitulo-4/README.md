---
layout:
  title:
    visible: true
  description:
    visible: false
  tableOfContents:
    visible: true
  outline:
    visible: true
  pagination:
    visible: false
---

# Capítulo 4

## <mark style="color:orange;">Descripción general del escaneo de puertos</mark>

### <mark style="color:blue;">Introducción</mark>

Si bien Nmap ha crecido en funcionalidad a lo largo de los años, comenzó como un escáner de puertos eficiente, y esa sigue siendo su función principal. El comando simple **nmap&#x20;**_**`<target>`**_ escanea los 1.000 TCP más utilizados puertos en el host _`<target>`_, clasificando cada uno de los puertos en el estado **`open`**, **`closed`**, **`filtered`**, **`unfiltered`**, **`open|filtered`** o **`closed|filtered`**.

#### <mark style="color:yellow;">¿Qué es exactamente un puerto?</mark>

Los puertos son simplemente una abstracción de software, que se utiliza para distinguir entre _**canales de comunicación**_. De manera similar a la forma en que se utilizan las direcciones IP para identificar máquinas en redes, los puertos _identifican aplicaciones en uso_ en una sola máquina. Por ejemplo, el navegador web se conectará de forma predeterminada al puerto TCP 80 de las máquinas en HTTP. Si especifica el protocolo seguro HTTPS en su lugar, el navegador intentará el puerto 443 de forma predeterminada.

Nmap funciona con dos protocolos que utilizan puertos: **`TCP`** y **`UDP`**. La conexión para cada protocolo se identifica de forma única mediante cuatro elementos:

* Dirección IP Origen
* Puerto Origen
* Dirección IP Destino
* Puerto Destino

Todos estos elementos son simplemente números colocados en los encabezados de cada paquete enviado entre hosts. El _**protocolo**_ es un campo de ocho bits, que especifica qué tipo de paquete está contenido en el campo _**sección de datos IP**_ (carga útil).&#x20;

Por ejemplo, TCP es el protocolo (número 6) y El UDP es el protocolo (número 17). Las direcciones IPv4 tienen una longitud de 32 bits, mientras que los puertos son 16 bits de largo. Las direcciones IPv6 tienen una longitud de 128 bits.&#x20;

Debido a que la mayoría de los servicios populares están registrados a nombre de una número de puerto, a menudo se puede adivinar lo que representan los puertos abiertos de los servicios. Nmap incluye un archivo `nmap-services`, que contiene el servicio conocido para el puerto y el protocolo registrado, así como puertos comunes para puertas traseras de troyanos y otros aplicaciones que no se molestan en registrarse en el sitio web asignado _**Autoridad de Números (IANA)**_. Nmap imprime este nombre de servicio como referencia junto con el número de puerto.

Dado que el campo de número de puerto tiene un ancho de 16 bits, los valores pueden alcanzar 65535. El valor más bajo posible, cero, _**no es válido**_.&#x20;

Algunas puertas traseras de troyanos maliciosos escuchan en el puerto cero de los sistemas comprometidos como una forma sigilosa de ofrecer acceso ilegítimo sin aparecer en la mayoría de los escaneos de puertos. Para combatir esto, Nmap permite el escaneo del puerto cero cuando se especifica explícitamente (p. ej. ).`-p0-65535`

La primera clase de puertos válidos, números del 1 al 1023, se conocen como _**puertos reservados**_. Los sistemas Unix (a diferencia de Windows) requieren que las aplicaciones tienen características especiales (root) para enlazar y escuchar en estos puertos.&#x20;

La idea es permitir que los usuarios remotos confíen que se están conectando a un servicio válido iniciado por un administrador y no por algún usuario malvado y sin privilegios. Si el registrado para SSH era 2222 en lugar de 22, un usuario malintencionado podría iniciar un demonio SSH fraudulento en ese puerto, recopilando contraseñas de cualquiera que se conecte. Como la mayoría de las aplicaciones de servidor comunes, escuchen en puertos, estos suelen ser los más fructíferos para escanear.

El intervalo de puertos efímeros es otra clase de puertos. El sistema pone a disposición este grupo de puertos para su asignación según sea necesario. Cuando la aplicación especifica el puerto cero (es decir, "cualquier puerto"), el sistema elige un puerto de este rango. El rango varía según el sistema operativo y es por lo general, configurable. Debe contener al menos un par miles de puertos para evitar que se agoten cuando se producen muchas conexiones simultáneas. El escaneo de conexión Nmap puede usar cientos a la vez tiempo mientras escanea cada puerto especificado en cada máquina de destino. En Linux, puede ver o establecer el rango usando el archivo **`/proc/sys/net/ipv4/ip_local_port_range`**.

Los puertos SunRPC se encuentran a menudo en el rango efímero. Las aplicaciones abren puertos efímeros temporalmente para una transferencia de archivos u otro evento. Los clientes FTP a menudo hacen esto cuando solicitan transferencia en modo activo. Algunos clientes P2P y de mensajería instantánea lo hacen como pozo.

La IANA tiene su propio esquema de clasificación de puertos, que difiere ligeramente de la lengua vernácula de este libro. Su lista de puertos autoritativa en [`http://www.iana.org/assignments/port-numbers`](http://www.iana.org/assignments/port-numbers) divide el espacio en las tres clases siguientes:

#### <mark style="color:yellow;">Puertos conocidos</mark>

Se trata de puertos reservados (dentro del rango de 1 a 1023) que han sido registrados en la IANA por un cierto servicio. Ejemplos conocidos son los puertos 22, 25 y 80 para el servicios SSH, SMTP y HTTP, respectivamente.

#### <mark style="color:yellow;">Puertos registrados</mark>

Estos puertos se encuentran dentro del rango de 1024 a 49151 y han sido registrados en la IANA de la misma manera que el pozo puertos conocidos tienen. La mayoría de estos no se usan tan comúnmente como el puertos conocidos.

La diferencia clave es que los usuarios sin privilegios pueden enlazar a estos puertos y, por lo tanto, ejecutar los servicios en sus puertos. Los usuarios no pueden hacerlo en la mayoría de las plataformas para puertos conocidos, ya que residen en el intervalo de puertos reservados.

#### <mark style="color:yellow;">Puertos dinámicos y/o privados</mark>

La IANA reserva los números de puerto desde 49152 hasta el 65535 para usos dinámicos como los discutidos en el Sección de puertos efímeros. Servicios propietarios que solo se utilizan dentro de una empresa también se pueden utilizar estos puertos.

Archivo de registro de puertos de Nmap (**`nmap-services`**) contiene datos empíricos sobre cómo con frecuencia, cada puerto TCP o UDP se encuentra abierto. De forma predeterminada, Nmap Escanea los 1000 puertos más populares de cada protocolo que se le pide escanear. Hay muchas opciones para especificar un conjunto alternativo de puertos (por frecuencia o enumerándolos explícitamente).

### <mark style="color:blue;">¿Cuáles son los puertos más populares?</mark>

Es importante estar familiarizado con los puertos de servicio más comunes, y también es interesante ver cuáles hizo la lista. Las dos listas siguientes proporcionan los principales puertos TCP y UDP según lo determinado por nuestros datos de escaneo empírico.&#x20;

<mark style="color:green;">Los 20 puertos TCP principales</mark>:

1. **`Puerto 80 (HTTP)`**: Esto representó más del 14% de los puertos abiertos que descubrimos.
2. **`Puerto 23 (Telnet)`**: Telnet sigue vivo (especialmente como puerto de administración en dispositivos como enrutadores y conmutadores inteligentes) aunque sea inseguro (sin cifrar).
3. **`Puerto 443 (HTTPS)`**: los servidores web cifrados con SSL utilizan este puerto de forma predeterminada.
4. **`Puerto 21 (FTP)`**: FTP, al igual que Telnet, es otro protocolo inseguro que debería morir. Incluso con FTP anónimo (evitando la preocupación de olfatear la autenticación), la transferencia de datos sigue estando sujeta a manipulación.
5. **`Puerto 22 (SSH)`**: Secure Shell, un sustituto cifrado de Telnet (y, en algunos casos, FTP).
6. **`Puerto 25 (SMTP)`**: protocolo simple de transferencia de correo (también inseguro).
7. **`Puerto 3389 (ms-term-server)`**: puerto de administración de Microsoft Terminal Services.
8. **`Puerto 110 (POP3)`**: protocolo de oficina postal versión 3 para la recuperación de correo electrónico (inseguro).
9. **`Puerto 445 (Microsoft-DS)`**: para la comunicación SMB a través de IP con servicios de MS Windows (como el uso compartido de archivos e impresoras).
10. **`Puerto 139 (NetBIOS-SSN)`**: servicio de sesión NetBIOS para la comunicación con los servicios de MS Windows (como el uso compartido de archivos/impresoras). Esto se ha admitido en máquinas con Windows de más de 445 has.
11. **`Puerto 143 (IMAP)`**: Protocolo de acceso a mensajes de Internet versión 2. Un protocolo de recuperación de correo electrónico inseguro.
12. **`Puerto 53 (dominio)`**: sistema de nombres de dominio (DNS), un sistema inseguro para la conversión entre nombres de host/dominio y direcciones IP.
13. **`Puerto 135 (MSRPC)`**: otro puerto común para los servicios de MS Windows.
14. **`Puerto 3306 (MySQL)`**: para la comunicación con bases de datos MySQL.
15. **`Puerto 8080 (HTTP-Proxy)`**: se utiliza habitualmente para proxies HTTP o como puerto alternativo para servidores web normales (por ejemplo, cuando otro servidor ya está escuchando en el puerto 80, o cuando lo ejecutan usuarios UNIX sin privilegios que solo pueden enlazar a puertos altos).
16. **`Puerto 1723 (PPTP)`**: protocolo de túnel punto a punto (un método de implementación de VPN que a menudo se requiere para las conexiones de banda ancha a los ISP).
17. **`Puerto 111 (RPCBind)`**: asigna los números de programa de SunRPC a sus números de puerto TCP o UDP actuales.
18. **`Puerto 995 (POP3S)`**: POP3 con SSL agregado por seguridad.
19. **`Puerto 993 (IMAPS)`**: IMAPv2 con SSL agregado por seguridad.
20. **`Puerto 5900 (VNC)`**: un sistema gráfico de uso compartido de escritorio (inseguro).

<mark style="color:green;">Los 20 puertos UDP principales</mark>

1. **`Puerto 631 (IPP)`**: protocolo de impresión de Internet.
2. **`Puerto 161 (SNMP)`**: protocolo simple de administración de red.
3. **`Puerto 137 (NETBIOS-NS)`**: uno de los muchos puertos UDP para servicios de Windows, como el uso compartido de archivos e impresoras.
4. **`Puerto 123 (NTP)`**: protocolo de tiempo de red.
5. **`Puerto 138 (NETBIOS-DGM)`**: otro servicio de Windows.
6. **`Puerto 1434 (MS-SQL-DS)`**: servidor de Microsoft SQL.
7. **`Puerto 445 (Microsoft-DS)`**: otro puerto de servicios de Windows.
8. **`Puerto 135 (MSRPC)`**: otro puerto de servicios de Windows.
9. **`Puerto 67 (DHCPS)`**: servidor de protocolo de configuración dinámica de host (proporciona direcciones IP a los clientes cuando se unen a la red).
10. **`Puerto 53 (dominio)`**: servidor del sistema de nombres de dominio (DNS).
11. **`Puerto 139 (NETBIOS-SSN)`**: otro puerto de servicios de Windows.
12. **`Puerto 500 (ISAKMP)`**: la Asociación de Seguridad de Internet y el Protocolo de administración de claves se utilizan para configurar VPN IPsec.
13. **`Puerto 68 (DHCPC)`**: puerto de cliente DHCP.
14. **`Puerto 520 (ruta)`**: protocolo de información de enrutamiento (RIP).
15. **`Puerto 1900 (UPNP)`**: protocolo de detección de servicios simples de Microsoft, que permite la detección de dispositivos universales plug-and-play.
16. **`Puerto 4500 (nat-t-ike)`**: para negociar el recorrido de traducción de direcciones de red mientras se inician conexiones IPsec (durante el intercambio de claves de Internet).
17. **`Puerto 514 (Syslog)`**: el demonio de registro estándar de UNIX.
18. **`Puerto 49152 (varía)`**: el primero de los puertos dinámicos/privados especificados por IANA. No se pueden registrar puertos oficiales desde aquí hasta el final del rango de puertos (65536). Algunos sistemas utilizan este rango para sus puertos efímeros, por lo que a los servicios que enlazan un puerto sin solicitar un número específico a menudo se les asigna 49152 si son el primer programa en hacerlo.
19. **`Puerto 162 (SNMPTrap)`**: puerto de captura del protocolo de administración de red simple (un agente SNMP normalmente usa 161, mientras que un administrador SNMP generalmente usa 162).
20. **`Puerto 69 (TFTP)`**: protocolo trivial de transferencia de archivos.

### <mark style="color:blue;">¿Qué es el escaneo de puertos?</mark>

El escaneo de puertos es el acto de probar de forma remota numerosos puertos para determinar en qué estado se encuentran. El estado más interesante es Por lo general, abierta, lo que significa que una aplicación está escuchando y aceptando conexiones en el puerto.

Si bien muchos escáneres de puertos tradicionalmente han agrupado todos los puertos en los estados abierto o cerrado, Nmap es mucho más granular. Eso Divide los puertos en seis estados. Estos estados no son intrínsecos propiedades del puerto en sí, sino que describe cómo Nmap las ve.

Los seis estados portuarios reconocidos por Nmap

#### <mark style="color:yellow;">Abierto (Open)</mark>

Una aplicación acepta conexiones de paquetes TCP o UDP de forma activa en este puerto. Encontrarlos es a menudo el objetivo principal del escaneo de puertos. Las personas preocupadas por la seguridad saben que cada puerto abierto es una vía de ataque.&#x20;

Atacantes y pen-testers quieren explotar los puertos abiertos, mientras que los administradores intentan cerrar o protegerlos con firewalls sin frustrar a los usuarios legítimos. Los puertos abiertos también son interesantes para los análisis no relacionados con la seguridad porque muestra los servicios disponibles para su uso en la red.&#x20;

Antes de que te pongas demasiado entusiasmado con un puerto abierto, tenga en cuenta que es posible que la aplicación está protegida con un contenedor TCP (TCPD) o que la propia aplicación está configurada para dar servicio solo a las direcciones IP de clientes aprobadas. Tales casos aún dejan más superficie de ataque que un puerto.

#### <mark style="color:yellow;">Cerrado (Closed)</mark>

Un puerto cerrado es accesible (recibe y responde a los paquetes de sonda Nmap), pero no hay ninguna aplicación escuchando en él. Pueden ser útiles para mostrar que un anfitrión está en línea mediante una dirección IP (descubrimiento de host o escaneo de ping), y como parte de la detección del sistema operativo.&#x20;

Debido a que se puede acceder a los puertos cerrados, puede valer la pena escanearlos más tarde en caso de que se abran algunos. Es posible que los administradores deseen considerar bloquear dichos puertos con un firewall para que aparezcan en el estado filtrado.

#### <mark style="color:yellow;">Filtrado (Filtered)</mark>

Nmap no puede determinar si el puerto está abierto porque el filtrado de paquetes evita que sus sondas lleguen al puerto. El filtrado puede provenir de un dispositivo de firewall dedicado, enrutador o software de firewall basado en host.&#x20;

Estos puertos frustran atacantes porque proporcionan muy poca información. A veces responden con mensajes de error ICMP, como el código 13 de tipo 3 (Destino inalcanzable: comunicación administrativa prohibido), sino filtros que simplemente dejan caer las sondas sin responder son mucho más comunes.&#x20;

Esto obliga a Nmap a volver a intentarlo varias veces, solo en caso de que la sonda se haya interrumpido debido a la congestión de la red en lugar de filtrado. Este tipo de filtrado ralentiza drásticamente los escaneos.

#### <mark style="color:yellow;">Sin filtrar (Unfiltered)</mark>

El estado sin filtrar significa que se puede acceder a un puerto, pero Nmap no puede determinar si está abierto o cerrado.&#x20;

Solamente el análisis ACK, que se utiliza para asignar conjuntos de reglas de firewall, clasifica puertos a este estado. Escaneo SYN o el escaneo FIN, pueden ayudar a resolver si el puerto está abierto.

#### <mark style="color:yellow;">Abierto|filtrado (Open|Filtered)</mark>

Nmap coloca los puertos en este estado cuando no puede determinar si un puerto está abierto o filtrado. Esto ocurre para el escaneo tipos en los que los puertos abiertos no dan respuesta.&#x20;

La falta de también podría significar que un filtro de paquetes descartó la sonda o cualquier respuesta que obtuviera. Por lo tanto, Nmap no sabe con certeza si el puerto está abierto o se está filtrando. El UDP, el protocolo IP, Los escaneos FIN, NULL y Xmas clasifican los puertos de esta manera.

#### <mark style="color:yellow;">Cerrado|filtrado (Closed|Filtered)</mark>

Este estado se utiliza cuando Nmap no puede determinar si un puerto está cerrado o filtrado.

Si bien Nmap intenta producir resultados precisos, tenga en cuenta que toda su información se basa en paquetes devueltos por el objetivo máquinas (o cortafuegos frente a ellas). Dichos hosts pueden ser no confiables y enviar respuestas destinadas a confundir o engañar a Nmap. Mucho más comunes son los hosts que no cumplen con RFC y que no responden como deben a las sondas Nmap. Los escaneos FIN, NULL y Xmas son particularmente susceptible a este problema.

### <mark style="color:blue;">¿Por qué escanear puertos?</mark>

El escaneo de puertos no solo se realiza por diversión. Existen numerosas ventajas prácticas de escanear regularmente sus redes. Primero se encuentra la seguridad. Uno de los principios centrales de la red; la seguridad es la reducción del número y la complejidad de los servicios que se ofrece reduce la oportunidad de que los atacantes irrumpan.&#x20;

Los compromisos de red provienen de la explotación de una aplicación de un servidor remoto escuchando en un puerto TCP o UDP. En muchos casos, la aplicación ni siquiera es utilizada por la organización objetivo, sino que fue habilitada de forma predeterminada cuando se configuró la máquina. Si ese servicio hubiera sido desactivado, o protegido por un firewall, el ataque habría sido frustrado.

Consciente de que cada puerto abierto es una oportunidad para el compromiso, los atacantes escanean regularmente los objetivos, haciendo un inventario de todos los puertos. Comparan esta lista de servicios de escucha con su lista de exploits favoritos para software vulnerable.&#x20;

Solo se necesita un partido comprometer una máquina, creando un punto de apoyo que a menudo se utiliza para infestar toda la red. Los atacantes que son menos discriminatorios a quién se dirigen a menudo buscará solo el puerto predeterminado de una aplicación explotable. Esto es mucho más rápido que escanear cada puerto, aunque el servicio se perderá cuando se ejecute en un puerto.&#x20;

Tales atacantes a menudo son ridiculizados como "script kiddles", porque a menudo saben poco más sobre seguridad que cómo ejecutar un script de exploit escrito por alguien más hábil. En muchas organizaciones, estos atacantes están obligados a encontrar hosts vulnerables. Pueden ser bastante molestos, aunque su gran número y golpeteo incesante contra máquinas accesibles a Internet personas para parchear los sistemas rápidamente. Esto reduce la probabilidad de más Ataques serios y dirigidos que tienen éxito.

Una defensa importante contra estos crackers es para los sistemas administradores para escanear sus propias redes regularmente con herramientas como Nmap. Tome la lista de puertos abiertos y cierre cualquier servicio que no se utilizan. Garantizar que los que deben permanecer disponibles estén plenamente parcheado y que está en la lista de notificaciones de seguridad del proveedor. Siempre que sea posible, se deben agregar reglas de firewall, limitando el acceso solo a usuarios legítimos.&#x20;

Las instrucciones de endurecimiento están disponibles en la Web para aplicaciones más populares, reduciendo incluso la oportunidad del cracker más lejos. Nmap no puede hacer la mayor parte de esto por usted, pero crea la lista de servicios disponibles para empezar. Algunos administradores intentan En su lugar, use **netstat**, pero eso no escala bien. Requiere acceso a cada máquina, y algunas máquinas móviles son fáciles de pasar por alto. Más no puede ejecutar **netstat** en su punto de acceso inalámbrico promedio, VoIP teléfono o impresora. Además, siempre existe el riesgo de que un La máquina comprometida tendrá un **Netstat** troyano que emite información. La mayoría de los modernos rootkits instalados por los atacantes incluyen esta funcionalidad. Confiar únicamente en Nmap es un Error también. Una combinación de diseño cuidadoso, auditoría de configuración, Y es aconsejable realizar exploraciones periódicas.

Si bien la seguridad es la razón más común para el escaneo de puertos, Los administradores a menudo descubren que también se adapta a otros propósitos. La creación de un inventario de las máquinas y los servicios que ofrecen puede ser útil para el seguimiento de activos, el diseño de redes, las comprobaciones de cumplimiento de políticas, seguimiento de licencias de software, pruebas de disponibilidad, depuración de red, y más.

### Un tutorial rápido de escaneo de puertos

Un novato puede comenzar con un comando tan simple como **nmap&#x20;**_**`<target>`**_. Mientras tanto, los usuarios avanzados a veces especifican tantas opciones que su La línea terminal se envuelve.

Se debe lograr un equilibrio similar con la salida del comando. Lo más Los resultados importantes deben sobresalir incluso para el usuario ocasional que Ni siquiera ha leído la página del manual. Sin embargo, el resultado debe ser exhaustivo y lo suficientemente conciso como para adaptarse a los probadores de penetración profesionales que ejecutan Nmap contra miles de máquinas al día. Los usuarios lo suficientemente inteligentes como para leer esto libro o el código fuente de Nmap se benefician de un mayor control de el escáner y la información sobre lo que realmente significa la salida de Nmap.

El comando Nmap más simple es **simplemente nmap** por se. Esto imprime una hoja de trucos de las opciones y sintaxis comunes de Nmap. Un comando más interesante es **nmap&#x20;**_**`<target>`**_, que hace el siguiente:

1. Convierte _`<target>`_ de un hostname en una dirección IPv4 mediante DNS. Si un Se especifica la dirección IP en lugar de un nombre de host, se omite esta búsqueda.
2. Hace ping al host, de forma predeterminada con un paquete de solicitud de eco ICMP y un paquete TCP ACK al puerto 80, para determinar si está activo y corriente. De lo contrario, Nmap informa de ese hecho y se va. Podría haberlo hecho especificado para omitir esta prueba. Consulte [el Capítulo 3, _Detección de hosts ("Escaneo de ping")_](https://nmap.org/book/host-discovery.html).`-Pn`
3. Convierte la dirección IP de destino de nuevo en el nombre mediante una consulta de DNS inverso. Debido a la forma en que funciona el DNS, el nombre inverso puede no ser el mismo que el _`<target>`_ especificado en la línea de comandos. Esta consulta se puede omitir con la opción de mejorar la velocidad y Sigilo.`-n`
4. Inicia un escaneo de puertos TCP de los 1.000 puertos más populares de la lista en. Un escaneo sigiloso SYN suele ser se utiliza, pero en su lugar se sustituye el escaneo de conexión para los usuarios de Unix no root que carecen de los privilegios necesarios para enviar Paquetes.`nmap-services`
5. Imprime los resultados en la salida estándar en modo normal formato legible por humanos, y salidas. Otros formatos y ubicaciones de salida (files), como se describe en [el Capítulo 13, _Formatos de salida de Nmap_](https://nmap.org/book/output.html). [En el ejemplo 4.2](https://nmap.org/book/port-scanning-tutorial.html#port-scanning-tutorial-nmap1) se muestran los resultados cuando scanme.nmap.org se utiliza como _`<objetivo>`_.

### Marcas de línea de comandos

#### Selección de técnicas de escaneo

Una de las primeras consideraciones a la hora de contemplar un escaneo de puertos es decidir qué técnicas usar. Nmap ofrece alrededor de una docena de tales y en esta sección se ofrece un breve resumen de los mismos. Lleno La cobertura viene en el siguiente capítulo. Solo se puede utilizar un método de exploración a la vez, excepto que el escaneo UDP () puede combinarse con cualquiera de los tipos de escaneo TCP. Como ayuda de memoria, el tipo de escaneo de puertos Las opciones son de la forma , donde _`<C>`_ es un carácter prominente en el escaneo nombre, generalmente el primero. La única excepción a esto es el obsoleto Escaneo de rebote FTP (). De forma predeterminada, Nmap realiza un SYN Scan, aunque sustituye a un escaneo de conexión si el usuario no lo hace tener los privilegios adecuados para enviar paquetes sin procesar (requiere acceso root en Unix) o si Se especificaron los destinos IPv6.`-sU-s`_`<C>`_`-b`

Métodos de escaneo de puertos compatibles con Nmap

[la sección llamada "TCP SYN (Stealth) Scan (`-sS`)"](https://nmap.org/book/synscan.html) (`-sS`)

Este es, de lejos, el tipo de escaneo más popular porque la forma más rápida de escanear puertos del protocolo más popular (TCP). Es más sigiloso que el escaneo de conexión y funciona contra todos los pilas TCP funcionales (a diferencia de algunos análisis de propósito especial, como FIN) escaneo).

[la sección llamada "TCP Connect Scan (`-sT`)"](https://nmap.org/book/scan-methods-connect-scan.html) (`-sT`)

El análisis de Connect utiliza la llamada al sistema del mismo nombre para escanear máquinas, en lugar de confiar en paquetes sin procesar, ya que la mayoría de los otros métodos sí lo hacen. Por lo general, es utilizado por usuarios de Unix sin privilegios y contra objetivos IPv6 porque el escaneo SYN no funciona en esos Casos.

[la sección llamada "Escaneo UDP (`-sU`)"](https://nmap.org/book/scan-methods-udp-scan.html) (`-sU`)

No olvide los puertos UDP, ya que ofrecen muchos Los agujeros de seguridad también.

[la sección denominada "TCP FIN, NULL y Xmas Scans (`-sF`, `-sN`, `-sX`)"](https://nmap.org/book/scan-methods-null-fin-xmas-scan.html) (`-sF`, `-sX`, `-sN`)

Estos tipos de escaneo de propósito especial son expertos en escabullirse más allá de los cortafuegos para explorar los sistemas que hay detrás de ellos. Desgraciadamente se basan en el comportamiento objetivo que algunos sistemas (en particular Windows variantes) no se exhiben.

[la sección llamada "TCP ACK Scan (`-sA`)"](https://nmap.org/book/scan-methods-ack-scan.html) (`-sA`)

El escaneo ACK se usa comúnmente para mapear el firewall conjuntos de reglas. En particular, ayuda a comprender si las reglas de firewall tienen estado o no. La desventaja es que no puede distinguir Abierto desde puertos cerrados.

[la sección llamada "TCP Window Scan (`-sW`)"](https://nmap.org/book/scan-methods-window-scan.html) (`-sW`)

El escaneo de ventana es como el escaneo ACK, excepto que es capaz de para detectar puertos abiertos frente a puertos cerrados contra ciertos Máquinas.

[la sección llamada "TCP Maimon Scan (`-sM`)"](https://nmap.org/book/scan-methods-maimon-scan.html) (`-sM`)

Este oscuro tipo de escaneo que evade el firewall es similar a un escaneo FIN, pero también incluye el indicador ACK. Esto permite para pasar por más firewalls de filtrado de paquetes, con la desventaja de que funciona incluso contra menos sistemas que el escaneo FIN.

[la sección llamada "TCP Idle `Scan (-sI`)"](https://nmap.org/book/idlescan.html) (`-sI`` `_`<host zombie>`_)

El análisis inactivo es el tipo de análisis más sigiloso de todos y, a veces, puede explotar las relaciones de direcciones IP de confianza. Desafortunadamente, también es lento y complejo.

[la sección llamada "Escaneo de protocolo IP (`-sO`)"](https://nmap.org/book/scan-methods-ip-protocol-scan.html) (`-sO`)

El análisis de protocolos determina qué protocolos IP (TCP, ICMP, IGMP, etc.) son compatibles con el equipo de destino. Técnicamente, esto no es un puerto escaneo, ya que recorre los números de protocolo IP en lugar de TCP o Números de puerto UDP. Sin embargo, sigue utilizando la opción de seleccionar los números de protocolo escaneados, informa de sus resultados con el formato de tabla de puertos, e incluso utiliza el mismo motor de análisis subyacente que los verdaderos métodos de escaneo de puertos. Por lo tanto, está lo suficientemente cerca de un escaneo de puertos que pertenece aquí.`-p`

[la sección llamada "TCP FTP Bounce Scan (`-b`)"](https://nmap.org/book/scan-methods-ftp-bounce-scan.html) (`-b`` `_`<FTP bounce proxy>`_)

Este tipo de análisis obsoleto engaña a los servidores FTP para que realicen análisis de puertos por poder. La mayoría de los servidores FTP ahora están parcheados para evitar esto, pero es una buena manera de escabullirse a través de las restricciones cortafuegos cuando funciona.

#### Selección de puertos para analizar

Archivo de registro de puertos de Nmap () contiene datos empíricos sobre cómo con frecuencia, cada puerto TCP o UDP se encuentra abierto. Estos datos fueron recopilados mediante el escaneo de decenas de millones de direcciones de Internet, combinando esos resultados con los datos de escaneo interno aportados por grandes empresas. De forma predeterminada, Nmap escanea los 1.000 puertos más populares de cada protocolo que se le pide que escanee. Como alternativa, puede especificar el (ayuno) Opción para escanear solo los 100 puertos más comunes en cada protocolo o para especificar un número arbitrario de puertos para escanear.`nmap-services-F--top-ports`

Cuando ninguno de estos conjuntos de puertos fijos se adapta a sus necesidades, se puede especificar una lista arbitraria de números de puerto en la línea de comandos con la opción. La sintaxis de la opción puede ser compleja y se describe mejor con ejemplos.`-p-p`

Ejemplos de selección de puertos con la opción`-p-p 22`Analice un solo puerto (en este caso, el puerto 22) por especificando solo ese número como argumento.`-p-p ssh`Los nombres de los puertos se pueden especificar en lugar de números. Tenga en cuenta que un nombre puede coincidir con varios puertos.`-p 22,25,80`Varios puertos pueden estar separados por comas. Nota que no se especifica ningún protocolo, por lo que estos mismos números de puerto se usarán para cualquier método de escaneo que se especifique en la línea de comandos. Si un escaneo TCP como Se especifica SYN scan (), puertos TCP 22, 25 y 80 se escanean. Estos corresponden a los servicios SSH, SMTP y HTTP, respectivamente. Si se selecciona un escaneo UDP (), se analizan esos tres puertos UDP. Si se especifican ambos, esos Se analizan tres puertos para cada protocolo, para un total de seis puertos escaneados. Con el escaneo del protocolo IP (), esos tres protocolos IP (correspondientes a XNS IDP, Leaf-1 e ISO-IP) son Escaneado.`-sS-sU-sO-p80-85,443,8000-8005,8080-8085`Los rangos de puertos se pueden especificar separando el puerto inicial y final con un guión. Múltiples gamas o individuales Los puertos se pueden especificar con comas. Esta opción escanea los puertos 80, 81, 82, 83, 84, 85, 443, 8000, etc. En función de los números de puerto, este usuario es probablemente escaneando TCP y buscando web Servidores.`-p-100,60000-`Puede omitir el comienzo de un intervalo para implicar el puerto uno, o el final para implicar el último puerto posible (65535 para TCP y UDP, 255 para el examen de protocolo). En este ejemplo se examinan los puertos del uno al 100 y todos los puertos mayores o iguales a 60.000.`-p-`Omita los números inicial y final para examinar todo el rango (excepto el cero).`-pT:21,23,110,U:53,111,137,161`Las listas separadas de puertos TCP y UDP pueden ser proporcionadas por precediendo a las listas con T: (para TCP) o U:. En este ejemplo se analiza tres puertos TCP (FTP, Telnet y POP3) y cuatro servicios UDP (DNS, rpcbind, NetBIOS y SNMP). Especificando solo los puertos TCP y UDP importa si también le dices a Nmap que haga un escaneo UDP () y uno de los métodos de exploración TCP, como , , o .`-sU-sS-sA-sF-p http*`

Los comodines se pueden usar para hacer coincidir puertos con nombres similares. Esta expresión coincide con ocho números de puerto, incluidos http (80), http-mgmt (280), https (443) y http-proxy (8080). Dependiendo de su shell de comandos, es posible que deba escapar del asterisco para que no se trate como un globo de nombre de archivo.

`-p 1-1023,[1024-]`

Encerrar un rango entre paréntesis hace que esos números de puerto para ser escaneados solo si están registrados en `nmap-services`. En este ejemplo, todos los puertos reservados (1–1.023), además de todos los puertos superiores registrados en `nmap-services`. Ese era el valor predeterminado de Nmap comportamiento antes `de nmap-services` se incrementó con Abra los datos de frecuencia del puerto para obtener datos más precisos selección.

#### Opciones relacionadas con el tiempo

El escaneo de puertos suele ser la parte que más tiempo consume de un Nmap (que también puede incluir la detección del sistema operativo, la detección de versiones y scripts NSE). Si bien Nmap intenta ser rápido y eficiente de forma predeterminada, La optimización manual a menudo ayuda. Nmap ofrece docenas de opciones para Adapte la intensidad y la velocidad del escaneo para que se adapte a sus necesidades exactas. Éste La sección enumera las opciones más importantes para optimizar el escaneo de puertos veces. Las opciones que tardan una cantidad de tiempo se expresan en segundos de forma predeterminada, o puede agregar `ms` (milisegundos), `s` (segundos), `m` (minutos) o `h` (horas) al valor. Para obtener más detalles sobre cualquiera de estas opciones, consulte [la sección denominada "Tiempo y rendimiento".](https://nmap.org/book/man-performance.html) Un tratamiento mucho más completo, con ejemplos y mejores prácticas para mejorar el rendimiento de Nmap es disponible en [el Capítulo 6, _Optimización del rendimiento de Nmap_](https://nmap.org/book/performance.html).

Principales opciones de rendimiento de escaneo de puertos`De -T0` a `-T5`

Estas plantillas de temporización afectan a muchas variables, ofreciendo una forma sencilla de ajustar la velocidad general de Nmap desde muy lento (`-T0`) a extremadamente agresivo ( `-T5`). Una plantilla de temporización se puede combinar con Las opciones más granulares se describen a continuación, y la opción más granular tiene prioridad.

`--min-rtt-timeout`, `--max-rtt-timeout`, `--initial-rtt-timeout`

La cantidad de tiempo mínima, máxima e inicial que Nmap esperará una respuesta de sondeo de escaneo de puertos.

`--host-timeout`

Pide a Nmap que renuncie a los hosts que toman más que el cantidad de tiempo dada para escanear.

`--tasa-min,` `--tasa-máx.`

Establece el suelo y el techo, respectivamente, en el número de paquetes de sondeo que Nmap envía por segundo.

`--max-retries`

Especifica el número máximo de retransmisiones de sondeo de detección de puertos a un solo puerto.

`--min-hostgroup`, `--max-hostgroup`

Establece el número mínimo y máximo de hosts que Nmap portará el escaneo en paralelo.

`--paralelismo-mínimo`, `--paralelismo-máximo`

Limita el número mínimo o máximo de análisis de puertos sondas (en todos los hosts escaneados simultáneamente) que Nmap puede tener excepcional.

`--retardo-de-escaneo`, `--retardo-de-escaneo-máximo`

Pide a Nmap que espere al menos la cantidad de tiempo dada entre el envío de sondeos a cualquier host individual. El retardo de escaneo puede crece a medida que Nmap detecta la pérdida de paquetes, por lo que se puede especificar un máximo con `--max-scan-delay`.

#### Opciones de formato de salida y verbosidad

Nmap ofrece la posibilidad de escribir sus informes en su estándar , un formato "grepable" orientado a líneas simples, o XML. Estos informes se habilitan con `-oN` (normal), `-oG` (grepable) y `-oX` (XML) Opciones. Cada opción toma un nombre de archivo, y se pueden combinar para Salida en varios formatos a la vez. También hay varias opciones disponibles para Aumente el nivel de detalle de la salida. En esta sección se enumeran las opciones relacionadas con la salida más importantes y cómo se aplican al análisis de puertos. Para obtener más detalles sobre cualquiera de estas opciones, consulte [la sección denominada "Salida".](https://nmap.org/book/man-output.html) Un tratamiento mucho más exhaustivo de las opciones y formatos de salida, con muchos ejemplos, está disponible en [el Capítulo 13, _Formatos de salida de Nmap_](https://nmap.org/book/output.html).

Principales opciones de salida de Nmap aplicables a los escaneos de puertos`-v`

Aumenta el nivel de verbosidad, lo que hace que Nmap imprima Más información sobre el análisis en curso. Se muestran los puertos abiertos a medida que se encuentran y se proporcionan estimaciones del tiempo de finalización cuando Nmap cree que un escaneo tomará más de unos pocos minutos. Úsalo dos veces o más para una verbosidad aún mayor.

`-d`

Aumenta el nivel de depuración, lo que hace que Nmap imprima detalles sobre su funcionamiento que pueden ser útiles para rastrear errores o simplemente entender cómo funciona. Los niveles más altos dan como resultado cantidades masivas de datos. El uso de la opción una vez establece la depuración level a uno, y se incrementa por cada `-d` adicional. O puede seguir la `-d` con el nivel deseado, como en `-d5`. Si no ves suficiente información, pruebe con un nivel superior. El nivel efectivo máximo es nueve. Si la pantalla está inundada con demasiados datos de depuración, Reduzca el nivel. Reducir la intensidad del escaneo, como el número de puertos u objetivos escaneados y las características utilizadas, también pueden ayudar a aislar solo los mensajes de depuración que desee.

`--packet-trace`

Hace que Nmap imprima un resumen de cada paquete enviado o recibidos. Esto se usa a menudo para la depuración, pero también es un una forma valiosa para que los nuevos usuarios entiendan exactamente lo que está haciendo Nmap debajo de las sábanas. Para evitar imprimir miles de líneas, puede Desea especificar un número limitado de puertos para analizar, como `-P20-30`.

`-oN`` `_`<nombre de archivo>`_ (salida normal)

Escriba la salida en el formato normal de Nmap en _`<nombre de archivo>`_. Este formato es aproximadamente el igual que la salida interactiva estándar impresa por Nmap en Ejecución.

`-oX`` `_`<nombre de archivo>`_ (salida XML)

Escriba la salida en formato XML de Nmap en _`<nombre de archivo>`_. Salida normal (legible por humanos) se seguirá imprimiendo en stdout a menos que pida que XML sea dirigido allí especificando `-` como _`<nombre de archivo>`_. Este es el formato preferido para su uso por scripts y programas que procesan Nmap Resultados.

`-oG`` `_`<nombre de archivo>`_ (salida en formato grepable)

Escriba la salida en el llamado formato grepable de Nmap a _`<nombre de archivo>`_. Este formato tabular se ajusta a la de cada host en una sola línea, lo que facilita el grep para puertos abiertos, ciertos sistemas operativos, nombres de aplicaciones u otros datos. La salida normal se seguirá imprimiendo en stdout a menos que usted lo solicite para que la salida grepable se dirija allí especificando `-` como _`<nombre de archivo>`_. Mientras Este formato funciona bien para analizar con grep y awk simples líneas de comandos, scripts y programas significativos deben usar el XML salida en su lugar. El formato XML contiene información sustancial ese formato grepable no tiene cabida y la extensibilidad hace que XML más fácil de actualizar con nueva información sin romper las herramientas que Confía en él.

`-oA`` `_`<basename>`_ (salida a todos los formatos)

Para mayor comodidad, puede especificar `-oA`` `_`<basename>`_ para almacenar el escaneo resultados en formatos normal, XML y grepable a la vez. Ellos se almacenan en _`<basename>`_.nmap, _`<basename>`_.xml y _`<basename>`_.gnmap, respectivamente. Al igual que con la mayoría de los programas, puede prefijar los nombres de archivo con un ruta de directorio, como `~/nmaplogs/foocorp/` en Unix o `c:\hacking\sco` en Windows.

`--resume`` `_`<filename>`_

Reanude un examen anulado especificando la opción normal (`-oN`) o archivo de salida grepable (`-oG`) que se creó durante el desafortunado escaneo. No uses ninguna opción aparte de `--resume`, ya que Nmap usará los especificado en el archivo de salida. A continuación, analiza el archivo y lo reanuda escaneando (y registrando en el archivo) en el host que el La ejecución anterior de Nmap estaba trabajando cuando cesó.

`--append-output`

Le dice a Nmap que agregue los resultados del escaneo a cualquier salida archivos especificados (con argumentos como `-oN` o `-oX`) en lugar de sobrescribirlos.

`--open`

Muestre solo los hosts que tienen puertos abiertos y solo muestre los puertos abiertos para esos. Aquí, los "puertos abiertos" son cualquier puerto que tenga la posibilidad de estar abierto, lo que incluye `abierto`, `abierto|filtrado` y `sin filtrar`.

#### Opciones de evasión de firewall e IDS

Nmap ofrece muchas opciones para escabullirse de los IDS sin ser detectado o Evadir las reglas del firewall. Para obtener una descripción general, consulte [la sección denominada "Evasión y suplantación de identidad de firewall/IDS".](https://nmap.org/book/man-bypass-firewalls-ids.html) Para una visión completa técnicas de evasión de cortafuegos e IDS, junto con ejemplos prácticos, consulte [el Capítulo 10, _Detección y subversión de firewalls y sistemas de detección de intrusiones_](https://nmap.org/book/firewalls.html).

#### Especificación de destinos

Para escanear un solo host (o algunos de ellos), simplemente agregue sus nombres o direcciones IP hasta el final de la línea de comandos de Nmap. Nmap también tiene un Sintaxis estructurada para facilitar el escaneo de grandes redes. Puedes dar Nmapear un archivo que enumera los objetivos, o incluso pedirle a Nmap que los genere al azar. Todo esto se describe en [la sección denominada "Especificación de hosts y redes de destino".](https://nmap.org/book/host-discovery-specify-targets.html)

#### Opciones misceláneas

Aquí hay algunas opciones que pueden ser bastante útiles a pesar de que no encajan en categorías específicas. Las descripciones se centran en cómo Cada opción se relaciona con el escaneo de puertos. Consulte el [Capítulo 15, _Guía de referencia de Nmap_](https://nmap.org/book/man.html) para obtener una cobertura más completa de cada opción.

`-6`

Pide a Nmap que escanee el objetivo utilizando el protocolo IPv6. Este proceso se describe en [la sección denominada "Escaneo de IPv6 (`-6`)".](https://nmap.org/book/port-scanning-ipv6.html)

`-r`

Nmap aleatoriza el orden de escaneo de puertos de forma predeterminada para hacer detección un poco más difícil. La opción `-r` hace que se escaneen en orden numérico en lugar de.

`-Pn`

Le dice a Nmap que se salte la prueba de ping y simplemente escanee todos los hosts de destino proporcionados. Otras opciones para controlar el host descubrimiento se describen en el [Capítulo 3, _Detección de host ("Escaneo de ping")_](https://nmap.org/book/host-discovery.html).

`--reason`

Agrega una columna a la tabla de puertos interesantes que describe por qué Nmap clasificó un puerto como lo hizo.

### Escaneo de IPv6 (`-6`)

Desde 2002, Nmap ha ofrecido soporte IPv6 para sus productos más populares. Funciones. En particular, escaneo de ping (solo TCP), conexión el escaneo y la detección de versiones son compatibles con IPv6. La sintaxis del comando es lo mismo que de costumbre, excepto que también agrega la opción. Por supuesto, debe utilizar la sintaxis IPv6 si especifica una dirección en lugar de un nombre de host. Una dirección puede parecerse a , por lo que los nombres de host se recomiendan. [En el ejemplo 4.4](https://nmap.org/book/port-scanning-ipv6.html#port-scanning-ex-ipv6) se muestra un Sesión típica de escaneo de puertos. La salida tiene el mismo aspecto que de costumbre lo hace, y la dirección IPv6 en la línea de "puertos interesantes" es el único indicio de IPv6.`-63ffe:7501:4819:2000:210:f3ff:fe03:14d0`

Ejemplo 4.4. Un simple escaneo de IPv6

Si bien IPv6 no ha conquistado el mundo exactamente, se uso significativo en algunos países y en la mayoría de los países Los sistemas operativos lo admiten. Para usar Nmap con IPv6, tanto la fuente y el destino de su escaneo debe estar configurado para IPv6. Si su proveedor de servicios de Internet (como la mayoría de ellos) no le asigna direcciones IPv6, gratis Los corredores de túneles están ampliamente disponibles y funcionan bien con Nmap. Utilizo el servicio gratuito de intermediario de túneles IPv6 en [`http://www.tunnelbroker.net`](http://www.tunnelbroker.net/). Se enumeran otros agentes de túneles [en Wikipedia](http://en.wikipedia.org/wiki/List_of_IPv6_tunnel_brokers). Los túneles 6to4 son otro túnel popular, gratuito acercarse.

Los sistemas que admiten IPv6 no siempre tienen sus IPv4 e IPv6 Reglas de firewall sincronizadas. [la sección llamada "Ataques IPv6"](https://nmap.org/book/firewall-subversion.html#defeating-firewalls-ipv6) muestra un ejemplo de la vida real de llegar a puertos a través de IPv6 que son filtrado en IPv4.

### SOLUCIÓN: Escanee una red grande en busca de un determinado puerto TCP abierto

#### Problema

Desea encontrar rápidamente todas las máquinas de una red que tienen un cierto puerto TCP abierto. Por ejemplo, después de un nuevo Microsoft IIS vulnerabilidad, es posible que desee buscar todas las máquinas con TCP puerto 80 abierto y asegúrese de que no estén ejecutando un versión de ese software. O si investiga una caja comprometida y descubra que el atacante dejó una puerta trasera ejecutándose en el puerto 31337, escaneando toda la red para ese puerto podría identificar rápidamente otros sistemas comprometidos. Más tarde se realizaría un análisis completo (de todos los puertos).

#### Solución

La forma sencilla es ejecutar:

**nmap -Pn -p**_**`<portnumber>`**_**&#x20;-oG&#x20;**_**`<logfilename.gnmap>`**_ _**`<redes de destino>`**_

A continuación, se muestra un ejemplo concreto de búsqueda de IP 4096 para servidores web (puerto 80 abierto):

**nmap -Pn -p80 -oG logs/pb-port80scan-%D.gnmap 216.163.128.0/20**

La "%D" en el nombre del archivo se sustituye por la fecha numérica en la que se ejecutó el análisis (por ejemplo, "090107" el 1 de septiembre de 2007). Si bien este comando de escaneo funciona, un poco de esfuerzo para elegir el momento adecuado Los valores de la red que se está analizando reducen el tiempo de exploración substancialmente. El escaneo anterior tardó 1.236 segundos, mientras que el optimizado La versión a continuación proporcionó los mismos resultados en 869 segundos:

**nmap -T4 -Pn -p80 --max-rtt-timeout 200ms --initial-rtt-timeout 150ms --min-hostgroup 512 -oG logs/pb-port80scan2-%D.gnmap 216.163.128.0/20**

Y gran parte de ese tiempo se dedica a hacer resolución de DNS inverso. Excluyendo eso agregando a la línea de comandos anterior Reduce el tiempo de análisis del host 4096 a 193 segundos. Ser paciente durante tres minutos es mucho más fácil que los 21 minutos tomados antes.`-n`

Los comandos anteriores almacenan los resultados en formato grepable en el archivo especificado. Un simple comando egrep encontrará las máquinas con el puerto 80 abierto:

**egrep '\[^0-9]80/open' logs/pb-port80scan2-\*.gnmap**

El patrón egrep está precedido por \[^0-9] para evitar errores falsos. puertos coincidentes como el 3180. Por supuesto, eso no puede suceder ya que estamos solo escaneando el puerto 80, pero es una buena práctica recordar para Escaneos de varios puertos. Si solo quieres las direcciones IP y nada más, Canalice la salida de egrep a **awk '{imprimir $2}'**.

#### Discusión

A veces, una historia es la mejor manera de entender las decisiones, como la forma en que decidí las líneas de comandos en la sección de soluciones. Estaba aburrido en casa y comencé a explorar la red de una revista popular llamada _Playboy_. Su sitio principal incluye un gran tesoro de imágenes, pero la mayoría están encerradas detrás de un sistema de autenticación de suscripción paga. Tenía curiosidad por saber si podía encontrar algún otro sistema en su red que ofreciera imágenes de forma gratuita. Supuse que podrían tener servidores de ensayo o desarrollo que se basan en la oscuridad en lugar de la autenticación con contraseña. Si bien estos servidores teóricamente podrían escuchar en cualquier número de puerto, lo más probable es que sea el puerto TCP 80. Así que decido escanear toda su red en busca de ese puerto abierto lo más rápido posible.

El primer paso es determinar qué direcciones IP escanear. Realizo una búsqueda whois de la Registro Americano de Números de Internet (ARIN) para organizaciones llamadas Playboy. Los resultados se muestran en el [Ejemplo 4.5](https://nmap.org/book/solution-find-open-port.html#port-scanning-ex-whois-playboy).

Esto muestra 4096 direcciones IP (el rango neto 216.163.128.0/20) registradas a Playboy. Usando las técnicas discutidas en [la sección llamada "Encontrar las direcciones IP de una organización",](https://nmap.org/book/host-discovery-find-ips.html) podría haber encontrado muchas más netblocks que controlan, pero las IP 4096 son suficiente para este ejemplo.

Siguiente quiero estimar latencia a estas máquinas, de modo que Nmap sabrá qué esperar. Esto no es necesario, pero alimentar Nmap Los valores de temporización adecuados pueden acelerarlo. Esto es particularmente cierto para escaneos de un solo puerto, como este. Nmapa no recibe suficientes respuestas de cada host para estimar la latencia y la tasa de caída de paquetes, por lo que lo ayudaré en el línea de comandos. Mi primer pensamiento es hacer ping a su servidor web principal, ya que que se muestra en [el Ejemplo 4.6](https://nmap.org/book/solution-find-open-port.html#port-scanning-ex-www-playboy-ping).`-Pn`

Ejemplo 4.6. Hacer ping al servidor web de Playboy para obtener una estimación de latencia

El tiempo máximo de ida y vuelta es de 58 milisegundos. Desgraciadamente esta dirección IP (209.247.228.201) no está dentro de 216.163.128.0/20 netblock que deseo escanear. Normalmente agregaría este nuevo bloque de red a la lista de objetivos, pero ya he decidido limitar mi escaneo a la IP 4096 originales. Estos tiempos son probablemente perfectamente buenos para usar, pero encontrar valores reales de las direcciones IP en la red de destino sería incluso mejor. Utilizo dig para obtener Playboy's registros DNS públicos de un servidor de nombres que se muestran en el whois anterior consulta. El resultado se muestra en [el Ejemplo 4.7](https://nmap.org/book/solution-find-open-port.html#port-scanning-ex-www-playboy-dig).

Ejemplo 4.7. Indagando en los registros DNS de Playboy

La consulta DNS revela dos servidores MX (correo) dentro del bloque de red 216.163.128.0/20 de destino. Dado que los nombres implican que están en diferentes regiones (Chicago y Los Ángeles), decido probarlos a ambos para ver la latencia. Los resultados **del ping** se muestran en [el Ejemplo 4.8](https://nmap.org/book/solution-find-open-port.html#port-scanning-ex-www-playboy-mxping).`mx.chimx.la`

Ejemplo 4.8. Hacer ping a los servidores MX

Bueno, ¡ese intento fue un fracaso miserable! Los anfitriones parecen estar bloqueando los paquetes de ping ICMP. Dado que son servidores de correo, deben tengo el puerto TCP 25 abierto, así que intento de nuevo usando [hping2](http://www.hping.org/) para realizar un TCP ping contra el puerto 25, como se muestra en el [Ejemplo 4.9](https://nmap.org/book/solution-find-open-port.html#port-scanning-ex-playboy-mxping-tcp).

Ejemplo 4.9. TCP haciendo ping a los servidores MX

Estos son los resultados que estaba buscando. El anfitrión de Los Ángeles nunca tarda más de 16 milisegundos en responder, mientras que el de Chicago tarda hasta 62 milisegundos. Esto no es sorprendente, dado que estoy sondeo desde una máquina en California. Vale la pena ser cauteloso, y la latencia puede aumentar durante el escaneo pesado, así que decido dejar que Nmap Espere hasta 200 milisegundos para recibir respuestas. Haré que comience con un tiempo de espera de 150 ms. Así que le paso las opciones. Para establecer un valor generalmente agresivo modo de temporización, especifico al principio de la línea.`--max-rtt-timeout 200ms --initial-rtt-timeout 150ms-T4`

Dado que valoro minimizar el tiempo de finalización de todo el escaneo Minimizar la cantidad de tiempo antes del primer lote de resultados del host , especifico un tamaño de grupo de escaneo grande. La opción se especifica de modo que al menos 512 Las direcciones IP se analizarán en paralelo (cuando sea posible). Usando un factor del tamaño de la red de destino (4096) evita que la pequeña y menor eficiente bloque de 96 hosts que ocurriría al final si especifico . Todos estos problemas de tiempo son explicado con mucha más profundidad en [el Capítulo 6, _Optimización del rendimiento de Nmap_](https://nmap.org/book/performance.html).`--min-hostgroup 512--min-hostgroup 500`

No hay necesidad de perder el tiempo con una etapa de ping previa, ya que un El ping tardaría tanto como el propio análisis de un solo puerto. Por lo tanto, se especifica para deshabilitar esa etapa. Substancial El tiempo se ahorra omitiendo la resolución de DNS inverso con el argumento. De lo contrario, con el escaneo de ping deshabilitado, Nmap intentaría buscar todas las IP 4096. Soy yo buscando servidores web, por lo que solicito el puerto 80 con . Por supuesto, echaré de menos cualquier servidor HTTP que se esté ejecutando en puertos no estándar como 81 u 8080. Servidores SSL en el puerto 443 tampoco se encontrará. Uno podría agregarlos a la opción, pero incluso un puerto más duplicaría el tiempo de escaneo, que es aproximadamente proporcional al número de puertos escaneados.`-Pn-n-p80-p`

A la última opción le sigue la opción nombre de archivo en el que quiero que se almacenen los resultados grepable. Añado el objetivo network al comando, luego presione enter para ejecutar Nmap. La salida se muestra en [el Ejemplo 4.10](https://nmap.org/book/solution-find-open-port.html#port-scanning-ex-playboy-port80-scan).`-oG`

Ejemplo 4.10. Iniciar el análisis

Nmap escanea las 4096 IP en aproximadamente tres minutos. Lo normal La salida muestra un montón de puertos en el estado. Es probable que la mayoría de esas direcciones IP no sean hosts activos, es decir, el puerto simplemente aparece filtrado porque Nmap no recibe ninguna respuesta a su SYN Sondas. Obtengo la lista de servidores web con un simple **egrep** en el archivo de salida, como se muestra en [el Ejemplo 4.11](https://nmap.org/book/solution-find-open-port.html#port-scanning-ex-playboy-port80-grep).`filtered`

Ejemplo 4.11. Egrep para puertos abiertos

espués de todo ese esfuerzo, solo dos servidores web accesibles son ¡Encontrado de 4096 IPs! A veces eso sucede. El primero, 216.163.140.20 (sin nombre DNS inverso) me lleva a un Microsoft Outlook Servidor de acceso web (webmail). Eso podría emocionarme si estuviera tratando de comprometer su red, pero no es gratificante ahora. El siguiente servidor (nombre inverso mirrors.playboy.com) es mucho mejor. Ofrece a aquellos ¡gigabytes de imágenes gratis que estaba esperando! En particular, ofrece imágenes ISO de Linux, así como FreeBSD, CPAN y ¡Archivos Apache! Descargo las últimas ISOs de Fedora Core en un respetables 6 Mbps. La abundancia de ancho de banda en Playboy es No es de extrañar. Más tarde escaneo otros bloques de red de Playboy, encontrando docenas de servidores web más, aunque parte de su contenido es inapropiado para este libro.

Si bien esta es una razón inusual para el escaneo de puertos, un solo puerto Los barridos son comunes para muchos otros propósitos expresados anteriormente. El Las técnicas descritas aquí se pueden aplicar fácilmente a cualquier TCP de un solo puerto barrer.

#### Consulte también

La detección de versiones se puede utilizar para encontrar aplicaciones específicas que estén escuchando en una red. Por ejemplo, podría buscar una determinada versión vulnerable de OpenSSH en lugar de buscar todos los hosts con el puerto 22 abierto. Esto también es útil para escaneos UDP de un solo puerto, ya que las técnicas de esta solución solo funcionan bien para TCP. Instrucciones se proporcionan en [la sección denominada "SOLUCIÓN: Buscar todos los servidores que ejecutan una versión de aplicación insegura o no estándar".](https://nmap.org/book/vscan-find-service-fast.html)

[El Capítulo 6, _Optimización del rendimiento de Nmap, analiza_](https://nmap.org/book/performance.html) la velocidad de escaneo optimización en mucha más profundidad.
