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

# Capítulo 3

## <mark style="color:orange;">Detección de host ("Escaneo de ping")</mark>

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

### <mark style="color:blue;">Encontrar las direcciones IP de una organización</mark>

Nmap automatiza muchos aspectos del escaneo de red, pero aún así debe decirle qué redes escanear. Es importante tener cuidado investigar los bloques de red objetivo antes de escanearlos. Incluso si se llevará a cabo una prueba de penetración y el cliente le dio una lista de sus bloques, es importante verificarlos dos veces. Los clientes a veces tienen registros desactualizados o simplemente los escriben mal. En muchos casos, se comienza con solo el nombre de dominio de una empresa.

#### <mark style="color:yellow;">Trucos de DNS</mark>

El propósito principal del DNS es resolver nombres de dominio en direcciones IP, por lo que es un lugar lógico para comenzar. Se utiliza el comando **`host`** de Linux para consultar algunos tipos de registros DNS comunes; existe un artículo con toda la descripción de este comando para una mayor compresión.

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

Si bien se puede generar una lista de nombres de host sustancial en este manera, la veta madre de los nombres de host proviene de un Transferencia de zona. Asegúrese de probar todos los servidores DNS que han encontrado a través de los registros NS del dominio y el escaneo de puertos los rangos de IP corporativas. Para realizar esto se utiliza el comando **`dig`**; que también hay un artículo dentro de este blog para una mejor comprensión del tema.

```
dig @ns1.google.com nmap.org
```

```
; <<>> DiG 9.20.0-Debian <<>> @ns1.google.com nmap.org
; (1 server found)
;; global options: +cmd
;; Got answer:
;; ->>HEADER<<- opcode: QUERY, status: NOERROR, id: 49693
;; flags: qr rd ra; QUERY: 1, ANSWER: 1, AUTHORITY: 13, ADDITIONAL: 13

;; QUESTION SECTION:
;nmap.org.			IN	A

;; ANSWER SECTION:
nmap.org.		2502	IN	A	50.116.1.184

;; AUTHORITY SECTION:
.			82422	IN	NS	j.root-servers.net.
.			82422	IN	NS	k.root-servers.net.
.			82422	IN	NS	l.root-servers.net.
.			82422	IN	NS	m.root-servers.net.
.			82422	IN	NS	a.root-servers.net.
.			82422	IN	NS	b.root-servers.net.
.			82422	IN	NS	c.root-servers.net.
.			82422	IN	NS	d.root-servers.net.
.			82422	IN	NS	e.root-servers.net.
.			82422	IN	NS	f.root-servers.net.
.			82422	IN	NS	g.root-servers.net.
.			82422	IN	NS	h.root-servers.net.
.			82422	IN	NS	i.root-servers.net.

;; ADDITIONAL SECTION:
j.root-servers.net.	82423	IN	A	192.58.128.30
k.root-servers.net.	82423	IN	A	193.0.14.129
l.root-servers.net.	82423	IN	A	199.7.83.42
m.root-servers.net.	79322	IN	A	202.12.27.33
a.root-servers.net.	19471	IN	A	198.41.0.4
b.root-servers.net.	82422	IN	A	170.247.170.2
c.root-servers.net.	82422	IN	A	192.33.4.12
d.root-servers.net.	82422	IN	A	199.7.91.13
e.root-servers.net.	82422	IN	A	192.203.230.10
f.root-servers.net.	82423	IN	A	192.5.5.241
g.root-servers.net.	82423	IN	A	192.112.36.4
h.root-servers.net.	82423	IN	A	198.97.190.53
i.root-servers.net.	82423	IN	A	192.36.148.17

;; Query time: 16 msec
;; SERVER: 216.239.32.10#53(ns1.google.com) (UDP)
;; WHEN: Sat Nov 23 22:27:31 CST 2024
;; MSG SIZE  rcvd: 461
```

Un error común al recopilar resultados de DNS hacia adelante como estos es asumir que todos los sistemas que se encuentran bajo un nombre de dominio deben ser parte de la red de esa organización y es seguro escanear. De hecho, nada Impide que una organización agregue registros que apunten a cualquier lugar de la Internet. Esto se hace comúnmente para externalizar servicios a terceros partes mientras se mantiene el nombre de dominio de origen para la marca.

Tres pruebas rápidas y sencillas son: Resolución inversa de DNS, traceroute y whois en el registro de direcciones IP correspondiente. El Los dos primeros pasos se pueden realizar mediante Nmap, mientras que el comando whois de Linux Funciona bien para la tercera.

```
sudo nmap -Pn -T4 --traceroute google.com
```

```
Starting Nmap 7.94SVN ( https://nmap.org ) at 2024-11-23 22:31 CST
Nmap scan report for google.com (142.250.138.100)
Host is up (0.15s latency).
Other addresses for google.com (not scanned): 142.250.138.138 142.250.138.102 142.250.138.139 142.250.138.113 142.250.138.101
rDNS record for 142.250.138.100: rw-in-f100.1e100.net
Not shown: 987 filtered tcp ports (no-response)
PORT      STATE  SERVICE
53/tcp    open   domain
80/tcp    open   http
425/tcp   closed icad-el
443/tcp   open   https
1174/tcp  closed fnet-remote-ui
2718/tcp  closed pn-requester2
6106/tcp  closed isdninfo
8086/tcp  closed d-s-n
8652/tcp  closed unknown
9103/tcp  closed jetdirect
16018/tcp closed unknown
31038/tcp closed unknown
34573/tcp closed unknown

TRACEROUTE (using port 9103/tcp)
HOP RTT     ADDRESS
1   1.97 ms 192.168.23.2
2   ... 30

Nmap done: 1 IP address (1 host up) scanned in 85.73 seconds
```

```
whois 142.250.138.100
```

```
#
# ARIN WHOIS data and services are subject to the Terms of Use
# available at: https://www.arin.net/resources/registry/whois/tou/
#
# If you see inaccuracies in the results, please report at
# https://www.arin.net/resources/registry/whois/inaccuracy_reporting/
#
# Copyright 1997-2024, American Registry for Internet Numbers, Ltd.
#


NetRange:       -
CIDR:           -
NetName:        GOOGLE

[...]
```

