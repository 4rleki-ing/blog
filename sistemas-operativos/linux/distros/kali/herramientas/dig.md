---
description: >-
  El comando dig (Domain Information Groper), es una herramienta potente de red
  para consultar servidores del sistema de nombres de dominio (DNS).
icon: face-clouds
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

# Dig

**`dig`** ayuda a diagnosticar y resolver problemas relacionados con el DNS, esenciales para mantener la estabilidad y el rendimiento de la red.

## <mark style="color:orange;">Instalación</mark>

```
sudo apt-get update
```

```
sudo apt-get install dnsutils
```

Después verifica que la instalación haya sido correcta

```
dig -v
```

## <mark style="color:orange;">Sintaxis</mark>

```
dig [server] [name] [type]
```

#### <mark style="color:green;">Donde</mark>

* **`[server]`**: Dirección IP o el nombre de host del servidor DNS a consultar. **dig** utilizará los servidores DNS listados en _**/etc/resolv.conf**_ si se omite. _(Opcional)_
* **`[name]`:** el nombre de dominio a consultar. Es el registro de recursos DNS sobre el que quieres información.
* **`[type]`:** el tipo de registro DNS a consultar, incluyendo A, MX y NS. **dig** consultará un registro A si no se especifica ningún tipo por defecto. _(Opcional)_

Para realizar una consulta del registro A:

```
dig google.com
```

Se obtendrá el resultado:

```
; <<>> DiG 9.20.0-Debian <<>> google.com
;; global options: +cmd
;; Got answer:
;; ->>HEADER<<- opcode: QUERY, status: NOERROR, id: 39976
;; flags: qr rd ra; QUERY: 1, ANSWER: 6, AUTHORITY: 4, ADDITIONAL: 3

;; QUESTION SECTION:
;google.com.			IN	A

;; ANSWER SECTION:
google.com.		5	IN	A	142.251.116.102
google.com.		5	IN	A	142.251.116.139
google.com.		5	IN	A	142.251.116.113
google.com.		5	IN	A	142.251.116.138
google.com.		5	IN	A	142.251.116.101
google.com.		5	IN	A	142.251.116.100

;; AUTHORITY SECTION:
google.com.		5	IN	NS	ns1.google.com.
google.com.		5	IN	NS	ns4.google.com.
google.com.		5	IN	NS	ns2.google.com.
google.com.		5	IN	NS	ns3.google.com.

;; ADDITIONAL SECTION:
ns1.google.com.		5	IN	A	216.239.32.10
ns4.google.com.		5	IN	A	216.239.38.10
ns2.google.com.		5	IN	A	216.239.34.10

;; Query time: 39 msec
;; SERVER: 192.168.23.2#53(192.168.23.2) (UDP)
;; WHEN: Sat Nov 23 20:44:43 CST 2024
;; MSG SIZE  rcvd: 244
```

## <mark style="color:orange;">Opciones</mark>

El comando **dig** ofrece varias opciones para personalizar las consultas y salidas DNS. Éstas son algunas de las más utilizadas:

* **+short:** muestra sólo la información más relevante, como la dirección IP de un registro A.
* **+noall:** suprime todas las secciones de la salida excepto las solicitadas explícitamente.
* **+answer:** muestra sólo la sección de respuesta de la salida. Suele utilizarse con **+noall**.
* **+trace:** realiza un rastreo completo del proceso de resolución DNS desde los servidores raíz hasta los servidores autoritativos.
* **@server:** especifica un servidor DNS diferente al que consultar en lugar del predeterminado.
* **-x:** realiza una búsqueda DNS inversa, traduciendo una dirección IP a un nombre de dominio.
* **+multi:** formatea la salida para que sea más legible, lo que resulta útil cuando se trabaja con múltiples registros DNS.
* **+nocmd:** omite la línea de órdenes inicial de la salida, mostrando sólo los resultados.
* **+stats:** muestra la sección de estadísticas, que incluye el tiempo de consulta y los detalles del servidor.

También puedes utilizar varias opciones en un comando para personalizar aún más la salida.

```
dig @8.8.8.8 google.com +short +trace
```

Obteniendo el siguiente resultado

