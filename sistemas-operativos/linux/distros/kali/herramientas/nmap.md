---
icon: mobile-signal
description: >-
  La guía oficial del proyecto Nmap para el descubrimiento de redes y el escaneo
  de seguridad.
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

<mark style="color:green;">**Puerto Escaneo**</mark>**.** Esta es la operación principal de Nmap. Se envían sondeos y las respuestas (o sin respuestas) a esas sondas que utiliza para clasificar los puertos remotos en estados tales como **`open`**, **`closed`**, o **`filtered`**. Esa breve descripción no comienza para abarcar los muchos tipos de escaneo de Nmap, la configurabilidad de los escaneos y algoritmos para mejorar la velocidad y la precisión.

<mark style="color:green;">**Detección de Versiones**</mark>**.** Si se encuentra algún puerto abierto, Nmap puede ser capaz de determinar qué software de servidor se está ejecutando en el sistema remoto. Lo hace enviando una variedad de sondas a los puertos abiertos y comparando las respuestas con una base de datos de más de 6,500 firmas de servicio.

<mark style="color:green;">**Detección de SISTEMA OPERATIVO**</mark>**.** Se utiliza la opción **`-O`**, Nmap procede a la detección del sistema operativo. Los sistemas operativos implementan estándares de red de maneras diferentes. Al medir estas diferencias, es posible determinar el sistema operativo que se ejecuta en un host remoto.

<mark style="color:green;">**Traceroute**</mark>**.** Nmap tiene integrada una implementación de traceroute optimizada, se habilita con la opción **`--traceroute`**. Puede encontrar las rutas de red para muchos hosts en paralelo, utilizando los mejores paquetes de sondeo disponibles según lo determinado por las fases de descubrimiento anteriores de Nmap. Traceroute generalmente implica otra ronda de resolución de DNS inverso para los hosts intermedios.

<mark style="color:green;">**Script escaneo**</mark>**.** La mayoría de los scripts de _**Nmap Scripting Engine (NSE)**_ se ejecutan durante esta fase principal de escaneo de scripts, en lugar de las fases de _preescaneo_ y _postescaneo_. NSE es impulsado por el lenguaje de programación **Lua** y una biblioteca estándar diseñada para la recopilación de información de la red. Por lo general, realizan tareas como la detección de vulnerabilidades del servicio, el descubrimiento de malware, la recopilación de más información de bases de datos y otros servicios de red, y la detección avanzada de versiones.

<mark style="color:green;">**Salida**</mark>**.** Por último, Nmap recopila toda la información y la escribe en la pantalla o en un archivo. Nmap puede escribir salidas en diversos formatos. Su valor predeterminado (formato interactivo). Nmap también ofrece un formato de salida basado en XML, entre otros.

<mark style="color:green;">**Script post-escaneo**</mark>**.** Después de que Nmap haya completado su escaneo y normal, los scripts en esta fase pueden procesar los resultados y entregar Informes finales y estadísticas. Nmap aún no incluye ningún script en esta fase, por lo que solo se ejecuta si el usuario incluye y ejecuta sus propios scripts.

## <mark style="color:orange;">Capítulo 2. Obtener, compilar, instalar y eliminar Nmap</mark>

El primer paso para obtener Nmap es comprobar si ya tenerlo. Muchas distribuciones de sistemas operativos libres (incluyendo la mayoría de las Linux y BSD) vienen con paquetes Nmap, aunque pueden no ser instalado de forma predeterminada.

Para obtener la versión de Nmap que se tiene instalado, se debe de abrir una terminal y pegar el siguiente comando:

```
nmap --version
```

