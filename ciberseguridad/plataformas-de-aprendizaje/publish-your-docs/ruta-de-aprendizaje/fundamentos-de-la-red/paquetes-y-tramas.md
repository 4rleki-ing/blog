---
icon: network-wired
description: >-
  Comprenda cómo se dividen los datos en partes más pequeñas y se transmiten a
  través de una red a otro dispositivo
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

# Paquetes y Tramas

{% embed url="https://www.youtube.com/watch?v=vzcLrE0SfiQ" %}

## <mark style="color:orange;">¿Qué son los paquetes y las tramas?</mark>

Los paquetes y las tramas son pequeñas piezas de datos que, al formarse juntas, forman una pieza más grande de información o mensaje. Sin embargo, son dos cosas diferentes en el modelo OSI. Un marco se encuentra en la capa 2, la capa de enlace de datos, lo que significa que no hay información como direcciones IP. Piense en esto como poner un sobre dentro de otro y enviarlo. El primer sobre será el paquete que envíe por correo, pero una vez que se abre, el sobre que contiene todavía existe y contiene datos (esto es un marco).

A este proceso se le llama encapsulación y del que hablamos en [la sala 3: el modelo OSI](https://tryhackme.com/room/osimodelzi). En esta etapa, es seguro asumir que cuando hablamos de cualquier cosa de direcciones IP, estamos hablando de paquetes. Cuando se elimina la información que la encapsula, estamos hablando del marco en sí.

Los paquetes son una forma eficiente de comunicar datos a través de dispositivos en red, como los que se explican en la Tarea 1. Debido a que estos datos se intercambian en partes pequeñas, hay menos posibilidades de que se produzcan cuellos de botella en una red que los mensajes grandes que se envían a la vez.

Por ejemplo, al cargar una imagen de un sitio web, esta imagen no se envía a su computadora en su conjunto, sino más bien pequeñas partes donde se reconstruye en su computadora. Tome la imagen a continuación como una ilustración de este proceso. La imagen del gato se divide en tres paquetes, donde se reconstruye cuando llega al ordenador para formar la imagen final.

<figure><img src="../../../../../.gitbook/assets/Captura de pantalla_18-11-2024_0649_tryhackme.com.jpeg" alt=""><figcaption></figcaption></figure>

Los paquetes tienen diferentes estructuras que dependen del tipo de paquete que se envía. Como veremos más adelante, las redes están llenas de estándares y protocolos que actúan como un conjunto de reglas sobre cómo se maneja el paquete en un dispositivo. Con miles de millones de dispositivos conectados a Internet, las cosas pueden colapsar rápidamente si no hay estandarización

Sigamos con nuestro ejemplo del Protocolo de Internet. Un paquete que usa este protocolo tendrá un conjunto de encabezados que contienen información adicional a los datos que se envían a través de una red.

Algunos encabezados notables incluyen:

| Encabezado           | Descripción                                                                                                                                                                      |
| -------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Tiempo de vida       | Este campo establece un temporizador de caducidad para que el paquete no obstruya su red si nunca logra llegar a un host o escapar.                                              |
| Checksum             | Este campo proporciona comprobación de integridad para protocolos como TCP/IP. Si se cambia algún dato, este valor será diferente de lo esperado y, por lo tanto, estará dañado. |
| Dirección de origen  | La dirección IP del dispositivo desde el que se envía el paquete para que los datos sepan a dónde regresar.                                                                      |
| Dirección de destino | La dirección IP del dispositivo a la que se envía el paquete para que los datos sepan a dónde viajar a continuación.                                                             |

#### _<mark style="color:purple;">Responda las siguientes preguntas</mark>_

1. ¿Cómo se llama un dato cuando tiene información de direccionamiento IP?  **`Packet`**
2. ¿Cómo se llama un dato cuando no tiene información de direccionamiento IP?  **`Frame`**

## <mark style="color:orange;">TCP/IP (el protocolo de enlace de tres vías)</mark>

**TCP** (o **T**ransmission **C**ontrol **P**rotocol para abreviar) es otra de estas reglas utilizadas en las redes.

Este protocolo es muy similar al modelo OSI que hemos comentado anteriormente en la sala tres de este módulo hasta ahora. El protocolo TCP/IP consta de cuatro capas y podría decirse que es solo una versión resumida del modelo OSI. Estas capas son:

* Aplicación
* Transporte
* Internet
* Interfaz de red

De manera muy similar a cómo funciona el modelo OSI, la información se agrega a cada capa del modelo TCP a medida que el fragmento de datos (o paquete) lo atraviesa. Como recordarás, este proceso se conoce como encapsulación, donde el reverso de este proceso es la desencapsulación.

Una característica definitoria de TCP es que se **basa en la conexión**, lo que significa que TCP debe establecer una conexión entre un cliente y un dispositivo que actúa como servidor **antes** de que se envíen los datos.

Debido a esto, TCP garantiza que cualquier dato enviado se recibirá en el otro extremo. Este proceso se denomina apretón de manos de tres vías, que es algo de lo que hablaremos en breve. A continuación se muestra una tabla que compara las ventajas y desventajas de TCP:

| Ventajas de TCP                                                                                          | Desventajas de TCP                                                                                                                                                                    |
| -------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Garantiza la integridad de los datos.                                                                    | Requiere una conexión confiable entre los dos dispositivos. Si no se recibe un pequeño fragmento de datos, no se puede utilizar todo el fragmento de datos y se debe volver a enviar. |
| Capaz de sincronizar dos dispositivos para evitar que el otro se inunde de datos en el orden incorrecto. | Una conexión lenta puede generar un cuello de botella en otro dispositivo, ya que la conexión estará reservada en el otro dispositivo todo el tiempo.                                 |
| Realiza muchos más procesos para mayor confiabilidad                                                     | TCP es significativamente más lento que UDP porque los dispositivos que utilizan este protocolo deben realizar más trabajo (computación).                                             |

Los paquetes TCP contienen varias secciones de información conocidas como encabezados que se agregan desde la encapsulación. Expliquemos algunos de los encabezados cruciales en la siguiente tabla:

| Encabezado                | Descripción                                                                                                                                                                                                                                             |
| ------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Puerto de origen          | Este valor es el puerto abierto por el remitente para enviar el paquete TCP. Este valor se elige aleatoriamente (de los puertos de 0 a 65535 que aún no están en uso en ese momento).                                                                   |
| Puerto de destino         | Este valor es el número de puerto que se ejecuta una aplicación o servicio en el host remoto (el que recibe los datos); Por ejemplo, un servidor web que se ejecuta en el puerto 80. A diferencia del puerto de origen, este valor no se elige al azar. |
| IP de origen              | Esta es la dirección IP del dispositivo que envía el paquete.                                                                                                                                                                                           |
| IP de destino             | Esta es la dirección IP del dispositivo al que está destinado el paquete.                                                                                                                                                                               |
| Número de secuencia       | Cuando se produce una conexión, al primer dato transmitido se le asigna un número aleatorio. Explicaremos esto más a fondo más adelante.                                                                                                                |
| Número de acuse de recibo | Después de que a un dato se le haya asignado un número de secuencia, el número del siguiente dato tendrá el número de secuencia + 1. También explicaremos esto más a fondo más adelante.                                                                |
| Checksum                  | Este valor es lo que le da integridad a TCP. Se realiza un cálculo matemático donde se recuerda la salida. Cuando el dispositivo receptor realiza el cálculo matemático, los datos deben estar dañados si la salida es diferente de la que se envió.    |
| Datos                     | Este encabezado es donde se almacenan los datos, es decir, los bytes de un archivo que se está transmitiendo.                                                                                                                                           |
| Bandera                   | Este encabezado determina cómo cualquiera de los dispositivos debe manejar el paquete durante el proceso de protocolo de enlace. Las banderas específicas determinarán comportamientos específicos, que es lo que explicaremos a continuación.          |

A continuación, hablaremos del _apretón de manos de tres vías,_ el término que se le da al proceso utilizado para establecer una conexión entre dos dispositivos. El protocolo de enlace de tres vías se comunica mediante algunos mensajes especiales: la siguiente tabla destaca los principales:

| Paso | Mensaje | Descripción                                                                                                                                                                                                                                                   |
| ---- | ------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 1    | SYN     | Un mensaje SYN es el paquete inicial enviado por un cliente durante el protocolo de enlace. Este paquete se utiliza para iniciar una conexión y sincronizar los dos dispositivos juntos (explicaremos esto más adelante).                                     |
| 2    | SYN/ACK | Este paquete es enviado por el dispositivo receptor (servidor) para reconocer el intento de sincronización del cliente.                                                                                                                                       |
| 3    | ACK     | El cliente o el servidor pueden utilizar el paquete de reconocimiento para confirmar que una serie de mensajes/paquetes se han recibido correctamente.                                                                                                        |
| 4    | DATOS   | Una vez que se ha establecido una conexión, los datos (como los bytes de un archivo) se envían a través del mensaje "DATA".                                                                                                                                   |
| 5    | ALETA   | Este paquete se utiliza para cerrar _limpiamente (correctamente)_ la conexión después de que se haya completado.                                                                                                                                              |
| #    | RST     | Este paquete finaliza abruptamente toda comunicación. Este es el último recurso e indica que hubo algún problema durante el proceso. Por ejemplo, si el servicio o la aplicación no funciona correctamente, o si el sistema tiene fallos como pocos recursos. |

El siguiente diagrama muestra un proceso normal de apretón de manos de tres vías entre Alice y Bob. En la vida real, esto sería entre dos dispositivos.

<figure><img src="../../../../../.gitbook/assets/Captura de pantalla_18-11-2024_01058_tryhackme.com.jpeg" alt="" width="563"><figcaption></figcaption></figure>

A los datos enviados se les asigna una secuencia numérica aleatoria y se reconstruyen utilizando esta secuencia numérica y aumentando en 1. Ambas computadoras deben coincidir en la misma secuencia numérica para que los datos se envíen en el orden correcto. Este pedido se acuerda a través de tres etapas:

1. SYN - Cliente: Aquí está mi número de secuencia inicial (ISN) para cronise SYNcon (0)
2. SYN/ACK - Servidor: Aquí está mi número de secuencia inicial (ISN) para cronise SYN(5,000), y ahora confirmosu secuencia numérica inicial (0)
3. ACK - Cliente: Ahora ACKsu Número de Secuencia Inicial (ISN) de (5,000), aquí hay algunos datos que es mi ISN+1 (0 + 1)

| <p>Dispositivo<br></p>         | <p>Secuencia numérica inicial (ISN)<br></p> | <p>Secuencia<br>numérica final</p> |
| ------------------------------ | ------------------------------------------- | ---------------------------------- |
| <p>Cliente (remitente)<br></p> | 0                                           |    0 + 1 = 1                       |
| <p>Cliente (remitente)<br></p> | 1                                           | <p>    1 + 1 = 2<br></p>           |
| <p>Cliente (remitente)<br></p> | 2                                           |      2 + 1 = 3                     |

### <mark style="color:yellow;">TCP Cierre de una conexión:</mark>

Expliquemos rápidamente el proceso detrás del cierre de una conexión por TCP. En primer lugar, TCP cerrará una conexión una vez que un dispositivo haya determinado que el otro dispositivo ha recibido correctamente todos los datos.

Dado que TCP reserva recursos del sistema en un dispositivo, se recomienda cerrar las conexiones TCP lo antes posible.

Para iniciar el cierre de una conexión TCP, el dispositivo enviará un paquete "FIN" al otro dispositivo. Por supuesto, con TCP, el otro dispositivo también tendrá que reconocer este paquete.

Vamos a mostrar este proceso usando a Alice y Bob como lo hemos hecho anteriormente.

<figure><img src="../../../../../.gitbook/assets/Captura de pantalla_18-11-2024_01226_tryhackme.com.jpeg" alt="" width="563"><figcaption></figcaption></figure>

En la ilustración, podemos ver que Alice le ha enviado a Bob un paquete "FIN". Debido a que Bob recibió esto, le hará saber a Alice que lo recibió y que también quiere cerrar la conexión (usando FIN). Alice ha escuchado a Bob alto y claro y le hará saber a Bob que lo reconoce.

#### _<mark style="color:purple;">Responda las siguientes preguntas</mark>_

1. ¿Cuál es el encabezado de un paquete TCP que garantiza la integridad de los datos?  **`checksum`**
2. Proporcione el orden de un protocolo de enlace triple normal (con cada paso separado por una coma)  **`SYN,SYN/ACK,ACK`**

## <mark style="color:orange;">Práctico - Apretón de manosVer sitio</mark>

Ayude a Alice y Bob a comunicarse volviendo a ensamblar el protocolo de enlace TCP en el orden correcto en el laboratorio estático adjunto a esta tarea.

Ingrese el valor de la bandera que se da al final de la conversación en la pregunta a continuación.

#### _<mark style="color:purple;">Responda las siguientes preguntas</mark>_

1. ¿Cuál es el valor de la bandera que se da al final de la conversación?  **`THM{TCP_CHATTER}`**

## <mark style="color:orange;">UDP/IP</mark>

El atagrama **U**ser **D**P rotocol (**UDP**) es otro protocolo que se utiliza para comunicar datos entre dispositivos.

A diferencia de su hermano TCP, UDP es un protocolo **sin estado** que no requiere una conexión constante entre los dos dispositivos para que se envíen los datos. Por ejemplo, no se produce el protocolo de enlace de tres vías ni hay ninguna sincronización entre los dos dispositivos.

Recordemos algunas de las comparaciones que se hicieron sobre estos dos protocolos en la Sala 3: "Modelo OSI". Es decir, UDP se utiliza en situaciones en las que las aplicaciones pueden tolerar la pérdida de datos (como la transmisión de vídeo o el chat de voz) o en escenarios en los que una conexión inestable no es el fin de todo. A continuación se muestra una tabla que compara las ventajas y desventajas de UDP:

| Ventajas de UDP                                                                                                                  | Desventajas de UDP                                                                                 |
| -------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------- |
| UDP es mucho más rápido que TCP.                                                                                                 | A UDP no le importa si los datos se reciben o no.                                                  |
| UDP deja que la aplicación (software de usuario) decida si hay algún control sobre la rapidez con la que se envían los paquetes. | Es bastante flexible para los desarrolladores de software en este sentido.                         |
| UDP no reserva una conexión continua en un dispositivo como lo hace TCP.                                                         | Esto significa que las conexiones inestables resultan en una experiencia terrible para el usuario. |

Como se mencionó, no se lleva a cabo ningún proceso para establecer una conexión entre dos dispositivos. Lo que significa que no hay que tener en cuenta si se reciben o no los datos, y no hay salvaguardas como las que ofrece TCP, como la integridad de los datos.

Los paquetes UDP son mucho más simples que los paquetes TCP y tienen menos encabezados. Sin embargo, ambos protocolos comparten algunos encabezados estándar, que son los que se anotan en la tabla a continuación:

| Encabezado                      | Descripción                                                                                                                                                                                                                                                     |
| ------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <p>Tiempo de vida (TTL)<br></p> | <p>Este campo establece un temporizador de caducidad para el paquete, por lo que no obstruye su red si nunca logra llegar a un host o escapar.<br></p>                                                                                                          |
| Dirección de origen             | La dirección IP del dispositivo desde el que se envía el paquete, para que los datos sepan a dónde regresar.                                                                                                                                                    |
| Dirección de destino            | La dirección IP del dispositivo a la que se envía el paquete para que los datos sepan a dónde viajar a continuación.                                                                                                                                            |
| Puerto de origen                | Este valor es el puerto que abre el remitente para enviar el paquete UDP. Este valor se elige aleatoriamente (de los puertos de 0 a 65535 que aún no están en uso en ese momento).                                                                              |
| Puerto de destino               | Este valor es el número de puerto que se está ejecutando una aplicación o servicio en el host remoto (el que recibe los datos); Por ejemplo, un servidor web que se ejecuta en el puerto 80. A diferencia del puerto de origen, este valor no se elige al azar. |
| Datos                           | Este encabezado es donde se almacenan los datos, es decir, los bytes de un archivo que se está transmitiendo.                                                                                                                                                   |

A continuación, discutiremos cómo el proceso de una conexión a través de UDP difiere del de algo como TCP. Debemos recordar que el UDP es apátrida. No se envía ninguna confirmación durante una conexión.

El siguiente diagrama muestra una conexión UDP normal entre Alice y Bob. En la vida real, esto sería entre dos dispositivos.

<figure><img src="../../../../../.gitbook/assets/Captura de pantalla_18-11-2024_01612_tryhackme.com.jpeg" alt="" width="563"><figcaption></figcaption></figure>

#### _<mark style="color:purple;">Responda las siguientes preguntas</mark>_

1. ¿Qué significa el término "UDP"?  **`User Datagram Protocol`**
2. ¿Qué tipo de conexión es "UDP"?  **`stateless`**
3. ¿Qué protocolo usarías para transferir un archivo?  **`TCP`**
4. ¿Qué protocolo usarías para tener una videollamada?  **`UDP`**

## <mark style="color:orange;">Puertos 101 (Práctico)</mark>

Quizás acertadamente titulados por su nombre, los puertos son un punto esencial en el que se pueden intercambiar datos. Piensa en un puerto y un puerto. Los buques que deseen atracar en el puerto deberán dirigirse a un puerto compatible con las dimensiones y las instalaciones ubicadas en el buque. Cuando el barco se alinee, se conectará a un **puerto** en el puerto. Tomemos, por ejemplo, que un crucero no puede atracar en un puerto hecho para un barco pesquero y viceversa.

Estos puertos imponen lo que puede estacionar y dónde: si no es compatible, no puede estacionarse aquí. Los dispositivos de red también utilizan puertos para aplicar reglas estrictas cuando se comunican entre sí. Cuando se ha establecido una conexión (recuperando desde la sala del modelo OSI), cualquier dato enviado o recibido por un dispositivo se enviará a través de estos puertos. En informática, los puertos son un valor numérico entre **0** y **65535** (65,535).

Debido a que los puertos pueden oscilar entre 0 y 65535, rápidamente se corre el riesgo de perder el rastro de qué aplicación está usando qué puerto. ¡Un puerto concurrido es un caos! Afortunadamente, asociamos las aplicaciones, el software y los comportamientos con un conjunto estándar de reglas. Por ejemplo, al imponer que los datos del navegador web se envíen a través del puerto 80, los desarrolladores de software pueden diseñar un navegador web como Google Chrome o Firefox para interpretar los datos de la misma manera que los demás.

Esto significa que todos los navegadores web ahora comparten una regla común: los datos se envían a través del puerto 80. El aspecto, la sensación y la facilidad de uso de los navegadores depende del diseñador o de la decisión del usuario.

Si bien la regla estándar para los datos web es el _puerto 80_, a algunos otros protocolos se les ha asignado una regla estándar. Cualquier puerto que esté entre **0** y **1024** (1.024) se conoce como puerto común. Exploremos algunos de estos otros protocolos a continuación:

| Protocolo                                  | Número de puerto | Descripción                                                                                                                                                                                |
| ------------------------------------------ | ---------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| File Transfer Protocol (FTP)               | 21               | Este protocolo es utilizado por una aplicación de intercambio de archivos basada en un modelo cliente-servidor, lo que significa que puede descargar archivos desde una ubicación central. |
| Secure Shell (SSH)                         | 22               | Este protocolo se utiliza para iniciar sesión de forma segura en los sistemas a través de una interfaz basada en texto para la administración.                                             |
| HyperText Transfer Protocol (HTTP)         | 80               | ¡Este protocolo impulsa la World Wide Web (WWW)! Su navegador utiliza esto para descargar texto, imágenes y videos de páginas web.                                                         |
| HyperText Transfer Protocol Secure (HTTPS) | 443              | Este protocolo hace exactamente lo mismo que el anterior; sin embargo, de forma segura mediante el cifrado.                                                                                |
| Server Message Block (SMB)                 | 445              | Este protocolo es similar al Protocolo de Transferencia de Archivos (FTP); sin embargo, además de archivos, SMB le permite compartir dispositivos como impresoras.                         |
| Remote Desktop Protocol (RDP)              | 3389             | Este protocolo es un medio seguro de iniciar sesión en un sistema mediante una interfaz de escritorio visual (a diferencia de las limitaciones basadas en texto del protocolo SSH).        |

Solo hemos cubierto brevemente los protocolos más comunes en ciberseguridad. Puede [encontrar una tabla de los 1024 puertos comunes enumerados](http://www.vmaxx.net/techinfo/ports.htm) para obtener más información.

Lo que vale la pena señalar aquí es que estos protocolos solo siguen los estándares. Es decir, puede administrar aplicaciones que interactúan con estos protocolos en un puerto diferente al estándar (ejecutando un servidor web en el puerto estándar 8080 en lugar del puerto estándar 80). Tenga en cuenta, sin embargo, que las aplicaciones supondrán que se está siguiendo el estándar, por lo que deberá proporcionar dos puntos (:) junto con el número de puerto.

#### <mark style="color:yellow;">Desafío práctico:</mark>

Abra el sitio adjunto a esta tarea y conéctese a la dirección IP "8.8.8.8" en el puerto "1234", y recibirá una bandera.

#### _<mark style="color:purple;">Responda las siguientes preguntas</mark>_

1. ¿Cuál es la bandera recibida del desafío?  **`THM{YOU_CONNECTED_TO_A_PORT}`**

## <mark style="color:orange;">Continúe su aprendizaje: Amplíe su red</mark>

Únete a la última sala de este módulo de networking: "[Extendiendo tu red](https://tryhackme.com/room/extendingyournetwork)", para continuar tu aprendizaje y completar este módulo.

#### _<mark style="color:purple;">Responda las siguientes preguntas</mark>_

1. Finalice el laboratorio de sitio estático implementado en las tareas 3 y 5.
2. Únete a la [sala "Extendiendo tu red"](https://tryhackme.com/room/extendingyournetwork) para continuar tu aprendizaje.
