---
icon: layer-plus
description: >-
  Conozca el marco de trabajo de red fundamental que determina las distintas
  etapas en las que se manejan los datos a través de una red.
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

# Modelo OSI

{% embed url="https://www.youtube.com/watch?v=hWIktHvNjeM" %}

## <mark style="color:orange;">¿Qué es el modelo OSI?</mark>

<figure><img src="../../../.gitbook/assets/Captura de pantalla_17-11-2024_232739_tryhackme.com.jpeg" alt=""><figcaption></figcaption></figure>

El modelo OSI (o Open Systems Interconnection Model) es un modelo absolutamente fundamental utilizado en redes. Este modelo crítico proporciona un marco que dicta cómo todos los dispositivos en red enviarán, recibirán e interpretarán los datos.

Uno de los principales beneficios del modelo OSI es que los dispositivos pueden tener diferentes funciones y diseños en una red mientras se comunican con otros dispositivos. Los datos enviados a través de una red que sigue la uniformidad del modelo OSI pueden ser entendidos por otros dispositivos.

El modelo OSI consta de siete capas que se ilustran en el diagrama a continuación. Cada capa tiene un conjunto diferente de responsabilidades y se organiza desde la Capa 7 hasta la Capa 1.

En cada capa individual por la que viajan los datos, se llevan a cabo procesos específicos y se agregan piezas de información a estos datos, que es lo que discutiremos en las próximas tareas dentro de esta sala. Sin embargo, por ahora, solo necesitamos entender que este proceso se llama encapsulación y cómo se ve el modelo OSI en el siguiente diagrama:

<figure><img src="../../../.gitbook/assets/Captura de pantalla_17-11-2024_232931_tryhackme.com.jpeg" alt=""><figcaption></figcaption></figure>

#### _<mark style="color:purple;">Responda las siguientes preguntas</mark>_

1. ¿Qué significa "OSI" en "Modelo OSI"?  **`Open Systems Interconnection`**
2. ¿Cuántas capas (en dígitos) tiene el modelo OSI? **`7`**
3. ¿Cuál es el término clave para cuando se agregan piezas de información a los datos? **`encapsulation`**

## <mark style="color:orange;">Capa 1 - Físico</mark>

<figure><img src="https://tryhackme-images.s3.amazonaws.com/user-uploads/5de96d9ca744773ea7ef8c00/room-content/ea4ccad8729e69f69b866f8094faa711.svg" alt="" width="563"><figcaption></figcaption></figure>

Esta capa es una de las más fáciles de agarrar. En pocas palabras, esta capa hace referencia a los componentes físicos del hardware utilizado en las redes y es la capa más baja que encontrará. Los dispositivos utilizan señales eléctricas para transferir datos entre sí en un sistema de numeración binario (1 y 0).

Por ejemplo, los cables Ethernet que conectan dispositivos, como en la imagen a continuación:

<figure><img src="../../../.gitbook/assets/Captura de pantalla_17-11-2024_233210_tryhackme.com.jpeg" alt=""><figcaption></figcaption></figure>

#### _<mark style="color:purple;">Responda las siguientes preguntas</mark>_

1. ¿Cómo se llama esta capa? **`Physical`**
2. ¿Cómo se llama el sistema de numeración que es tanto 0 como 1? **`Binary`**
3. ¿Cómo se llaman los cables que se utilizan para conectar los dispositivos? **`Ethernet Cables`**

## <mark style="color:orange;">Capa 2 - Enlace de datos</mark>

<div align="center" data-full-width="true">

<img src="https://tryhackme-images.s3.amazonaws.com/user-uploads/5de96d9ca744773ea7ef8c00/room-content/e069ff061f0ab837c48e82a70cda2f1e.svg" alt="" width="563">

</div>

La capa de enlace de datos se centra en el direccionamiento físico de la transmisión. Recibe un paquete de la capa de red (incluida la dirección IP del equipo remoto) y agrega la dirección **MAC** física (Media Access Control) del punto final receptor. Dentro de cada computadora habilitada para la red hay una tarjeta **de**interfaz **de red (NIC**) que viene con una dirección MAC única para identificarla.

Las direcciones MAC son establecidas por el fabricante y literalmente grabadas en la tarjeta; No se pueden cambiar, aunque se pueden falsificar. Cuando la información se envía a través de una red, en realidad es la dirección física la que se utiliza para identificar dónde exactamente enviar la información.

Además, también es trabajo de la capa de enlace de datos presentar los datos en un formato adecuado para la transmisión.

#### _<mark style="color:purple;">Responda las siguientes preguntas</mark>_

1. ¿Cómo se llama esta capa? **`Data Link`**
2. ¿Cómo se llama la pieza de hardware con la que vienen todos los dispositivos en red?  **`Network Interface Card`**

## <mark style="color:orange;">Capa 3 - Red</mark>

<div align="center">

