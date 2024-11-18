---
description: >-
  La guía oficial del proyecto Nmap para el descubrimiento de redes y el escaneo
  de seguridad.
icon: mobile-signal
cover: ../../../../../.gitbook/assets/NMAP.jpg
coverY: -10.841930116472545
layout:
  cover:
    visible: true
    size: full
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

# Nmap

Nmap se convirtió en la red más popular del mundo escáner de seguridad, con millones de usuarios de todo el mundo. A lo largo de los años, Nmap ha seguido añadiendo como la detección remota del sistema operativo, la detección de versiones/servicios, y el motor de secuencias de comandos Nmap. Ahora es compatible con los principales sistemas operativos Unix, Windows y Mac Plataformas con consola e interfaces gráficas. Publicaciones como _Linux Journal_, _Info World_, _LinuxQuestions.Org_ y _Codetalker Digest_ han reconocido a Nmap como "herramienta de seguridad del año".

Nmap ("Network Mapper") es una utilidad gratuita y de código abierto para Exploración de redes y auditoría de seguridad. Muchos sistemas y redes Los administradores también lo encuentran útil para tareas como la red inventario, la administración de programas de actualización de servicio y la supervisión del host o Tiempo de actividad del servicio. Nmap utiliza paquetes IP sin procesar de formas novedosas para determinar qué hosts están disponibles en la red, qué servicios (aplicación nombre y versión) que ofrecen esos hosts, qué sistemas operativos (y versiones del sistema operativo) que se están ejecutando, qué tipo de paquete Se utilizan filtros/cortafuegos, y docenas de otras características. Eso fue diseñado para escanear rápidamente grandes redes, pero funciona bien contra Anfitriones individuales.

Si bien Nmap es extremadamente poderoso, también es complejo. Más que 100 opciones de línea de comandos añaden expresividad para los gurús de las redes, pero puede confundir a los novatos. Algunas de sus opciones ni siquiera lo han sido documentado. Este libro documenta todas las características de Nmap y, más Y lo que es más importante, enseña las formas más efectivas de usarlos. Cuenta con tardó casi cuatro años en escribirse, con una actualización constante a medida que Nmap Evolucionado.