```
NS a.root-servers.net. from server 8.8.8.8 in 68 ms.
NS b.root-servers.net. from server 8.8.8.8 in 68 ms.
NS c.root-servers.net. from server 8.8.8.8 in 68 ms.
NS d.root-servers.net. from server 8.8.8.8 in 68 ms.
NS e.root-servers.net. from server 8.8.8.8 in 68 ms.
NS f.root-servers.net. from server 8.8.8.8 in 68 ms.
NS g.root-servers.net. from server 8.8.8.8 in 68 ms.
NS h.root-servers.net. from server 8.8.8.8 in 68 ms.
NS i.root-servers.net. from server 8.8.8.8 in 68 ms.
NS j.root-servers.net. from server 8.8.8.8 in 68 ms.
NS k.root-servers.net. from server 8.8.8.8 in 68 ms.
NS l.root-servers.net. from server 8.8.8.8 in 68 ms.
NS m.root-servers.net. from server 8.8.8.8 in 68 ms.
A 142.250.113.100 from server 192.5.5.241 in 20 ms.
A 142.250.113.138 from server 192.5.5.241 in 20 ms.
A 142.250.113.113 from server 192.5.5.241 in 20 ms.
A 142.250.113.101 from server 192.5.5.241 in 20 ms.
A 142.250.113.139 from server 192.5.5.241 in 20 ms.
A 142.250.113.102 from server 192.5.5.241 in 20 ms.
```

## <mark style="color:orange;">Uso</mark>

### <mark style="color:yellow;">Consultar DNS específico</mark>

#### <mark style="color:green;">Registro SOA</mark>

```
dig google.com SOA
```

```
; <<>> DiG 9.20.0-Debian <<>> google.com SOA
;; global options: +cmd
;; Got answer:
;; ->>HEADER<<- opcode: QUERY, status: NOERROR, id: 14038
;; flags: qr rd ra; QUERY: 1, ANSWER: 1, AUTHORITY: 4, ADDITIONAL: 3

;; QUESTION SECTION:
;google.com.			IN	SOA

;; ANSWER SECTION:
google.com.		5	IN	SOA	ns1.google.com. dns-admin.google.com. 698728253 900 900 1800 60

;; AUTHORITY SECTION:
google.com.		5	IN	NS	ns2.google.com.
google.com.		5	IN	NS	ns3.google.com.
google.com.		5	IN	NS	ns1.google.com.
google.com.		5	IN	NS	ns4.google.com.

;; ADDITIONAL SECTION:
ns2.google.com.		5	IN	A	216.239.34.10
ns1.google.com.		5	IN	A	216.239.32.10
ns4.google.com.		5	IN	A	216.239.38.10

;; Query time: 32 msec
;; SERVER: 192.168.23.2#53(192.168.23.2) (UDP)
;; WHEN: Sat Nov 23 21:23:29 CST 2024
;; MSG SIZE  rcvd: 194
```

#### <mark style="color:green;">Registro MX</mark>

```
dig google.com MX
```

```
; <<>> DiG 9.20.0-Debian <<>> google.com MX
;; global options: +cmd
;; Got answer:
;; ->>HEADER<<- opcode: QUERY, status: NOERROR, id: 22319
;; flags: qr rd ra; QUERY: 1, ANSWER: 1, AUTHORITY: 4, ADDITIONAL: 3

;; QUESTION SECTION:
;google.com.			IN	MX

;; ANSWER SECTION:
google.com.		5	IN	MX	10 smtp.google.com.

;; AUTHORITY SECTION:
google.com.		5	IN	NS	ns2.google.com.
google.com.		5	IN	NS	ns3.google.com.
google.com.		5	IN	NS	ns1.google.com.
google.com.		5	IN	NS	ns4.google.com.

;; ADDITIONAL SECTION:
ns2.google.com.		5	IN	A	216.239.34.10
ns1.google.com.		5	IN	A	216.239.32.10
ns4.google.com.		5	IN	A	216.239.38.10

;; Query time: 75 msec
;; SERVER: 192.168.23.2#53(192.168.23.2) (UDP)
;; WHEN: Sat Nov 23 21:24:30 CST 2024
;; MSG SIZE  rcvd: 169
```

#### <mark style="color:green;">Registro NS</mark>