Automáticamente mostrará la versión que está instalada; y en caso de no tener instalada la herramienta, también mostrará el mensaje de notificación, para comprobar la versión más reciente tendrá que dirigirse al siguiente sitio: [versiones](https://nmap.org/changelog.html).

## <mark style="color:orange;">Capítulo 3. Detección de host ("Escaneo de ping")</mark>

El primer paso en cualquier reconocimiento de red es reducir el rango de IP a una lista de hosts activos o interesantes. Escaneando cada puerto de cada una de las direcciones IP es lenta y, por lo general, innecesaria.&#x20;

Es posible que los administradores solo estén interesados en los hosts que ejecutan un determinado servicio, mientras que los auditores de seguridad pueden preocuparse por cada uno de los dispositivos con una dirección IP.&#x20;

Un administrador puede sentirse cómodo usando solo un ping ICMP para localizar hosts en su red interna, mientras que un probador de penetración puede usar un conjunto diverso de docenas de sondas en un intento por evadir las restricciones del firewall.

Debido a que las necesidades de descubrimiento de host son tan diversas, Nmap ofrece un amplia variedad de opciones para personalizar las técnicas utilizadas. Los usuarios pueden omitir el paso de ping por completo con un escaneo de lista **`-sL`**; o desactivando ping **`-Pn`**, o involucrar la red con combinaciones arbitrarias de TCP multipuerto sondas SYN/ACK, UDP e ICMP.&#x20;

Nmap ofrece muchas técnicas de ping porque a menudo toma combinaciones cuidadosamente elaboradas para atravesar una serie de firewall y filtros de enrutador que conducen a una red de destino.

### <mark style="color:blue;">Especificación de hosts y redes de destino</mark>

Todo lo que aparece en la línea de comandos de Nmap que no sea una opción se trata como una especificación de host de destino. El caso más simple es especificar una dirección IP de destino o un nombre de host para el escaneo.

#### <mark style="color:yellow;">Entrada de la lista</mark> <mark style="color:yellow;"></mark><mark style="color:yellow;">`-iL`</mark>

Escribir una lista enorme de hosts es incómodo en la terminal, sin embargo, es una necesidad común. Por ejemplo, el servidor DHCP podría exportar una lista de 10.000 concesiones actuales que desee analizar. O tal vez desee escanear todas las direcciones IP, _excepto_ aquellas para localizar hosts que utilizan direcciones IP estáticas no autorizadas.&#x20;

Simplemente genere la lista de hosts para escanear y pase ese nombre de archivo a Nmap como un argumento para la opción.&#x20;

```
nmap -iL directorio.txt
```

Las entradas pueden estar en cualquier de los formatos aceptados por Nmap en la línea de comandos (dirección IP, nombre de host, CIDR, IPv6 o rangos de octetos). Cada entrada debe estar separada por uno o más espacios, tabulaciones o saltos de línea.

#### <mark style="color:yellow;">Objetivos aleatorios</mark> <mark style="color:yellow;"></mark><mark style="color:yellow;">`-iR`</mark>

En el caso de investigaciones por Internet, es posible que desee elegir objetivos al azar. Esto se hace con la opción **`-iR`**, que toma como argumento el número de IPs a generar.

```
nmap -iR 50
```

Nmap omite automáticamente ciertas IPs, tales como como los de rangos de direcciones privadas, multidifusión o no asignadas. El argumento se puede especificar para un argumento interminable escanear.

Si te encuentras aburrido una tarde lluviosa, prueba el siguiente comando para localizar servidores web aleatorios.

```
nmap -sS -PS80 -iR 0 -p 80
```

#### <mark style="color:yellow;">Exclusión de objetivos</mark> <mark style="color:yellow;"></mark><mark style="color:yellow;">`--exclude`</mark> <mark style="color:yellow;"></mark><mark style="color:yellow;">,</mark> <mark style="color:yellow;"></mark><mark style="color:yellow;">`--excludefile archivo.txt`</mark>

Es común tener máquinas que no quieres escanear bajo cualquier circunstancia. Las máquinas pueden ser tan críticas que no correrá ningún riesgo de sufrir una reacción adversa. Es posible que se le culpe por un interrupción coincidente, incluso si el escaneo de Nmap no tuvo nada que ver con eso. O tal vez tenga hardware heredado que se sabe que se bloquea cuando escaneado, pero aún no ha podido arreglarlo o reemplazarlo. O tal vez ciertos rangos de IP representan empresas subsidiarias, clientes o Socios que no está autorizado a examinar.&#x20;

Los consultores a menudo no lo hacen quieren que su propia máquina se incluya en un escaneo de las redes de sus clientes. Cualquiera que sea el motivo, puede excluir hosts o redes completas con la opción **`--exclude`**.&#x20;

Simplemente pase la opción a lista separada por comas de destinos excluidos y bloques de red mediante el método sintaxis normal de Nmap.&#x20;

```
nmap 192.168.0.* --exclude 192.168.0.10,20,30
```

Alternativamente, puede crear un archivo de excluidos hosts/redes y pasarlo a Nmap con la opción.

```
nmap 192.168.0.* --excludefile hosts.txt
```

### <mark style="color:yellow;">Encontrar las direcciones IP de una organización</mark>

Nmap automatiza muchos aspectos del escaneo de red, pero aún así debe decirle qué redes escanear. Es importante tener cuidado investigar los bloques de red objetivo antes de escanearlos. Incluso si se llevará a cabo una prueba de penetración y el cliente le dio una lista de sus bloques, es importante verificarlos dos veces. Los clientes a veces tienen registros desactualizados o simplemente los escriben mal. En muchos casos, se comienza con solo el nombre de dominio de una empresa.

#### <mark style="color:yellow;">Trucos de DNS</mark>

El propósito principal del DNS es resolver nombres de dominio en direcciones IP, por lo que es un lugar lógico para comenzar. En el Ejemplo 3.1, utilizo el comando **host** de Linux para consultar algunos tipos de registros DNS comunes.

```
┌──(nato㉿kali)-[~]
└─$ host -t ns nmap.org
nmap.org name server ns1.linode.com.
nmap.org name server ns2.linode.com.
nmap.org name server ns3.linode.com.
nmap.org name server ns4.linode.com.
nmap.org name server ns5.linode.com.
```

```
┌──(nato㉿kali)-[~]
└─$ host -t a nmap.org
nmap.org has address 50.116.1.184
```

```
┌──(nato㉿kali)-[~]
└─$ host -t aaaa nmap.org
nmap.org has no AAAA record
```

```
┌──(nato㉿kali)-[~]
└─$ host -t mx nmap.org
nmap.org mail is handled by 5 alt1.aspmx.l.google.com.
nmap.org mail is handled by 10 aspmx2.googlemail.com.
nmap.org mail is handled by 1 aspmx.l.google.com.
nmap.org mail is handled by 5 alt2.aspmx.l.google.com.
nmap.org mail is handled by 10 aspmx3.googlemail.com.
```

```
┌──(nato㉿kali)-[~]
└─$ host -t soa nmap.org
nmap.org has SOA record ns1.linode.com. hostmaster.insecure.org. 2021000013 14400 14400 1209600 3600
```

