---
icon: block-brick
description: >-
  Conozca algunas de las tecnologías utilizadas para extender las redes a
  Internet y las motivaciones para ello.
layout:
  title:
    visible: true
  description:
    visible: true
  tableOfContents:
    visible: true
  outline:
    visible: true
  pagination:
    visible: false
---

# Ampliación de la Red

## Introducción al reenvío de puertos

El reenvío de puertos es un componente esencial para conectar aplicaciones y servicios a Internet. Sin el reenvío de puertos, las aplicaciones y los servicios, como los servidores web, solo están disponibles para los dispositivos dentro de la misma red directa.

Tomemos como ejemplo la siguiente red. Dentro de esta red, el servidor con una dirección IP de "192.168.1.10" ejecuta un servidor web en el puerto 80. Solo los otros dos equipos de esta red podrán acceder a ella (esto se conoce como intranet).

<figure><img src="../../../.gitbook/assets/Captura de pantalla_18-11-2024_0442_tryhackme.com.jpeg" alt="" width="506"><figcaption></figcaption></figure>

Si el administrador quisiera que el sitio web fuera accesible al público (utilizando Internet), tendría que implementar el reenvío de puertos, como se muestra en el siguiente diagrama:

<figure><img src="../../../.gitbook/assets/Captura de pantalla_18-11-2024_04447_tryhackme.com.jpeg" alt=""><figcaption></figcaption></figure>

Con este diseño, la red #2 ahora podrá acceder al servidor web que se ejecuta en la red #1 utilizando la dirección IP pública de la red #1 (82.62.51.70).

Es fácil confundir el reenvío de puertos con los comportamientos de un firewall (una tecnología de la que hablaremos más adelante). Sin embargo, en esta etapa, solo comprenda que el reenvío de puertos abre puertos específicos (recuerde cómo funcionan los paquetes). En comparación, los firewalls determinan si el tráfico puede viajar a través de estos puertos (incluso si estos puertos están abiertos por el reenvío de puertos).

El reenvío de puertos se configura en el router de una red.

#### _<mark style="color:purple;">Responda las siguientes preguntas</mark>_

1. ¿Cuál es el nombre del dispositivo que se utiliza para configurar el reenvío de puertos?  **`router`**

## <mark style="color:orange;">Cortafuegos 101</mark>

<figure><img src="https://tryhackme-images.s3.amazonaws.com/user-uploads/5de96d9ca744773ea7ef8c00/room-content/8dc0c3153b51b02f404128e8aef10059.svg" alt="" width="375"><figcaption></figcaption></figure>

Un firewall es un dispositivo dentro de una red responsable de determinar qué tráfico puede entrar y salir. Piense en un firewall como la seguridad fronteriza de una red. Un administrador puede configurar un firewall para **permitir** o **denegar** la entrada o salida del tráfico de una red en función de numerosos factores, como:

* ¿De dónde viene el tráfico? (¿Se le ha dicho al firewall que acepte/deniegue el tráfico de una red específica?)
* ¿Hacia dónde va el tráfico? (¿Se le ha dicho al firewall que acepte/deniegue el tráfico destinado a una red específica?)
* ¿Para qué puerto es el tráfico? (¿Se le ha dicho al firewall que acepte/deniegue el tráfico destinado solo al puerto 80?)
* ¿Qué protocolo está utilizando el tráfico? (¿Se le ha dicho al firewall que acepte/deniegue el tráfico que es UDP, TCP o ambos?)

Los firewalls realizan la inspección de paquetes para determinar las respuestas a estas preguntas.