```
dig google.com NS
```

```
; <<>> DiG 9.20.0-Debian <<>> google.com NS
;; global options: +cmd
;; Got answer:
;; ->>HEADER<<- opcode: QUERY, status: NOERROR, id: 49494
;; flags: qr rd ra; QUERY: 1, ANSWER: 4, AUTHORITY: 4, ADDITIONAL: 6

;; QUESTION SECTION:
;google.com.			IN	NS

;; ANSWER SECTION:
google.com.		5	IN	NS	ns1.google.com.
google.com.		5	IN	NS	ns4.google.com.
google.com.		5	IN	NS	ns2.google.com.
google.com.		5	IN	NS	ns3.google.com.

;; AUTHORITY SECTION:
google.com.		5	IN	NS	ns4.google.com.
google.com.		5	IN	NS	ns2.google.com.
google.com.		5	IN	NS	ns3.google.com.
google.com.		5	IN	NS	ns1.google.com.

;; ADDITIONAL SECTION:
ns1.google.com.		5	IN	A	216.239.32.10
ns4.google.com.		5	IN	A	216.239.38.10
ns2.google.com.		5	IN	A	216.239.34.10
ns4.google.com.		5	IN	A	216.239.38.10
ns2.google.com.		5	IN	A	216.239.34.10
ns1.google.com.		5	IN	A	216.239.32.10

;; Query time: 39 msec
;; SERVER: 192.168.23.2#53(192.168.23.2) (UDP)
;; WHEN: Sat Nov 23 21:25:04 CST 2024
;; MSG SIZE  rcvd: 252
```

### <mark style="color:yellow;">Consultar un servidor DNS concreto</mark>

Puedes utilizar **dig** para pedir información a un servidor DNS concreto en lugar de confiar en los configurados por defecto en tu sistema. Es útil para probar y comparar las respuestas de distintos servidores DNS.

<mark style="color:green;">**Consulta al servidor DNS público de Google.com**</mark>

```
dig @8.8.8.8 google.com
```

```
; <<>> DiG 9.20.0-Debian <<>> @8.8.8.8 google.com
; (1 server found)
;; global options: +cmd
;; Got answer:
;; ->>HEADER<<- opcode: QUERY, status: NOERROR, id: 35077
;; flags: qr rd ra; QUERY: 1, ANSWER: 6, AUTHORITY: 4, ADDITIONAL: 3

;; QUESTION SECTION:
;google.com.			IN	A

;; ANSWER SECTION:
google.com.		136	IN	A	142.250.113.139
google.com.		136	IN	A	142.250.113.113
google.com.		136	IN	A	142.250.113.138
google.com.		136	IN	A	142.250.113.102
google.com.		136	IN	A	142.250.113.101
google.com.		136	IN	A	142.250.113.100

;; AUTHORITY SECTION:
google.com.		11788	IN	NS	ns3.google.com.
google.com.		11788	IN	NS	ns1.google.com.
google.com.		11788	IN	NS	ns4.google.com.
google.com.		11788	IN	NS	ns2.google.com.

;; ADDITIONAL SECTION:
ns1.google.com.		44390	IN	A	216.239.32.10
ns4.google.com.		44390	IN	A	216.239.38.10
ns2.google.com.		44390	IN	A	216.239.34.10

;; Query time: 87 msec
;; SERVER: 8.8.8.8#53(8.8.8.8) (UDP)
;; WHEN: Sat Nov 23 21:28:42 CST 2024
;; MSG SIZE  rcvd: 244
```

### <mark style="color:yellow;">Servidores DNS</mark>

<mark style="color:green;">OpenDNS</mark>

OpenDNS lleva casi 20 año siendo una de las principales referencias en el mundo de las DNS públicas. Además de su opción básica, ofrece también un paquete familiar (igualmente gratuito, aunque con distinta dirección de DNS) que bloquea por defecto contenido adulto. Conocido por su robustez y seguridad, OpenDNS filtra por defecto webs vinculadas a estafas de phishing y ofrece hasta 50 filtros personalizables para controlar el tipo de contenidos que deseas bloquear, lo que lo hace ideal para familias y empresas.

* DNS primario: 208.67.222.222
* DNS Secundario: 208.67.220.220