Las bases de datos web también se pueden utilizar para encontrar nombres de host en un determinado dominio. Por ejemplo [Netcraft](https://searchdns.netcraft.com/?host) tiene una función de búsqueda de DNS.

#### <mark style="color:yellow;">Consultas Whois</mark>

Después de detectar un conjunto de direcciones IP "_iniciales_", deben de investigarse para asegurarse de que pertenecen a la empresa que usted espera y determinar cuáles bloques de red forman parte de la misma.&#x20;

Una empresa mediana puede tener una pequeña asignación de 1 a 16 direcciones IP, mientras que las grandes corporaciones a menudo tienen miles.&#x20;

Esta información se guarda en bases de datos regionales, como _**ARIN**_ (Registro Americano de Números de Internet) para América del Norte y _**RIPE**_ para Europa y Oriente Medio.&#x20;

Las herramientas whois modernas toman una dirección IP y consultan automáticamente el registro apropiado. Normalmente, las pequeñas y medianas empresas no disponen de espacio en materia de PI asignados por empresas como ARIN.&#x20;

```
whois 142.250.138.100
```

```
#
# ARIN WHOIS data and services are subject to the Terms of Use
# available at: https://www.arin.net/resources/registry/whois/tou/
#
# If you see inaccuracies in the results, please report at
# https://www.arin.net/resources/registry/whois/inaccuracy_reporting/
#
# Copyright 1997-2024, American Registry for Internet Numbers, Ltd.
#

[...]
```

El siguiente paso es buscar de manera similar todos las IPs descubiertas que no se encuentran dentro de este rango. Entonces puedes empezar con las consultas avanzadas.&#x20;

El comando **whois -h whois.arin.net \\?** proporciona la sintaxis de consulta ARIN.&#x20;

```
whois -h whois.arin.net \?
```

```
#
# ARIN WHOIS data and services are subject to the Terms of Use
# available at: https://www.arin.net/resources/registry/whois/tou/
#
# If you see inaccuracies in the results, please report at
# https://www.arin.net/resources/registry/whois/inaccuracy_reporting/
#
# Copyright 1997-2024, American Registry for Internet Numbers, Ltd.
#



ARIN's WHOIS service provides a mechanism for finding contact and registration
information for resources registered with ARIN. ARIN's database contains IP
addresses, autonomous system numbers, organizations, or customers that are
associated with these resources, and related Points of Contact [POC].

ARIN's WHOIS will NOT locate any domain related information, nor any
information relating to military networks. Please use whois.internic.net to
locate domain information, and whois.nic.mil for military network information.

Many operating systems provide a whois utility. To conduct a query from the
command line, such as:
    whois -h hostname <query string>
    (e.g. whois -h whois.arin.net foo)

To obtain a more specific response, you may conduct a search by using certain
flags. Many of these flags can be combined to tailor the desired output.
Flags must be separated from each other and from the search term by a space.
Your results will vary depending on the refinements you apply in your search.
Listed below are the flags currently available; you may only use one flag from
each flag-type in a query, i.e. one record type, one attribute, etc.


Query-by-record-type:
---------------------
To limit your query to a specific record type, include one of the following
flags:
      n       Network address space
      r       CIDRized network space
      d       Delegations
      a       Autonomous systems
      p       Points-of-contact
      o       Organizations
      c       End-user customers
      e       Points-of-contact, Organizations, End-user customers
      z       All of the above


Query-by-attribute:
-------------------
To limit your query to a specific record attribute, include one of the
following flags:
      @<domain name>     Searches for matches by domain-portion of an
                         email address
      ! <handle>         Searches for matches by handle or id
      / <name>           Searches for matches by name
      . <name>           Searches for matches by name
                         (same as above, but some WHOIS clients have problems with)

Searches that retrieve a single record will display the full record. Searches
that retrieve more than one record will be displayed in list output.


Display flags:
--------------
To modify the way that the query results display, include one of the
following flags:
      +       FULL output shows detailed display for EACH match
      -       LIST output shows summary only, even if single match
              returned

The + flag cannot be used with the sub-query features described below.


Record hierarchy:
-----------------
Records in the ARIN WHOIS database have hierarchical relationships with other
records. To display those related records, use the following flags:

      <       Displays the record related up the hierarchy. For a network,
              display the supernet, or parent network in detailed format.
      >       Displays the record related down the hierarchy. For a network,
              display the subdelegations, or subnets, below the network, in
              list format. For an organization or customer, display the
              resources registered to that organization or customer, in
              list format.
      =       Display only an exact match in the hierarchy.


Wild card queries:
------------------
WHOIS supports wild card queries. This feature is only supported as a trailing
character option. To take advantage of this append the query with an asterisk
[*]. This can also be used in combination with any flags defined above.


Other helpful hints:
--------------------
To guarantee matching only a single record, look it up by its handle using a
handle-only search.  In the record summary line, the handle is shown in
parenthesis after the name.

When using a handle to conduct a search for POC information, be sure to add
the -ARIN extension.

Queries that return more than 256
results will stop displaying data after the limit has been reached for each
record type. You may want to narrow your search criteria or add flags to your
query to limit the results.    

To search on an individual's name, you may enter the last name, or to further
restrict results, use the last name and first name, separated by a comma. For
example: Smith, John.


Contact us:
-----------
For operational problems with WHOIS please contact noc@arin.net with the
appropriate details.

To correct information within your area of responsibility, submit a template
to hostmaster@arin.net. Information on how to fill out the appropriate template
can be found at: http://www.arin.net/resources/guide/request/documentation/

To notify ARIN of invalid POC information, contact hostmaster@arin.net with
the relevant information.


Terms of Service:
-----------------
ARIN WHOIS data and services are subject to the Terms of Use available at:
https://www.arin.net/resources/registry/whois/tou/


#
# ARIN WHOIS data and services are subject to the Terms of Use
# available at: https://www.arin.net/resources/registry/whois/tou/
#
# If you see inaccuracies in the results, please report at
# https://www.arin.net/resources/registry/whois/inaccuracy_reporting/
#
# Copyright 1997-2024, American Registry for Internet Numbers, Ltd.
#
```

Sin embargo Se permiten muchas otras consultas útiles. Por ejemplo, **whois -h whois.arin.net @target.com** muestra todos los contactos de ARIN con direcciones de correo electrónico en target.com.&#x20;

```
whois -h whois.arin.net @google.com
```

La consulta **whois -h whois.arin.net "n target\*"** muestra todos los identificadores de netblock A partir de target.&#x20;

```
whois -h whois.arin.net "n google*"
```

No distingue entre mayúsculas y minúsculas. Del mismo modo, **whois -h whois.arin.net "o target\*"** muestra todos los nombres de la organización que comienzan con target.

```
whois -h whois.arin.net "o google*"
```

Puede buscar la dirección, el teléfono número de teléfono y correo electrónico de contacto asociado con cada entrada para determinar si forman parte de la empresa que desea escanear.

#### <mark style="color:yellow;">Información de enrutamiento de Internet</mark>

El protocolo de enrutamiento central de Internet es la puerta de enlace fronteriza Protocolo (BGP). Al analizar organizaciones medianas y grandes, BGP Las tablas de enrutamiento pueden ayudarle a encontrar sus subredes IP en todo el mundo.

Una herramienta útil para determinar el AS El número anunciado para una dirección IP determinada está disponible en [`http://asn.cymru.com/`](http://asn.cymru.com/). A continuación, quiero encontrar todas las IP prefijos que ruta a este AS. Una herramienta útil para hacerlo es Disponible en [`http://www.robtex.com/as/`](http://www.robtex.com/as/). Mecanografía y golpeando en Esa página conduce a una pantalla de resumen que muestra 42 prefijos encontrados.

Al obtener información de BGP de formularios web enlatados, como estos es conveniente, la obtención de datos de enrutamiento de enrutadores reales es más divertido y puede permitir consultas personalizadas más potentes. Varios Las organizaciones proporcionan este servicio. Por ejemplo, telnet o visite [`http://routeviews.org`](http://routeviews.org/). Por supuesto, estos servicios Proporcionar acceso de solo lectura a los datos.

### <mark style="color:blue;">Resolución DNS</mark>

El enfoque clave de la detección de hosts es determinar qué hosts están activos y responden en la red. Eso reduce el campo de objetivos. Pero no dejes que el descubrimiento termine ahí. Una gran fuente de información (sobre hosts en red) es DNS, (Nombre de dominio del sistema).

Nmap realiza _resolución de DNS inverso_ para cada IP que responde a los sondeos de detección de host (los que están en línea). La detección de hosts se omite con **`-Pn`**, la resolución se realiza para todas las direcciones IP. En lugar de utilizar el DNS estándar lento bibliotecas de resolución, Nmap utiliza un resolutor de código auxiliar personalizado que realiza docenas de solicitudes en paralelo.

Si bien los valores predeterminados generalmente funcionan bien, Nmap ofrece cuatro opciones para controlar la resolución DNS. Pueden afectar sustancialmente la velocidad de escaneo y la cantidad de información recopilada.

#### <mark style="color:yellow;">`-n`</mark> <mark style="color:yellow;"></mark><mark style="color:yellow;">(Sin resolución DNS)</mark>

Le dice a Nmap que _nunca_ haga resolución DNS inversa en las direcciones IP activas que encuentra. El DNS puede ser lento incluso con el código auxiliar incorporado de Nmap, esta opción reduce los tiempos de escaneo.

#### <mark style="color:yellow;">`-R`</mark> <mark style="color:yellow;"></mark><mark style="color:yellow;">(resolución DNS para todos los objetivos)</mark>

Le dice a Nmap que _siempre_ haga resolución DNS inverso en las direcciones IP de destino. Normalmente, el DNS inverso solo se realiza en hosts responsivos (en línea).

#### <mark style="color:yellow;">`--system-dns`</mark> <mark style="color:yellow;"></mark><mark style="color:yellow;">(Usar el solucionador de DNS del sistema)</mark>

De forma predeterminada, Nmap resuelve las direcciones IP enviando consultas directamente a los servidores de nombres configurados en su host y luego escucha las respuestas. Muchas solicitudes (a menudo docenas) se realizan en paralelo para mejorar el rendimiento. Especifique esta opción para utilizar el solucionador del sistema en su lugar (una IP a la vez a través de la llamada `getnameinfo`). Esto es lento y rara vez es útil a menos que encuentre un error en el paralelo Nmap. El sistema resolver siempre se utiliza para análisis de IPv6.

#### <mark style="color:yellow;">`--dns-servers`</mark><mark style="color:yellow;">` `</mark>_<mark style="color:yellow;">`<server1>`</mark>_<mark style="color:yellow;">`[,`</mark>_<mark style="color:yellow;">`<server2>`</mark>_<mark style="color:yellow;">`[,...]]`</mark> <mark style="color:yellow;"></mark><mark style="color:yellow;">(Servidores a usar para consultas DNS inversas)</mark>

De forma predeterminada, Nmap determina sus servidores DNS (para la resolución de rDNS) desde su archivo _**resolv.conf**_ (Unix) o el archivo **Registro** (Win32). Alternativamente, puede utilizar esta opción para especificar servidores alternativos. Esta opción no se respeta si están usando `--system-dns` o un escaneo de IPv6. Usando múltiples servidores DNS suele ser más rápido, especialmente si elige servidores autorizados para su espacio IP de destino. Esta opción mejora el sigilo, ya que sus solicitudes pueden ser rebotadas sobre cualquier servidor DNS recursivo en Internet.

Esta opción también es útil cuando se escanea redes privadas. A veces, solo unos pocos servidores de nombres proporcionan información adecuada de rDNS, y es posible que ni siquiera sepa dónde son. Puede escanear la red en busca del puerto 53 (tal vez con detección de versiones), luego pruebe los escaneos de la lista Nmap (`-sL`) especificando cada servidor de nombres uno en un tiempo con `--dns-servers` hasta que encuentres uno que funciona.

### <mark style="color:blue;">Controles de detección de hosts</mark>

De forma predeterminada, Nmap incluirá un escaneo de ping a sondeos más intrusivos, como escaneos de puertos, detección de sistemas operativos, Nmap Scripting Engine, o detección de versiones.&#x20;

Por lo general, Nmap solo realiza escaneos intrusivos en Máquinas que se muestran disponibles durante la etapa de escaneo de ping. Éste Ahorra mucho tiempo y ancho de banda en comparación con la realización de escaneos completos en cada uno de los Dirección IP.&#x20;

Sin embargo, este enfoque no es ideal para todas las circunstancias. Hay momentos en los que _sí_ quieres para escanear todas las IP (**`-Pn`**), y otras veces cuando desee realizar la detección de hosts sin un análisis de puertos (**`-sn`**). Allí son incluso momentos en los que desea imprimir los hosts de destino y salir incluso antes de enviar sondas de ping (**`-sL`**).

#### <mark style="color:yellow;">Escaneo de lista (</mark><mark style="color:yellow;">`-sL`</mark><mark style="color:yellow;">)</mark>

El análisis de lista es una forma degenerada de descubrimiento de host que simplemente enumera cada host en las redes especificadas, sin enviar cualquier paquete a los hosts de destino. De forma predeterminada, Nmap sigue realizando una resolución de DNS inverso en los hosts para aprender sus nombres. El escaneo de la lista es una buena verificación de cordura para asegurarse de que tiene direcciones IP adecuadas para sus objetivos.

Otra razón para un escaneo de lista anticipada es el sigilo. En algunos casos, no se quiere comenzar con un asalto a gran escala contra el red de destino que es probable que active alertas IDS y traiga atención. Un escaneo de lista es discreto y proporciona información que puede ser útil para elegir qué máquinas individuales seleccionar.

A continuación se muestra el análisis de lista que se está utilizando para enumerar el rango de red CIDR /28 (16 IP addresses) que rodean el servidor web principal de Google.

```
sudo nmap -sL google.com/28              

Starting Nmap 7.94SVN ( https://nmap.org ) at 2024-11-24 00:04 CST
Nmap scan report for rr-in-f112.1e100.net (142.250.114.112)
Nmap scan report for google.com (142.250.114.113)
Other addresses for google.com (not scanned): 142.250.114.100 142.250.114.102 142.250.114.138 142.250.114.101 142.250.114.139
rDNS record for 142.250.114.113: rr-in-f113.1e100.net
Nmap scan report for rr-in-f114.1e100.net (142.250.114.114)
Nmap scan report for rr-in-f115.1e100.net (142.250.114.115)
Nmap scan report for rr-in-f116.1e100.net (142.250.114.116)
Nmap scan report for rr-in-f117.1e100.net (142.250.114.117)
Nmap scan report for rr-in-f118.1e100.net (142.250.114.118)
Nmap scan report for rr-in-f119.1e100.net (142.250.114.119)
Nmap scan report for rr-in-f120.1e100.net (142.250.114.120)
Nmap scan report for rr-in-f121.1e100.net (142.250.114.121)
Nmap scan report for rr-in-f122.1e100.net (142.250.114.122)
Nmap scan report for rr-in-f123.1e100.net (142.250.114.123)
Nmap scan report for rr-in-f124.1e100.net (142.250.114.124)
Nmap scan report for rr-in-f125.1e100.net (142.250.114.125)
Nmap scan report for rr-in-f126.1e100.net (142.250.114.126)
Nmap scan report for rr-in-f127.1e100.net (142.250.114.127)
Nmap done: 16 IP addresses (0 hosts up) scanned in 0.24 seconds
```

#### <mark style="color:yellow;">Deshabilitar el escaneo de puertos (</mark><mark style="color:yellow;">`-sn`</mark><mark style="color:yellow;">)</mark>

Esta opción le dice a Nmap que no ejecute un escaneo de puertos después del descubrimiento del host. Cuando se usa por sí mismo, hace que Nmap descubra el host, a continuación, imprime los hosts disponibles que respondieron al análisis.&#x20;

Esto a menudo se denomina "_**escaneo de ping**_". A pesar de que no hay puerto se realiza el escaneo, aún puede solicitar el motor de secuencias de comandos Nmap (**`--script`**) scripts de host y sondeo de traceroute (**`--traceroute`**).&#x20;

Un escaneo de solo ping es un paso más intrusivo que un escaneo de lista y, a menudo, se puede usar con los mismos fines. Realiza un reconocimiento ligero de un objetivo red rápida y sin llamar mucho la atención. Saber cómo muchos hosts están activos es más valioso para los atacantes que la lista de todos los IP  y nombre de host proporcionados por el escaneo de lista.

Los administradores de sistemas a menudo también consideran que esta opción es valiosa. Se puede utilizar fácilmente para contar las máquinas disponibles en una red o Supervise la disponibilidad del servidor. Esto a menudo se denomina barrido de ping, y es más confiable que hacer ping a la dirección de transmisión porque muchos hosts No responda a las consultas de difusión.

A continuación se muestra un escaneo de ping rápido contra el CIDR /24 (256 IPs) en torno al sitio oficial de Google.

```
sudo nmap -sn -T4 google.com/24

Starting Nmap 7.94SVN ( https://nmap.org ) at 2024-11-24 00:13 CST
Nmap scan report for rs-in-f0.1e100.net (142.250.113.0)
Host is up (0.000040s latency).
Nmap scan report for rs-in-f1.1e100.net (142.250.113.1)
Host is up (0.046s latency).
Nmap scan report for rs-in-f2.1e100.net (142.250.113.2)
Host is up (0.046s latency).
Nmap scan report for rs-in-f3.1e100.net (142.250.113.3)
Host is up (0.047s latency).
Nmap scan report for rs-in-f4.1e100.net (142.250.113.4)
Host is up (0.0013s latency).
Nmap scan report for rs-in-f5.1e100.net (142.250.113.5)
Host is up (0.0011s latency).
Nmap scan report for rs-in-f6.1e100.net (142.250.113.6)
Host is up (0.00099s latency).
Nmap scan report for rs-in-f7.1e100.net (142.250.113.7)
Host is up (0.00080s latency).
Nmap scan report for rs-in-f8.1e100.net (142.250.113.8)
Host is up (0.00069s latency).
Nmap scan report for rs-in-f9.1e100.net (142.250.113.9)
Host is up (0.00058s latency).
Nmap scan report for rs-in-f10.1e100.net (142.250.113.10)
Host is up (0.00050s latency).
Nmap scan report for rs-in-f11.1e100.net (142.250.113.11)
Host is up (0.00076s latency).
Nmap scan report for rs-in-f12.1e100.net (142.250.113.12)
Host is up (0.00041s latency).
Nmap scan report for rs-in-f13.1e100.net (142.250.113.13)
Host is up (0.0015s latency).
Nmap scan report for rs-in-f14.1e100.net (142.250.113.14)
Host is up (0.051s latency).
Nmap scan report for rs-in-f15.1e100.net (142.250.113.15)
Host is up (0.0014s latency).
Nmap scan report for rs-in-f16.1e100.net (142.250.113.16)
Host is up (0.051s latency).
Nmap scan report for rs-in-f17.1e100.net (142.250.113.17)
Host is up (0.056s latency).
Nmap scan report for rs-in-f18.1e100.net (142.250.113.18)
Host is up (0.048s latency).
Nmap scan report for rs-in-f19.1e100.net (142.250.113.19)
Host is up (0.050s latency).
Nmap scan report for rs-in-f20.1e100.net (142.250.113.20)
Host is up (0.00077s latency).
Nmap scan report for rs-in-f21.1e100.net (142.250.113.21)
Host is up (0.0027s latency).
Nmap scan report for rs-in-f22.1e100.net (142.250.113.22)
Host is up (0.0026s latency).
Nmap scan report for rs-in-f23.1e100.net (142.250.113.23)
Host is up (0.0025s latency).
Nmap scan report for rs-in-f24.1e100.net (142.250.113.24)
Host is up (0.0029s latency).
Nmap scan report for rs-in-f25.1e100.net (142.250.113.25)
Host is up (0.0028s latency).
Nmap scan report for rs-in-f26.1e100.net (142.250.113.26)
Host is up (0.052s latency).
Nmap scan report for rs-in-f27.1e100.net (142.250.113.27)
Host is up (0.052s latency).
Nmap scan report for rs-in-f28.1e100.net (142.250.113.28)
Host is up (0.051s latency).
Nmap scan report for rs-in-f29.1e100.net (142.250.113.29)
Host is up (0.0028s latency).
Nmap scan report for rs-in-f30.1e100.net (142.250.113.30)
Host is up (0.0024s latency).
Nmap scan report for rs-in-f31.1e100.net (142.250.113.31)
Host is up (0.053s latency).
Nmap scan report for rs-in-f32.1e100.net (142.250.113.32)
Host is up (0.0023s latency).
Nmap scan report for rs-in-f33.1e100.net (142.250.113.33)
Host is up (0.0022s latency).
Nmap scan report for rs-in-f34.1e100.net (142.250.113.34)
Host is up (0.00074s latency).
Nmap scan report for rs-in-f35.1e100.net (142.250.113.35)
Host is up (0.00065s latency).
Nmap scan report for rs-in-f36.1e100.net (142.250.113.36)
Host is up (0.00054s latency).
Nmap scan report for rs-in-f37.1e100.net (142.250.113.37)
Host is up (0.00044s latency).
Nmap scan report for rs-in-f38.1e100.net (142.250.113.38)
Host is up (0.00068s latency).
Nmap scan report for rs-in-f39.1e100.net (142.250.113.39)
Host is up (0.00059s latency).
Nmap scan report for rs-in-f40.1e100.net (142.250.113.40)
Host is up (0.00051s latency).
Nmap scan report for rs-in-f41.1e100.net (142.250.113.41)
Host is up (0.00094s latency).
Nmap scan report for rs-in-f42.1e100.net (142.250.113.42)
Host is up (0.00091s latency).
Nmap scan report for rs-in-f43.1e100.net (142.250.113.43)
Host is up (0.00049s latency).
Nmap scan report for rs-in-f44.1e100.net (142.250.113.44)
Host is up (0.00043s latency).
Nmap scan report for rs-in-f45.1e100.net (142.250.113.45)
Host is up (0.0012s latency).
Nmap scan report for rs-in-f46.1e100.net (142.250.113.46)
Host is up (0.0011s latency).
Nmap scan report for rs-in-f47.1e100.net (142.250.113.47)
Host is up (0.0013s latency).
Nmap scan report for rs-in-f48.1e100.net (142.250.113.48)
Host is up (0.0012s latency).
Nmap scan report for rs-in-f49.1e100.net (142.250.113.49)
Host is up (0.0018s latency).
Nmap scan report for rs-in-f50.1e100.net (142.250.113.50)
Host is up (0.0017s latency).
Nmap scan report for rs-in-f51.1e100.net (142.250.113.51)
Host is up (0.0017s latency).
Nmap scan report for rs-in-f52.1e100.net (142.250.113.52)
Host is up (0.0023s latency).
Nmap scan report for rs-in-f53.1e100.net (142.250.113.53)
Host is up (0.0022s latency).
Nmap scan report for rs-in-f54.1e100.net (142.250.113.54)
Host is up (0.0021s latency).
Nmap scan report for rs-in-f55.1e100.net (142.250.113.55)
Host is up (0.0020s latency).
Nmap scan report for rs-in-f56.1e100.net (142.250.113.56)
Host is up (0.0019s latency).
Nmap scan report for rs-in-f57.1e100.net (142.250.113.57)
Host is up (0.00041s latency).
Nmap scan report for rs-in-f58.1e100.net (142.250.113.58)
Host is up (0.00034s latency).
Nmap scan report for rs-in-f59.1e100.net (142.250.113.59)
Host is up (0.0028s latency).
Nmap scan report for rs-in-f60.1e100.net (142.250.113.60)
Host is up (0.0038s latency).
Nmap scan report for rs-in-f61.1e100.net (142.250.113.61)
Host is up (0.0037s latency).
Nmap scan report for rs-in-f62.1e100.net (142.250.113.62)
Host is up (0.0035s latency).
Nmap scan report for rs-in-f63.1e100.net (142.250.113.63)
Host is up (0.0032s latency).
Nmap scan report for rs-in-f64.1e100.net (142.250.113.64)
Host is up (0.0031s latency).
Nmap scan report for rs-in-f65.1e100.net (142.250.113.65)
Host is up (0.0030s latency).
Nmap scan report for rs-in-f66.1e100.net (142.250.113.66)
Host is up (0.00033s latency).
Nmap scan report for rs-in-f67.1e100.net (142.250.113.67)
Host is up (0.000043s latency).
Nmap scan report for rs-in-f68.1e100.net (142.250.113.68)
Host is up (0.0029s latency).
Nmap scan report for rs-in-f69.1e100.net (142.250.113.69)
Host is up (0.0028s latency).
Nmap scan report for rs-in-f70.1e100.net (142.250.113.70)
Host is up (0.0012s latency).
Nmap scan report for rs-in-f71.1e100.net (142.250.113.71)
Host is up (0.0012s latency).
Nmap scan report for rs-in-f72.1e100.net (142.250.113.72)
Host is up (0.0012s latency).
Nmap scan report for rs-in-f73.1e100.net (142.250.113.73)
Host is up (0.00089s latency).
Nmap scan report for rs-in-f74.1e100.net (142.250.113.74)
Host is up (0.00069s latency).
Nmap scan report for rs-in-f75.1e100.net (142.250.113.75)
Host is up (0.0011s latency).
Nmap scan report for rs-in-f76.1e100.net (142.250.113.76)
Host is up (0.0011s latency).
Nmap scan report for rs-in-f77.1e100.net (142.250.113.77)
Host is up (0.0013s latency).
Nmap scan report for rs-in-f78.1e100.net (142.250.113.78)
Host is up (0.0012s latency).
Nmap scan report for rs-in-f79.1e100.net (142.250.113.79)
Host is up (0.00012s latency).
Nmap scan report for rs-in-f80.1e100.net (142.250.113.80)
Host is up (0.000077s latency).
Nmap scan report for rs-in-f81.1e100.net (142.250.113.81)
Host is up (0.046s latency).
Nmap scan report for rs-in-f82.1e100.net (142.250.113.82)
Host is up (0.053s latency).
Nmap scan report for rs-in-f83.1e100.net (142.250.113.83)
Host is up (0.063s latency).
Nmap scan report for rs-in-f84.1e100.net (142.250.113.84)
Host is up (0.063s latency).
Nmap scan report for rs-in-f85.1e100.net (142.250.113.85)
Host is up (0.000039s latency).
Nmap scan report for rs-in-f86.1e100.net (142.250.113.86)
Host is up (0.000039s latency).
Nmap scan report for rs-in-f87.1e100.net (142.250.113.87)
Host is up (0.0018s latency).
Nmap scan report for rs-in-f88.1e100.net (142.250.113.88)
Host is up (0.059s latency).
Nmap scan report for rs-in-f89.1e100.net (142.250.113.89)
Host is up (0.0017s latency).
Nmap scan report for rs-in-f90.1e100.net (142.250.113.90)
Host is up (0.055s latency).
Nmap scan report for rs-in-f91.1e100.net (142.250.113.91)
Host is up (0.070s latency).
Nmap scan report for rs-in-f92.1e100.net (142.250.113.92)
Host is up (0.069s latency).
Nmap scan report for rs-in-f93.1e100.net (142.250.113.93)
Host is up (0.0016s latency).
Nmap scan report for rs-in-f94.1e100.net (142.250.113.94)
Host is up (0.070s latency).
Nmap scan report for rs-in-f95.1e100.net (142.250.113.95)
Host is up (0.060s latency).
Nmap scan report for rs-in-f96.1e100.net (142.250.113.96)
Host is up (0.060s latency).
Nmap scan report for rs-in-f97.1e100.net (142.250.113.97)
Host is up (0.046s latency).
Nmap scan report for rs-in-f98.1e100.net (142.250.113.98)
Host is up (0.059s latency).
Nmap scan report for rs-in-f99.1e100.net (142.250.113.99)
Host is up (0.060s latency).
Nmap scan report for rs-in-f100.1e100.net (142.250.113.100)
Host is up (0.053s latency).
Nmap scan report for rs-in-f101.1e100.net (142.250.113.101)
Host is up (0.055s latency).
Nmap scan report for google.com (142.250.113.102)
Host is up (0.059s latency).
Other addresses for google.com (not scanned): 142.250.113.138 142.250.113.139 142.250.113.113 142.250.113.100 142.250.113.101
rDNS record for 142.250.113.102: rs-in-f102.1e100.net
Nmap scan report for rs-in-f103.1e100.net (142.250.113.103)
Host is up (0.060s latency).
Nmap scan report for rs-in-f104.1e100.net (142.250.113.104)
Host is up (0.052s latency).
Nmap scan report for rs-in-f105.1e100.net (142.250.113.105)
Host is up (0.057s latency).
Nmap scan report for rs-in-f106.1e100.net (142.250.113.106)
Host is up (0.057s latency).
Nmap scan report for rs-in-f107.1e100.net (142.250.113.107)
Host is up (0.055s latency).
Nmap scan report for rs-in-f108.1e100.net (142.250.113.108)
Host is up (0.055s latency).
Nmap scan report for rs-in-f109.1e100.net (142.250.113.109)
Host is up (0.051s latency).
Nmap scan report for rs-in-f110.1e100.net (142.250.113.110)
Host is up (0.054s latency).
Nmap scan report for rs-in-f111.1e100.net (142.250.113.111)
Host is up (0.00067s latency).
Nmap scan report for rs-in-f112.1e100.net (142.250.113.112)
Host is up (0.053s latency).
Nmap scan report for rs-in-f113.1e100.net (142.250.113.113)
Host is up (0.054s latency).
Nmap scan report for rs-in-f114.1e100.net (142.250.113.114)
Host is up (0.054s latency).
Nmap scan report for rs-in-f115.1e100.net (142.250.113.115)
Host is up (0.0011s latency).
Nmap scan report for rs-in-f116.1e100.net (142.250.113.116)
Host is up (0.072s latency).
Nmap scan report for rs-in-f117.1e100.net (142.250.113.117)
Host is up (0.068s latency).
Nmap scan report for rs-in-f118.1e100.net (142.250.113.118)
Host is up (0.051s latency).
Nmap scan report for rs-in-f119.1e100.net (142.250.113.119)
Host is up (0.051s latency).
Nmap scan report for rs-in-f120.1e100.net (142.250.113.120)
Host is up (0.070s latency).
Nmap scan report for rs-in-f121.1e100.net (142.250.113.121)
Host is up (0.066s latency).
Nmap scan report for rs-in-f122.1e100.net (142.250.113.122)
Host is up (0.065s latency).
Nmap scan report for rs-in-f123.1e100.net (142.250.113.123)
Host is up (0.070s latency).
Nmap scan report for rs-in-f124.1e100.net (142.250.113.124)
Host is up (0.064s latency).
Nmap scan report for rs-in-f125.1e100.net (142.250.113.125)
Host is up (0.0011s latency).
Nmap scan report for rs-in-f126.1e100.net (142.250.113.126)
Host is up (0.058s latency).
Nmap scan report for rs-in-f127.1e100.net (142.250.113.127)
Host is up (0.058s latency).
Nmap scan report for rs-in-f128.1e100.net (142.250.113.128)
Host is up (0.064s latency).
Nmap scan report for rs-in-f129.1e100.net (142.250.113.129)
Host is up (0.059s latency).
Nmap scan report for rs-in-f130.1e100.net (142.250.113.130)
Host is up (0.00063s latency).
Nmap scan report for rs-in-f131.1e100.net (142.250.113.131)
Host is up (0.00047s latency).
Nmap scan report for rs-in-f132.1e100.net (142.250.113.132)
Host is up (0.059s latency).
Nmap scan report for rs-in-f133.1e100.net (142.250.113.133)
Host is up (0.055s latency).
Nmap scan report for rs-in-f134.1e100.net (142.250.113.134)
Host is up (0.069s latency).
Nmap scan report for rs-in-f135.1e100.net (142.250.113.135)
Host is up (0.059s latency).
Nmap scan report for rs-in-f136.1e100.net (142.250.113.136)
Host is up (0.055s latency).
Nmap scan report for rs-in-f137.1e100.net (142.250.113.137)
Host is up (0.055s latency).
Nmap scan report for rs-in-f138.1e100.net (142.250.113.138)
Host is up (0.069s latency).
Nmap scan report for rs-in-f139.1e100.net (142.250.113.139)
Host is up (0.064s latency).
Nmap scan report for rs-in-f140.1e100.net (142.250.113.140)
Host is up (0.00060s latency).
Nmap scan report for rs-in-f141.1e100.net (142.250.113.141)
Host is up (0.077s latency).
Nmap scan report for rs-in-f142.1e100.net (142.250.113.142)
Host is up (0.072s latency).
Nmap scan report for rs-in-f143.1e100.net (142.250.113.143)
Host is up (0.074s latency).
Nmap scan report for rs-in-f144.1e100.net (142.250.113.144)
Host is up (0.074s latency).
Nmap scan report for rs-in-f145.1e100.net (142.250.113.145)
Host is up (0.074s latency).
Nmap scan report for rs-in-f146.1e100.net (142.250.113.146)
Host is up (0.075s latency).
Nmap scan report for rs-in-f147.1e100.net (142.250.113.147)
Host is up (0.074s latency).
Nmap scan report for rs-in-f148.1e100.net (142.250.113.148)
Host is up (0.076s latency).
Nmap scan report for rs-in-f149.1e100.net (142.250.113.149)
Host is up (0.076s latency).
Nmap scan report for rs-in-f150.1e100.net (142.250.113.150)
Host is up (0.00025s latency).
Nmap scan report for rs-in-f151.1e100.net (142.250.113.151)
Host is up (0.00022s latency).
Nmap scan report for rs-in-f152.1e100.net (142.250.113.152)
Host is up (0.060s latency).
Nmap scan report for rs-in-f153.1e100.net (142.250.113.153)
Host is up (0.060s latency).
Nmap scan report for rs-in-f154.1e100.net (142.250.113.154)
Host is up (0.059s latency).
Nmap scan report for rs-in-f155.1e100.net (142.250.113.155)
Host is up (0.069s latency).
Nmap scan report for rs-in-f156.1e100.net (142.250.113.156)
Host is up (0.068s latency).
Nmap scan report for rs-in-f157.1e100.net (142.250.113.157)
Host is up (0.074s latency).
Nmap scan report for rs-in-f158.1e100.net (142.250.113.158)
Host is up (0.00084s latency).
Nmap scan report for rs-in-f159.1e100.net (142.250.113.159)
Host is up (0.00077s latency).
Nmap scan report for rs-in-f160.1e100.net (142.250.113.160)
Host is up (0.075s latency).
Nmap scan report for rs-in-f161.1e100.net (142.250.113.161)
Host is up (0.074s latency).
Nmap scan report for rs-in-f162.1e100.net (142.250.113.162)
Host is up (0.068s latency).
Nmap scan report for rs-in-f163.1e100.net (142.250.113.163)
Host is up (0.073s latency).
Nmap scan report for rs-in-f164.1e100.net (142.250.113.164)
Host is up (0.074s latency).
Nmap scan report for rs-in-f165.1e100.net (142.250.113.165)
Host is up (0.075s latency).
Nmap scan report for rs-in-f166.1e100.net (142.250.113.166)
Host is up (0.070s latency).
Nmap scan report for rs-in-f167.1e100.net (142.250.113.167)
Host is up (0.00019s latency).
Nmap scan report for rs-in-f168.1e100.net (142.250.113.168)
Host is up (0.055s latency).
Nmap scan report for rs-in-f169.1e100.net (142.250.113.169)
Host is up (0.0014s latency).
Nmap scan report for rs-in-f170.1e100.net (142.250.113.170)
Host is up (0.0013s latency).
Nmap scan report for rs-in-f171.1e100.net (142.250.113.171)
Host is up (0.0012s latency).
Nmap scan report for rs-in-f172.1e100.net (142.250.113.172)
Host is up (0.00017s latency).
Nmap scan report for rs-in-f173.1e100.net (142.250.113.173)
Host is up (0.000040s latency).
Nmap scan report for rs-in-f174.1e100.net (142.250.113.174)
Host is up (0.00087s latency).
Nmap scan report for rs-in-f175.1e100.net (142.250.113.175)
Host is up (0.00078s latency).
Nmap scan report for rs-in-f176.1e100.net (142.250.113.176)
Host is up (0.00033s latency).
Nmap scan report for rs-in-f177.1e100.net (142.250.113.177)
Host is up (0.00030s latency).
Nmap scan report for rs-in-f178.1e100.net (142.250.113.178)
Host is up (0.00083s latency).
Nmap scan report for rs-in-f179.1e100.net (142.250.113.179)
Host is up (0.00079s latency).
Nmap scan report for rs-in-f180.1e100.net (142.250.113.180)
Host is up (0.00075s latency).
Nmap scan report for rs-in-f181.1e100.net (142.250.113.181)
Host is up (0.056s latency).
Nmap scan report for rs-in-f182.1e100.net (142.250.113.182)
Host is up (0.057s latency).
Nmap scan report for rs-in-f183.1e100.net (142.250.113.183)
Host is up (0.069s latency).
Nmap scan report for rs-in-f184.1e100.net (142.250.113.184)
Host is up (0.071s latency).
Nmap scan report for rs-in-f185.1e100.net (142.250.113.185)
Host is up (0.071s latency).
Nmap scan report for rs-in-f186.1e100.net (142.250.113.186)
Host is up (0.058s latency).
Nmap scan report for rs-in-f187.1e100.net (142.250.113.187)
Host is up (0.063s latency).
Nmap scan report for rs-in-f188.1e100.net (142.250.113.188)
Host is up (0.060s latency).
Nmap scan report for rs-in-f189.1e100.net (142.250.113.189)
Host is up (0.055s latency).
Nmap scan report for rs-in-f190.1e100.net (142.250.113.190)
Host is up (0.062s latency).
Nmap scan report for rs-in-f191.1e100.net (142.250.113.191)
Host is up (0.067s latency).
Nmap scan report for rs-in-f192.1e100.net (142.250.113.192)
Host is up (0.060s latency).
Nmap scan report for rs-in-f193.1e100.net (142.250.113.193)
Host is up (0.062s latency).
Nmap scan report for rs-in-f194.1e100.net (142.250.113.194)
Host is up (0.062s latency).
Nmap scan report for rs-in-f195.1e100.net (142.250.113.195)
Host is up (0.074s latency).
Nmap scan report for rs-in-f196.1e100.net (142.250.113.196)
Host is up (0.075s latency).
Nmap scan report for rs-in-f197.1e100.net (142.250.113.197)
Host is up (0.074s latency).
Nmap scan report for rs-in-f198.1e100.net (142.250.113.198)
Host is up (0.074s latency).
Nmap scan report for rs-in-f199.1e100.net (142.250.113.199)
Host is up (0.074s latency).
Nmap scan report for rs-in-f200.1e100.net (142.250.113.200)
Host is up (0.074s latency).
Nmap scan report for rs-in-f201.1e100.net (142.250.113.201)
Host is up (0.078s latency).
Nmap scan report for rs-in-f202.1e100.net (142.250.113.202)
Host is up (0.085s latency).
Nmap scan report for rs-in-f203.1e100.net (142.250.113.203)
Host is up (0.00040s latency).
Nmap scan report for rs-in-f204.1e100.net (142.250.113.204)
Host is up (0.00023s latency).
Nmap scan report for rs-in-f205.1e100.net (142.250.113.205)
Host is up (0.00019s latency).
Nmap scan report for rs-in-f206.1e100.net (142.250.113.206)
Host is up (0.060s latency).
Nmap scan report for rs-in-f207.1e100.net (142.250.113.207)
Host is up (0.059s latency).
Nmap scan report for rs-in-f208.1e100.net (142.250.113.208)
Host is up (0.00026s latency).
Nmap scan report for rs-in-f209.1e100.net (142.250.113.209)
Host is up (0.00025s latency).
Nmap scan report for rs-in-f210.1e100.net (142.250.113.210)
Host is up (0.00015s latency).
Nmap scan report for rs-in-f211.1e100.net (142.250.113.211)
Host is up (0.00021s latency).
Nmap scan report for rs-in-f212.1e100.net (142.250.113.212)
Host is up (0.00012s latency).
Nmap scan report for rs-in-f213.1e100.net (142.250.113.213)
Host is up (0.0018s latency).
Nmap scan report for rs-in-f214.1e100.net (142.250.113.214)
Host is up (0.063s latency).
Nmap scan report for rs-in-f215.1e100.net (142.250.113.215)
Host is up (0.063s latency).
Nmap scan report for rs-in-f216.1e100.net (142.250.113.216)
Host is up (0.00011s latency).
Nmap scan report for rs-in-f217.1e100.net (142.250.113.217)
Host is up (0.000050s latency).
Nmap scan report for rs-in-f218.1e100.net (142.250.113.218)
Host is up (0.063s latency).
Nmap scan report for rs-in-f219.1e100.net (142.250.113.219)
Host is up (0.000057s latency).
Nmap scan report for rs-in-f220.1e100.net (142.250.113.220)
Host is up (0.000042s latency).
Nmap scan report for rs-in-f221.1e100.net (142.250.113.221)
Host is up (0.000051s latency).
Nmap scan report for rs-in-f222.1e100.net (142.250.113.222)
Host is up (0.000040s latency).
Nmap scan report for rs-in-f223.1e100.net (142.250.113.223)
Host is up (0.000038s latency).
Nmap scan report for rs-in-f224.1e100.net (142.250.113.224)
Host is up (0.000042s latency).
Nmap scan report for rs-in-f225.1e100.net (142.250.113.225)
Host is up (0.00020s latency).
Nmap scan report for rs-in-f226.1e100.net (142.250.113.226)
Host is up (0.00019s latency).
Nmap scan report for rs-in-f227.1e100.net (142.250.113.227)
Host is up (0.00014s latency).
Nmap scan report for rs-in-f228.1e100.net (142.250.113.228)
Host is up (0.00016s latency).
Nmap scan report for rs-in-f229.1e100.net (142.250.113.229)
Host is up (0.00023s latency).
Nmap scan report for rs-in-f230.1e100.net (142.250.113.230)
Host is up (0.00020s latency).
Nmap scan report for rs-in-f231.1e100.net (142.250.113.231)
Host is up (0.00037s latency).
Nmap scan report for rs-in-f232.1e100.net (142.250.113.232)
Host is up (0.00025s latency).
Nmap scan report for rs-in-f233.1e100.net (142.250.113.233)
Host is up (0.00022s latency).
Nmap scan report for rs-in-f234.1e100.net (142.250.113.234)
Host is up (0.00017s latency).
Nmap scan report for rs-in-f235.1e100.net (142.250.113.235)
Host is up (0.00013s latency).
Nmap scan report for rs-in-f236.1e100.net (142.250.113.236)
Host is up (0.000086s latency).
Nmap scan report for rs-in-f237.1e100.net (142.250.113.237)
Host is up (0.00030s latency).
Nmap scan report for rs-in-f238.1e100.net (142.250.113.238)
Host is up (0.000039s latency).
Nmap scan report for rs-in-f239.1e100.net (142.250.113.239)
Host is up (0.000039s latency).
Nmap scan report for rs-in-f240.1e100.net (142.250.113.240)
Host is up (0.00025s latency).
Nmap scan report for rs-in-f241.1e100.net (142.250.113.241)
Host is up (0.00033s latency).
Nmap scan report for rs-in-f242.1e100.net (142.250.113.242)
Host is up (0.00033s latency).
Nmap scan report for rs-in-f243.1e100.net (142.250.113.243)
Host is up (0.00087s latency).
Nmap scan report for rs-in-f244.1e100.net (142.250.113.244)
Host is up (0.00086s latency).
Nmap scan report for rs-in-f245.1e100.net (142.250.113.245)
Host is up (0.000052s latency).
Nmap scan report for rs-in-f246.1e100.net (142.250.113.246)
Host is up (0.000039s latency).
Nmap scan report for rs-in-f247.1e100.net (142.250.113.247)
Host is up (0.0021s latency).
Nmap scan report for rs-in-f248.1e100.net (142.250.113.248)
Host is up (0.0020s latency).
Nmap scan report for rs-in-f249.1e100.net (142.250.113.249)
Host is up (0.0019s latency).
Nmap scan report for rs-in-f250.1e100.net (142.250.113.250)
Host is up (0.0018s latency).
Nmap scan report for rs-in-f251.1e100.net (142.250.113.251)
Host is up (0.0016s latency).
Nmap scan report for rs-in-f252.1e100.net (142.250.113.252)
Host is up (0.0016s latency).
Nmap scan report for rs-in-f253.1e100.net (142.250.113.253)
Host is up (0.0015s latency).
Nmap scan report for rs-in-f254.1e100.net (142.250.113.254)
Host is up (0.0013s latency).
Nmap scan report for rs-in-f255.1e100.net (142.250.113.255)
Host is up (0.0011s latency).
Nmap done: 256 IP addresses (256 hosts up) scanned in 6.30 seconds
```

Si las máquinas resultan ser muy seguras, un atacante podría ir tras una de esas máquinas vecinas y luego realizar un ataque de ethernet local con herramientas como _**Ettercap**_ o _**Dsniff**_.&#x20;

Un uso ético de estos datos sería un Administrador de red que está considerando mover máquinas a este proveedor. Podría enviar un correo electrónico a algunas de las organizaciones enumeradas y preguntar su opinión del servicio antes de firmar un contrato a largo plazo o de realizar el costoso y disruptivo traslado del centro de datos.

#### <mark style="color:yellow;">Desactivar ping (</mark><mark style="color:yellow;">`-Pn`</mark><mark style="color:yellow;">)</mark>

Otra opción es omitir por completo la etapa de descubrimiento de Nmap. De forma predeterminada, Nmap realiza un sondeo pesado como escaneos de puertos, detección de versiones o detección del sistema operativo en hosts que se encuentran activos.&#x20;

Des habilitación de la detección de hosts con la opción **`-Pn`** hace que Nmap intente el escaneo solicitado contra _cada_ dirección IP de destino especificada. Por lo tanto, se omite la detección de host adecuada como con un escaneo de lista, pero en lugar de detenerse e imprimir el objetivo lista, Nmap continúa realizando las funciones solicitadas como si cada IP objetivo está activa.

Hay muchas razones para deshabilitar las pruebas de ping. Una de los más comunes es la evaluación de vulnerabilidades intrusivas. Se puede especificar docenas de sondeos de ping diferentes en un intento de obtener una respuesta de todos los hosts disponibles, pero aún es posible que el equipo esté activo pero con muchos firewall no responda a ninguno de esos sondeos.

Por lo tanto, los auditores realizan con frecuencia una intensa exploración, para los 65.536 puertos TCP, contra cada IP en el red de destino. Puede parecer un desperdicio enviar cientos de miles de paquetes a direcciones IP que probablemente no tengan host escuchando, y puede ralentizar tiempos de escaneo en un orden de magnitud o más. Pero los probadores de penetración serios están dispuestos a pagar este precio para evitar incluso un ligero riesgo de perder máquinas activas. Ellos Siempre pueden hacer un escaneo rápido también, dejando que el escaneo masivo se ejecute en segundo plano mientras trabajan.

### <mark style="color:blue;">Técnicas de detección de hosts</mark>

Nmap ofrece una amplia variedad de técnicas de descubrimiento de hosts más allá de la solicitud de eco ICMP estándar. Se describen en las siguientes secciones. Tenga en cuenta que si especifica cualquiera de los siguientes opciones analizadas en esta sección, _reemplazan_ los sondeos de detección predeterminados en lugar de que añadirles algo.

#### <mark style="color:yellow;">Ping TCP SYN (</mark><mark style="color:yellow;">`-PS`</mark>_<mark style="color:yellow;">`<port list>`</mark>_<mark style="color:yellow;">)</mark>

La opción envía un paquete TCP vacío con el conjunto de indicadores SYN. El puerto de destino predeterminado es 80 (configurable en tiempo de compilación cambiando en `-PSDEFAULT_TCP_PROBE_PORT_SPECnmap.h`), puede especificar un puerto alternativo como parámetro. Se puede especificar una lista de puertos (p. ej. _**-PS22-25,80,113,1050,35000**_), en cuyo caso el sondeo se intentarán contra cada puerto en paralelo.

El indicador SYN sugiere al sistema remoto que usted está intentando establecer una conexión. Normalmente, el puerto de destino se cerrará y se devolverá un paquete RST (reinicio). Si el puerto está abierto, el objetivo dará el segundo paso de un TCP protocolo de enlace de tres vías respondiendo con un paquete TCP SYN/ACK. La máquina la ejecución de Nmap luego rompe la conexión naciente respondiendo con un RST en lugar de enviar un paquete ACK que completaría el apretón de manos de tres vías y establecer una conexión completa.

A Nmap no le importa si el puerto está abierto o cerrado. Cualquiera de los dos la respuesta RST o SYN/ACK discutida anteriormente le dice a Nmap que el El host está disponible y responde.

En las máquinas Unix, solo el usuario privilegiado puede enviar y recibir Paquetes TCP sin procesar. Para los usuarios sin privilegios, se emplea automáticamente una solución alternativa mediante la cual la llamada al sistema se inicia en cada puerto de destino. Esto ha el efecto de enviar un paquete SYN al host de destino, en un intento de para establecer una conexión. Si regresa con un éxito rápido o un error ECONNREFUSED, la pila TCP subyacente debe tener recibió un SYN/ACK o RST y el host está marcado como disponible. Si el intento de conexión se deja en suspenso hasta que se alcanza un tiempo de espera, el host está marcado como inactivo. Esta solución alternativa también se utiliza para las conexiones IPv6, ya que la compatibilidad con la creación de paquetes IPv6 sin procesar aún no está disponible en Nmap.

```
sudo nmap -sn -PS80 -R -v google.com 

Starting Nmap 7.94SVN ( https://nmap.org ) at 2024-11-24 00:43 CST
Initiating Ping Scan at 00:43
Scanning google.com (142.250.115.100) [1 port]
Completed Ping Scan at 00:43, 0.09s elapsed (1 total hosts)
Initiating Parallel DNS resolution of 1 host. at 00:43
Completed Parallel DNS resolution of 1 host. at 00:43, 0.11s elapsed
Nmap scan report for google.com (142.250.115.100)
Host is up (0.061s latency).
Other addresses for google.com (not scanned): 142.250.115.138 142.250.115.139 142.250.115.101 142.250.115.113 142.250.115.102
rDNS record for 142.250.115.100: rq-in-f100.1e100.net
Nmap done: 1 IP address (1 host up) scanned in 0.28 seconds
           Raw packets sent: 1 (44B) | Rcvd: 1 (44B)
```

#### <mark style="color:yellow;">Ping TCP ACK (</mark><mark style="color:yellow;">`-PA`</mark>_<mark style="color:yellow;">`<port list>`</mark>_<mark style="color:yellow;">)</mark>

El ping TCP ACK es bastante similar al ping SYN. La diferencia es que el indicador TCP ACK está configurado en lugar de la marca SYN. Un paquete ACK pretende reconocer datos a través de una conexión TCP establecida, pero no existe tal conexión. Por lo tanto, los hosts remotos siempre deben responder con un paquete RST, revelando su existencia en el proceso.

La opción utiliza el mismo puerto predeterminado que la sonda SYN (80) y también puede tomar una lista de puertos de destino en el mismo formato. Si un usuario sin privilegios intenta esto, o un destino IPv6 es especificado, se utiliza la solución alternativa. Esta solución es imperfecta porque en realidad está enviando un SYN en lugar de un ACK.

La razón para ofrecer sondas de ping SYN y ACK es maximizar las posibilidades de eludir los firewall. Muchos administradores configurar routers y otros firewall sencillos para bloquear las entradas paquetes SYN, excepto los destinados a servicios públicos como el sitio web de la empresa o servidor de correo.

Otro tipo común de firewall utiliza reglas con estado que descartan paquetes inesperados. Esta característica se encontró inicialmente principalmente en firewalls de gama alta, aunque se ha vuelto mucho más común a lo largo de los años.

Los estados posibles son INVALID, lo que significa que el paquete no está asociado con ninguna conexión conocida, significado ESTABLECIDO que el paquete está asociado a una conexión que ha visto paquetes en ambas direcciones, NEW significa que el paquete ha iniciado un nuevo conexión, o de otro modo asociada con una conexión que no ha paquetes vistos en ambas direcciones, y RELATED significa que el paquete está iniciando una nueva conexión, pero está asociada a una conexión, como una transferencia de datos FTP o una ICMP error.

```
sudo nmap -sn -PA google.com

Starting Nmap 7.94SVN ( https://nmap.org ) at 2024-11-24 00:53 CST
Nmap scan report for google.com (142.251.116.139)
Host is up (0.00020s latency).
Other addresses for google.com (not scanned): 142.251.116.102 142.251.116.100 142.251.116.101 142.251.116.113 142.251.116.138
rDNS record for 142.251.116.139: rt-in-f139.1e100.net
Nmap done: 1 IP address (1 host up) scanned in 0.19 seconds
```

#### <mark style="color:yellow;">Ping UDP (</mark><mark style="color:yellow;">`-PU`</mark>_<mark style="color:yellow;">`<port list>`</mark>_<mark style="color:yellow;">)</mark>

Otra opción de detección de host es el ping UDP, que envía un paquete UDP a los puertos dados. Si no se especifica ningún puerto, el valor predeterminado es 40.125. Un puerto muy poco común se utiliza de forma predeterminada porque el envío a los puertos abiertos a menudo no son deseables para este tipo de escaneo en particular.

Para la mayoría de los puertos, el paquete estará vacío, aunque para algunos puertos comunes como 53 y 161, un protocolo específico se enviará una carga útil que tenga más probabilidades de obtener una respuesta. La opción envía una carga útil aleatoria de longitud fija para todos los puertos.

Al golpear un puerto cerrado en la máquina de destino, la sonda UDP debería obtener un paquete inalcanzable del puerto ICMP a cambio. Éste significa para Nmap que la máquina está activa y disponible. Muchos otros tipos de errores ICMP, como inalcanzables de host/red o TTL excedidos son indicativos de un host inactivo o inalcanzable. La falta de respuesta también es interpretado de esta manera.&#x20;

Si se llega a un puerto abierto, la mayoría de los servicios simplemente ignora el paquete vacío y no devuelve ninguna respuesta. Éste es por eso que el puerto de sondeo predeterminado es 40,125, que es muy poco probable que esté en uso. Algunos servicios, como el protocolo Character Generator (chargen), responderán a un paquete UDP vacío, y por lo tanto revelar a Nmap que la máquina está disponible. Las cargas útiles personalizadas, para los puertos que las tienen, lo hacen más probable que una sonda obtenga una respuesta.&#x20;

La principal ventaja de este tipo de análisis es que omite firewalls y filtros que solo filtran TCP.

```
sudo nmap -sn -PU google.com

Starting Nmap 7.94SVN ( https://nmap.org ) at 2024-11-24 01:00 CST
Note: Host seems down. If it is really up, but blocking our ping probes, try -Pn
Nmap done: 1 IP address (0 hosts up) scanned in 2.18 seconds
```

#### <mark style="color:yellow;">Tipos de ping ICMP (</mark><mark style="color:yellow;">`-PE, -PP, -PM`</mark><mark style="color:yellow;">)</mark>

Nmap puede enviar los paquetes estándar enviados por el Programa de ping ubicuo. Nmap envía un mensaje ICMP tipo 8 (solicitud de eco) a las direcciones IP de destino, esperando un tipo 0 (respuesta de eco) a cambio de los hosts disponibles. Por lo tanto, los escaneos solo ICMP rara vez son lo suficientemente confiables contra desconocidos objetivos a través de Internet. Pero para los administradores de sistemas de monitoreo una red interna, este puede ser un enfoque práctico y eficiente. Utilice la opción **`-PE`** para habilitar esta solicitud de eco comportamiento.

```
sudo nmap -sn -PE google.com

Starting Nmap 7.94SVN ( https://nmap.org ) at 2024-11-24 01:06 CST
Nmap scan report for google.com (142.250.113.102)
Host is up (0.047s latency).
Other addresses for google.com (not scanned): 142.250.113.100 142.250.113.101 142.250.113.139 142.250.113.113 142.250.113.138
rDNS record for 142.250.113.102: rs-in-f102.1e100.net
Nmap done: 1 IP address (1 host up) scanned in 0.15 seconds
```

Mientras que la solicitud de eco es la consulta de ping ICMP estándar, Nmap no se detiene ahí. **`-PP`** especifica la solicitud de marca de tiempo, la solicitud de información y la máscara de dirección de paquetes de solicitud como códigos 13, 15 y 17, respectivamente.&#x20;

```
sudo nmap -sn -PP google.com

Starting Nmap 7.94SVN ( https://nmap.org ) at 2024-11-24 01:06 CST
Note: Host seems down. If it is really up, but blocking our ping probes, try -Pn
Nmap done: 1 IP address (0 hosts up) scanned in 2.08 seconds
```

Mientras que **`-PM`** su propósito aparente de estas consultas es obtener información como máscaras de dirección y las horas actuales, se pueden usar fácilmente para el host descubrimiento.

```
sudo nmap -sn -PM google.com

Starting Nmap 7.94SVN ( https://nmap.org ) at 2024-11-24 01:06 CST
Note: Host seems down. If it is really up, but blocking our ping probes, try -Pn
Nmap done: 1 IP address (0 hosts up) scanned in 2.17 seconds
```

#### <mark style="color:yellow;">Ping de protocolo IP (</mark><mark style="color:yellow;">`-PO`</mark>_<mark style="color:yellow;">`<protocol list>`</mark>_<mark style="color:yellow;">)</mark>

La opción de detección de host más reciente es el ping del protocolo IP, que envía paquetes IP con el número de protocolo especificado establecido en su encabezado IP. La lista de protocolos toma el mismo formato que las listas de puertos en las opciones de detección de host TCP y UDP.&#x20;

Si no se define ningún protocolo, el valor predeterminado es enviar varios paquetes IP para ICMP (_**protocolo 1**_), IGMP (_**protocolo 2**_) e IP en IP (_**protocolo 4**_).&#x20;

Nota que para el ICMP, IGMP, TCP (_**protocolo 6**_) y UDP (_**protocolo 17**_), los paquetes se envían con los encabezados de protocolo adecuados, mientras que los otros protocolos se envían sin datos adicionales más allá del encabezado IP (a menos que se especifique la opción).

Este método de detección de host busca respuestas mediante el mismo método que una sonda, o mensajes inalcanzables de protocolo ICMP que significan que el protocolo dado no es compatible con el destino anfitrión. Cualquiera de los dos tipos de respuesta significa que el host de destino es vivo.

```
sudo nmap -sn -PO1 google.com

Starting Nmap 7.94SVN ( https://nmap.org ) at 2024-11-24 01:13 CST
Nmap scan report for google.com (142.251.116.101)
Host is up (0.047s latency).
Other addresses for google.com (not scanned): 142.251.116.113 142.251.116.139 142.251.116.100 142.251.116.102 142.251.116.138
rDNS record for 142.251.116.101: rt-in-f101.1e100.net
Nmap done: 1 IP address (1 host up) scanned in 0.18 seconds
```

```
sudo nmap -sn -PO2 google.com
Starting Nmap 7.94SVN ( https://nmap.org ) at 2024-11-24 01:13 CST
Note: Host seems down. If it is really up, but blocking our ping probes, try -Pn
Nmap done: 1 IP address (0 hosts up) scanned in 2.11 seconds

sudo nmap -sn -Pn -PO2 google.com
Starting Nmap 7.94SVN ( https://nmap.org ) at 2024-11-24 01:14 CST
Nmap scan report for google.com (142.250.113.113)
Host is up.
Other addresses for google.com (not scanned): 142.250.113.139 142.250.113.102 142.250.113.100 142.250.113.138 142.250.113.101
rDNS record for 142.250.113.113: rs-in-f113.1e100.net
Nmap done: 1 IP address (1 host up) scanned in 0.09 seconds
```

```
sudo nmap -sn -PO4 google.com
Starting Nmap 7.94SVN ( https://nmap.org ) at 2024-11-24 01:13 CST
Note: Host seems down. If it is really up, but blocking our ping probes, try -Pn
Nmap done: 1 IP address (0 hosts up) scanned in 2.08 seconds

sudo nmap -sn -Pn -PO4 google.com
Starting Nmap 7.94SVN ( https://nmap.org ) at 2024-11-24 01:14 CST
Nmap scan report for google.com (142.250.113.101)
Host is up.
Other addresses for google.com (not scanned): 142.250.113.113 142.250.113.139 142.250.113.102 142.250.113.100 142.250.113.138
rDNS record for 142.250.113.101: rs-in-f101.1e100.net
Nmap done: 1 IP address (1 host up) scanned in 0.05 seconds
```

```
sudo nmap -sn -PO6 google.com
Starting Nmap 7.94SVN ( https://nmap.org ) at 2024-11-24 01:13 CST
Nmap scan report for google.com (142.251.116.138)
Host is up (0.00036s latency).
Other addresses for google.com (not scanned): 142.251.116.102 142.251.116.100 142.251.116.139 142.251.116.113 142.251.116.101
rDNS record for 142.251.116.138: rt-in-f138.1e100.net
Nmap done: 1 IP address (1 host up) scanned in 0.16 seconds

```

```
sudo nmap -sn -PO17 google.com
Starting Nmap 7.94SVN ( https://nmap.org ) at 2024-11-24 01:13 CST
Note: Host seems down. If it is really up, but blocking our ping probes, try -Pn
Nmap done: 1 IP address (0 hosts up) scanned in 2.07 seconds

sudo nmap -sn -Pn -PO17 google.com
Starting Nmap 7.94SVN ( https://nmap.org ) at 2024-11-24 01:14 CST
Nmap scan report for google.com (142.250.113.138)
Host is up.
Other addresses for google.com (not scanned): 142.250.113.101 142.250.113.113 142.250.113.139 142.250.113.102 142.250.113.100
rDNS record for 142.250.113.138: rs-in-f138.1e100.net
Nmap done: 1 IP address (1 host up) scanned in 2.06 seconds
```

#### <mark style="color:yellow;">Escaneo ARP (</mark><mark style="color:yellow;">`-PR`</mark><mark style="color:yellow;">)</mark>

Uno de los escenarios de uso más comunes de Nmap es escanear una LAN Ethernet. En la mayoría de las LAN, especialmente aquellos que utilizan rangos de direcciones privadas otorgados por RFC 1918, la gran mayoría de las direcciones IP no se utilizan en un momento dado. Cuando Nmap intenta enviar un paquete IP sin procesar, como una solicitud de eco ICMP, el sistema operativo debe determinar la dirección de hardware de destino (ARP) correspondiente a la IP de destino para que pueda direccionar correctamente la trama Ethernet. Esto requiere que emita una serie de solicitudes ARP.

La opción le dice a Nmap que envíe paquetes de nivel IP (en lugar de que Ethernet sin procesar) a pesar de que es una red local. Salida de Wireshark de las tres solicitudes ARP y su tiempo se ha pegado en el archivo sesión.

```
sudo nmap -n -sn --send-ip 192.168.23.2   

Starting Nmap 7.94SVN ( https://nmap.org ) at 2024-11-24 01:23 CST
Nmap scan report for 192.168.23.2
Host is up (0.00074s latency).
MAC Address: 08::a6:C3:1D:36 (VMware)
Nmap done: 1 IP address (1 host up) scanned in 0.10 seconds

```

Dado que las respuestas ARP suelen estar en un _**par de milisegundos**_, las esperas de varios segundos son excesivas. Disminuyendo esto el período de tiempo de espera no es una prioridad para los proveedores de sistemas operativos porque la gran mayoría de paquetes se envían a hosts que realmente existen. Nmap, por otro lado, debe enviar paquetes a 16 millones de direcciones IP cuando se le asigna un objetivo como _**10.0.0.0/8**_. Una espera de dos segundos para cada uno se convierte en un gran retraso incluso aunque muchos objetivos se marcan en paralelo.

```
sudo nmap -n -sn --send-ip 10.0.0.0/8  

Starting Nmap 7.94SVN ( https://nmap.org ) at 2024-11-24 01:27 CST
Nmap scan report for 10.0.0.0
Host is up (0.00051s latency).
Nmap scan report for 10.0.0.1
Host is up (0.00011s latency).
Nmap scan report for 10.0.0.2
Host is up (0.000069s latency).
Nmap scan report for 10.0.0.3
Host is up (0.0045s latency).
Nmap scan report for 10.0.0.4
Host is up (0.00072s latency).
Nmap scan report for 10.0.0.5
Host is up (0.0028s latency).
Nmap scan report for 10.0.0.6
Host is up (0.00092s latency).
Nmap scan report for 10.0.0.7
Host is up (0.00013s latency).
Nmap scan report for 10.0.0.8
Host is up (0.000086s latency).
Nmap scan report for 10.0.0.9
Host is up (0.0021s latency).
Nmap scan report for 10.0.0.10

[...]
```

Hay otro problema con los escaneos de ping IP sin procesar en las LAN. Cuando se encuentra que el host de destino no responde, el host de origen generalmente agrega una entrada incompleta para esa IP de destino en la tabla ARP de su kernel.&#x20;

El espacio de la tabla ARP es finito, Y algunos sistemas operativos reaccionan mal cuando se llena. Cuando Nmap es utilizado en modo IP sin procesar (**`--send-ip`**), Nmap a veces tiene esperar varios minutos a que caduquen las entradas de caché ARP antes de que pueda Continúe con la detección de hosts.

El escaneo ARP resuelve ambos problemas al poner a Nmap en control. Nmap emite las solicitudes ARP sin procesar y maneja la retransmisión y períodos de tiempo de espera a su propia discreción. La caché ARP del sistema es Evitado.

El escaneo ARP no solo es más eficiente como se mencionó anteriormente, sino que también es más preciso. Los hosts bloquean con frecuencia los paquetes de ping basados en IP, pero por lo general, no pueden bloquear las solicitudes o respuestas de ARP y aún así comunicarse en la red. Incluso si se especifican diferentes tipos de ping (como **`-PE`** o **`-PS`**), Nmap utiliza ARP en lugar de cualquiera de los objetivos que están en la misma LAN.

Si no desea en absoluto realizar un escaneo ARP, especifique **`--send-ip.`**

Darle a Nmap el control para enviar tramas Ethernet sin procesar también le permite controlar la dirección MAC de origen. Si inicia un escaneo ARP masivo desde una dirección MAC registrada en Apple, es posible que la gente se vuelva hacia usted. Puede falsificar su dirección MAC con la opción **`--spoof-mac.`**

#### <mark style="color:yellow;">Combinación predeterminada</mark>

Si no se elige ninguna de estas técnicas de descubrimiento de host, Nmap utiliza una combinación predeterminada que es equivalente a los argumentos **`-PE -PS443 -PA80 -PP`** para usuarios de Windows o Unix privilegiados (root).&#x20;

```
sudo nmap -PE -PS443 -PA80 -PP google.com

Starting Nmap 7.94SVN ( https://nmap.org ) at 2024-11-24 01:40 CST
Nmap scan report for google.com (142.250.113.113)
Host is up (0.013s latency).
Other addresses for google.com (not scanned): 142.250.113.102 142.250.113.101 142.250.113.139 142.250.113.138 142.250.113.100
rDNS record for 142.250.113.113: rs-in-f113.1e100.net
Not shown: 997 filtered tcp ports (no-response)
PORT    STATE SERVICE
53/tcp  open  domain
80/tcp  open  http
443/tcp open  https

Nmap done: 1 IP address (1 host up) scanned in 5.33 seconds
```

Los lectores atentos saben que esto significa que se envía una solicitud de eco ICMP, un paquete TCP SYN, un paquete TCP ACK y una solicitud de marca de tiempo ICMP a cada máquina. Una excepción a esto es que se utiliza un escaneo ARP para cualquier destino que esté en una red Ethernet local. Para usuarios de shell Unix sin privilegios, el valor predeterminado es equivalente a **`-PS80,443`** (una llamada de conexión TCP contra los puertos 80 y 443 de los hosts de destino).

### <mark style="color:blue;">Juntando todo: Estrategias de descubrimiento de host</mark>

#### <mark style="color:yellow;">Opciones relacionadas</mark>

En las secciones anteriores se describen las principales opciones que se utilizan para controlar la fase de descubrimiento de host de Nmap y personalizar las técnicas utilizadas. Sin embargo, existen muchas más opciones generales de Nmap que son relevantes aquí. Esta sección proporciona una breve descripción de cómo se relacionan estas opciones con el escaneo de ping.

#### <mark style="color:yellow;">-v (igual que --verbose)</mark>

Por defecto, Nmap normalmente sólo imprime los hosts activos y que responden. El modo _**Verbose**_ hace que Nmap imprima los hosts inactivos, así como información adicional sobre los activos.

```
sudo nmap -v google.com

Starting Nmap 7.94SVN ( https://nmap.org ) at 2024-11-24 01:49 CST
Initiating Ping Scan at 01:49
Scanning google.com (142.250.114.139) [4 ports]
Completed Ping Scan at 01:49, 0.02s elapsed (1 total hosts)
Initiating Parallel DNS resolution of 1 host. at 01:49
Completed Parallel DNS resolution of 1 host. at 01:49, 0.06s elapsed
Initiating SYN Stealth Scan at 01:49
Scanning google.com (142.250.114.139) [1000 ports]
Discovered open port 53/tcp on 142.250.114.139
Discovered open port 443/tcp on 142.250.114.139
Discovered open port 80/tcp on 142.250.114.139
Increasing send delay for 142.250.114.139 from 0 to 5 due to 11 out of 15 dropped probes since last increase.
Increasing send delay for 142.250.114.139 from 5 to 10 due to 11 out of 11 dropped probes since last increase.
Completed SYN Stealth Scan at 01:50, 49.93s elapsed (1000 total ports)
Nmap scan report for google.com (142.250.114.139)
Host is up (0.0086s latency).
Other addresses for google.com (not scanned): 142.250.114.138 142.250.114.102 142.250.114.101 142.250.114.100 142.250.114.113
rDNS record for 142.250.114.139: rr-in-f139.1e100.net
Not shown: 997 filtered tcp ports (no-response)
PORT    STATE SERVICE
53/tcp  open  domain
80/tcp  open  http
443/tcp open  https

Read data files from: /usr/bin/../share/nmap
Nmap done: 1 IP address (1 host up) scanned in 50.17 seconds
           Raw packets sent: 2038 (89.500KB) | Rcvd: 1118 (44.732KB)
```

#### <mark style="color:yellow;">--source-port (igual que -g)</mark>&#x20;

Establecer un puerto de origen constante funciona para el escaneo de ping (TCP y UDP) como lo hace con otras características de Nmap. Algunos administradores de firewall ingenuos hacen una excepción de conjunto de reglas para mantener el DNS (puerto 53) o FTP-DATA (puerto 20) funcionando. Por supuesto, esto abre un agujero lo suficientemente grande como para realizar un escaneo de ping de Nmap.

```
sudo nmap --source-port 53 google.com

Starting Nmap 7.94SVN ( https://nmap.org ) at 2024-11-24 01:56 CST
Nmap scan report for google.com (142.250.113.138)
Host is up (0.061s latency).
Other addresses for google.com (not scanned): 142.250.113.139 142.250.113.102 142.250.113.100 142.250.113.101 142.250.113.113
rDNS record for 142.250.113.138: rs-in-f138.1e100.net
All 1000 scanned ports on google.com (142.250.113.138) are in ignored states.
Not shown: 1000 filtered tcp ports (no-response)
```

#### <mark style="color:yellow;">-n, -R</mark>&#x20;

La opción -n deshabilita toda resolución DNS, mientras que la opción -R habilita las consultas DNS para todos los hosts, incluso los inactivos. El comportamiento predeterminado es limitar la resolución DNS a los hosts activos. Estas opciones son particularmente importantes para el escaneo de ping porque la resolución DNS puede afectar en gran medida los tiempos de escaneo.

```
sudo nmap -n nmap.org

Starting Nmap 7.94SVN ( https://nmap.org ) at 2024-11-24 02:01 CST
Failed to resolve "nmap.org".
WARNING: No targets were specified, so 0 hosts scanned.
Nmap done: 0 IP addresses (0 hosts up) scanned in 12.31 seconds
```

```
sudo nmap -R nmap.org

Starting Nmap 7.94SVN ( https://nmap.org ) at 2024-11-24 02:02 CST
Failed to resolve "nmap.org".
WARNING: No targets were specified, so 0 hosts scanned.
Nmap done: 0 IP addresses (0 hosts up) scanned in 9.67 seconds
```

#### <mark style="color:yellow;">--dns-servers \[server1, server2] (Servidores para consultas DNS inversas)</mark>&#x20;

De forma predeterminada, Nmap intentará determinar sus servidores DNS (para la resolución de rDNS) a partir de su archivo resolv.conf (Unix) o del Registro (Win32). Como alternativa, puede utilizar esta opción para especificar servidores alternativos. Esta opción no se respeta si está utilizando **`--system-dns`** o un escaneo de IPv6. El uso de varios servidores DNS suele ser más rápido y más discreto que consultar solo uno. El mejor rendimiento se obtiene a menudo especificando todos los servidores autorizados para el espacio de IP de destino.

```
nmap -Pn --dns-servers 8.8.8.8, 1.1.1.1 ochobitshacenunbyte.com 

Starting Nmap 7.94SVN ( https://nmap.org ) at 2024-11-24 02:25 CST
Failed to resolve "ochobitshacenunbyte.com".
Failed to resolve "ochobitshacenunbyte.com".
Nmap scan report for 1.1.1.1
Host is up (0.063s latency).
All 1000 scanned ports on 1.1.1.1 are in ignored states.
Not shown: 990 filtered tcp ports (no-response), 10 filtered tcp ports (host-unreach)

Failed to resolve "ochobitshacenunbyte.com".
Nmap done: 1 IP address (1 host up) scanned in 54.84 seconds

```

#### <mark style="color:yellow;">--data-length  \<valor></mark>

Esta opción añade bytes aleatorios de datos a cada paquete y funciona con los tipos de escaneo de ping TCP, UDP e ICMP (para usuarios privilegiados que escanean IPv4). Esto ayuda a que el escaneo sea menos visible y más parecido a los paquetes generados por el omnipresente programa de diagnóstico de ping. Varios sistemas de detección de intrusiones (IDS), incluido Snort, tienen alertas para paquetes de ping de cero bytes. Esta opción evade esas alertas. Un valor de opción de 32 hace que una solicitud de eco parezca más como si viniera de Windows, mientras que 56 simula el ping predeterminado de Linux.

```
sudo nmap --data-length 32 github.com             

Starting Nmap 7.94SVN ( https://nmap.org ) at 2024-11-24 02:36 CST
Nmap scan report for github.com (140.82.112.3)
Host is up (0.070s latency).
rDNS record for 140.82.112.3: lb-140-82-112-3-iad.github.com
Not shown: 997 filtered tcp ports (no-response)
PORT    STATE SERVICE
22/tcp  open  ssh
80/tcp  open  http
443/tcp open  https

Nmap done: 1 IP address (1 host up) scanned in 60.78 seconds

```

```
sudo nmap --data-length 56 github.com
Starting Nmap 7.94SVN ( https://nmap.org ) at 2024-11-24 02:38 CST
Nmap scan report for github.com (140.82.112.4)
Host is up (0.022s latency).
rDNS record for 140.82.112.4: lb-140-82-112-4-iad.github.com
Not shown: 997 filtered tcp ports (no-response)
PORT    STATE SERVICE
22/tcp  open  ssh
80/tcp  open  http
443/tcp open  https

Nmap done: 1 IP address (1 host up) scanned in 21.05 seconds
```

#### <mark style="color:yellow;">--ttl \<valor></mark>

La configuración del TTL de salida es compatible con los usuarios privilegiados que realizan escaneos de ping IPv4. Esto puede ser útil como medida de seguridad para garantizar que un escaneo no se propague más allá de la red local. También se puede utilizar para simular un programa de ping nativo de forma aún más convincente. Algunas redes empresariales sufren bucles de enrutamiento conocidos que no pueden solucionar fácilmente. Reducir el TTL de salida con --ttl ayuda a reducir la carga de la CPU del enrutador cuando se encuentran bucles.

#### <mark style="color:yellow;">Tiempo predefinidas (-T3, -T4, -T5, etc.)</mark>&#x20;

Los valores de **`-T`** más altos aceleran el escaneo de ping, al igual que aceleran otras funciones de Nmap. Con una conexión moderadamente rápida y confiable entre las redes de origen y destino (es decir, cualquier cosa que no sea un módem de acceso telefónico), se recomienda la opción -T4.

```
sudo nmap -T4 github.com

Starting Nmap 7.94SVN ( https://nmap.org ) at 2024-11-24 02:34 CST
Nmap scan report for github.com (140.82.113.3)
Host is up (0.066s latency).
rDNS record for 140.82.113.3: lb-140-82-113-3-iad.github.com
Not shown: 987 filtered tcp ports (no-response)
PORT      STATE  SERVICE
22/tcp    open   ssh
80/tcp    open   http
443/tcp   open   https
1029/tcp  closed ms-lsa
2106/tcp  closed ekshell
3269/tcp  closed globalcatLDAPssl
3878/tcp  closed fotogcad
3920/tcp  closed exasoftport1
5100/tcp  closed admd
5998/tcp  closed ncd-diag
7911/tcp  closed unknown
14000/tcp closed scotty-ft
49167/tcp closed unknown

Nmap done: 1 IP address (1 host up) scanned in 74.05 seconds
```

#### <mark style="color:yellow;">--max-parallelism, --min-parallelism \<valor></mark>

Estas opciones afectan la cantidad de sondas que pueden estar pendientes a la vez. Con el tipo de ping predeterminado (2 sondas), el valor de paralelismo es aproximadamente la cantidad de máquinas escaneadas en paralelo. Reducir las técnicas de ping a una sonda por host (por ejemplo, -PE) duplicará la cantidad de hosts escaneados a la vez para un nivel de paralelismo dado, mientras que aumentar a cuatro sondas por host (por ejemplo, -PE -PS22,113,50000) lo reduce a la mitad. La mayoría de los usuarios simplemente se apegan a las opciones de tiempo predeterminadas, como -T4.

#### <mark style="color:yellow;">--min-rtt-timeout, --max-rtt-timeout, --initial-rtt-timeout \<tiempo></mark>

Estas opciones controlan cuánto tiempo espera Nmap una respuesta de ping.

#### <mark style="color:yellow;">Opciones de entrada (-iL \<archivo.txt> , -iR \<número>)</mark>&#x20;

Las opciones de entrada de host se admiten como en el resto de Nmap. Los usuarios suelen combinar la opción de entrada desde lista **`-iL`** con -Pn para evitar escanear con ping los hosts que ya se sabe que están activos.&#x20;

La opción **`-iR`** elige hosts al azar del espacio de IP de Internet asignado. Toma como argumento la cantidad de hosts aleatorios que desea escanear. Use cero para un escaneo sin fin (hasta que cancele o mate el proceso de Nmap).

#### <mark style="color:yellow;">Opciones de salida (-oA, -oN, -oG, -oX, etc.)</mark>&#x20;

Todos los tipos de salida de Nmap (normal, grepable y XML) admiten el escaneo con ping.

#### <mark style="color:yellow;">--randomize-hosts</mark>&#x20;

Si se cambia el orden de escaneo de los hosts con esta opción, el escaneo puede resultar menos visible, aunque también puede hacer que la salida del escaneo sea un poco más difícil de seguir.

#### <mark style="color:yellow;">--reason</mark>&#x20;

La salida normal de Nmap indica si un host está activo o no, pero no describe a qué prueba(s) de descubrimiento respondió el host. Para este detalle, agregue la opción **`--reason`**. Los resultados pueden ser confusos para el descubrimiento de hosts, ya que Nmap no siempre prueba cada sonda. Se detiene tan pronto como obtiene una primera respuesta. Por lo tanto, Nmap puede informar una respuesta de eco ICMP de un host durante la ejecución, pero luego puede recibir una respuesta RST primero durante una segunda ejecución y hacer que Nmap informe eso.

#### <mark style="color:yellow;">--packet-trace</mark>&#x20;

Si desea más detalles que los que ofrece **`--reason`**, pruebe con **`--packet-trace`**. Esta opción muestra todos los paquetes enviados y recibidos por Nmap, incluidos detalles como números de secuencia, valores TTL y banderas TCP.

#### <mark style="color:yellow;">-D \<señuelo1, señuelo2, señuelo3></mark>&#x20;

Los señuelos son totalmente compatibles con los escaneos de ping de IPv4 privilegiados, lo que camufla al verdadero atacante.

#### <mark style="color:yellow;">-6</mark>&#x20;

Los escaneos de ping basados ​​en conexión TCP (-PS) admiten el protocolo IPv6, incluido el modo multipuerto (como -PS22,80,113.

#### <mark style="color:yellow;">-S \<IP origen>, -e \<Dispositivo de envío></mark>&#x20;

Al igual que con otras funciones de Nmap, la dirección de origen y el dispositivo de envío se pueden especificar con estas opciones.

#### <mark style="color:yellow;">Opciones generales</mark>

De manera predeterminada, a menos que se especifiquen **`-sn`** o **`-sL`**, Nmap pasa a un escaneo más intrusivo después de la etapa de descubrimiento del host. Por lo tanto, se pueden utilizar muchas docenas de opciones generales de escaneo de puertos, detección de SO y detección de versiones. Consulte la guía de referencia o los capítulos relevantes para obtener más información.

#### <mark style="color:yellow;">Elección y combinación de opciones de ping</mark>

Para que el escaneo sea eficaz, es necesario algo más que conocer todas las opciones descritas en esta sección y en las anteriores. Los usuarios deben comprender cómo y cuándo utilizarlas para adaptarse a la topología de la red de destino y a los objetivos del escaneo.
