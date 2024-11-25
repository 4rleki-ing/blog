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

# Capítulo 1

## <mark style="color:orange;">Primeros pasos con Nmap</mark>

`Nmap ("Network Mapper")` es una utilidad gratuita y de código abierto para Exploración de redes y auditoría de seguridad. Muchos sistemas y redes Los administradores también lo encuentran útil para tareas como la red inventario, la administración de programas de actualización de servicio y la supervisión del host o Tiempo de actividad del servicio. Nmap utiliza paquetes IP sin procesar de formas novedosas para determinar qué hosts están disponibles en la red, qué servicios (aplicación nombre y versión) que ofrecen esos hosts, qué sistemas operativos (y versiones del sistema operativo) que se están ejecutando, qué tipo de paquete Se utilizan filtros/cortafuegos, y docenas de otras características. Eso fue diseñado para escanear rápidamente grandes redes, pero funciona bien contra Anfitriones individuales. Nmap se ejecuta en todos los principales sistemas operativos de computadoras, y Están disponibles tanto la versión de consola como la gráfica.

El primer paso en una evaluación de vulnerabilidades es la red descubrimiento. Esta etapa de reconocimiento determina qué dirección IP rangos que está utilizando el objetivo, qué hosts están disponibles, qué servicios que ofrecen esos hosts, detalles generales de la topología de la red y qué Las políticas de firewall/filtrado están en vigor.

### <mark style="color:blue;">Las fases de un escaneo Nmap</mark>

Los escaneos se realizan en fases, con cada fase termina antes de que comience la siguiente. Como se puede ver en las descripciones de las fases a continuación, hay mucho más en Nmap que solo el puerto Escaneo.

<mark style="color:green;">**Script Pre-escaneo**</mark>**.** El motor de secuencias de comandos _**Nmap (NSE)**_ utiliza un colección de scripts de propósito especial para obtener más información sobre sistemas remotos. **NSE** no se ejecuta a menos que lo solicite con opciones como **`--script`** o **`-sC`**, y La fase de pre-escaneo solo ocurre cuando los scripts que lo necesitan son seleccionado. Esta fase es para scripts que solo deben ejecutarse una vez por ejecución de Nmap en lugar de ejecutarse por separado contra individuos Objetivos.&#x20;

<mark style="color:green;">**Enumeración de Objetivos**</mark>**.** En esta fase, Nmap investiga el host proporcionado por el usuario, que pueden ser una combinación de (_host_, _Nombres DNS_, _direcciones IP_, notaciones de red CIDR y mucho más). Esta fase no se puede omitir ya que es esencial para el escaneo posterior, pero puede simplificar el procesamiento pasando solo direcciones IP para que Nmap no tenga que reenviar resolución.

<mark style="color:green;">**Detección de host**</mark>**.** Los análisis de red suelen comenzar descubriendo qué objetivos de la red están en línea y, por lo tanto, vale la pena una investigación más profunda. Este proceso se denomina _detección de host_ o _ping escaneo_. Nmap ofrece muchas técnicas de descubrimiento de hosts, que van desde solicitudes rápidas de ARP hasta combinaciones elaboradas de TCP, ICMP y otros tipos de sondas.

<mark style="color:green;">**Resolución de DNS inverso**</mark>**.** Una vez que Nmap ha terminado el escaneo, busca los nombres de DNS inverso de todos los hosts encontrados en línea por el escaneo de ping. A veces, el nombre de un host proporciona pistas sobre su función y los nombres hacen que los informes sean más legibles que proporcionar solo IP Números.

<mark style="color:green;">**Puerto Escaneo**</mark>**.** Esta es la operación principal de Nmap. Se envían sondeos y las respuestas (o sin respuestas) a esas sondas que utiliza para clasificar los puertos remotos en estados tales como **`open`**, **`closed`**, o **`filtered`**. Esa breve descripción no comienza para abarcar los muchos tipos de escaneo de Nmap, la configurabilidad de los escaneos y algoritmos para mejorar la velocidad y la precisión.

<mark style="color:green;">**Detección de Versiones**</mark>**.** Si se encuentra algún puerto abierto, Nmap puede ser capaz de determinar qué software de servidor se está ejecutando en el sistema remoto. Lo hace enviando una variedad de sondas a los puertos abiertos y comparando las respuestas con una base de datos de más de 6,500 firmas de servicio.

<mark style="color:green;">**Detección de SISTEMA OPERATIVO**</mark>**.** Se utiliza la opción **`-O`**, Nmap procede a la detección del sistema operativo. Los sistemas operativos implementan estándares de red de maneras diferentes. Al medir estas diferencias, es posible determinar el sistema operativo que se ejecuta en un host remoto.

<mark style="color:green;">**Traceroute**</mark>**.** Nmap tiene integrada una implementación de traceroute optimizada, se habilita con la opción **`--traceroute`**. Puede encontrar las rutas de red para muchos hosts en paralelo, utilizando los mejores paquetes de sondeo disponibles según lo determinado por las fases de descubrimiento anteriores de Nmap. Traceroute generalmente implica otra ronda de resolución de DNS inverso para los hosts intermedios.

<mark style="color:green;">**Script escaneo**</mark>**.** La mayoría de los scripts de _**Nmap Scripting Engine (NSE)**_ se ejecutan durante esta fase principal de escaneo de scripts, en lugar de las fases de _preescaneo_ y _postescaneo_. NSE es impulsado por el lenguaje de programación **Lua** y una biblioteca estándar diseñada para la recopilación de información de la red. Por lo general, realizan tareas como la detección de vulnerabilidades del servicio, el descubrimiento de malware, la recopilación de más información de bases de datos y otros servicios de red, y la detección avanzada de versiones.

<mark style="color:green;">**Salida**</mark>**.** Por último, Nmap recopila toda la información y la escribe en la pantalla o en un archivo. Nmap puede escribir salidas en diversos formatos. Su valor predeterminado (formato interactivo). Nmap también ofrece un formato de salida basado en XML, entre otros.

<mark style="color:green;">**Script post-escaneo**</mark>**.** Después de que Nmap haya completado su escaneo y normal, los scripts en esta fase pueden procesar los resultados y entregar Informes finales y estadísticas. Nmap aún no incluye ningún script en esta fase, por lo que solo se ejecuta si el usuario incluye y ejecuta sus propios scripts.