#### <mark style="color:green;">Google Public DNS</mark> <a href="#id-2-google-public-dns-3" id="id-2-google-public-dns-3"></a>

Lanzado por Google a finales de 2009, su documentación online está pensada para los usuarios más inexpertos. No cuenta con filtros para personalizar tu navegación (como OpenDNS), pero sí nos ofrece protección contra ataques populares (como los DDoS o el de envenenamiento de caché DNS​). Google Public DNS es popular por su velocidad (es uno de los servicios DNS más veloces). Es fácil de usar para principiantes y promete privacidad mediante la eliminación de IPs en 24-48 horas.

* DNS Primario: 8.8.8.8
* DNS Secundario: 8.8.4.4

#### <mark style="color:green;">Cloudflare</mark> <a href="#id-3-cloudflare-4" id="id-3-cloudflare-4"></a>

Como el de Google, el DNS de Cloudflare es un servicio tan básico como veloz... pero, al contrario que aquél, incide mucho en la privacidad, prometiendo que jamás escribirá nuestra IP en un disco duro, por ejemplo (aspecto que respalda con auditorías externas). Cloudflare se destaca por su velocidad excepcional y su compromiso con la privacidad, prometiendo no utilizar tus datos para publicidad y borrar cualquier log dentro de un margen de 24 horas.

* DNS Primario: 1.1.1.1
* DNS Secundario: 1.0.0.1

#### <mark style="color:green;">Quad9</mark> <a href="#id-4-quad9-5" id="id-4-quad9-5"></a>

Más joven que sus principales rivales (activo desde 2016), este servicio no pretende destacar en velocidad (aunque se sitúe aún por encima de la media), sino en seguridad, ofreciendo funcionalidades como la protección frente a amenazas online, el bloqueo por defecto los dominios maliciosos, o el whitelisting. Quad9 ofrece un enfoque en la seguridad, utilizando múltiples bases de datos de inteligencia sobre amenazas para bloquear sitios peligrosos. Ofrece un buen balance entre velocidad, seguridad y privacidad.

* DNS Primario: 9.9.9.9
* DNS Secundario: 149.112.112.112

#### <mark style="color:green;">Comodo Secure DNS</mark> <a href="#id-5-comodo-secure-dns-6" id="id-5-comodo-secure-dns-6"></a>

Siendo un servicio de una empresa de ciberseguridad, no es de extrañar que éste sea su fuerte: no sólo bloquea webs de phishing, sino que nos advierte cuando accedemos a sitios web con malware, spyware o meramente con excesos de anuncios. Su función Dome Shield ofrece, en su versión gratuita, bloqueo de peticiones de IP maliciosas. Especializado en seguridad, Comodo Secure DNS bloquea sitios peligrosos y ofrece configuraciones personalizables para una navegación más segura.

* DNS Primario: 8.26.56.26
* DNS Secundario: 8.20.247.20

#### <mark style="color:green;">AdGuard</mark> <a href="#id-6-adguard-7" id="id-6-adguard-7"></a>

Especializado en el bloqueo de anuncios a nivel de red (tanto en vídeos o páginas web como en videojuegos), AdGuard DNS ofrece también filtros para contenidos inapropiados y protección contra phishing y malware.

* DNS Primario: 185.228.168.168
* DNS Secundario: 185.228.169.168

#### <mark style="color:green;">Verisign</mark>

Este servicio ofrece una velocidad que no es la más alta, pero sí buena, con conexiones fiables. Así, evitarás las molestas caídas de conexión que se suelen dar en algunos de estos servicios. Solo recopilan los datos con fines de análisis. La privacidad y seguridad son sus principales puntos fuertes. Incluye 13 servidores gratuitos que ofertan conexiones seguras y rápidas desde cualquier lugar del mundo. Aunque **no tiene adblocker** (bloqueador de anuncios), sí que protege tu ordenador ante **ataques y vulnerabilidades** para protegerte mientras lo estás utilizando, así te protegerás ante los ciberataques que puedan presentarte en su navegación.

* DNS Primario: 64.6.64.6
* DNS Secundario: 64.6.65.6

#### <mark style="color:green;">FreeDNS</mark>

