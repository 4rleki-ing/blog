---
description: >-
  El comando host es una utilidad simple para realizar búsquedas de DNS.
  Normalmente se utiliza para convertir nombres a direcciones IP y viceversa.
icon: list-timeline
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

# Host

Le debemos pasar el nombre que dominio que queremos buscar. También puede ser una dirección **IPv4** decimal con puntos o bien una dirección **IPv6** delimitada por puntos, en cuyo caso el host realizará por defecto una búsqueda inversa para esa dirección.

### <mark style="color:yellow;">Sin parámetros</mark>

Podemos utilizar el sitio de la página web

```
┌──(nato㉿kali)-[~]
└─$ host nmap.org
nmap.org has address 50.116.1.184
nmap.org mail is handled by 5 alt1.aspmx.l.google.com.
nmap.org mail is handled by 10 aspmx3.googlemail.com.
nmap.org mail is handled by 1 aspmx.l.google.com.
nmap.org mail is handled by 10 aspmx2.googlemail.com.
nmap.org mail is handled by 5 alt2.aspmx.l.google.com.
```

O podemos utilizar la misma IP del sitio web

```
┌──(nato㉿kali)-[~]
└─$ host 50.116.1.184
184.1.116.50.in-addr.arpa domain name pointer ack.nmap.org.
```

### <mark style="color:yellow;">En modo detalle</mark>

Para que muestre más información se debe habilitar el modo _**verbose**_, que se encuentra en la mayoría de los comandos en GNU/Linux. Para ello se utiliza los parámetros **`-v`** o **`-a`**.

```
┌──(nato㉿kali)-[~]
└─$ host -v nmap.org 
Trying "nmap.org"
;; ->>HEADER<<- opcode: QUERY, status: NOERROR, id: 61082
;; flags: qr rd ra; QUERY: 1, ANSWER: 1, AUTHORITY: 0, ADDITIONAL: 0

;; QUESTION SECTION:
;nmap.org.			IN	A

;; ANSWER SECTION:
nmap.org.		5	IN	A	50.116.1.184

Received 42 bytes from 192.168.23.2#53 in 8 ms
Trying "nmap.org"
;; ->>HEADER<<- opcode: QUERY, status: NOERROR, id: 19687
;; flags: qr rd ra; QUERY: 1, ANSWER: 0, AUTHORITY: 0, ADDITIONAL: 0

;; QUESTION SECTION:
;nmap.org.			IN	AAAA

Received 26 bytes from 192.168.23.2#53 in 28 ms
Trying "nmap.org"
;; ->>HEADER<<- opcode: QUERY, status: NOERROR, id: 39893
;; flags: qr rd ra; QUERY: 1, ANSWER: 5, AUTHORITY: 0, ADDITIONAL: 0

;; QUESTION SECTION:
;nmap.org.			IN	MX

;; ANSWER SECTION:
nmap.org.		5	IN	MX	10 aspmx3.googlemail.com.
nmap.org.		5	IN	MX	1 aspmx.l.google.com.
nmap.org.		5	IN	MX	10 aspmx2.googlemail.com.
nmap.org.		5	IN	MX	5 alt2.aspmx.l.google.com.
nmap.org.		5	IN	MX	5 alt1.aspmx.l.google.com.

Received 159 bytes from 192.168.23.2#53 in 32 ms
```

### <mark style="color:yellow;">Especificar el tipo de consulta</mark>

Para especificar el tipo de consulta que queremos hacer debemos utilizar el parámetro **`-t`**.

#### <mark style="color:green;">Registro ns</mark>

```
┌──(nato㉿kali)-[~]
└─$ host -t ns nmap.org
nmap.org name server ns1.linode.com.
nmap.org name server ns2.linode.com.
nmap.org name server ns3.linode.com.
nmap.org name server ns4.linode.com.
nmap.org name server ns5.linode.com.
```

#### <mark style="color:green;">Registro SOA</mark>

```
┌──(nato㉿kali)-[~]
└─$ host -t soa nmap.org
nmap.org has SOA record ns1.linode.com. hostmaster.insecure.org. 2021000013 14400 14400 1209600 3600
```

#### <mark style="color:green;">Registro TXT</mark>