Los firewalls vienen en todas las formas y tamaños. Desde piezas de hardware dedicadas (que a menudo se encuentran en grandes redes como empresas) que pueden manejar una gran cantidad de datos hasta enrutadores residenciales (¡como en su hogar!) o software como [Snort](https://www.snort.org/), los firewalls se pueden clasificar en 2 a 5 categorías.

En la siguiente tabla hablaremos de las dos categorías principales de cortafuegos:

<table data-header-hidden><thead><tr><th width="242"></th><th></th></tr></thead><tbody><tr><td>Cortafuegos Categoría</td><td>Descripción</td></tr><tr><td>Stateful</td><td><p>Este tipo de firewall utiliza toda la información de una conexión; En lugar de inspeccionar un paquete individual, este cortafuegos determina el comportamiento de un dispositivo en función de toda la conexión.</p><p>Este tipo de cortafuegos consume muchos recursos en comparación con los cortafuegos sin estado, ya que la toma de decisiones es dinámica. Por ejemplo, un firewall podría permitir las primeras partes de un protocolo de enlace TCP que luego fallarían.</p><p>Si una conexión de un host es mala, bloqueará todo el dispositivo.</p></td></tr><tr><td>Apátrida</td><td><p>Este tipo de firewall utiliza un conjunto estático de reglas para determinar si los paquetes individuales son aceptables o no. Por ejemplo, un dispositivo que envía un paquete incorrecto no significa necesariamente que todo el dispositivo esté bloqueado.</p><p>Aunque estos cortafuegos utilizan muchos menos recursos que las alternativas, son mucho más tontos. Por ejemplo, estos firewalls solo son efectivos como las reglas que se definen dentro de ellos. Si una regla no coincide exactamente, es efectivamente inútil.</p><p>Sin embargo, estos firewalls son excelentes cuando se reciben grandes cantidades de tráfico de un conjunto de hosts (como un ataque de denegación de servicio distribuido)</p></td></tr></tbody></table>

_<mark style="color:purple;">Responda las siguientes preguntas</mark>_

1. ¿En qué capas del modelo OSI operan los firewalls?  **`Layer 3, Layer 4`**
2. ¿Qué categoría de firewall inspecciona toda la conexión?  **`stateful`**
3. ¿Qué categoría de firewall inspecciona paquetes individuales?  **`stateless`**

## <mark style="color:orange;">Práctico - Cortafuegos</mark>

Implemente el sitio estático asociado a esta tarea. ¡Debe configurar correctamente el firewall para evitar que el dispositivo se sobrecargue para recibir la bandera!&#x20;

_<mark style="color:purple;">Responda las siguientes preguntas</mark>_

1. ¿Qué es la bandera?  **`THM{FIREWALLS_RULE}`**

## <mark style="color:orange;">Conceptos básicos de VPN</mark>

Un **P**rivate **N**etwork (o **VPN** para abreviar) es una tecnología que permite que los dispositivos en redes separadas se comuniquen de forma segura mediante la creación de una ruta dedicada entre sí a través de Internet (conocida como túnel). Los dispositivos conectados dentro de este túnel forman su propia red privada.

Por ejemplo, solo los dispositivos dentro de la misma red (como dentro de una empresa) pueden comunicarse directamente. Sin embargo, una VPN permite conectar dos oficinas. Tomemos el siguiente diagrama, donde hay tres redes:

<figure><img src="../../../.gitbook/assets/Captura de pantalla_18-11-2024_05124_tryhackme.com.jpeg" alt=""><figcaption></figcaption></figure>

1. Red #1 (Oficina #1)
2. Red #2 (Oficina #2)
3. Red #3 (Dos dispositivos conectados a través de una VPN)

Los dispositivos conectados en la Red #3 siguen siendo parte de la Red #1 y la Red #2, pero también se forman juntos para crear una red privada (Red #3) por la que solo los dispositivos que están conectados a través de esta VPN pueden comunicarse.

Vamos a cubrir algunos de los otros beneficios que ofrece una VPN en la siguiente tabla:

<table><thead><tr><th width="227">Beneficio</th><th>Descripción</th></tr></thead><tbody><tr><td>Permite conectar redes en diferentes ubicaciones geográficas.</td><td>Por ejemplo, una empresa con varias oficinas encontrará beneficiosas las VPN, ya que significa que se puede acceder a recursos como servidores/infraestructura desde otra oficina.</td></tr><tr><td>Ofrece privacidad.</td><td><p>La tecnología VPN utiliza el cifrado para proteger los datos. Esto significa que solo se puede entender entre los dispositivos desde los que se enviaba y a los que está destinado, lo que significa que los datos no son vulnerables al rastreo.</p><p>Este cifrado es útil en lugares con WiFi público, donde la red no proporciona cifrado. Puede usar una VPN para proteger su tráfico de ser visto por otras personas.</p></td></tr><tr><td>Ofrece anonimato.</td><td><p>Periodistas y activistas dependen de las VPN para informar de forma segura sobre temas globales en países donde la libertad de expresión está controlada.</p><p>Por lo general, su tráfico puede ser visto por su ISP y otros intermediarios y, por lo tanto, rastreado.</p><p>El nivel de anonimato que proporciona una VPN es tanto como la forma en que otros dispositivos en la red respetan la privacidad. Por ejemplo, una VPN que registra todos sus datos/historial es esencialmente lo mismo que no usar una VPN en este sentido.</p></td></tr></tbody></table>

¡TryHackMe usa una VPN para conectarlo a nuestras máquinas vulnerables sin que sean directamente accesibles en Internet! Esto significa que:

* Puede interactuar de forma segura con nuestras máquinas
* Los proveedores de servicios, como los ISP, no creen que esté atacando a otra máquina en Internet (lo que podría ir en contra de los términos de servicio)
* La VPN proporciona seguridad a TryHackMe, ya que no se puede acceder a las máquinas vulnerables a través de Internet.

La tecnología VPN ha mejorado a lo largo de los años. Exploremos algunas tecnologías VPN existentes a continuación:

<table data-header-hidden><thead><tr><th width="153"></th><th></th></tr></thead><tbody><tr><td>VPN Tecnología</td><td>Descripción</td></tr><tr><td>PPP</td><td><p>Esta tecnología es utilizada por PPTP (explicado a continuación) para permitir la autenticación y proporcionar cifrado de datos. Las VPN funcionan mediante el uso de una clave privada y un certificado público (similar a SSH). Una clave privada y un certificado deben coincidir para que pueda conectarse.</p><p>Esta tecnología no es capaz de salir de una red por sí misma (no enrutable).</p></td></tr><tr><td>PPTP</td><td><p>El Point-to-P oint Tunneling Protocol (PPTP) es la tecnología que permite que los datos de PPP viajen y salgan de una red.</p><p>PPTP es muy fácil de configurar y es compatible con la mayoría de los dispositivos. Sin embargo, está débilmente encriptado en comparación con las alternativas.</p></td></tr><tr><td>IPSec</td><td><p>El protocolo de seguridad de Internet (IPsec) encripta los datos utilizando el marco Internet Protocol (IP) existente.</p><p>IPSec es difícil de configurar en comparación con las alternativas; Sin embargo, si tiene éxito, cuenta con un cifrado sólido y también es compatible con muchos dispositivos.</p></td></tr></tbody></table>

_<mark style="color:purple;">Responda las siguientes preguntas</mark>_

1. ¿Qué tecnología VPN solo encripta y proporciona la autenticación de datos?  **`PPP`**
2. ¿Qué tecnología VPN utiliza el marco IP?  **`IPSec`**

## <mark style="color:orange;">Dispositivos de red LAN</mark>&#x20;

### <mark style="color:yellow;">¿Qué es un router?</mark>&#x20;

El trabajo de un router es conectar redes y pasar datos entre ellas. Lo hace mediante el uso de enrutamiento (¡de ahí el nombre de enrutador!).

El enrutamiento es la etiqueta que se le da al proceso de datos que viajan a través de las redes. El enrutamiento implica la creación de una ruta entre redes para que estos datos se puedan entregar con éxito. Los routers funcionan en la capa 3 del modelo OSI. A menudo cuentan con una interfaz interactiva (como un sitio web o una consola) que permite a un administrador configurar varias reglas, como el reenvío de puertos o el cortafuegos.

El enrutamiento es útil cuando los dispositivos están conectados por muchas rutas, como en el diagrama de ejemplo a continuación, donde se toma la ruta más óptima:

<figure><img src="../../../.gitbook/assets/Captura de pantalla_18-11-2024_05447_tryhackme.com.jpeg" alt=""><figcaption></figcaption></figure>

Los routers son dispositivos dedicados y no realizan las mismas funciones que los switches.

Podemos ver que la red de la computadora A está conectada a la red de la computadora B por dos enrutadores en el medio. La pregunta es: ¿qué camino se tomará? Diferentes protocolos decidirán qué camino se debe tomar, pero los factores incluyen:

* ¿Qué camino es el más corto?
* ¿Qué camino es el más fiable?
* ¿Qué camino tiene el medio más rápido (por ejemplo, cobre o fibra)?

### <mark style="color:yellow;">¿Qué es un interruptor?</mark>

Un conmutador es un dispositivo de red dedicado responsable de proporcionar un medio para conectarse a varios dispositivos. Los conmutadores pueden facilitar el uso de muchos dispositivos (de 3 a 63) mediante cables Ethernet.

Los switches pueden funcionar tanto en la capa 2 como en la capa 3 del modelo OSI. Sin embargo, estos son exclusivos en el sentido de que los switches de capa 2 no pueden funcionar en la capa 3.

Tomemos, por ejemplo, un interruptor de capa 2 en el diagrama a continuación. Estos switches reenviarán tramas (recuerde que ya no son paquetes, ya que se ha eliminado el protocolo IP) a los dispositivos conectados utilizando su dirección MAC.Los routers son dispositivos dedicados y no realizan las mismas funciones que los switches.

Podemos ver que la red de la computadora A está conectada a la red de la computadora B por dos enrutadores en el medio. La pregunta es: ¿qué camino se tomará? Diferentes protocolos decidirán qué camino se debe tomar, pero los factores incluyen:

* ¿Qué camino es el más corto?
* ¿Qué camino es el más fiable?
* ¿Qué camino tiene el medio más rápido (por ejemplo, cobre o fibra)?

### <mark style="color:yellow;">¿Qué es un interruptor?</mark>

Un conmutador es un dispositivo de red dedicado responsable de proporcionar un medio para conectarse a varios dispositivos. Los conmutadores pueden facilitar el uso de muchos dispositivos (de 3 a 63) mediante cables Ethernet.

Los switches pueden funcionar tanto en la capa 2 como en la capa 3 del modelo OSI. Sin embargo, estos son exclusivos en el sentido de que los switches de capa 2 no pueden funcionar en la capa 3.

Tomemos, por ejemplo, un interruptor de capa 2 en el diagrama a continuación. Estos switches reenviarán tramas (recuerde que ya no son paquetes, ya que se ha eliminado el protocolo IP) a los dispositivos conectados utilizando su dirección MAC.

<figure><img src="../../../.gitbook/assets/Captura de pantalla_18-11-2024_0576_tryhackme.com.jpeg" alt="" width="409"><figcaption></figcaption></figure>

Estos interruptores son los únicos responsables de enviar tramas al dispositivo correcto.

Ahora, pasemos a los interruptores de capa 3. Estos switches son más sofisticados que la capa 2, ya que pueden realizar _algunas_ de las responsabilidades de un router. Es decir, estos switches enviarán tramas a los dispositivos (como lo hace la capa 2) y enrutarán paquetes a otros dispositivos mediante el protocolo IP.

Echemos un vistazo al siguiente diagrama de un interruptor de capa 3 en acción. Podemos ver que hay dos direcciones IP:

* 192.168.1.1
* 192.168.2.1

Una tecnología llamada VLAN (Virtual Local Area Network) permite que dispositivos específicos dentro de una red se dividan virtualmente. Esta división significa que todos pueden beneficiarse de cosas como una conexión a Internet, pero se tratan por separado. Esta separación de red proporciona seguridad porque significa que las reglas establecidas determinan cómo se comunican entre sí dispositivos específicos. Esta segregación se ilustra en el siguiente diagrama:

<figure><img src="../../../.gitbook/assets/Captura de pantalla_18-11-2024_05810_tryhackme.com.jpeg" alt="" width="563"><figcaption></figcaption></figure>

En el contexto del diagrama anterior, el "Departamento de Ventas" y el "Departamento de Contabilidad" podrán acceder a Internet, pero no podrán comunicarse entre sí (aunque estén conectados al mismo interruptor).

_<mark style="color:purple;">Responda las siguientes preguntas</mark>_

1. ¿Cuál es el verbo de la acción que realiza un router?  **`routing`**
2. ¿Cuáles son las dos capas diferentes de interruptores? Separe estos con una coma, es decir: LayerX, LayerY   **`Layer2,Layer3`**

## <mark style="color:orange;">Práctico - Simulador de red</mark>

Implemente el sitio estático asociado a esta tarea. Y experimenta con el simulador de red. El simulador desglosará todos los pasos que debe dar un paquete para ir del punto a al b. Intente enviar un paquete TCP desde el equipo1 al equipo3 para revelar una marca.

**Nota**: Utilice el navegador Chrome o Firefox para completar este ejercicio práctico.

_<mark style="color:purple;">Responda las siguientes preguntas</mark>_

1. ¿Cuál es la bandera del simulador de red?  **`THM{YOU'VE_GOT_DATA}`**
2. ¿Cuántas entradas de HANDSHAKE hay en el registro de red?  **`5`**