Este servicio cuenta con servidores en **Austria, Alemania, Estados Unidos y Singapur.** No guarda registros de actividad ni requiere que te crees una cuenta para utilizarlo. Es una buena solución gratuita a la que recurren muchas personas, pero no tiene protección contra webs maliciosas, bots, estafas de suplantación de identidad ni ciberataques, por lo que tendrás que extremar las precauciones. Destaca por ser fácil de utilizar y contar con una gran cantidad de características. No necesitas registrarte ni recurrir a un redireccionador de DNS con este servicio, ya que lo podrás hacer con sus IP.

* DNS Primario: 37.235.1.174
* DNS Secundario: 37.235.1.177

#### <mark style="color:green;">NextDNS</mark>

NextDNS es una solución de filtrado y seguridad DNS en la nube que proporciona diversas funciones avanzadas. Además de bloquear el acceso a sitios web maliciosos, NextDNS permite a los usuarios personalizar sus políticas de filtrado según sus necesidades específicas.

* DNS Primario IPv4: 45.90.28.0
* DNS Primario IPv6: 2a07:a8c0::

#### <mark style="color:green;">SafeServe</mark>

SafeServe es un producto de Namecheap que también funciona orientándose a la protección de los datos y la privacidad del usuario. Sus principales ventajas son: seguridad, protegiéndote frente a ataques como los denominados Man in the Middle, porque ahora este «medio» es completamente seguro; privacidad total, al mantener las solicitudes y respuestas DNS privadas, y los datos del usuario lejos de cualquier actor externo; confianza, pudiendo disfrutar de «los más altos niveles de tiempo de actividad a través de nuestros servidores DNS en Europa y Estados Unidos», como explican desde Namecheap.

* DNS Primario: 198.54.117.10
* DNS Secundario: 198.54.117.11

#### <mark style="color:green;">CyberGhost</mark>

Estos son unos de los mejores **públicos y gratuitos** con los que podrás disfrutar de una mayor privacidad, seguridad y velocidad en el acceso a Internet. Son una excelente alternativa si estás buscando un servicio gratuito con el que acceder a contenidos de Internet como vídeos, página web y muchos otros. También podrás incrementar tu seguridad online con CyberGhost VPN.

* DNS Primario: 38.132.106.139
* DNS Secundario: 194.187.251.67

#### <mark style="color:green;">Más DNS gratuitos que debes conocer</mark>

Aunque antes te hemos mencionado los que suelen ser más famosos y que están más recomendados, la realidad es que vas a encontrar decenas de DNS que pueden resultarte interesantes. Posiblemente necesitaríamos páginas y páginas para compartirte todas las opciones posibles, pero hemos decidido reunir una **pequeña selección de otras opciones gratis** que son recomendables. Toma nota de ellos

* Level3 – 209.244.0.3 y 209.244.0.4
* WATCH – 84.200.69.80 y 84.200.70.40
* GreenTeamDNS – 81.218.119.11 y 209.88.198.133
* SafeDNS – 195.46.39.39 y 195.46.39.40
* OpenNIC – 96.90.175.167 y 193.183.98.154
* SmartViper – 208.76.50.50 y 208.76.51.51
* Dyn – 216.146.35.35 y 216.146.36.36
* Alternate DNS – 198.101.242.72 y 23.253.163.53
* DNS – 77.88.8.8 y 77.88.8.1
* UncensoredDNS – 91.239.100.100 y 89.233.43.71
* Hurricane Electric – 74.82.42.42
* puntCAT – 109.69.8.51
* Neustar – 156.154.70.1 y 156.154.71.1
* Fourth Estate – 45.77.165.194
* UltraDNS – 156.154.70.1, 156.154.71.1
* UltraDNS Family – 156.154.70.3 y 156.154.71.3

### <mark style="color:yellow;">**Consulta a un servidor de nombres autoritativo**</mark>

Los servidores de nombres autoritativos proporcionan la respuesta definitiva a las consultas DNS sobre dominios, garantizando que obtienes la respuesta más precisa.

```
dig @ns1.ejemplo.com google.com
```

Si tus configuraciones son correctas, verás una salida similar a la anterior.

### <mark style="color:yellow;">Rastrear la ruta DNS</mark>