<img src="https://tryhackme-images.s3.amazonaws.com/user-uploads/5de96d9ca744773ea7ef8c00/room-content/b43ee29ba7634ee67fb641b95fb44d00.svg" alt="" width="563">

</div>

La tercera capa del modelo OSI (capa de red) es donde tiene lugar la magia del enrutamiento y el reensamblaje de datos (desde estos pequeños fragmentos hasta el trozo más grande). En primer lugar, el enrutamiento simplemente determina la ruta más óptima a la que se deben enviar estos fragmentos de datos.

Si bien algunos protocolos en esta capa determinan exactamente cuál es la ruta "óptima" que deben tomar los datos para llegar a un dispositivo, solo deberíamos saber sobre su existencia en esta etapa del módulo de red. En resumen, estos protocolos incluyen OSPF (Open Shortest Path Ffirst) y RIP (Routing Information Protocol). Los factores que deciden qué ruta se toma se deciden por lo siguiente:

* ¿Cuál es el camino más corto? Es decir, tiene la menor cantidad de dispositivos por los que el paquete necesita viajar.
* ¿Qué camino es el más fiable? Es decir, ¿se han perdido paquetes en esa ruta antes?
* ¿Qué ruta tiene la conexión física más rápida? Es decir, ¿hay un camino que utiliza una conexión de cobre (más lenta) o una fibra (considerablemente más rápida)?

En esta capa, todo se trata a través de direcciones IP como 192.168.1.100. Los dispositivos como los routers capaces de entregar paquetes mediante direcciones IP se conocen como dispositivos de capa 3, porque son capaces de trabajar en la tercera capa del modelo OSI.

<figure><img src="../../../.gitbook/assets/Captura de pantalla_17-11-2024_233741_tryhackme.com.jpeg" alt="" width="563"><figcaption></figcaption></figure>

#### _<mark style="color:purple;">Responda las siguientes preguntas</mark>_

1. ¿Cómo se llama esta capa?  **`Network`**
2. ¿Los paquetes tomarán la ruta más óptima a través de una red? (S/N)  **`Y`**
3. ¿Qué significa el acrónimo "OSPF"?  **`Open Shortest Path First`**
4. ¿Qué significa el acrónimo "RIP"?  **`Routing Information Protocol`**
5. ¿Qué tipo de direcciones se tratan en esta capa?  **`IP Addresses`**

## <mark style="color:orange;">Capa 4 - Transporte</mark>

![](https://tryhackme-images.s3.amazonaws.com/user-uploads/5de96d9ca744773ea7ef8c00/room-content/4d2048a25276f3b764578c8245d4392f.svg)

La capa 4 del modelo OSI desempeña un papel vital en la transmisión de datos a través de una red y puede ser un poco difícil de entender. Cuando los datos se envían entre dispositivos, se sigue uno de dos protocolos diferentes que se deciden en función de varios factores:

* TCP
* UDP

Comencemos con TCP. La Transmission Control Protocol (TCP). Potencialmente insinuado por el nombre, este protocolo está diseñado teniendo en cuenta la fiabilidad y la garantía. Este protocolo reserva una conexión constante entre los dos dispositivos durante la cantidad de tiempo que tardan los datos en enviarse y recibirse.

No solo esto, sino que TCP incorpora la comprobación de errores en su diseño. La comprobación de errores es la forma en que TCP puede garantizar que los datos enviados desde los fragmentos pequeños de la capa de sesión (capa 5) se hayan recibido y vuelto a ensamblar en el mismo orden.

Vamos a resumir las ventajas y desventajas de TCP en la siguiente tabla:

|                                  <p>Ventajas de TCP<br></p>                                  | <p>Desventajas de TCP<br></p>                                                                                                                                          |
| :------------------------------------------------------------------------------------------: | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
|                        <p>Garantiza la exactitud de los datos.<br></p>                       | <p>Requiere una conexión confiable entre los dos dispositivos. Si no se recibe un pequeño fragmento de datos, no se puede utilizar todo el fragmento de datos.<br></p> |
| <p>Capaz de sincronizar dos dispositivos para evitar que el otro se inunde de datos.<br></p> | <p>Una conexión lenta puede generar un cuello de botella en otro dispositivo, ya que la conexión estará reservada en la computadora receptora todo el tiempo.<br></p>  |
|               <p>Realiza muchos más procesos para mayor confiabilidad.<br></p>               | <p>TCP es significativamente más lento que UDP porque los dispositivos que utilizan este protocolo deben realizar más trabajo.<br></p>                                 |

\
TCP se utiliza para situaciones como el intercambio de archivos, la navegación por Internet o el envío de un correo electrónico. Este uso se debe a que estos servicios requieren que los datos sean precisos y completos (¡no sirve de nada tener la mitad de un archivo!).

En el siguiente diagrama, podemos ver cómo una imagen de un gato se descompone en pequeños fragmentos de datos (conocidos como paquetes) desde el "servidor web", donde la "computadora" reconstruye la imagen del gato en el orden correcto.

\