La página web de Nmap en [`https://nmap.org`](https://nmap.org/) no es solo para descargas. También proporciona documentación sustancial de los desarrolladores de Nmap y terceros.

Este libro asume una familiaridad básica con TCP/IP y Conceptos de redes.

<figure><img src="../../../../../.gitbook/assets/image (6).png" alt=""><figcaption><p>Figura 1. Encabezado IPv4</p></figcaption></figure>

<figure><img src="../../../../../.gitbook/assets/image (8).png" alt=""><figcaption><p>Figura 2. Encabezado TCP</p></figcaption></figure>

<figure><img src="../../../../../.gitbook/assets/image (9).png" alt=""><figcaption><p>Figura 3. Encabezado UDP</p></figcaption></figure>

<figure><img src="../../../../../.gitbook/assets/image (10).png" alt=""><figcaption><p>Figura 4. Encabezado ICMP</p></figcaption></figure>

## <mark style="color:orange;">Capítulo 1. Primeros pasos con Nmap</mark>

Nmap ("Network Mapper") es una utilidad gratuita y de código abierto para Exploración de redes y auditoría de seguridad. Muchos sistemas y redes Los administradores también lo encuentran útil para tareas como la red inventario, la administración de programas de actualización de servicio y la supervisión del host o Tiempo de actividad del servicio. Nmap utiliza paquetes IP sin procesar de formas novedosas para determinar qué hosts están disponibles en la red, qué servicios (aplicación nombre y versión) que ofrecen esos hosts, qué sistemas operativos (y versiones del sistema operativo) que se están ejecutando, qué tipo de paquete Se utilizan filtros/cortafuegos, y docenas de otras características. Eso fue diseñado para escanear rápidamente grandes redes, pero funciona bien contra Anfitriones individuales. Nmap se ejecuta en todos los principales sistemas operativos de computadoras, y Están disponibles tanto la versión de consola como la gráfica.

El primer paso en una evaluación de vulnerabilidades es la red descubrimiento. Esta etapa de reconocimiento determina qué dirección IP rangos que está utilizando el objetivo, qué hosts están disponibles, qué servicios que ofrecen esos hosts, detalles generales de la topología de la red y qué Las políticas de firewall/filtrado están en vigor.

### <mark style="color:blue;">Las fases de un escaneo Nmap</mark>

Los escaneos se realizan en fases, con cada fase termina antes de que comience la siguiente. Como se puede ver en las descripciones de las fases a continuación, hay mucho más en Nmap que solo el puerto Escaneo.

<mark style="color:green;">**Script Pre-escaneo**</mark>**.** El motor de secuencias de comandos _**Nmap (NSE)**_ utiliza un colección de scripts de propósito especial para obtener más información sobre sistemas remotos. **NSE** no se ejecuta a menos que lo solicite con opciones como **`--script`** o **`-sC`**, y La fase de pre-escaneo solo ocurre cuando los scripts que lo necesitan son seleccionado. Esta fase es para scripts que solo deben ejecutarse una vez por ejecución de Nmap en lugar de ejecutarse por separado contra individuos Objetivos.&#x20;

<mark style="color:green;">**Enumeración de Objetivos**</mark>**.** En esta fase, Nmap investiga el host proporcionado por el usuario, que pueden ser una combinación de (_host_, _Nombres DNS_, _direcciones IP_, notaciones de red CIDR y mucho más). Esta fase no se puede omitir ya que es esencial para el escaneo posterior, pero puede simplificar el procesamiento pasando solo direcciones IP para que Nmap no tenga que reenviar resolución.

<mark style="color:green;">**Detección de host**</mark>**.** Los análisis de red suelen comenzar descubriendo qué objetivos de la red están en línea y, por lo tanto, vale la pena una investigación más profunda. Este proceso se denomina _detección de host_ o _ping escaneo_. Nmap ofrece muchas técnicas de descubrimiento de hosts, que van desde solicitudes rápidas de ARP hasta combinaciones elaboradas de TCP, ICMP y otros tipos de sondas.

<mark style="color:green;">**Resolución de DNS inverso**</mark>**.** Una vez que Nmap ha terminado el escaneo, busca los nombres de DNS inverso de todos los hosts encontrados en línea por el escaneo de ping. A veces, el nombre de un host proporciona pistas sobre su función y los nombres hacen que los informes sean más legibles que proporcionar solo IP Números.

**Puerto Escaneo.** Esta es la operación principal de Nmap. Se envían sondeos y las respuestas (o no respuestas) a esas sondas se utilizan para clasificar los puertos remotos en estados tales como , , o. Esa breve descripción no comienza para abarcar los muchos tipos de escaneo de Nmap, la configurabilidad de los escaneos y algoritmos para mejorar la velocidad y la precisión. Una visión general del puerto se encuentra en [el Capítulo 4](https://nmap.org/book/port-scanning.html). Información detallada sobre algoritmos y opciones de línea de comandos se encuentran en [el Capítulo 5](https://nmap.org/book/scan-methods.html). Puerto El escaneo se realiza de forma predeterminada, aunque puede omitirlo con la opción y aún así realizar algunos de los seguimientos posteriores y el motor de scripting Nmap parcial fases especificando sus opciones particulares de línea de comandos (tales como y ).`openclosedfiltered-sn--traceroute--script`

**Versión detección.** Si se encuentra algún puerto abierto, Nmap puede ser capaz de determinar qué software de servidor se está ejecutando en el sistema remoto. Lo hace enviando una variedad de sondas a los puertos abiertos y comparando las respuestas con una base de datos de miles de más de 6.500 Firmas de servicio. La detección de versiones se habilita con la opción y se describe en detalle en el [Capítulo 7](https://nmap.org/book/vscan.html).`-sV`

**SISTEMA OPERATIVO detección.** Si se solicita con la opción, Nmap procede a la detección del sistema operativo. Diferentes sistemas operativos implementan estándares de red de maneras sutilmente diferentes. Al medir estas diferencias, a menudo se Es posible determinar el sistema operativo que se ejecuta en un host remoto. Nmapa compara las respuestas a un conjunto estándar de sondeos con una base de datos de Más de mil respuestas conocidas del sistema operativo. La detección del sistema operativo se trata en el [Capítulo 8](https://nmap.org/book/osdetect.html).`-O`

**Traceroute.** Nmap contiene una implementación de traceroute optimizada, habilitada por la opción. Puede encontrar las rutas de red para muchos hosts en paralelo, utilizando los mejores paquetes de sondeo disponibles según lo determinado por las fases de descubrimiento anteriores de Nmap. Traceroute generalmente implica otra ronda de resolución de DNS inverso para los hosts intermedios. Encontrará más información en [la sección denominada "Descubrimiento de hosts".](https://nmap.org/book/man-host-discovery.html)`--traceroute`

**Guión Escaneo.** La mayoría de los scripts de Nmap Scripting Engine (NSE) se ejecutan durante esta fase principal de escaneo de scripts, en lugar de las fases de preescaneo y postescaneo. NSE es impulsado por el lenguaje de programación Lua y una biblioteca estándar diseñada para la recopilación de información de la red. Los scripts que se ejecutan durante esta fase generalmente se ejecutan una vez para cada host de destino y número de puerto con el que interactúan. Por lo general, realizan tareas como la detección de vulnerabilidades del servicio, el descubrimiento de malware, la recopilación de más información de bases de datos y otros servicios de red, y la detección avanzada de versiones. NSE no se ejecuta a menos que lo solicite con opciones como o .`--script-sC`

**Salida.** Por último, Nmap recopila toda la información que ha recopilado y la escribe en la pantalla o en un archivo. Nmap puede escribir salidas en varios formatos. Su valor predeterminado, El formato legible por el ser humano (formato interactivo) generalmente se presenta en este libro. Nmap también ofrece un formato de salida basado en XML, entre otros. Los entresijos de la producción son el tema del [Capítulo 13](https://nmap.org/book/output.html).

Como ya se ha comentado, Nmap ofrece muchas opciones para controlar ¿Cuál de estas fases se ejecuta? En el caso de los análisis de redes de gran tamaño, cada se repite muchas veces, ya que Nmap se ocupa de los hosts en grupos más pequeños. Escanea cada grupo por completo y los genera resultados y, a continuación, pasa al siguiente lote de hosts.

**Guión Después del escaneo.** Después de que Nmap haya completado su escaneo y normal, los scripts en esta fase pueden procesar los resultados y entregar Informes finales y estadísticas. Consulte [la sección denominada "Tipos de scripts y fases".](https://nmap.org/book/nse-usage.html#nse-script-types) Nmap aún no incluye ningún script en esta fase, por lo que solo Se ejecuta si el usuario incluye y ejecuta sus propios scripts posteriores al examen.