Rastrear la ruta DNS implica seguir una consulta DNS desde tu ordenador hasta el servidor de nombres autoritativo. Este proceso te permite ver la ruta que siguen las consultas hasta el servidor DNS final.

```
dig google.com +trace
```

```
; <<>> DiG 9.20.0-Debian <<>> google.com +trace
;; global options: +cmd
.			5	IN	NS	g.root-servers.net.
.			5	IN	NS	h.root-servers.net.
.			5	IN	NS	i.root-servers.net.
.			5	IN	NS	j.root-servers.net.
.			5	IN	NS	k.root-servers.net.
.			5	IN	NS	l.root-servers.net.
.			5	IN	NS	m.root-servers.net.
.			5	IN	NS	a.root-servers.net.
.			5	IN	NS	b.root-servers.net.
.			5	IN	NS	c.root-servers.net.
.			5	IN	NS	d.root-servers.net.
.			5	IN	NS	e.root-servers.net.
.			5	IN	NS	f.root-servers.net.
.			5	IN	NS	h.root-servers.net.
.			5	IN	NS	i.root-servers.net.
.			5	IN	NS	j.root-servers.net.
.			5	IN	NS	k.root-servers.net.
.			5	IN	NS	l.root-servers.net.
.			5	IN	NS	m.root-servers.net.
.			5	IN	NS	a.root-servers.net.
.			5	IN	NS	b.root-servers.net.
.			5	IN	NS	c.root-servers.net.
.			5	IN	NS	d.root-servers.net.
.			5	IN	NS	e.root-servers.net.
.			5	IN	NS	f.root-servers.net.
.			5	IN	NS	g.root-servers.net.
;; Received 509 bytes from 192.168.23.2#53(192.168.23.2) in 20 ms

google.com.		9	IN	A	142.250.114.113
google.com.		9	IN	A	142.250.114.139
google.com.		9	IN	A	142.250.114.101
google.com.		9	IN	A	142.250.114.100
google.com.		9	IN	A	142.250.114.102
google.com.		9	IN	A	142.250.114.138
google.com.		10189	IN	NS	ns2.google.com.
google.com.		10189	IN	NS	ns3.google.com.
google.com.		10189	IN	NS	ns1.google.com.
google.com.		10189	IN	NS	ns4.google.com.
;; Received 244 bytes from 192.36.148.17#53(i.root-servers.net) in 72 ms
```

### <mark style="color:yellow;">Mostrar sólo la sección de respuestas</mark>

Utilizando el comando **dig**, puedes filtrar la salida para mostrar una información más limpia y legible, al tiempo que eliminas detalles innecesarios, lo que agiliza el análisis de los resultados.

```
dig google.com +noall +answer
```

```
google.com.		5	IN	A	142.250.113.102
google.com.		5	IN	A	142.250.113.138
google.com.		5	IN	A	142.250.113.139
google.com.		5	IN	A	142.250.113.113
google.com.		5	IN	A	142.250.113.101
google.com.		5	IN	A	142.250.113.100
```

### <mark style="color:yellow;">Formatear la salida</mark>

De forma similar a mostrar sólo la sección de respuestas, formatear la salida te permite personalizar la forma en que se muestran los resultados para hacerlos más legibles y fáciles de analizar.

#### <mark style="color:green;">+short</mark>

```
dig google.com +short
```

```
142.250.113.100
142.250.113.101
142.250.113.113
142.250.113.139
142.250.113.138
142.250.113.102
```

#### <mark style="color:green;">+multi</mark>

```
dig google.com +multi
```

```
; <<>> DiG 9.20.0-Debian <<>> google.com +multi
;; global options: +cmd
;; Got answer:
;; ->>HEADER<<- opcode: QUERY, status: NOERROR, id: 10326
;; flags: qr rd ra; QUERY: 1, ANSWER: 6, AUTHORITY: 0, ADDITIONAL: 1

;; OPT PSEUDOSECTION:
; EDNS: version: 0, flags:; MBZ: 0x0005, udp: 4096
;; QUESTION SECTION:
;google.com.		IN A

;; ANSWER SECTION:
google.com.		5 IN A	142.250.113.102
google.com.		5 IN A	142.250.113.100
google.com.		5 IN A	142.250.113.101
google.com.		5 IN A	142.250.113.113
google.com.		5 IN A	142.250.113.139
google.com.		5 IN A	142.250.113.138

;; Query time: 4 msec
;; SERVER: 192.168.23.2#53(192.168.23.2) (UDP)
;; WHEN: Sat Nov 23 21:59:00 CST 2024
;; MSG SIZE  rcvd: 135
```