```
┌──(nato㉿kali)-[~]
└─$ host -t txt nmap.org
nmap.org descriptive text "google-site-verification=SrtYpJGxZzMTcczZG44XtLVK-sEPit9bputDjWc0lF4"
nmap.org descriptive text "v=spf1 a mx ptr ip4:50.116.1.184 ip6:2600:3c01::f03c:91ff:fe98:ff4e ip6:2600:3c01:e000:3e6::6d4e:7061 include:_spf.google.com ~all"
```

#### <mark style="color:green;">Registro a</mark>

```
┌──(nato㉿kali)-[~]
└─$ host -t a nmap.org
nmap.org has address 50.116.1.184
```

#### <mark style="color:green;">Registro aaaa</mark>

```
┌──(nato㉿kali)-[~]
└─$ host -t aaaa nmap.org
nmap.org has no AAAA record
```

#### <mark style="color:green;">Registro mx</mark>

```
┌──(nato㉿kali)-[~]
└─$ host -t mx nmap.org
nmap.org mail is handled by 5 alt1.aspmx.l.google.com.
nmap.org mail is handled by 10 aspmx2.googlemail.com.
nmap.org mail is handled by 1 aspmx.l.google.com.
nmap.org mail is handled by 5 alt2.aspmx.l.google.com.
nmap.org mail is handled by 10 aspmx3.googlemail.com.
```

#### <mark style="color:green;">Registro CNAME</mark>

```
┌──(nato㉿kali)-[~]
└─$ host -t CNAME nmap.org
nmap.org has no CNAME record
```

### <mark style="color:yellow;">Forzar consultas</mark>

#### <mark style="color:green;">IPv4</mark>

```
┌──(nato㉿kali)-[~]
└─$ host -4 nmap.org  
nmap.org has address 50.116.1.184
nmap.org mail is handled by 10 aspmx2.googlemail.com.
nmap.org mail is handled by 5 alt2.aspmx.l.google.com.
nmap.org mail is handled by 5 alt1.aspmx.l.google.com.
nmap.org mail is handled by 10 aspmx3.googlemail.com.
nmap.org mail is handled by 1 aspmx.l.google.com.                                                                                                                                                                                                                                              
```

#### <mark style="color:green;">IPv6</mark>

```
┌──(nato㉿kali)-[~]
└─$ host -6 nmap.org
;; communications error to ::1#53: connection refused
;; communications error to ::1#53: connection refused
;; no servers could be reached
```

### <mark style="color:yellow;">Consultar Registros SOA</mark>

Para realizar este tipo de consultas de los registros SOA en servidores de nombre autorizados, se utiliza el parámetro **`-C`**.

```
┌──(nato㉿kali)-[~]
└─$ host -C nmap.org    
Nameserver 92.123.94.3:
	nmap.org has SOA record ns1.linode.com. hostmaster.insecure.org. 2021000013 14400 14400 1209600 3600
Nameserver 92.123.95.2:
	nmap.org has SOA record ns1.linode.com. hostmaster.insecure.org. 2021000013 14400 14400 1209600 3600
Nameserver 92.123.94.2:
	nmap.org has SOA record ns1.linode.com. hostmaster.insecure.org. 2021000013 14400 14400 1209600 3600
Nameserver 92.123.95.4:
	nmap.org has SOA record ns1.linode.com. hostmaster.insecure.org. 2021000013 14400 14400 1209600 3600
Nameserver 92.123.95.3:
	nmap.org has SOA record ns1.linode.com. hostmaster.insecure.org. 2021000013 14400 14400 1209600 3600
```

### <mark style="color:yellow;">Comprobar número de reintentos</mark>

Para definir esto se utiliza el parámetro **`-R`** seguido del número de reintentos que se le desea otorgar.

```
┌──(nato㉿kali)-[~]
└─$ host -R 3 nmap.org 
nmap.org has address 50.116.1.184
nmap.org mail is handled by 1 aspmx.l.google.com.
nmap.org mail is handled by 10 aspmx2.googlemail.com.
nmap.org mail is handled by 5 alt2.aspmx.l.google.com.
nmap.org mail is handled by 5 alt1.aspmx.l.google.com.
nmap.org mail is handled by 10 aspmx3.googlemail.com.
```

### <mark style="color:yellow;">Enumerar todos los hosts</mark>

Para que este comando funcione, se debe ser el administrador del nodo, si se cumple esta condición, con el parámetro **`-l`** puedes obtener la información.

```
┌──(nato㉿kali)-[~]
└─$ host -l nmap.org 
Host nmap.org not found: 5(REFUSED)
; Transfer failed.
```