#### <mark style="color:green;">+nocmd</mark>

```
dig google.com +nocmd
```

```
;; Got answer:
;; ->>HEADER<<- opcode: QUERY, status: NOERROR, id: 40878
;; flags: qr rd ra; QUERY: 1, ANSWER: 6, AUTHORITY: 0, ADDITIONAL: 1

;; OPT PSEUDOSECTION:
; EDNS: version: 0, flags:; MBZ: 0x0005, udp: 4096
;; QUESTION SECTION:
;google.com.			IN	A

;; ANSWER SECTION:
google.com.		5	IN	A	142.250.113.138
google.com.		5	IN	A	142.250.113.102
google.com.		5	IN	A	142.250.113.100
google.com.		5	IN	A	142.250.113.101
google.com.		5	IN	A	142.250.113.113
google.com.		5	IN	A	142.250.113.139

;; Query time: 4 msec
;; SERVER: 192.168.23.2#53(192.168.23.2) (UDP)
;; WHEN: Sat Nov 23 21:59:39 CST 2024
;; MSG SIZE  rcvd: 135
```

#### <mark style="color:green;">+comments</mark>

```
dig google.com +comments
```

```
; <<>> DiG 9.20.0-Debian <<>> google.com +comments
;; global options: +cmd
;; Got answer:
;; ->>HEADER<<- opcode: QUERY, status: NOERROR, id: 37947
;; flags: qr rd ra; QUERY: 1, ANSWER: 6, AUTHORITY: 4, ADDITIONAL: 3

;; QUESTION SECTION:
;google.com.			IN	A

;; ANSWER SECTION:
google.com.		5	IN	A	142.250.114.100
google.com.		5	IN	A	142.250.114.102
google.com.		5	IN	A	142.250.114.113
google.com.		5	IN	A	142.250.114.139
google.com.		5	IN	A	142.250.114.138
google.com.		5	IN	A	142.250.114.101

;; AUTHORITY SECTION:
google.com.		5	IN	NS	ns3.google.com.
google.com.		5	IN	NS	ns1.google.com.
google.com.		5	IN	NS	ns4.google.com.
google.com.		5	IN	NS	ns2.google.com.

;; ADDITIONAL SECTION:
ns1.google.com.		5	IN	A	216.239.32.10
ns4.google.com.		5	IN	A	216.239.38.10
ns2.google.com.		5	IN	A	216.239.34.10

;; Query time: 56 msec
;; SERVER: 192.168.23.2#53(192.168.23.2) (UDP)
;; WHEN: Sat Nov 23 22:00:34 CST 2024
;; MSG SIZE  rcvd: 244
```

### <mark style="color:yellow;">Realizar una búsqueda DNS inversa</mark>

Una búsqueda inversa convierte una dirección IP en un nombre de dominio, lo contrario de la búsqueda DNS directa, más habitual. Esto ayuda a verificar que la dirección IP está correctamente asignada a un nombre de dominio concreto.

```
dig -x 142.250.114.100
```

```
; <<>> DiG 9.20.0-Debian <<>> -x 142.250.114.100
;; global options: +cmd
;; Got answer:
;; ->>HEADER<<- opcode: QUERY, status: NOERROR, id: 78
;; flags: qr rd ra; QUERY: 1, ANSWER: 1, AUTHORITY: 13, ADDITIONAL: 13

;; QUESTION SECTION:
;100.114.250.142.in-addr.arpa.	IN	PTR

;; ANSWER SECTION:
100.114.250.142.in-addr.arpa. 5	IN	PTR	rr-in-f100.1e100.net.

;; AUTHORITY SECTION:
.			5	IN	NS	c.root-servers.net.
.			5	IN	NS	d.root-servers.net.
.			5	IN	NS	e.root-servers.net.
.			5	IN	NS	f.root-servers.net.
.			5	IN	NS	g.root-servers.net.
.			5	IN	NS	h.root-servers.net.
.			5	IN	NS	i.root-servers.net.
.			5	IN	NS	j.root-servers.net.
.			5	IN	NS	k.root-servers.net.
.			5	IN	NS	l.root-servers.net.
.			5	IN	NS	m.root-servers.net.
.			5	IN	NS	a.root-servers.net.
.			5	IN	NS	b.root-servers.net.

;; ADDITIONAL SECTION:
c.root-servers.net.	5	IN	A	192.33.4.12
d.root-servers.net.	5	IN	A	199.7.91.13
e.root-servers.net.	5	IN	A	192.203.230.10
f.root-servers.net.	5	IN	A	192.5.5.241
g.root-servers.net.	5	IN	A	192.112.36.4
h.root-servers.net.	5	IN	A	198.97.190.53
i.root-servers.net.	5	IN	A	192.36.148.17
j.root-servers.net.	5	IN	A	192.58.128.30
k.root-servers.net.	5	IN	A	193.0.14.129
l.root-servers.net.	5	IN	A	199.7.83.42
m.root-servers.net.	5	IN	A	202.12.27.33
a.root-servers.net.	5	IN	A	198.41.0.4
b.root-servers.net.	5	IN	A	170.247.170.2

;; Query time: 88 msec
;; SERVER: 192.168.23.2#53(192.168.23.2) (UDP)
;; WHEN: Sat Nov 23 22:02:04 CST 2024
;; MSG SIZE  rcvd: 496
```

Ten en cuenta que si no se define un registro PTR para una dirección IP, no es posible realizar una búsqueda DNS inversa, ya que el registro PTR apunta al dominio o nombre de host.

### <mark style="color:yellow;">Ejecutar consultas por lotes</mark>

También puedes utilizar **dig** para ejecutar varias búsquedas DNS en un solo comando. Ayuda a consultar información sobre varios nombres de dominio o direcciones IP, ahorrando tiempo y simplificando el proceso.

Para ejecutar consultas por lotes, sigue estos pasos:

* Crea un archivo llamado **`dominios.txt`** o con el nombre que prefieras
* Añade las direcciones IP o los dominios que quieras consultar, uno por línea
* Guarda tus modificaciones y sal

```
dig -f dominios.txt
```

### <mark style="color:yellow;">Verificar DNSSEC</mark>

Las extensiones de seguridad DNS, o DNSSEC, son un conjunto de protocolos que aseguran el proceso de búsqueda DNS. Garantiza que las respuestas son auténticas y no han sido manipuladas. Verificar DNSSEC ayuda a protegerse contra los ataques de suplantación de DNS.

```
dig google.com +dnssec
```

```
; <<>> DiG 9.20.0-Debian <<>> google.com +dnssec
;; global options: +cmd
;; Got answer:
;; ->>HEADER<<- opcode: QUERY, status: NOERROR, id: 15815
;; flags: qr rd ra; QUERY: 1, ANSWER: 6, AUTHORITY: 4, ADDITIONAL: 3

;; QUESTION SECTION:
;google.com.			IN	A

;; ANSWER SECTION:
google.com.		5	IN	A	142.251.116.113
google.com.		5	IN	A	142.251.116.102
google.com.		5	IN	A	142.251.116.100
google.com.		5	IN	A	142.251.116.138
google.com.		5	IN	A	142.251.116.101
google.com.		5	IN	A	142.251.116.139

;; AUTHORITY SECTION:
google.com.		5	IN	NS	ns3.google.com.
google.com.		5	IN	NS	ns1.google.com.
google.com.		5	IN	NS	ns4.google.com.
google.com.		5	IN	NS	ns2.google.com.

;; ADDITIONAL SECTION:
ns1.google.com.		5	IN	A	216.239.32.10
ns4.google.com.		5	IN	A	216.239.38.10
ns2.google.com.		5	IN	A	216.239.34.10

;; Query time: 28 msec
;; SERVER: 192.168.23.2#53(192.168.23.2) (UDP)
;; WHEN: Sat Nov 23 22:05:39 CST 2024
;; MSG SIZE  rcvd: 244
```
