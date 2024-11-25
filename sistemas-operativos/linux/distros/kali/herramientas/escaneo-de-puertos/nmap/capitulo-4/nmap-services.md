---
icon: tablet-rugged
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

# nmap-services

```
# THIS FILE IS GENERATED AUTOMATICALLY FROM A MASTER - DO NOT EDIT.
# EDIT /nmap-private-dev/nmap-services-all IN SVN INSTEAD.
# Well known service port numbers -*- mode: fundamental; -*-
# From the Nmap Security Scanner ( https://nmap.org/ )
#
# $Id: nmap-services 9746 2008-08-26 18:45:24Z fyodor $
#
# Derived from IANA data and our own research
#
# This collection of service data is (C) 1996-2020 by Insecure.Com
# LLC.  It is distributed under the Nmap Public Source license as
# provided in the LICENSE file of the source distribution or at
# https://svn.nmap.org/nmap/LICENSE .  Note that this license
# requires you to license your own work under a compatable open source
# license.  If you wish to embed Nmap technology into proprietary
# software, we sell alternative licenses (contact sales@insecure.com).
# Dozens of software vendors already license Nmap technology such as
# host discovery, port scanning, OS detection, and version detection.
# For more details, see https://nmap.org/book/man-legal.html
#
# Fields in this file are: 
# Service name, portnum/protocol, open-frequency, optional comments
#
tcpmux	1/tcp	0.001995	# TCP Port Service Multiplexer [rfc-1078] | TCP Port Service Multiplexer
tcpmux	1/udp	0.001236	# TCP Port Service Multiplexer
compressnet	2/tcp	0.000013	# Management Utility
compressnet	2/udp	0.001845	# Management Utility
compressnet	3/tcp	0.001242	# Compression Process
compressnet	3/udp	0.001532	# Compression Process
unknown	4/tcp	0.000477
rje	5/tcp	0.000000	# Remote Job Entry
rje	5/udp	0.000593	# Remote Job Entry
unknown	6/tcp	0.000502
echo	7/sctp	0.000000
echo	7/tcp	0.004855
echo	7/udp	0.024679
unknown	8/tcp	0.000013
discard	9/sctp	0.000000	# sink null
discard	9/tcp	0.003764	# sink null
discard	9/udp	0.015733	# sink null
unknown	10/tcp	0.000063
systat	11/tcp	0.000075	# Active Users
systat	11/udp	0.000577	# Active Users
unknown	12/tcp	0.000063
daytime	13/tcp	0.003927
daytime	13/udp	0.004827
unknown	14/tcp	0.000038
netstat	15/tcp	0.000038
unknown	16/tcp	0.000050
qotd	17/tcp	0.002346	# Quote of the Day
qotd	17/udp	0.009209	# Quote of the Day
msp	18/tcp	0.000000	# Message Send Protocol | Message Send Protocol (historic)
msp	18/udp	0.000610	# Message Send Protocol
chargen	19/tcp	0.002559	# ttytst source Character Generator | Character Generator
chargen	19/udp	0.015865	# ttytst source Character Generator
ftp-data	20/sctp	0.000000	# File Transfer [Default Data] | FTP
ftp-data	20/tcp	0.001079	# File Transfer [Default Data]
ftp-data	20/udp	0.001878	# File Transfer [Default Data]
ftp	21/sctp	0.000000	# File Transfer [Control] | File Transfer Protocol [Control]
ftp	21/tcp	0.197667	# File Transfer [Control]
ftp	21/udp	0.004844	# File Transfer [Control]
ssh	22/sctp	0.000000	# Secure Shell Login | The Secure Shell (SSH) Protocol
ssh	22/tcp	0.182286	# Secure Shell Login
ssh	22/udp	0.003905	# Secure Shell Login
telnet	23/tcp	0.221265
telnet	23/udp	0.006211
priv-mail	24/tcp	0.001154	# any private mail system
priv-mail	24/udp	0.000329	# any private mail system
smtp	25/tcp	0.131314	# Simple Mail Transfer
smtp	25/udp	0.001285	# Simple Mail Transfer
rsftp	26/tcp	0.007991
nsw-fe	27/tcp	0.000138	# NSW User System FE
nsw-fe	27/udp	0.000395	# NSW User System FE
unknown	28/tcp	0.000050
msg-icp	29/tcp	0.000025	# MSG ICP
msg-icp	29/udp	0.000560	# MSG ICP
unknown	30/tcp	0.000527
msg-auth	31/tcp	0.000025	# MSG Authentication
msg-auth	31/udp	0.000939	# MSG Authentication
unknown	32/tcp	0.000339
dsp	33/tcp	0.001016	# Display Support Protocol
dsp	33/udp	0.000560	# Display Support Protocol
unknown	34/tcp	0.000025
priv-print	35/tcp	0.000038	# any private printer server
priv-print	35/udp	0.000708	# any private printer server
time	37/tcp	0.003161	# timserver
time	37/udp	0.006458	# timserver
rap	38/tcp	0.000025	# Route Access Protocol
rap	38/udp	0.002043	# Route Access Protocol
rlp	39/tcp	0.000000	# Resource Location Protocol
rlp	39/udp	0.000478	# Resource Location Protocol
unknown	40/tcp	0.000038
graphics	41/tcp	0.000000
graphics	41/udp	0.000445
nameserver	42/tcp	0.000803	# name | Host Name Server
nameserver	42/udp	0.005288	# Host Name Server
whois	43/tcp	0.000314	# nicname | Who Is
whois	43/udp	0.000313	# nicname
mpm-flags	44/tcp	0.000025	# MPM FLAGS Protocol
mpm-flags	44/udp	0.000659	# MPM FLAGS Protocol
mpm	45/tcp	0.000050	# Message Processing Module [recv]
mpm	45/udp	0.000741	# Message Processing Module [recv]
mpm-snd	46/tcp	0.000000	# MPM [default send]
mpm-snd	46/udp	0.000494	# MPM [default send]
ni-ftp	47/tcp	0.000075	# NI FTP
ni-ftp	47/udp	0.001071	# NI FTP
auditd	48/tcp	0.000013	# Digital Audit Daemon
auditd	48/udp	0.000708	# Digital Audit Daemon
tacacs	49/tcp	0.000665	# Login Host Protocol (TACACS)
tacacs	49/udp	0.014020	# Login Host Protocol (TACACS)
re-mail-ck	50/tcp	0.000050	# Remote Mail Checking Protocol
re-mail-ck	50/udp	0.000428	# Remote Mail Checking Protocol
la-maint	51/tcp	0.000038	# IMP Logical Address Maintenance
la-maint	51/udp	0.000280	# IMP Logical Address Maintenance
xns-time	52/tcp	0.000063	# XNS Time Protocol
xns-time	52/udp	0.000362	# XNS Time Protocol
domain	53/tcp	0.048463	# Domain Name Server
domain	53/udp	0.213496	# Domain Name Server
xns-ch	54/tcp	0.000013	# XNS Clearinghouse
xns-ch	54/udp	0.000659	# XNS Clearinghouse
isi-gl	55/tcp	0.000125	# ISI Graphics Language
isi-gl	55/udp	0.000478	# ISI Graphics Language
xns-auth	56/tcp	0.000013	# XNS Authentication
xns-auth	56/udp	0.001285	# XNS Authentication
priv-term	57/tcp	0.000125	# any private terminal access
priv-term	57/udp	0.000774	# any private terminal access
xns-mail	58/tcp	0.000025	# XNS Mail
xns-mail	58/udp	0.000428	# XNS Mail
priv-file	59/tcp	0.000088	# any private file service
priv-file	59/udp	0.000478	# any private file service
unknown	60/tcp	0.000038
ni-mail	61/tcp	0.000000	# NI MAIL
ni-mail	61/udp	0.000461	# NI MAIL
acas	62/tcp	0.000000	# ACA Services
acas	62/udp	0.000264	# ACA Services
via-ftp	63/tcp	0.000000	# whoispp | VIA Systems - FTP & whois++ | whois++
via-ftp	63/udp	0.000445	# VIA Systems - FTP & whois++
covia	64/tcp	0.000000	# Communications Integrator (CI)
covia	64/udp	0.000593	# Communications Integrator (CI)
tacacs-ds	65/tcp	0.000013	# TACACS-Database Service
tacacs-ds	65/udp	0.000741	# TACACS-Database Service
sqlnet	66/tcp	0.000075	# sql*net | sql-net | Oracle SQL*NET
sqlnet	66/udp	0.000544	# Oracle SQL*NET
dhcps	67/tcp	0.000013	# bootps | DHCP/Bootstrap Protocol Server | Bootstrap Protocol Server
dhcps	67/udp	0.228010	# DHCP/Bootstrap Protocol Server
dhcpc	68/tcp	0.000063	# bootpc | DHCP/Bootstrap Protocol Client | Bootstrap Protocol Client
dhcpc	68/udp	0.140118	# DHCP/Bootstrap Protocol Client
tftp	69/tcp	0.000038	# Trivial File Transfer
tftp	69/udp	0.102835	# Trivial File Transfer
gopher	70/tcp	0.000226
gopher	70/udp	0.000544
netrjs-1	71/tcp	0.000025	# Remote Job Service
netrjs-1	71/udp	0.000560	# Remote Job Service
netrjs-2	72/tcp	0.000013	# Remote Job Service
netrjs-2	72/udp	0.000494	# Remote Job Service
netrjs-3	73/tcp	0.000025	# Remote Job Service
netrjs-3	73/udp	0.000428	# Remote Job Service
netrjs-4	74/tcp	0.000025	# Remote Job Service
netrjs-4	74/udp	0.000478	# Remote Job Service
priv-dial	75/tcp	0.000063	# any private dial out service
priv-dial	75/udp	0.000577	# any private dial out service
deos	76/tcp	0.000063	# Distributed External Object Store
deos	76/udp	0.000675	# Distributed External Object Store
priv-rje	77/tcp	0.000113	# any private RJE service, netrjs
priv-rje	77/udp	0.000741	# any private RJE service, netjrs
vettcp	78/tcp	0.000000
vettcp	78/udp	0.000626
finger	79/tcp	0.006022
finger	79/udp	0.000956
http	80/sctp	0.000000	# www-http | www | World Wide Web HTTP
http	80/tcp	0.484143	# World Wide Web HTTP
http	80/udp	0.035767	# World Wide Web HTTP
hosts2-ns	81/tcp	0.012056	# HOSTS2 Name Server
hosts2-ns	81/udp	0.001005	# HOSTS2 Name Server
xfer	82/tcp	0.002923	# XFER Utility
xfer	82/udp	0.000659	# XFER Utility
mit-ml-dev	83/tcp	0.000539	# MIT ML Device
mit-ml-dev	83/udp	0.001203	# MIT ML Device
ctf	84/tcp	0.000276	# Common Trace Facility
ctf	84/udp	0.000610	# Common Trace Facility
mit-ml-dev	85/tcp	0.000690	# MIT ML Device
mit-ml-dev	85/udp	0.000610	# MIT ML Device
mfcobol	86/tcp	0.000138	# Micro Focus Cobol
mfcobol	86/udp	0.000824	# Micro Focus Cobol
priv-term-l	87/tcp	0.000125	# any private terminal link, ttylink
kerberos-sec	88/tcp	0.006072	# kerberos | Kerberos (v5) | Kerberos
kerberos-sec	88/udp	0.013476	# Kerberos (v5)
su-mit-tg	89/tcp	0.000376	# SU/MIT Telnet Gateway
su-mit-tg	89/udp	0.000494	# SU/MIT Telnet Gateway
dnsix	90/tcp	0.000652	# DNSIX Securit Attribute Token Map
dnsix	90/udp	0.000511	# DNSIX Securit Attribute Token Map
mit-dov	91/tcp	0.000063	# MIT Dover Spooler
mit-dov	91/udp	0.000478	# MIT Dover Spooler
npp	92/tcp	0.000050	# Network Printing Protocol
npp	92/udp	0.000478	# Network Printing Protocol
dcp	93/tcp	0.000025	# Device Control Protocol
dcp	93/udp	0.000774	# Device Control Protocol
objcall	94/tcp	0.000025	# Tivoli Object Dispatcher
objcall	94/udp	0.000428	# Tivoli Object Dispatcher
supdup	95/tcp	0.000025	# BSD supdupd(8)
supdup	95/udp	0.000379
dixie	96/tcp	0.000013	# DIXIE Protocol Specification
dixie	96/udp	0.000939	# DIXIE Protocol Specification
swift-rvf	97/tcp	0.000038	# Swift Remote Virtural File Protocol
swift-rvf	97/udp	0.000362	# Swift Remote Virtural File Protocol
linuxconf	98/tcp	0.000088	# tacnews | TAC News
tacnews	98/udp	0.000560	# TAC News
metagram	99/tcp	0.000326	# Metagram Relay
metagram	99/udp	0.000972	# Metagram Relay
newacct	100/tcp	0.002133	# [unauthorized use]
hostname	101/tcp	0.000063	# hostnames NIC Host Name Server | NIC Host Name Server
hostname	101/udp	0.000560	# hostnames NIC Host Name Server
iso-tsap	102/tcp	0.000138	# tsap ISO-TSAP Class 0 | ISO-TSAP Class 0
iso-tsap	102/udp	0.000544	# tsap ISO-TSAP Class 0
gppitnp	103/tcp	0.000038	# Genesis Point-to-Point Trans Net, or x400 ISO Email | Genesis Point-to-Point Trans Net
gppitnp	103/udp	0.000527	# Genesis Point-to-Point Trans Net
acr-nema	104/tcp	0.000063	# ACR-NEMA Digital Imag. & Comm. 300
acr-nema	104/udp	0.000643	# ACR-NEMA Digital Imag. & Comm. 300
csnet-ns	105/tcp	0.000000	# cso | Mailbox Name Nameserver | CCSO name server protocol
csnet-ns	105/udp	0.000478	# Mailbox Name Nameserver
pop3pw	106/tcp	0.005934	# 3com-tsmux | Eudora compatible PW changer | 3COM-TSMUX
3com-tsmux	106/udp	0.000544
rtelnet	107/tcp	0.000000	# Remote Telnet | Remote Telnet Service
rtelnet	107/udp	0.000478	# Remote Telnet Service
snagas	108/tcp	0.000013	# SNA Gateway Access Server
snagas	108/udp	0.000494	# SNA Gateway Access Server
pop2	109/tcp	0.000188	# PostOffice V.2 | Post Office Protocol - Version 2
pop2	109/udp	0.000461	# PostOffice V.2
pop3	110/tcp	0.077142	# PostOffice V.3 | Post Office Protocol - Version 3
pop3	110/udp	0.001104	# PostOffice V.3
rpcbind	111/tcp	0.030034	# sunrpc | portmapper, rpcbind | SUN Remote Procedure Call
rpcbind	111/udp	0.093988	# portmapper, rpcbind
mcidas	112/tcp	0.000050	# McIDAS Data Transmission Protocol
mcidas	112/udp	0.002208	# McIDAS Data Transmission Protocol
ident	113/tcp	0.012370	# auth | ident, tap, Authentication Service | Authentication Service
auth	113/udp	0.003031	# ident, tap, Authentication Service
audionews	114/tcp	0.000025	# Audio News Multicast
audionews	114/udp	0.000362	# Audio News Multicast
sftp	115/tcp	0.000025	# Simple File Transfer Protocol
sftp	115/udp	0.000346	# Simple File Transfer Protocol
ansanotify	116/tcp	0.000013	# ANSA REX Notify
ansanotify	116/udp	0.000445	# ANSA REX Notify
uucp-path	117/tcp	0.000013	# UUCP Path Service
uucp-path	117/udp	0.000527	# UUCP Path Service
sqlserv	118/tcp	0.000025	# SQL Services
sqlserv	118/udp	0.000791	# SQL Services
nntp	119/tcp	0.003262	# Network News Transfer Protocol
nntp	119/udp	0.000428	# Network News Transfer Protocol
cfdptkt	120/tcp	0.000025
cfdptkt	120/udp	0.010181
erpc	121/tcp	0.000000	# Encore Expedited Remote Pro.Call
erpc	121/udp	0.000675	# Encore Expedited Remote Pro.Call
smakynet	122/tcp	0.000063
smakynet	122/udp	0.000428
ntp	123/tcp	0.000138	# Network Time Protocol
ntp	123/udp	0.330879	# Network Time Protocol
ansatrader	124/tcp	0.000013	# ANSA REX Trader
ansatrader	124/udp	0.000610	# ANSA REX Trader
locus-map	125/tcp	0.000176	# Locus PC-Interface Net Map Ser
locus-map	125/udp	0.000478	# Locus PC-Interface Net Map Ser
unitary	126/tcp	0.000000	# nxedit | Unisys Unitary Login | NXEdit
unitary	126/udp	0.000610	# Unisys Unitary Login
locus-con	127/tcp	0.000113	# Locus PC-Interface Conn Server
locus-con	127/udp	0.000412	# Locus PC-Interface Conn Server
gss-xlicen	128/tcp	0.000013	# GSS X License Verification
gss-xlicen	128/udp	0.000494	# GSS X License Verification
pwdgen	129/tcp	0.000025	# Password Generator Protocol
pwdgen	129/udp	0.000412	# Password Generator Protocol
cisco-fna	130/tcp	0.000013	# cisco FNATIVE
cisco-fna	130/udp	0.000774	# cisco FNATIVE
cisco-tna	131/tcp	0.000000	# cisco TNATIVE
cisco-tna	131/udp	0.000560	# cisco TNATIVE
cisco-sys	132/tcp	0.000013	# cisco SYSMAINT
cisco-sys	132/udp	0.000923	# cisco SYSMAINT
statsrv	133/tcp	0.000025	# Statistics Service
statsrv	133/udp	0.000758	# Statistics Service
ingres-net	134/tcp	0.000000	# INGRES-NET Service
ingres-net	134/udp	0.001203	# INGRES-NET Service
msrpc	135/tcp	0.047798	# epmap | Microsoft RPC services | DCE endpoint resolution
msrpc	135/udp	0.244452	# Microsoft RPC services
profile	136/tcp	0.000025	# PROFILE Naming System
profile	136/udp	0.051862	# PROFILE Naming System
netbios-ns	137/tcp	0.000038	# NETBIOS Name Service
netbios-ns	137/udp	0.365163	# NETBIOS Name Service
netbios-dgm	138/tcp	0.000025	# NETBIOS Datagram Service
netbios-dgm	138/udp	0.297830	# NETBIOS Datagram Service
netbios-ssn	139/tcp	0.050809	# NETBIOS Session Service
netbios-ssn	139/udp	0.193726	# NETBIOS Session Service
emfis-data	140/tcp	0.000000	# EMFIS Data Service
emfis-data	140/udp	0.000692	# EMFIS Data Service
emfis-cntl	141/tcp	0.000013	# EMFIS Control Service
emfis-cntl	141/udp	0.000428	# EMFIS Control Service
bl-idm	142/tcp	0.000013	# Britton-Lee IDM
bl-idm	142/udp	0.000428	# Britton-Lee IDM
imap	143/tcp	0.050420	# Interim Mail Access Protocol v2 | Internet Message Access Protocol
imap	143/udp	0.000659	# Interim Mail Access Protocol v2
news	144/tcp	0.004981	# uma | NewS window system | Universal Management Architecture
news	144/udp	0.000346	# NewS window system
uaac	145/tcp	0.000000	# UAAC Protocol
uaac	145/udp	0.001153	# UAAC Protocol
iso-tp0	146/tcp	0.000577	# ISO-IP0
iso-tp0	146/udp	0.000890
iso-ip	147/tcp	0.000000
iso-ip	147/udp	0.000511
cronus	148/tcp	0.000013	# jargon | CRONUS-SUPPORT | Jargon
cronus	148/udp	0.000445	# CRONUS-SUPPORT
aed-512	149/tcp	0.000013	# AED 512 Emulation Service
aed-512	149/udp	0.000445	# AED 512 Emulation Service
sql-net	150/tcp	0.000013
sql-net	150/udp	0.000840
hems	151/tcp	0.000013
hems	151/udp	0.000412
bftp	152/tcp	0.000000	# Background File Transfer Program
bftp	152/udp	0.000988	# Background File Transfer Program
sgmp	153/tcp	0.000000
sgmp	153/udp	0.000346
netsc-prod	154/tcp	0.000000	# NETSC
netsc-prod	154/udp	0.000379
netsc-dev	155/tcp	0.000000	# NETSC
netsc-dev	155/udp	0.000659
sqlsrv	156/tcp	0.000000	# SQL Service
sqlsrv	156/udp	0.000461	# SQL Service
knet-cmp	157/tcp	0.000113	# KNET/VM Command/Message Protocol
knet-cmp	157/udp	0.000247	# KNET/VM Command/Message Protocol
pcmail-srv	158/tcp	0.000063	# PCMail Server
pcmail-srv	158/udp	0.010148	# PCMail Server
nss-routing	159/tcp	0.000000
nss-routing	159/udp	0.000329
sgmp-traps	160/tcp	0.000000
sgmp-traps	160/udp	0.000824
snmp	161/tcp	0.000790
snmp	161/udp	0.433467	# Simple Net Mgmt Proto
snmptrap	162/tcp	0.000013	# snmp-trap
snmptrap	162/udp	0.103346	# snmp-trap
cmip-man	163/tcp	0.000590	# CMIP/TCP Manager
cmip-man	163/udp	0.000840	# CMIP/TCP Manager
cmip-agent	164/tcp	0.000000	# CMIP/TCP Agent
smip-agent	164/udp	0.000626	# CMIP/TCP Agent
xns-courier	165/tcp	0.000000	# Xerox
xns-courier	165/udp	0.000379	# Xerox
s-net	166/tcp	0.000000	# Sirius Systems
s-net	166/udp	0.000461	# Sirius Systems
namp	167/tcp	0.000000
namp	167/udp	0.000395
rsvd	168/tcp	0.000013
rsvd	168/udp	0.000412
send	169/tcp	0.000000
send	169/udp	0.000494
print-srv	170/tcp	0.000000	# Network PostScript
print-srv	170/udp	0.001071	# Network PostScript
multiplex	171/tcp	0.000000	# Network Innovations Multiplex
multiplex	171/udp	0.000412	# Network Innovations Multiplex
cl-1	172/tcp	0.000000	# cl/1 | Network Innovations CL/1
cl-1	172/udp	0.000494	# Network Innovations CL/1
xyplex-mux	173/tcp	0.000013	# Xyplex
xyplex-mux	173/udp	0.000329
mailq	174/tcp	0.000013
mailq	174/udp	0.000379
vmnet	175/tcp	0.000000
vmnet	175/udp	0.000379
genrad-mux	176/tcp	0.000025
genrad-mux	176/udp	0.000313
xdmcp	177/tcp	0.000025	# X Display Mgr. Control Proto | X Display Manager Control Protocol
xdmcp	177/udp	0.018551	# X Display Manager Control Protocol
nextstep	178/tcp	0.000000	# NextStep Window Server
nextstep	178/udp	0.000346	# NextStep Window Server
bgp	179/sctp	0.000000	# Border Gateway Protocol
bgp	179/tcp	0.010538	# Border Gateway Protocol
bgp	179/udp	0.000494	# Border Gateway Protocol
ris	180/tcp	0.000038	# Intergraph
ris	180/udp	0.000478	# Intergraph
unify	181/tcp	0.000025
unify	181/udp	0.000181
audit	182/tcp	0.000038	# Unisys Audit SITP
audit	182/udp	0.000297	# Unisys Audit SITP
ocbinder	183/tcp	0.000000
ocbinder	183/udp	0.000560
ocserver	184/tcp	0.000013
ocserver	184/udp	0.000461
remote-kis	185/tcp	0.000013
remote-kis	185/udp	0.000428
kis	186/tcp	0.000000	# KIS Protocol
kis	186/udp	0.000280	# KIS Protocol
aci	187/tcp	0.000000	# Application Communication Interface
aci	187/udp	0.000395	# Application Communication Interface
mumps	188/tcp	0.000000	# Plus Five's MUMPS
mumps	188/udp	0.000527	# Plus Five's MUMPS
qft	189/tcp	0.000013	# Queued File Transport
qft	189/udp	0.000461	# Queued File Transport
gacp	190/tcp	0.000013	# Gateway Access Control Protocol
cacp	190/udp	0.000428	# Gateway Access Control Protocol
prospero	191/tcp	0.000013	# Prospero Directory Service
prospero	191/udp	0.000857	# Prospero Directory Service
osu-nms	192/tcp	0.000013	# OSU Network Monitoring System
osu-nms	192/udp	0.004168	# OSU Network Monitoring System
srmp	193/tcp	0.000025	# Spider Remote Monitoring Protocol
srmp	193/udp	0.000412	# Spider Remote Monitoring Protocol
irc	194/tcp	0.000038	# Internet Relay Chat | Internet Relay Chat Protocol
irc	194/udp	0.000643	# Internet Relay Chat Protocol
dn6-nlm-aud	195/tcp	0.000000	# DNSIX Network Level Module Audit
dn6-nlm-aud	195/udp	0.000395	# DNSIX Network Level Module Audit
dn6-smm-red	196/tcp	0.000025	# DNSIX Session Mgt Module Audit Redir
dn6-smm-red	196/udp	0.000428	# DNSIX Session Mgt Module Audit Redir
dls	197/tcp	0.000000	# Directory Location Service
dls	197/udp	0.000659	# Directory Location Service
dls-mon	198/tcp	0.000000	# Directory Location Service Monitor
dls-mon	198/udp	0.001252	# Directory Location Service Monitor
smux	199/tcp	0.015945	# SNMP Unix Multiplexer
smux	199/udp	0.004152
src	200/tcp	0.000025	# IBM System Resource Controller
src	200/udp	0.000626	# IBM System Resource Controller
at-rtmp	201/tcp	0.000038	# AppleTalk Routing Maintenance
at-rtmp	201/udp	0.000988	# AppleTalk Routing Maintenance
at-nbp	202/tcp	0.000025	# AppleTalk Name Binding
at-nbp	202/udp	0.000445	# AppleTalk Name Binding
at-3	203/tcp	0.000000	# AppleTalk Unused
at-3	203/udp	0.000461	# AppleTalk Unused
at-echo	204/tcp	0.000025	# AppleTalk Echo
at-echo	204/udp	0.000412	# AppleTalk Echo
at-5	205/tcp	0.000013	# AppleTalk Unused
at-5	205/udp	0.000890	# AppleTalk Unused
at-zis	206/tcp	0.000025	# AppleTalk Zone Information
at-zis	206/udp	0.000956	# AppleTalk Zone Information
at-7	207/tcp	0.000000	# AppleTalk Unused
at-7	207/udp	0.001351	# AppleTalk Unused
at-8	208/tcp	0.000000	# AppleTalk Unused
at-8	208/udp	0.000511	# AppleTalk Unused
tam	209/tcp	0.000013	# qmtp | Trivial Authenticated Mail Protocol | The Quick Mail Transfer Protocol
tam	209/udp	0.000395	# Trivial Authenticated Mail Protocol
z39.50	210/tcp	0.000125	# z39-50 | wais, ANSI Z39.50 | ANSI Z39.50
z39.50	210/udp	0.000511	# wais, ANSI Z39.50
914c-g	211/tcp	0.000427	# 914c/g | Texas Instruments 914C/G Terminal
914c-g	211/udp	0.000329	# Texas Instruments 914C/G Terminal
anet	212/tcp	0.000364	# ATEXSSTR
anet	212/udp	0.000329	# ATEXSSTR
ipx	213/tcp	0.000038
ipx	213/udp	0.000478
vmpwscs	214/tcp	0.000038	# VM PWSCS
vmpwscs	214/udp	0.000445
softpc	215/tcp	0.000000	# Insignia Solutions
softpc	215/udp	0.000412	# Insignia Solutions
atls	216/tcp	0.000013	# CAIlic | Access Technology License Server | Computer Associates Int'l License Server
atls	216/udp	0.000461	# Access Technology License Server
dbase	217/tcp	0.000013	# dBASE Unix
dbase	217/udp	0.001993	# dBASE Unix
mpp	218/tcp	0.000000	# Netix Message Posting Protocol
mpp	218/udp	0.000593	# Netix Message Posting Protocol
uarps	219/tcp	0.000063	# Unisys ARPs
uarps	219/udp	0.000395	# Unisys ARPs
imap3	220/tcp	0.000113	# Interactive Mail Access Protocol v3
imap3	220/udp	0.000445	# Interactive Mail Access Protocol v3
fln-spx	221/tcp	0.000050	# Berkeley rlogind with SPX auth
fln-spx	221/udp	0.000577	# Berkeley rlogind with SPX auth
rsh-spx	222/tcp	0.000941	# Berkeley rshd with SPX auth
rsh-spx	222/udp	0.000774	# Berkeley rshd with SPX auth
cdc	223/tcp	0.000125	# Certificate Distribution Center
cdc	223/udp	0.000346	# Certificate Distribution Center
masqdialer	224/tcp	0.000025
masqdialer	224/udp	0.000000
unknown	225/tcp	0.000100
unknown	225/udp	0.000330
unknown	226/tcp	0.000013
unknown	228/tcp	0.000013
unknown	229/tcp	0.000013
unknown	230/tcp	0.000050
unknown	231/tcp	0.000038
unknown	233/tcp	0.000025
unknown	234/tcp	0.000013
unknown	235/tcp	0.000025
unknown	236/tcp	0.000025
unknown	236/udp	0.000330
unknown	237/tcp	0.000063
unknown	238/tcp	0.000013
unknown	238/udp	0.000330
unknown	239/udp	0.000330
direct	242/tcp	0.000000
direct	242/udp	0.000362
sur-meas	243/tcp	0.000000	# Survey Measurement
sur-meas	243/udp	0.000494	# Survey Measurement
dayna	244/tcp	0.000000	# inbusiness
dayna	244/udp	0.000461
link	245/tcp	0.000000
link	245/udp	0.000626
dsp3270	246/tcp	0.000000	# Display Systems Protocol
dsp3270	246/udp	0.000593	# Display Systems Protocol
subntbcst_tftp	247/tcp	0.000000	# subntbcst-tftp
subntbcst_tftp	247/udp	0.000412
bhfhs	248/tcp	0.000013
bhfhs	248/udp	0.000511
unknown	249/tcp	0.000050
unknown	250/tcp	0.000138
unknown	251/tcp	0.000125
unknown	252/tcp	0.000088
unknown	253/tcp	0.000038
unknown	254/tcp	0.001832
unknown	255/tcp	0.002409
fw1-secureremote	256/tcp	0.000163	# rap | also "rap" | RAP
rap	256/udp	0.000692
fw1-mc-fwmodule	257/tcp	0.000100	# set | FW1 management console for communication w/modules and also secure electronic transaction (set) port | Secure Electronic Transaction
set	257/udp	0.000511	# secure electronic transaction
fw1-mc-gui	258/tcp	0.000013	# also yak winsock personal chat
yak-chat	258/udp	0.000494	# yak winsock personal chat
esro-gen	259/tcp	0.000201	# efficient short remote operations | Efficient Short Remote Operations
firewall1-rdp	259/udp	0.000840	# Firewall 1 proprietary RDP protocol http://www.inside-security.de/fw1_rdp_poc.html
openport	260/tcp	0.000025
openport	260/udp	0.000362
nsiiops	261/tcp	0.000025	# iiop name service over tls/ssl | IIOP Name Service over TLS/SSL
nsiiops	261/udp	0.000659	# iiop name service over tls/ssl
arcisdms	262/tcp	0.000038
arcisdms	262/udp	0.000577
hdap	263/tcp	0.000000
hdap	263/udp	0.000544
bgmp	264/tcp	0.001029
fw1-or-bgmp	264/udp	0.000461	# FW1 secureremote alternate
maybe-fw1	265/tcp	0.000013	# x-bone-ctl | X-Bone CTL
x-bone-ctl	265/udp	0.000000	# X-Bone CTL
sst	266/tcp	0.000000	# SCSI on ST
sst	266/udp	0.000000	# SCSI on ST
td-service	267/tcp	0.000013	# Tobit David Service Layer
td-service	267/udp	0.000000	# Tobit David Service Layer
td-replica	268/tcp	0.000050	# Tobit David Replica
td-replica	268/udp	0.000000	# Tobit David Replica
manet	269/tcp	0.000000	# MANET Protocols
manet	269/udp	0.000000	# MANET Protocols
gist	270/tcp	0.000013	# Q-mode encapsulation for GIST messages
gist	270/udp	0.000000	# Q-mode encapsulation for GIST messages
pt-tls	271/tcp	0.000013	# IETF Network Endpoint Assessment (NEA) Posture Transport Protocol over TLS (PT-TLS)
unknown	273/tcp	0.000025
unknown	276/tcp	0.000025
unknown	277/tcp	0.000013
http-mgmt	280/tcp	0.001844
http-mgmt	280/udp	0.000379
personal-link	281/tcp	0.000000	# Personal Link
personal-link	281/udp	0.000544
cableport-ax	282/tcp	0.000000	# cable port a/x | Cable Port A/X
cableport-ax	282/udp	0.000494	# cable port a/x
rescap	283/tcp	0.000000
rescap	283/udp	0.000000
corerjd	284/tcp	0.000013
corerjd	284/udp	0.000000
fxp	286/tcp	0.000000	# FXP Communication
fxp	286/udp	0.000000	# FXP Communication
k-block	287/tcp	0.000000
k-block	287/udp	0.000000
unknown	288/tcp	0.000013
unknown	289/tcp	0.000013
unknown	293/tcp	0.000013
unknown	294/tcp	0.000013
unknown	294/udp	0.000330
unknown	295/tcp	0.000013
unknown	300/tcp	0.000050
unknown	301/tcp	0.000213
unknown	303/tcp	0.000025
unknown	304/udp	0.000991
unknown	305/tcp	0.000013
unknown	306/tcp	0.000464
unknown	307/udp	0.000330
novastorbakcup	308/tcp	0.000025	# novastor backup | Novastor Backup
novastorbakcup	308/udp	0.000329	# novastor backup
entrusttime	309/tcp	0.000000
entrusttime	309/udp	0.000527
bhmds	310/tcp	0.000000
bhmds	310/udp	0.000445
asip-webadmin	311/tcp	0.001857	# appleshare ip webadmin | AppleShare IP WebAdmin
asip-webadmin	311/udp	0.000494	# appleshare ip webadmin
vslmp	312/tcp	0.000000
vslmp	312/udp	0.000593
magenta-logic	313/tcp	0.000000	# Magenta Logic
magenta-logic	313/udp	0.000297
opalis-robot	314/tcp	0.000000	# Opalis Robot
opalis-robot	314/udp	0.000840
dpsi	315/tcp	0.000025
dpsi	315/udp	0.000379
decauth	316/tcp	0.000013
decauth	316/udp	0.000461
zannet	317/tcp	0.000000
zannet	317/udp	0.000346
pkix-timestamp	318/tcp	0.000000	# PKIX TimeStamp
pkix-timestamp	318/udp	0.000000	# PKIX TimeStamp
ptp-event	319/tcp	0.000000	# PTP Event
ptp-event	319/udp	0.000000	# PTP Event
ptp-general	320/tcp	0.000000	# PTP General
ptp-general	320/udp	0.000000	# PTP General
pip	321/tcp	0.000000
pip	321/udp	0.000593
rtsps	322/tcp	0.000013
rtsps	322/udp	0.000000
rpki-rtr	323/tcp	0.000000	# Resource PKI to Router Protocol
unknown	323/udp	0.000330
rpki-rtr-tls	324/tcp	0.000000	# Resource PKI to Router Protocol over TLS
unknown	325/tcp	0.000025
unknown	326/tcp	0.000013
unknown	326/udp	0.000330
unknown	329/tcp	0.000013
texar	333/tcp	0.000113	# Texar Security Port
texar	333/udp	0.000330	# Texar Security Port
unknown	334/tcp	0.000050
unknown	336/tcp	0.000025
unknown	337/tcp	0.000013
unknown	340/tcp	0.000627
unknown	340/udp	0.000330
unknown	343/tcp	0.000050
pdap	344/tcp	0.000000	# Prospero Data Access Protocol
pdap	344/udp	0.000445	# Prospero Data Access Protocol
pawserv	345/tcp	0.000000	# Perf Analysis Workbench
pawserv	345/udp	0.000428	# Perf Analysis Workbench
zserv	346/tcp	0.000013	# Zebra server
zserv	346/udp	0.000428	# Zebra server
fatserv	347/tcp	0.000000	# Fatmen Server
fatserv	347/udp	0.000708	# Fatmen Server
csi-sgwp	348/tcp	0.000000	# Cabletron Management Protocol
csi-sgwp	348/udp	0.000511	# Cabletron Management Protocol
mftp	349/tcp	0.000000
mftp	349/udp	0.000297
matip-type-a	350/tcp	0.000025	# MATIP Type A
matip-type-a	350/udp	0.000379
matip-type-b	351/tcp	0.000013	# MATIP Type B or bhoetty also safetp | MATIP Type B | bhoetty
matip-type-b	351/udp	0.000313	# MATIP Type B or bhoetty
dtag-ste-sb	352/tcp	0.000013	# DTAG, or bhoedap4 | DTAG | bhoedap4
dtag-ste-sb	352/udp	0.000593	# DTAG, or bhoedap4
ndsauth	353/tcp	0.000050
ndsauth	353/udp	0.000264
bh611	354/tcp	0.000000
bh611	354/udp	0.000560
datex-asn	355/tcp	0.000025
datex-asn	355/udp	0.000774
cloanto-net-1	356/tcp	0.000000	# Cloanto Net 1
cloanto-net-1	356/udp	0.000610
bhevent	357/tcp	0.000000
bhevent	357/udp	0.000478
shrinkwrap	358/tcp	0.000013
shrinkwrap	358/udp	0.000445
tenebris_nts	359/tcp	0.000000	# nsrmp | Tenebris Network Trace Service | Network Security Risk Management Protocol
tenebris_nts	359/udp	0.000494	# Tenebris Network Trace Service
scoi2odialog	360/tcp	0.000013
scoi2odialog	360/udp	0.000560
semantix	361/tcp	0.000013
semantix	361/udp	0.000346
srssend	362/tcp	0.000025	# SRS Send
srssend	362/udp	0.000445	# SRS Send
rsvp_tunnel	363/tcp	0.000000	# rsvp-tunnel | RSVP Tunnel
rsvp_tunnel	363/udp	0.002125
aurora-cmgr	364/tcp	0.000013	# Aurora CMGR
aurora-cmgr	364/udp	0.000395
dtk	365/tcp	0.000000	# Deception Tool Kit (www.all.net)
dtk	365/udp	0.000395	# Deception Tool Kit (www.all.net)
odmr	366/tcp	0.000715
odmr	366/udp	0.000478
mortgageware	367/tcp	0.000000
mortgageware	367/udp	0.000445
qbikgdp	368/tcp	0.000000
qbikgdp	368/udp	0.000264
rpc2portmap	369/tcp	0.000013
rpc2portmap	369/udp	0.000725
codaauth2	370/tcp	0.000013
codaauth2	370/udp	0.001038
clearcase	371/tcp	0.000000
clearcase	371/udp	0.000593
ulistserv	372/tcp	0.000000	# ulistproc | Unix Listserv | ListProcessor
ulistserv	372/udp	0.000593	# Unix Listserv
legent-1	373/tcp	0.000013	# Legent Corporation (now Computer Associates Intl.) | Legent Corporation
legent-1	373/udp	0.000395	# Legent Corporation (now Computer Associates Intl.)
legent-2	374/tcp	0.000000	# Legent Corporation (now Computer Associates Intl.) | Legent Corporation
legent-2	374/udp	0.000610	# Legent Corporation (now Computer Associates Intl.)
hassle	375/tcp	0.000000
hassle	375/udp	0.000544
nip	376/tcp	0.000000	# Amiga Envoy Network Inquiry Protocol
nip	376/udp	0.001120	# Amiga Envoy Network Inquiry Proto
tnETOS	377/tcp	0.000000	# NEC Corporation
tnETOS	377/udp	0.000725	# NEC Corporation
dsETOS	378/tcp	0.000000	# NEC Corporation
dsETOS	378/udp	0.000544	# NEC Corporation
is99c	379/tcp	0.000000	# TIA/EIA/IS-99 modem client
is99c	379/udp	0.000395	# TIA/EIA/IS-99 modem client
is99s	380/tcp	0.000013	# TIA/EIA/IS-99 modem server
is99s	380/udp	0.000494	# TIA/EIA/IS-99 modem server
hp-collector	381/tcp	0.000000	# hp performance data collector
hp-collector	381/udp	0.000577	# hp performance data collector
hp-managed-node	382/tcp	0.000000	# hp performance data managed node
hp-managed-node	382/udp	0.000346	# hp performance data managed node
hp-alarm-mgr	383/tcp	0.000013	# hp performance data alarm manager
hp-alarm-mgr	383/udp	0.000362	# hp performance data alarm manager
arns	384/tcp	0.000000	# A Remote Network Server System
arns	384/udp	0.000412	# A Remote Network Server System
ibm-app	385/tcp	0.000000	# IBM Application
ibm-app	385/udp	0.000692	# IBM Application
asa	386/tcp	0.000000	# ASA Message Router Object Def.
asa	386/udp	0.000741	# ASA Message Router Object Def.
aurp	387/tcp	0.000000	# Appletalk Update-Based Routing Pro.
aurp	387/udp	0.001285	# Appletalk Update-Based Routing Pro.
unidata-ldm	388/tcp	0.000088	# Unidata LDM Version 4 | Unidata LDM
unidata-ldm	388/udp	0.000329	# Unidata LDM Version 4
ldap	389/tcp	0.004717	# Lightweight Directory Access Protocol
ldap	389/udp	0.004300	# Lightweight Directory Access Protocol
uis	390/tcp	0.000000
uis	390/udp	0.000478
synotics-relay	391/tcp	0.000013	# SynOptics SNMP Relay Port
synotics-relay	391/udp	0.000988	# SynOptics SNMP Relay Port
synotics-broker	392/tcp	0.000013	# SynOptics Port Broker Port
synotics-broker	392/udp	0.000280	# SynOptics Port Broker Port
dis	393/tcp	0.000000	# meta5 | Data Interpretation System | Meta5
dis	393/udp	0.001302	# Data Interpretation System
embl-ndt	394/tcp	0.000000	# EMBL Nucleic Data Transfer
embl-ndt	394/udp	0.000461	# EMBL Nucleic Data Transfer
netcp	395/tcp	0.000000	# NETscout Control Protocol | NetScout Control Protocol
netcp	395/udp	0.000428	# NETscout Control Protocol
netware-ip	396/tcp	0.000000	# Novell Netware over IP
netware-ip	396/udp	0.000379	# Novell Netware over IP
mptn	397/tcp	0.000025	# Multi Protocol Trans. Net.
mptn	397/udp	0.000511	# Multi Protocol Trans. Net.
kryptolan	398/tcp	0.000000
kryptolan	398/udp	0.000659
iso-tsap-c2	399/tcp	0.000025	# ISO-TSAP Class 2 | ISO Transport Class 2 Non-Control over TCP | ISO Transport Class 2 Non-Control over UDP
iso-tsap-c2	399/udp	0.000395	# ISO-TSAP Class 2
work-sol	400/tcp	0.000075	# osb-sd | Workstation Solutions | Oracle Secure Backup
work-sol	400/udp	0.000643	# Workstation Solutions
ups	401/tcp	0.000025	# Uninterruptible Power Supply
ups	401/udp	0.000560	# Uninterruptible Power Supply
genie	402/tcp	0.000038	# Genie Protocol
genie	402/udp	0.001730	# Genie Protocol
decap	403/tcp	0.000025
decap	403/udp	0.001021
nced	404/tcp	0.000025
nced	404/udp	0.000478
ncld	405/tcp	0.000000
ncld	405/udp	0.000379
imsp	406/tcp	0.000163	# Interactive Mail Support Protocol
imsp	406/udp	0.000560	# Interactive Mail Support Protocol
timbuktu	407/tcp	0.001129
timbuktu	407/udp	0.005305
prm-sm	408/tcp	0.000013	# Prospero Resource Manager Sys. Man.
prm-sm	408/udp	0.000445	# Prospero Resource Manager Sys. Man.
prm-nm	409/tcp	0.000000	# Prospero Resource Manager Node Man.
prm-nm	409/udp	0.000461	# Prospero Resource Manager Node Man.
decladebug	410/tcp	0.000025	# DECLadebug Remote Debug Protocol
decladebug	410/udp	0.000494	# DECLadebug Remote Debug Protocol
rmt	411/tcp	0.000088	# Remote MT Protocol
rmt	411/udp	0.000560	# Remote MT Protocol
synoptics-trap	412/tcp	0.000025	# Trap Convention Port
synoptics-trap	412/udp	0.000511	# Trap Convention Port
smsp	413/tcp	0.000013	# Storage Management Services Protocol
smsp	413/udp	0.000395
infoseek	414/tcp	0.000013
infoseek	414/udp	0.000346
bnet	415/tcp	0.000025
bnet	415/udp	0.000445
silverplatter	416/tcp	0.000201
silverplatter	416/udp	0.000675
onmux	417/tcp	0.000226	# Meeting maker
onmux	417/udp	0.000774	# Meeting maker
hyper-g	418/tcp	0.000025
hyper-g	418/udp	0.000544
ariel1	419/tcp	0.000138	# Ariel 1
ariel1	419/udp	0.000544
smpte	420/tcp	0.000013
smpte	420/udp	0.000511
ariel2	421/tcp	0.000000	# Ariel 2
ariel2	421/udp	0.000428
ariel3	422/tcp	0.000025	# Ariel 3
ariel3	422/udp	0.000346
opc-job-start	423/tcp	0.000013	# IBM Operations Planning and Control Start
opc-job-start	423/udp	0.000329	# IBM Operations Planning and Control Start
opc-job-track	424/tcp	0.000000	# IBM Operations Planning and Control Track
opc-job-track	424/udp	0.000610	# IBM Operations Planning and Control Track
icad-el	425/tcp	0.000326	# ICAD
icad-el	425/udp	0.000428
smartsdp	426/tcp	0.000000
smartsdp	426/udp	0.001104
svrloc	427/tcp	0.005382	# Server Location
svrloc	427/udp	0.018270	# Server Location
ocs_cmu	428/tcp	0.000013	# ocs-cmu
ocs_cmu	428/udp	0.000329
ocs_amu	429/tcp	0.000000	# ocs-amu
ocs_amu	429/udp	0.000428
utmpsd	430/tcp	0.000000
utmpsd	430/udp	0.000362
utmpcd	431/tcp	0.000000
utmpcd	431/udp	0.000461
iasd	432/tcp	0.000013
iasd	432/udp	0.000577
nnsp	433/tcp	0.000000	# Usenet, Network News Transfer | NNTP for transit servers (NNSP)
nnsp	433/udp	0.000445
mobileip-agent	434/tcp	0.000013
mobileip-agent	434/udp	0.002257
mobilip-mn	435/tcp	0.000013
mobilip-mn	435/udp	0.000511
dna-cml	436/tcp	0.000000
dna-cml	436/udp	0.000379
comscm	437/tcp	0.000025
comscm	437/udp	0.000741
dsfgw	438/tcp	0.000013
dsfgw	438/udp	0.000725
dasp	439/tcp	0.000013
dasp	439/udp	0.000412
sgcp	440/tcp	0.000063
sgcp	440/udp	0.000807
decvms-sysmgt	441/tcp	0.000138
decvms-sysmgt	441/udp	0.000395
cvc_hostd	442/tcp	0.000138	# cvc-hostd
cvc_hostd	442/udp	0.000774
https	443/sctp	0.000000	# http protocol over TLS/SSL
https	443/tcp	0.208669	# secure http (SSL)
https	443/udp	0.010840
snpp	444/tcp	0.004466	# Simple Network Paging Protocol
snpp	444/udp	0.000873	# Simple Network Paging Protocol
microsoft-ds	445/tcp	0.056944	# SMB directly over IP
microsoft-ds	445/udp	0.253118
ddm-rdb	446/tcp	0.000075	# DDM-Remote Relational Database Access
ddm-rdb	446/udp	0.000461
ddm-dfm	447/tcp	0.000138	# DDM-Distributed File Management
ddm-dfm	447/udp	0.000675
ddm-ssl	448/tcp	0.000050	# ddm-byte | DDM-Remote DB Access Using Secure Sockets
ddm-ssl	448/udp	0.000511	# ddm-byte
as-servermap	449/tcp	0.000063	# AS Server Mapper
as-servermap	449/udp	0.000675	# AS Server Mapper
tserver	450/tcp	0.000050	# Computer Supported Telecomunication Applications
tserver	450/udp	0.000692
sfs-smp-net	451/tcp	0.000013	# Cray Network Semaphore server
sfs-smp-net	451/udp	0.000774	# Cray Network Semaphore server
sfs-config	452/tcp	0.000013	# Cray SFS config server
sfs-config	452/udp	0.000297	# Cray SFS config server
creativeserver	453/tcp	0.000025
creativeserver	453/udp	0.000280
contentserver	454/tcp	0.000038
contentserver	454/udp	0.000329
creativepartnr	455/tcp	0.000000
creativepartnr	455/udp	0.000758
macon	456/tcp	0.000050	# macon-tcp | macon-udp
macon	456/udp	0.000494
scohelp	457/tcp	0.000013
scohelp	457/udp	0.000610
appleqtc	458/tcp	0.000314	# apple quick time
appleqtc	458/udp	0.000725	# apple quick time
ampr-rcmd	459/tcp	0.000000
ampr-rcmd	459/udp	0.000362
skronk	460/tcp	0.000013
skronk	460/udp	0.000610
datasurfsrv	461/tcp	0.000000	# DataRampSrv
datasurfsrv	461/udp	0.000379
datasurfsrvsec	462/tcp	0.000025	# DataRampSrvSec
datasurfsrvsec	462/udp	0.000560
alpes	463/tcp	0.000000
alpes	463/udp	0.000494
kpasswd5	464/tcp	0.001192	# Kerberos (v5) | kpasswd
kpasswd5	464/udp	0.004300	# Kerberos (v5)
smtps	465/tcp	0.013888	# submissions | igmpv3lite | urd | smtp protocol over TLS/SSL (was ssmtp) | URL Rendesvous Directory for SSM | IGMP over UDP for SSM | URL Rendezvous Directory for SSM | Message Submission over TLS protocol
smtps	465/udp	0.000527	# smtp protocol over TLS/SSL (was ssmtp)
digital-vrc	466/tcp	0.000025
digital-vrc	466/udp	0.000297
mylex-mapd	467/tcp	0.000000
mylex-mapd	467/udp	0.000445
photuris	468/tcp	0.000000	# Photuris Key Management | proturis
photuris	468/udp	0.000560
rcp	469/tcp	0.000000	# Radio Control Protocol
rcp	469/udp	0.000692	# Radio Control Protocol
scx-proxy	470/tcp	0.000013
scx-proxy	470/udp	0.000395
mondex	471/tcp	0.000000
mondex	471/udp	0.000478
ljk-login	472/tcp	0.000013
ljk-login	472/udp	0.000758
hybrid-pop	473/tcp	0.000013
hybrid-pop	473/udp	0.000445
tn-tl-w1	474/tcp	0.000000	# tn-tl-w2
tn-tl-w2	474/udp	0.000214
tcpnethaspsrv	475/tcp	0.000138
tcpnethaspsrv	475/udp	0.000643
tn-tl-fd1	476/tcp	0.000000
tn-tl-fd1	476/udp	0.000346
ss7ns	477/tcp	0.000000
ss7ns	477/udp	0.000626
spsc	478/tcp	0.000000
spsc	478/udp	0.000610
iafserver	479/tcp	0.000013
iafserver	479/udp	0.000675
loadsrv	480/tcp	0.000013	# iafdbase
iafdbase	480/udp	0.000461
dvs	481/tcp	0.000176	# ph | Ph service
ph	481/udp	0.000445
bgs-nsi	482/tcp	0.000000
xlog	482/udp	0.000577
ulpnet	483/tcp	0.000000
ulpnet	483/udp	0.000461
integra-sme	484/tcp	0.000000	# Integra Software Management Environment
integra-sme	484/udp	0.001186	# Integra Software Management Environment
powerburst	485/tcp	0.000013	# Air Soft Power Burst
powerburst	485/udp	0.000725	# Air Soft Power Burst
sstats	486/tcp	0.000025	# avian
avian	486/udp	0.000379
saft	487/tcp	0.000013	# saft Simple Asynchronous File Transfer
saft	487/udp	0.000428	# saft Simple Asynchronous File Transfer
gss-http	488/tcp	0.000000
gss-http	488/udp	0.000643
nest-protocol	489/tcp	0.000000
nest-protocol	489/udp	0.000544
micom-pfs	490/tcp	0.000000
micom-pfs	490/udp	0.000577
go-login	491/tcp	0.000050
go-login	491/udp	0.000297
ticf-1	492/tcp	0.000050	# Transport Independent Convergence for FNA
ticf-1	492/udp	0.000610	# Transport Independent Convergence for FNA
ticf-2	493/tcp	0.000025	# Transport Independent Convergence for FNA
ticf-2	493/udp	0.000560	# Transport Independent Convergence for FNA
pov-ray	494/tcp	0.000000
pov-ray	494/udp	0.000478
intecourier	495/tcp	0.000000
intecourier	495/udp	0.000362
pim-rp-disc	496/tcp	0.000013
pim-rp-disc	496/udp	0.001153
retrospect	497/tcp	0.001179	# Retrospect backup and restore service
retrospect	497/udp	0.017348
siam	498/tcp	0.000000
siam	498/udp	0.000461
iso-ill	499/tcp	0.000000	# ISO ILL Protocol
iso-ill	499/udp	0.000511	# ISO ILL Protocol
isakmp	500/tcp	0.001129
isakmp	500/udp	0.163742
stmf	501/tcp	0.000063
stmf	501/udp	0.001186
mbap	502/tcp	0.000151	# Modbus Application Protocol
mbap	502/udp	0.001318	# Modbus Application Protocol
intrinsa	503/tcp	0.000000
intrinsa	503/udp	0.000708
citadel	504/tcp	0.000000
citadel	504/udp	0.000758
mailbox-lm	505/tcp	0.000038
mailbox-lm	505/udp	0.000807
ohimsrv	506/tcp	0.000000
ohimsrv	506/udp	0.000577
crs	507/tcp	0.000050
crs	507/udp	0.000593
xvttp	508/tcp	0.000000
xvttp	508/udp	0.000461
snare	509/tcp	0.000075
snare	509/udp	0.000643
fcp	510/tcp	0.000063	# FirstClass Protocol
fcp	510/udp	0.000923	# FirstClass Protocol
passgo	511/tcp	0.000038
passgo	511/udp	0.000610
exec	512/tcp	0.000841	# biff | comsat | BSD rexecd(8) | remote process execution; authentication performed using passwords and UNIX login names | used by mail system to notify users of new mail received; currently receives messages only from processes on the same machine
biff	512/udp	0.002142	# comsat
login	513/tcp	0.005595	# who | BSD rlogind(8) | remote login a la telnet; automatic authentication performed based on priviledged port numbers and distributed data bases which identify "authentication domains" | maintains data bases showing who's logged in to machines on a local net and the load average of the machine
who	513/udp	0.002323	# BSD rwhod(8)
shell	514/tcp	0.011078	# syslog | BSD rshd(8) | cmd like exec, but automatic authentication is performed as for login server
syslog	514/udp	0.119804	# BSD syslogd(8)
printer	515/tcp	0.007214	# spooler (lpd) | spooler
printer	515/udp	0.011022	# spooler (lpd)
videotex	516/tcp	0.000013
videotex	516/udp	0.000807
talk	517/tcp	0.000000	# like tenex link, but across | like tenex link, but across machine - unfortunately, doesn't use link protocol (this is actually just a rendezvous port from which a tcp connection is established)
talk	517/udp	0.004794	# BSD talkd(8)
ntalk	518/tcp	0.000013	# (talkd)
ntalk	518/udp	0.022208	# (talkd)
utime	519/tcp	0.000000	# unixtime
utime	519/udp	0.000560	# unixtime
efs	520/tcp	0.000000	# router | extended file name server | local routing process (on site); uses variant of Xerox NS routing information protocol - RIP
route	520/udp	0.139376	# router routed -- RIP
ripng	521/tcp	0.000000
ripng	521/udp	0.000708
ulp	522/tcp	0.000013
ulp	522/udp	0.000511
ibm-db2	523/tcp	0.000113
ibm-db2	523/udp	0.000461
ncp	524/tcp	0.000213
ncp	524/udp	0.000873
timed	525/tcp	0.000063	# timeserver
timed	525/udp	0.000890	# timeserver
tempo	526/tcp	0.000013	# newdate
tempo	526/udp	0.000346	# newdate
stx	527/tcp	0.000000	# Stock IXChange
stx	527/udp	0.000362	# Stock IXChange
custix	528/tcp	0.000013	# Customer IXChange
custix	528/udp	0.000329	# Customer IXChange
irc	529/tcp	0.000000	# irc-serv | IRC-SERV
irc	529/udp	0.000544
courier	530/tcp	0.000013	# rpc
courier	530/udp	0.000873	# rpc
conference	531/tcp	0.000000	# chat
conference	531/udp	0.000824	# chat
netnews	532/tcp	0.000000	# readnews
netnews	532/udp	0.000758	# readnews
netwall	533/tcp	0.000013	# for emergency broadcasts
netwall	533/udp	0.000461	# for emergency broadcasts
mm-admin	534/tcp	0.000000	# windream | MegaMedia Admin | windream Admin
mm-admin	534/udp	0.000379	# MegaMedia Admin
iiop	535/tcp	0.000013
iiop	535/udp	0.000329
opalis-rdv	536/tcp	0.000025
opalis-rdv	536/udp	0.000428
nmsp	537/tcp	0.000000	# Networked Media Streaming Protocol
nmsp	537/udp	0.000774	# Networked Media Streaming Protocol
gdomap	538/tcp	0.000063
gdomap	538/udp	0.000461
apertus-ldp	539/tcp	0.000000	# Apertus Technologies Load Determination
apertus-ldp	539/udp	0.002274	# Apertus Technologies Load Determination
uucp	540/tcp	0.000138	# uucpd
uucp	540/udp	0.000791	# uucpd
uucp-rlogin	541/tcp	0.000489
uucp-rlogin	541/udp	0.000807
commerce	542/tcp	0.000013
commerce	542/udp	0.000675
klogin	543/tcp	0.005282	# Kerberos (v4/v5)
klogin	543/udp	0.000610	# Kerberos (v4/v5)
kshell	544/tcp	0.005269	# krcmd Kerberos (v4/v5) | krcmd
kshell	544/udp	0.000527	# krcmd Kerberos (v4/v5)
ekshell	545/tcp	0.000276	# Kerberos encrypted remote shell -kfall | appleqtcsrvr
appleqtcsrvr	545/udp	0.000478
dhcpv6-client	546/tcp	0.000000	# DHCPv6 Client
dhcpv6-client	546/udp	0.000840	# DHCPv6 Client
dhcpv6-server	547/tcp	0.000000	# DHCPv6 Server
dhcpv6-server	547/udp	0.000807	# DHCPv6 Server
afp	548/tcp	0.012395	# afpovertcp | AFP over TCP
afp	548/udp	0.000774	# AFP over UDP
idfp	549/tcp	0.000000
idfp	549/udp	0.000461
new-rwho	550/tcp	0.000000	# new-who
new-rwho	550/udp	0.001170	# new-who
cybercash	551/tcp	0.000000
cybercash	551/udp	0.000774
deviceshare	552/tcp	0.000013	# devshr-nts
deviceshare	552/udp	0.000840
pirp	553/tcp	0.000038
pirp	553/udp	0.000593
rtsp	554/tcp	0.008104	# Real Time Stream Control Protocol | Real Time Streaming Protocol (RTSP)
rtsp	554/udp	0.000593	# Real Time Stream Control Protocol
dsf	555/tcp	0.000238
dsf	555/udp	0.000329
remotefs	556/tcp	0.000125	# rfs, rfs_server, Brunhoff remote filesystem | rfs server
remotefs	556/udp	0.000428	# rfs, rfs_server, Brunhoff remote filesystem
openvms-sysipc	557/tcp	0.000113
openvms-sysipc	557/udp	0.000461
sdnskmp	558/tcp	0.000000
sdnskmp	558/udp	0.000461
teedtap	559/tcp	0.000000
teedtap	559/udp	0.001433
rmonitor	560/tcp	0.000038	# rmonitord
rmonitor	560/udp	0.000626	# rmonitord
monitor	561/tcp	0.000038
monitor	561/udp	0.000544
chshell	562/tcp	0.000000	# chcmd
chshell	562/udp	0.000346	# chcmd
snews	563/tcp	0.000916	# nntps | nntp protocol over TLS/SSL (was snntp)
snews	563/udp	0.000675
9pfs	564/tcp	0.000013	# plan 9 file service
9pfs	564/udp	0.000527	# plan 9 file service
whoami	565/tcp	0.000000
whoami	565/udp	0.000445
streettalk	566/tcp	0.000000
streettalk	566/udp	0.000000
banyan-rpc	567/tcp	0.000000
banyan-rpc	567/udp	0.000544
ms-shuttle	568/tcp	0.000025	# Microsoft shuttle | microsoft shuttle
ms-shuttle	568/udp	0.000824	# Microsoft shuttle
ms-rome	569/tcp	0.000013	# Microsoft rome | microsoft rome
ms-rome	569/udp	0.000758	# Microsoft rome
meter	570/tcp	0.000013	# demon
meter	570/udp	0.000461	# demon
umeter	571/tcp	0.000013	# meter | udemon
umeter	571/udp	0.000692	# udemon
sonar	572/tcp	0.000013
sonar	572/udp	0.000297
banyan-vip	573/tcp	0.000000
banyan-vip	573/udp	0.000939
ftp-agent	574/tcp	0.000000	# FTP Software Agent System
ftp-agent	574/udp	0.000428	# FTP Software Agent System
vemmi	575/tcp	0.000000
vemmi	575/udp	0.000379
ipcd	576/tcp	0.000000
ipcd	576/udp	0.000346
vnas	577/tcp	0.000063
vnas	577/udp	0.000972
ipdd	578/tcp	0.000075
ipdd	578/udp	0.000527
decbsrv	579/tcp	0.000000
decbsrv	579/udp	0.000544
sntp-heartbeat	580/tcp	0.000000	# SNTP HEARTBEAT
sntp-heartbeat	580/udp	0.000428
bdp	581/tcp	0.000000	# Bundle Discovery Protocol
bdp	581/udp	0.000395	# Bundle Discovery Protocol
scc-security	582/tcp	0.000013	# SCC Security
scc-security	582/udp	0.000280
philips-vc	583/tcp	0.000013	# Philips Video-Conferencing
philips-vc	583/udp	0.000544	# Philips Video-Conferencing
keyserver	584/tcp	0.000000	# Key Server
keyserver	584/udp	0.001005
imap4-ssl	585/tcp	0.000000	# IMAP4+SSL (use of 585 is not recommended,
imap4-ssl	585/udp	0.000412	# use 993 instead)
password-chg	586/tcp	0.000000	# Password Change
password-chg	586/udp	0.000758
submission	587/tcp	0.019721	# Message Submission
submission	587/udp	0.000692
cal	588/tcp	0.000000
cal	588/udp	0.000544
eyelink	589/tcp	0.000000
eyelink	589/udp	0.000461
tns-cml	590/tcp	0.000000	# TNS CML
tns-cml	590/udp	0.000577
http-alt	591/tcp	0.000075	# FileMaker, Inc. - HTTP Alternate | FileMaker, Inc. - HTTP Alternate (see Port 80)
http-alt	591/udp	0.000527	# FileMaker, Inc. - HTTP Alternate
eudora-set	592/tcp	0.000000	# Eudora Set
eudora-set	592/udp	0.000626
http-rpc-epmap	593/tcp	0.001242	# HTTP RPC Ep Map
http-rpc-epmap	593/udp	0.022933	# HTTP RPC Ep Map
tpip	594/tcp	0.000000
tpip	594/udp	0.000873
cab-protocol	595/tcp	0.000000	# CAB Protocol
cab-protocol	595/udp	0.000445
smsd	596/tcp	0.000013
smsd	596/udp	0.000544
ptcnameservice	597/tcp	0.000000	# PTC Name Service
ptcnameservice	597/udp	0.000214	# PTC Name Service
sco-websrvrmg3	598/tcp	0.000013	# SCO Web Server Manager 3
sco-websrvrmg3	598/udp	0.000626	# SCO Web Server Manager 3
acp	599/tcp	0.000013	# Aeolon Core Protocol
acp	599/udp	0.000412	# Aeolon Core Protocol
ipcserver	600/tcp	0.000100	# Sun IPC server
ipcserver	600/udp	0.000741	# Sun IPC server
syslog-conn	601/tcp	0.000025	# Reliable Syslog Service
syslog-conn	601/udp	0.000330	# Reliable Syslog Service
xmlrpc-beep	602/tcp	0.000100	# XML-RPC over BEEP
xmlrpc-beep	602/udp	0.000000	# XML-RPC over BEEP
mnotes	603/tcp	0.000063	# idxp | CommonTime Mnotes PDA Synchronization | IDXP
idxp	603/udp	0.000991
tunnel	604/tcp	0.000025
tunnel	604/udp	0.000000
soap-beep	605/tcp	0.000050	# SOAP over BEEP
soap-beep	605/udp	0.000661	# SOAP over BEEP
urm	606/tcp	0.000088	# Cray Unified Resource Manager
urm	606/udp	0.000494	# Cray Unified Resource Manager
nqs	607/tcp	0.000025
nqs	607/udp	0.000758
sift-uft	608/tcp	0.000025	# Sender-Initiated/Unsolicited File Transfer
sift-uft	608/udp	0.000544	# Sender-Initiated/Unsolicited File Transfer
npmp-trap	609/tcp	0.000050
npmp-trap	609/udp	0.000379
npmp-local	610/tcp	0.000113
npmp-local	610/udp	0.000741
npmp-gui	611/tcp	0.000038
npmp-gui	611/udp	0.000577
hmmp-ind	612/tcp	0.000013	# HMMP Indication
hmmp-ind	612/udp	0.000000	# HMMP Indication
hmmp-op	613/tcp	0.000013	# HMMP Operation
hmmp-op	613/udp	0.000330	# HMMP Operation
sshell	614/tcp	0.000013	# SSLshell
sshell	614/udp	0.000330	# SSLshell
sco-inetmgr	615/tcp	0.000063	# Internet Configuration Manager
sco-inetmgr	615/udp	0.000330	# Internet Configuration Manager
sco-sysmgr	616/tcp	0.000289	# SCO System Administration Server
sco-sysmgr	616/udp	0.000330	# SCO System Administration Server
sco-dtmgr	617/tcp	0.000226	# SCO Desktop Administration Server or Arkeia (www.arkeia.com) backup software | SCO Desktop Administration Server
sco-dtmgr	617/udp	0.001302	# SCO Desktop Administration Server
dei-icda	618/tcp	0.000013
dei-icda	618/udp	0.000000
compaq-evm	619/tcp	0.000025	# Compaq EVM
compaq-evm	619/udp	0.000991	# Compaq EVM
sco-websrvrmgr	620/tcp	0.000063	# SCO WebServer Manager
sco-websrvrmgr	620/udp	0.000991	# SCO WebServer Manager
escp-ip	621/tcp	0.000088	# ESCP
escp-ip	621/udp	0.000661	# ESCP
collaborator	622/tcp	0.000038
collaborator	622/udp	0.000000
oob-ws-http	623/tcp	0.000151	# asf-rmcp | DMTF out-of-band web services management protocol | ASF Remote Management and Control Protocol
asf-rmcp	623/udp	0.007929	# ASF Remote Management and Control
cryptoadmin	624/tcp	0.000038	# Crypto Admin
cryptoadmin	624/udp	0.000000	# Crypto Admin
apple-xsrvr-admin	625/tcp	0.001869	# dec_dlm | dec-dlm | Apple Mac Xserver admin | DEC DLM
dec_dlm	625/udp	0.000000	# DEC DLM
apple-imap-admin	626/tcp	0.000025	# asia | Apple IMAP mail admin | ASIA
serialnumberd	626/udp	0.021473	# Mac OS X Server serial number (licensing) daemon
passgo-tivoli	627/tcp	0.000050	# PassGo Tivoli
passgo-tivoli	627/udp	0.000000	# PassGo Tivoli
qmqp	628/tcp	0.000038	# Qmail Quick Mail Queueing
qmqp	628/udp	0.000661
3com-amp3	629/tcp	0.000063	# 3Com AMP3
3com-amp3	629/udp	0.000000	# 3Com AMP3
rda	630/tcp	0.000050
rda	630/udp	0.000330
ipp	631/tcp	0.006160	# ipps | Internet Printing Protocol -- for one implementation see http://www.cups.org (Common UNIX Printing System) | IPP (Internet Printing Protocol) | Internet Printing Protocol over HTTPS
ipp	631/udp	0.450281	# Internet Printing Protocol
bmpp	632/tcp	0.000050
bmpp	632/udp	0.000661
servstat	633/tcp	0.000038	# Service Status update (Sterling Software)
servstat	633/udp	0.000000	# Service Status update (Sterling Software)
ginad	634/tcp	0.000063
ginad	634/udp	0.000692
rlzdbase	635/tcp	0.000075	# RLZ DBase
mount	635/udp	0.000511	# NFS Mount Service
ldapssl	636/tcp	0.002083	# ldaps | LDAP over SSL | ldap protocol over TLS/SSL (was sldap)
ldaps	636/udp	0.000661	# ldap protocol over TLS/SSL (was sldap)
lanserver	637/tcp	0.000038
lanserver	637/udp	0.000428
mcns-sec	638/tcp	0.000050
mcns-sec	638/udp	0.000000
msdp	639/tcp	0.000151
msdp	639/udp	0.001321
entrust-sps	640/tcp	0.000050
pcnfs	640/udp	0.000890	# PC-NFS DOS Authentication
repcmd	641/tcp	0.000088
repcmd	641/udp	0.000661
esro-emsdp	642/tcp	0.000075	# ESRO-EMSDP V1.3
esro-emsdp	642/udp	0.000000	# ESRO-EMSDP V1.3
sanity	643/tcp	0.000013
sanity	643/udp	0.001982
dwr	644/tcp	0.000038
dwr	644/udp	0.000991
pssc	645/tcp	0.000025
pssc	645/udp	0.000000
ldp	646/tcp	0.006549	# Label Distribution
ldp	646/udp	0.000000	# Label Distribution
dhcp-failover	647/tcp	0.000050	# DHCP Failover
dhcp-failover	647/udp	0.000000	# DHCP Failover
rrp	648/tcp	0.000577	# Registry Registrar Protocol (RRP)
rrp	648/udp	0.000330	# Registry Registrar Protocol (RRP)
cadview-3d	649/tcp	0.000063	# Cadview-3d - streaming 3d models over the internet
cadview-3d	649/udp	0.000330	# Cadview-3d - streaming 3d models over the internet
obex	650/tcp	0.000000
bwnfs	650/udp	0.000544	# BW-NFS DOS Authentication
ieee-mms	651/tcp	0.000050	# IEEE MMS
ieee-mms	651/udp	0.000000	# IEEE MMS
hello-port	652/tcp	0.000013	# HELLO_PORT
hello-port	652/udp	0.000330	# HELLO_PORT
repscmd	653/tcp	0.000063	# RepCmd
repscmd	653/udp	0.000661	# RepCmd
aodv	654/tcp	0.000038
aodv	654/udp	0.000000
tinc	655/tcp	0.000100
tinc	655/udp	0.000330
spmp	656/tcp	0.000038
spmp	656/udp	0.000000
rmc	657/tcp	0.000113
rmc	657/udp	0.001321
tenfold	658/tcp	0.000050
tenfold	658/udp	0.000000
unknown	659/tcp	0.000100
unknown	659/udp	0.000661
mac-srvr-admin	660/tcp	0.000100	# MacOS Server Admin
mac-srvr-admin	660/udp	0.000577	# MacOS Server Admin
hap	661/tcp	0.000050
hap	661/udp	0.000000
pftp	662/tcp	0.000013
pftp	662/udp	0.000330
purenoise	663/tcp	0.000050
purenoise	663/udp	0.000000
secure-aux-bus	664/tcp	0.000063	# asf-secure-rmcp | oob-ws-https | DMTF out-of-band secure web services management protocol | ASF Secure Remote Management and Control Protocol
secure-aux-bus	664/udp	0.003634
sun-dr	665/tcp	0.000063	# Sun DR
sun-dr	665/udp	0.000000	# Sun DR
doom	666/tcp	0.000289	# mdqs | Id Software Doom | doom Id Software
doom	666/udp	0.000956	# doom Id Software
disclose	667/tcp	0.000238	# campaign contribution disclosures - SDR Technologies
disclose	667/udp	0.000330	# campaign contribution disclosures - SDR Technologies
mecomm	668/tcp	0.000213
mecomm	668/udp	0.000000
meregister	669/tcp	0.000088
meregister	669/udp	0.000000
vacdsm-sws	670/tcp	0.000038
vacdsm-sws	670/udp	0.000000
vacdsm-app	671/tcp	0.000000
vacdsm-app	671/udp	0.000000
vpps-qua	672/tcp	0.000025
vpps-qua	672/udp	0.000991
cimplex	673/tcp	0.000050
cimplex	673/udp	0.000000
acap	674/tcp	0.000113	# ACAP server of Communigate (www.stalker.com)
acap	674/udp	0.000661
dctp	675/tcp	0.000038
dctp	675/udp	0.000330
vpps-via	676/tcp	0.000038	# VPPS Via
vpps-via	676/udp	0.000000	# VPPS Via
vpp	677/tcp	0.000025	# Virtual Presence Protocol
vpp	677/udp	0.000000	# Virtual Presence Protocol
ggf-ncp	678/tcp	0.000075	# GNU Generation Foundation NCP
ggf-ncp	678/udp	0.000000	# GNU Generation Foundation NCP
mrm	679/tcp	0.000000
mrm	679/udp	0.000330
entrust-aaas	680/tcp	0.000038
entrust-aaas	680/udp	0.000661
entrust-aams	681/tcp	0.000038
entrust-aams	681/udp	0.000991
xfr	682/tcp	0.000063
xfr	682/udp	0.002643
corba-iiop	683/tcp	0.000176	# CORBA IIOP
corba-iiop	683/udp	0.003304
corba-iiop-ssl	684/tcp	0.000113	# CORBA IIOP SSL
corba-iiop-ssl	684/udp	0.002313	# CORBA IIOP SSL
mdc-portmapper	685/tcp	0.000038	# MDC Port Mapper
mdc-portmapper	685/udp	0.002973	# MDC Port Mapper
hcp-wismar	686/tcp	0.000025	# Hardware Control Protocol Wismar
hcp-wismar	686/udp	0.002973	# Hardware Control Protocol Wismar
asipregistry	687/tcp	0.000188
asipregistry	687/udp	0.001982
realm-rusd	688/tcp	0.000025	# ApplianceWare managment protocol
realm-rusd	688/udp	0.001982	# ApplianceWare managment protocol
nmap	689/tcp	0.000038
nmap	689/udp	0.001321
vatp	690/tcp	0.000088	# Velazquez Application Transfer Protocol | Velneo Application Transfer Protocol
vatp	690/udp	0.000330	# Velazquez Application Transfer Protocol
resvc	691/tcp	0.000376	# msexch-routing | The Microsoft Exchange 2000 Server Routing Service | MS Exchange Routing
msexch-routing	691/udp	0.000330	# MS Exchange Routing
hyperwave-isp	692/tcp	0.000038
hyperwave-isp	692/udp	0.000000
connendp	693/tcp	0.000000	# almanid Connection Endpoint
connendp	693/udp	0.000000	# almanid Connection Endpoint
ha-cluster	694/tcp	0.000038
ha-cluster	694/udp	0.000661
ieee-mms-ssl	695/tcp	0.000063
ieee-mms-ssl	695/udp	0.000000
rushd	696/tcp	0.000050
rushd	696/udp	0.000330
uuidgen	697/tcp	0.000025
uuidgen	697/udp	0.000330
olsr	698/tcp	0.000025
olsr	698/udp	0.000000
accessnetwork	699/tcp	0.000025	# Access Network
accessnetwork	699/udp	0.000000	# Access Network
epp	700/tcp	0.000289	# Extensible Provisioning Protocol
epp	700/udp	0.000330	# Extensible Provisioning Protocol
lmp	701/tcp	0.000151	# Link Management Protocol (LMP)
lmp	701/udp	0.000330	# Link Management Protocol (LMP)
iris-beep	702/tcp	0.000050	# IRIS over BEEP
iris-beep	702/udp	0.000000	# IRIS over BEEP
unknown	703/tcp	0.000038
elcsd	704/tcp	0.000038	# errlog copy/server daemon
elcsd	704/udp	0.000923	# errlog copy/server daemon
agentx	705/tcp	0.000414
agentx	705/udp	0.000661
silc	706/tcp	0.000075	# Secure Internet Live Conferencing -- http://silcnet.org
silc	706/udp	0.000330
borland-dsj	707/tcp	0.000063	# Borland DSJ
borland-dsj	707/udp	0.000000	# Borland DSJ
unknown	708/tcp	0.000038
unknown	708/udp	0.000330
entrustmanager	709/tcp	0.000125	# entrust-kmsh | EntrustManager - NorTel DES auth network see 389/tcp | Entrust Key Management Service Handler
entrustmanager	709/udp	0.000741	# EntrustManager - NorTel DES auth network see 389/tcp
entrust-ash	710/tcp	0.000151	# Entrust Administration Service Handler
entrust-ash	710/udp	0.000330	# Entrust Administration Service Handler
cisco-tdp	711/tcp	0.000401	# Cisco TDP
cisco-tdp	711/udp	0.000330	# Cisco TDP
tbrpf	712/tcp	0.000025
tbrpf	712/udp	0.000000
iris-xpc	713/tcp	0.000125	# IRIS over XPC
iris-xpc	713/udp	0.000000	# IRIS over XPC
iris-xpcs	714/tcp	0.000226	# IRIS over XPCS
iris-xpcs	714/udp	0.000330	# IRIS over XPCS
iris-lwz	715/tcp	0.000088
iris-lwz	715/udp	0.000330
pana	716/tcp	0.000063	# PANA Messages
pana	716/udp	0.000330	# PANA Messages
unknown	717/tcp	0.000025
unknown	717/udp	0.000330
unknown	718/tcp	0.000038
unknown	719/tcp	0.000050
unknown	719/udp	0.000661
unknown	720/tcp	0.000238
unknown	720/udp	0.000991
unknown	721/tcp	0.000038
unknown	721/udp	0.000330
unknown	722/tcp	0.000226
unknown	722/udp	0.000661
omfs	723/tcp	0.000038	# OpenMosix File System
unknown	724/tcp	0.000050
unknown	724/udp	0.000330
unknown	725/tcp	0.000151
unknown	726/tcp	0.000188
unknown	726/udp	0.000330
unknown	727/tcp	0.000063
unknown	727/udp	0.000991
unknown	728/tcp	0.000088
unknown	728/udp	0.000661
netviewdm1	729/tcp	0.000100	# IBM NetView DM/6000 Server/Client
netviewdm1	729/udp	0.000857	# IBM NetView DM/6000 Server/Client
netviewdm2	730/tcp	0.000100	# IBM NetView DM/6000 send/tcp
netviewdm2	730/udp	0.000758	# IBM NetView DM/6000 send/tcp
netviewdm3	731/tcp	0.000100	# IBM NetView DM/6000 receive/tcp
netviewdm3	731/udp	0.000741	# IBM NetView DM/6000 receive/tcp
unknown	732/tcp	0.000113
unknown	732/udp	0.000991
unknown	733/tcp	0.000063
unknown	734/tcp	0.000038
unknown	734/udp	0.000991
unknown	735/tcp	0.000050
unknown	736/tcp	0.000050
unknown	736/udp	0.000330
unknown	737/tcp	0.000025
sometimes-rpc2	737/udp	0.000560	# Rusersd on my OpenBSD box
unknown	738/tcp	0.000025
unknown	738/udp	0.000330
unknown	739/tcp	0.000013
unknown	739/udp	0.000330
netcp	740/tcp	0.000088	# NETscout Control Protocol
netcp	740/udp	0.000873	# NETscout Control Protocol
netgw	741/tcp	0.000050
netgw	741/udp	0.000428
netrcs	742/tcp	0.000013	# Network based Rev. Cont. Sys.
netrcs	742/udp	0.000956	# Network based Rev. Cont. Sys.
unknown	743/tcp	0.000075
unknown	743/udp	0.000330
flexlm	744/tcp	0.000013	# Flexible License Manager
flexlm	744/udp	0.000659	# Flexible License Manager
unknown	745/tcp	0.000050
unknown	745/udp	0.000991
unknown	746/tcp	0.000025
unknown	746/udp	0.000330
fujitsu-dev	747/tcp	0.000025	# Fujitsu Device Control
fujitsu-dev	747/udp	0.000791	# Fujitsu Device Control
ris-cm	748/tcp	0.000113	# Russell Info Sci Calendar Manager
ris-cm	748/udp	0.001120	# Russell Info Sci Calendar Manager
kerberos-adm	749/tcp	0.000326	# Kerberos 5 admin/changepw | kerberos administration
kerberos-adm	749/udp	0.000939	# Kerberos 5 admin/changepw
kerberos	750/tcp	0.000063	# kerberos-iv | loadav | rfile | kdc Kerberos (v4) | kerberos version iv
kerberos	750/udp	0.001269	# kdc Kerberos (v4)
kadmin	751/tcp	0.000038	# pump | Kerberos `kadmin' (v4)
kadmin	751/udp	0.000923	# Kerberos `kadmin' (v4)
qrh	752/tcp	0.000013
qrh	752/udp	0.000725
rrh	753/tcp	0.000013
rrh	753/udp	0.000675
krb_prop	754/tcp	0.000088	# tell | kerberos/v5 server propagation | send
tell	754/udp	0.000330	# send
unknown	755/tcp	0.000025
unknown	756/tcp	0.000038
unknown	756/udp	0.000330
unknown	757/tcp	0.000100
nlogin	758/tcp	0.000088
nlogin	758/udp	0.000708
con	759/tcp	0.000025
con	759/udp	0.000972
krbupdate	760/tcp	0.000050	# ns | kreg Kerberos (v4) registration
ns	760/udp	0.001153
kpasswd	761/tcp	0.000050	# rxe | kpwd Kerberos (v4) "passwd"
rxe	761/udp	0.000956
quotad	762/tcp	0.000075
quotad	762/udp	0.000626
cycleserv	763/tcp	0.000025
cycleserv	763/udp	0.000741
omserv	764/tcp	0.000025
omserv	764/udp	0.001351
webster	765/tcp	0.000213
webster	765/udp	0.000659
unknown	766/tcp	0.000013
unknown	766/udp	0.000330
phonebook	767/tcp	0.000013	# phone
phonebook	767/udp	0.002257	# phone
unknown	768/tcp	0.000013
vid	769/tcp	0.000075
vid	769/udp	0.001252
cadlock	770/tcp	0.000038
cadlock	770/udp	0.001269
rtip	771/tcp	0.000063
rtip	771/udp	0.001219
cycleserv2	772/tcp	0.000000
cycleserv2	772/udp	0.001796
submit	773/tcp	0.000013	# notify
notify	773/udp	0.001713
rpasswd	774/tcp	0.000025	# acmaint_dbd | acmaint-dbd
acmaint_dbd	774/udp	0.001664
entomb	775/tcp	0.000013	# acmaint_transd | acmaint-transd
acmaint_transd	775/udp	0.001993
wpages	776/tcp	0.000025
wpages	776/udp	0.002043
multiling-http	777/tcp	0.000226	# Multiling HTTP
multiling-http	777/udp	0.000661	# Multiling HTTP
unknown	778/tcp	0.000100
unknown	779/tcp	0.000075
unknown	779/udp	0.000330
wpgs	780/tcp	0.000151
wpgs	780/udp	0.002718
hp-collector	781/tcp	0.000013	# hp performance data collector
hp-collector	781/udp	0.002636	# hp performance data collector
hp-managed-node	782/tcp	0.000100	# hp performance data managed node
hp-managed-node	782/udp	0.002933	# hp performance data managed node
spamassassin	783/tcp	0.000163	# Apache SpamAssassin spamd
unknown	784/tcp	0.000025
unknown	784/udp	0.000661
unknown	785/tcp	0.000025
unknown	785/udp	0.000330
concert	786/tcp	0.000100
concert	786/udp	0.002900
qsc	787/tcp	0.001455
unknown	787/udp	0.000330
unknown	788/tcp	0.000038
unknown	788/udp	0.000330
unknown	789/tcp	0.000075
unknown	789/udp	0.001321
unknown	790/tcp	0.000100
unknown	791/tcp	0.000050
unknown	792/tcp	0.000113
unknown	793/tcp	0.000025
unknown	794/tcp	0.000038
unknown	795/tcp	0.000100
unknown	795/udp	0.000330
unknown	796/tcp	0.000038
unknown	797/tcp	0.000038
unknown	797/udp	0.000330
unknown	798/tcp	0.000063
unknown	798/udp	0.000330
controlit	799/tcp	0.000038	# Remotely possible
mdbs_daemon	800/tcp	0.000427	# mdbs-daemon
mdbs_daemon	800/udp	0.004333
device	801/tcp	0.000238
device	801/udp	0.000939
mbap-s	802/tcp	0.000088	# Modbus Application Protocol Secure
unknown	803/tcp	0.000151
unknown	804/tcp	0.000063
unknown	804/udp	0.000330
unknown	805/tcp	0.000088
unknown	805/udp	0.000661
unknown	806/tcp	0.000088
unknown	806/udp	0.000330
unknown	807/tcp	0.000063
unknown	807/udp	0.000330
ccproxy-http	808/tcp	0.002296	# CCProxy HTTP/Gopher/FTP (over HTTP) proxy
unknown	808/udp	0.000330
unknown	809/tcp	0.000075
unknown	809/udp	0.000661
fcp-udp	810/tcp	0.000063	# FCP | FCP Datagram
fcp-udp	810/udp	0.000661	# FCP Datagram
unknown	811/tcp	0.000075
unknown	811/udp	0.000330
unknown	812/tcp	0.000038
unknown	812/udp	0.000991
unknown	813/tcp	0.000050
unknown	814/tcp	0.000063
unknown	814/udp	0.001652
unknown	815/tcp	0.000075
unknown	815/udp	0.000661
unknown	816/tcp	0.000050
unknown	817/tcp	0.000075
unknown	818/tcp	0.000025
unknown	818/udp	0.000991
unknown	819/tcp	0.000050
unknown	819/udp	0.000991
unknown	820/tcp	0.000050
unknown	821/tcp	0.000038
unknown	821/udp	0.000661
unknown	822/tcp	0.000100
unknown	822/udp	0.000330
unknown	823/tcp	0.000100
unknown	823/udp	0.000661
unknown	824/tcp	0.000063
unknown	825/tcp	0.000113
unknown	826/tcp	0.000050
unknown	826/udp	0.001321
unknown	827/tcp	0.000025
itm-mcell-s	828/tcp	0.000063
itm-mcell-s	828/udp	0.000330
pkix-3-ca-ra	829/tcp	0.000125	# PKIX-3 CA/RA
pkix-3-ca-ra	829/udp	0.001982	# PKIX-3 CA/RA
netconf-ssh	830/tcp	0.000075	# NETCONF over SSH
netconf-ssh	830/udp	0.000000	# NETCONF over SSH
netconf-beep	831/tcp	0.000050	# NETCONF over BEEP
netconf-beep	831/udp	0.000661	# NETCONF over BEEP
netconfsoaphttp	832/tcp	0.000038	# NETCONF for SOAP over HTTPS
netconfsoaphttp	832/udp	0.000000	# NETCONF for SOAP over HTTPS
netconfsoapbeep	833/tcp	0.000063	# NETCONF for SOAP over BEEP
netconfsoapbeep	833/udp	0.000661	# NETCONF for SOAP over BEEP
unknown	834/tcp	0.000075
unknown	835/tcp	0.000063
unknown	836/tcp	0.000050
unknown	836/udp	0.000330
unknown	837/tcp	0.000038
unknown	838/tcp	0.000025
unknown	838/udp	0.001652
unknown	839/tcp	0.000100
unknown	839/udp	0.000661
unknown	840/tcp	0.000113
unknown	840/udp	0.000330
unknown	841/tcp	0.000050
unknown	841/udp	0.000991
unknown	842/tcp	0.000025
unknown	842/udp	0.000330
unknown	843/tcp	0.000163
unknown	844/tcp	0.000075
unknown	844/udp	0.000330
unknown	845/tcp	0.000013
unknown	845/udp	0.000661
unknown	846/tcp	0.000100
unknown	846/udp	0.000330
dhcp-failover2	847/tcp	0.000063	# dhcp-failover 2
dhcp-failover2	847/udp	0.000330	# dhcp-failover 2
gdoi	848/tcp	0.000025
gdoi	848/udp	0.000330
unknown	849/tcp	0.000025
unknown	849/udp	0.000330
unknown	850/tcp	0.000050
unknown	851/tcp	0.000050
unknown	851/udp	0.000330
unknown	852/tcp	0.000025
domain-s	853/tcp	0.000025	# DNS query-response protocol run over TLS/DTLS | DNS query-response protocol run over TLS | DNS query-response protocol run over DTLS or QUIC
unknown	853/udp	0.000330
dlep	854/tcp	0.000038	# Dynamic Link Exchange Protocol (DLEP)
unknown	855/tcp	0.000050
unknown	856/tcp	0.000138
unknown	857/tcp	0.000025
unknown	857/udp	0.000661
unknown	858/tcp	0.000075
unknown	859/tcp	0.000088
unknown	859/udp	0.000330
iscsi	860/tcp	0.000063
iscsi	860/udp	0.000000
owamp-control	861/tcp	0.000063	# owamp-test | OWAMP-Test
owamp-control	861/udp	0.000330
twamp-control	862/tcp	0.000100	# twamp-test | Two-way Active Measurement Protocol (TWAMP) Control | TWAMP-Test Receiver Port
twamp-control	862/udp	0.000000	# Two-way Active Measurement Protocol (TWAMP) Control
unknown	863/tcp	0.000075
unknown	863/udp	0.000330
unknown	864/tcp	0.000088
unknown	865/tcp	0.000025
unknown	866/tcp	0.000050
unknown	866/udp	0.000330
unknown	867/tcp	0.000038
unknown	868/tcp	0.000038
unknown	868/udp	0.000330
unknown	869/tcp	0.000038
unknown	869/udp	0.000661
unknown	870/tcp	0.000050
supfilesrv	871/tcp	0.000025	# SUP server
unknown	872/tcp	0.000050
unknown	872/udp	0.000330
rsync	873/tcp	0.003400	# Rsync server ( http://rsync.samba.org )
rsync	873/udp	0.000661
unknown	874/tcp	0.000138
unknown	875/tcp	0.000050
unknown	876/tcp	0.000025
unknown	876/udp	0.000991
unknown	877/tcp	0.000025
unknown	877/udp	0.000330
unknown	878/tcp	0.000088
unknown	879/tcp	0.000038
unknown	880/tcp	0.000464
unknown	880/udp	0.000330
unknown	881/tcp	0.000050
unknown	881/udp	0.000661
unknown	882/tcp	0.000025
unknown	883/tcp	0.000050
unknown	884/tcp	0.000025
unknown	884/udp	0.000330
unknown	885/tcp	0.000025
iclcnet-locate	886/tcp	0.000038	# ICL coNETion locate server
iclcnet-locate	886/udp	0.000330	# ICL coNETion locate server
iclcnet_svinfo	887/tcp	0.000025	# iclcnet-svinfo | ICL coNETion server info
iclcnet_svinfo	887/udp	0.000991	# ICL coNETion server info
accessbuilder	888/tcp	0.000928	# cddbp | or Audio CD Database | CD Database Protocol
accessbuilder	888/udp	0.000923
unknown	889/tcp	0.000063
unknown	889/udp	0.000991
unknown	890/tcp	0.000025
unknown	890/udp	0.000330
unknown	891/tcp	0.000038
unknown	892/tcp	0.000025
unknown	893/tcp	0.000013
unknown	893/udp	0.000991
unknown	894/tcp	0.000063
unknown	895/tcp	0.000038
unknown	895/udp	0.000330
unknown	896/tcp	0.000013
unknown	897/tcp	0.000063
unknown	897/udp	0.000661
sun-manageconsole	898/tcp	0.000339	# Solaris Management Console Java listener (Solaris 8 & 9)
unknown	898/udp	0.000991
unknown	899/tcp	0.000063
unknown	899/udp	0.000330
omginitialrefs	900/tcp	0.000452	# OMG Initial Refs
omginitialrefs	900/udp	0.000661	# OMG Initial Refs
samba-swat	901/tcp	0.000552	# smpnameres | Samba SWAT tool.  Also used by ISS RealSecure. | SMPNAMERES
smpnameres	901/udp	0.000330
iss-realsecure	902/tcp	0.001468	# ideafarm-door | ISS RealSecure Sensor | self documenting Telnet Door | self documenting Door: send 0x00 for info
ideafarm-door	902/udp	0.001982	# self documenting Door: send 0x00 for info
iss-console-mgr	903/tcp	0.000176	# ideafarm-panic | ISS Console Manager | self documenting Telnet Panic Door | self documenting Panic Door: send 0x00 for info
ideafarm-panic	903/udp	0.001652	# self documenting Panic Door: send 0x00 for info
unknown	904/tcp	0.000113
unknown	904/udp	0.000330
unknown	905/tcp	0.000100
unknown	905/udp	0.000330
unknown	906/tcp	0.000050
unknown	907/tcp	0.000025
unknown	908/tcp	0.000025
unknown	908/udp	0.000661
unknown	909/tcp	0.000038
kink	910/tcp	0.000013	# Kerberized Internet Negotiation of Keys (KINK)
kink	910/udp	0.000330	# Kerberized Internet Negotiation of Keys (KINK)
xact-backup	911/tcp	0.000188
xact-backup	911/udp	0.000000
apex-mesh	912/tcp	0.000527	# APEX relay-relay service
apex-mesh	912/udp	0.000000	# APEX relay-relay service
apex-edge	913/tcp	0.000151	# APEX endpoint-relay service
apex-edge	913/udp	0.000000	# APEX endpoint-relay service
rift-lies	914/tcp	0.000075	# Routing in Fat Trees Link Information Elements (TEMPORARY - registered 2023-02-17, extension registered 2024-01-12, expires 2025-02-17)
unknown	914/udp	0.000330
rift-ties	915/tcp	0.000025	# Routing in Fat Trees Topology Information Elements (TEMPORARY - registered 2023-02-17, extension registered 2024-01-12, expires 2025-02-17)
unknown	915/udp	0.000330
unknown	916/tcp	0.000063
unknown	917/udp	0.000991
unknown	918/tcp	0.000088
unknown	919/tcp	0.000050
unknown	919/udp	0.000330
unknown	920/tcp	0.000025
unknown	921/tcp	0.000088
unknown	921/udp	0.000661
unknown	922/tcp	0.000088
unknown	922/udp	0.000661
unknown	923/tcp	0.000063
unknown	923/udp	0.000330
unknown	924/tcp	0.000088
unknown	925/tcp	0.000075
unknown	926/tcp	0.000075
unknown	927/tcp	0.000050
unknown	927/udp	0.000661
unknown	928/tcp	0.000088
unknown	929/tcp	0.000050
unknown	930/tcp	0.000151
unknown	931/tcp	0.000138
unknown	931/udp	0.000991
unknown	932/tcp	0.000013
unknown	932/udp	0.000330
unknown	933/tcp	0.000038
unknown	934/tcp	0.000025
unknown	934/udp	0.000991
unknown	935/tcp	0.000075
unknown	935/udp	0.000330
unknown	936/tcp	0.000050
unknown	937/tcp	0.000013
unknown	937/udp	0.000661
unknown	938/tcp	0.000050
unknown	938/udp	0.000330
unknown	939/tcp	0.000038
unknown	940/udp	0.000991
unknown	941/tcp	0.000050
unknown	941/udp	0.000661
unknown	942/tcp	0.000075
unknown	943/tcp	0.000113
unknown	943/udp	0.000330
unknown	944/tcp	0.000038
unknown	944/udp	0.001321
unknown	945/tcp	0.000050
unknown	945/udp	0.000330
unknown	946/tcp	0.000063
unknown	946/udp	0.000661
unknown	947/tcp	0.000038
unknown	947/udp	0.000991
unknown	948/tcp	0.000050
unknown	949/tcp	0.000063
unknown	949/udp	0.000991
oftep-rpc	950/tcp	0.000050	# Often RPC.statd (on Redhat Linux)
unknown	950/udp	0.000661
unknown	951/tcp	0.000038
unknown	951/udp	0.000661
unknown	952/tcp	0.000063
unknown	952/udp	0.000661
rndc	953/tcp	0.000138	# RNDC is used by BIND 9 (& probably other NS) | BIND9 remote name daemon controller
unknown	953/udp	0.000991
unknown	954/tcp	0.000013
unknown	954/udp	0.000330
unknown	955/tcp	0.000013
unknown	956/tcp	0.000025
unknown	957/tcp	0.000025
unknown	957/udp	0.000330
unknown	958/tcp	0.000063
unknown	958/udp	0.000330
unknown	959/tcp	0.000038
unknown	959/udp	0.001982
unknown	960/tcp	0.000038
unknown	960/udp	0.000661
unknown	961/tcp	0.000075
unknown	961/udp	0.000991
unknown	962/tcp	0.000050
unknown	962/udp	0.000330
unknown	963/tcp	0.000038
unknown	963/udp	0.000330
unknown	964/tcp	0.000038
unknown	965/tcp	0.000075
unknown	965/udp	0.001652
unknown	966/tcp	0.000025
unknown	966/udp	0.000661
unknown	967/tcp	0.000075
unknown	968/tcp	0.000038
unknown	968/udp	0.000330
unknown	969/tcp	0.000100
unknown	970/tcp	0.000038
unknown	970/udp	0.000330
unknown	971/tcp	0.000100
unknown	971/udp	0.000330
unknown	972/tcp	0.000025
unknown	972/udp	0.000330
unknown	973/tcp	0.000075
unknown	973/udp	0.000991
unknown	974/tcp	0.000063
securenetpro-sensor	975/tcp	0.000038
unknown	975/udp	0.000330
unknown	976/tcp	0.000013
unknown	977/tcp	0.000013
unknown	977/udp	0.000991
unknown	978/tcp	0.000025
unknown	978/udp	0.000330
unknown	979/tcp	0.000075
unknown	979/udp	0.000991
unknown	980/tcp	0.000125
unknown	981/tcp	0.000226
unknown	981/udp	0.000661
unknown	982/tcp	0.000025
unknown	982/udp	0.000991
unknown	983/tcp	0.000075
unknown	983/udp	0.002643
unknown	984/tcp	0.000063
unknown	984/udp	0.000991
unknown	985/tcp	0.000063
unknown	985/udp	0.000661
unknown	986/tcp	0.000013
unknown	986/udp	0.000661
unknown	987/tcp	0.000427
unknown	987/udp	0.000330
unknown	988/tcp	0.000050
unknown	988/udp	0.000661
ftps-data	989/tcp	0.000063	# ftp protocol, data, over TLS/SSL
ftps-data	989/udp	0.006277	# ftp protocol, data, over TLS/SSL
ftps	990/tcp	0.005570	# ftp protocol, control, over TLS/SSL
ftps	990/udp	0.004625	# ftp protocol, control, over TLS/SSL
nas	991/tcp	0.000038	# Netnews Administration System
nas	991/udp	0.000000	# Netnews Administration System
telnets	992/tcp	0.000903	# telnet protocol over TLS/SSL
telnets	992/udp	0.000000	# telnet protocol over TLS/SSL
imaps	993/tcp	0.027199	# imap4 protocol over TLS/SSL | IMAP over TLS protocol
imaps	993/udp	0.000661	# imap4 protocol over TLS/SSL
ircs	994/tcp	0.000038	# irc protocol over TLS/SSL
ircs	994/udp	0.000000	# irc protocol over TLS/SSL
pop3s	995/tcp	0.029921	# POP3 protocol over TLS/SSL | pop3 protocol over TLS/SSL (was spop3) | POP3 over TLS protocol
pop3s	995/udp	0.000991	# pop3 protocol over TLS/SSL (was spop3)
xtreelic	996/tcp	0.000100	# XTREE License Server | vsinet
vsinet	996/udp	0.073362
maitrd	997/tcp	0.000038
maitrd	997/udp	0.073247
busboy	998/tcp	0.000100	# puparp
puparp	998/udp	0.073395
garcon	999/tcp	0.000966	# puprouter | applix | Applix ac
applix	999/udp	0.073230	# Applix ac
cadlock	1000/tcp	0.003149	# cadlock2
ock	1000/udp	0.002142
webpush	1001/tcp	0.000364	# HTTP Web Push
unknown	1001/udp	0.004955
windows-icfw	1002/tcp	0.000690	# Windows Internet Connection Firewall or Internet Locator Server for NetMeeting.
unknown	1002/udp	0.000330
unknown	1003/tcp	0.000038
unknown	1003/udp	0.000661
unknown	1004/tcp	0.000088
unknown	1004/udp	0.000661
unknown	1005/tcp	0.000088
unknown	1005/udp	0.000330
unknown	1006/tcp	0.000113
unknown	1006/udp	0.000330
unknown	1007/tcp	0.000201
unknown	1007/udp	0.001652
ufsd	1008/tcp	0.000125	# ufsd		# UFS-aware server
ufsd	1008/udp	0.004020
unknown	1009/tcp	0.000226
unknown	1009/udp	0.000330
surf	1010/tcp	0.000188
surf	1010/udp	0.000661
unknown	1011/tcp	0.000176
unknown	1011/udp	0.000661
unknown	1012/tcp	0.000100
sometimes-rpc1	1012/udp	0.001993	# This is rstatd on my openBSD box
unknown	1013/tcp	0.000125
unknown	1013/udp	0.001321
unknown	1014/tcp	0.000100
unknown	1014/udp	0.002643
unknown	1015/tcp	0.000100
unknown	1015/udp	0.000991
unknown	1016/tcp	0.000050
unknown	1016/udp	0.000330
unknown	1017/tcp	0.000038
unknown	1018/tcp	0.000050
unknown	1018/udp	0.000991
unknown	1019/tcp	0.000075
unknown	1019/udp	0.003304
unknown	1020/tcp	0.000113
unknown	1020/udp	0.001321
exp1	1021/tcp	0.000301	# RFC3692-style Experiment 1 (*)    [RFC4727] | RFC3692-style Experiment 1
exp1	1021/udp	0.003634	# RFC3692-style Experiment 1 (*)    [RFC4727]
exp2	1022/tcp	0.001217	# RFC3692-style Experiment 2 (*)    [RFC4727] | RFC3692-style Experiment 2
exp2	1022/udp	0.007929	# RFC3692-style Experiment 2 (*)    [RFC4727]
netvenuechat	1023/tcp	0.000953	# Nortel NetVenue Notification, Chat, Intercom
unknown	1023/udp	0.016188
kdm	1024/tcp	0.002722	# K Display Manager (KDE version of xdm)
unknown	1024/udp	0.003964
NFS-or-IIS	1025/tcp	0.022406	# blackjack | IIS, NFS, or listener RFS remote_file_sharing | network blackjack
blackjack	1025/udp	0.041813	# network blackjack
LSA-or-nterm	1026/tcp	0.010237	# cap | nterm remote_login network_terminal | Calendar Access Protocol
win-rpc	1026/udp	0.024777	# Commonly used to send MS Messenger spam
IIS	1027/tcp	0.006724	# 6a44 | IPv6 Behind NAT44 CPEs
unknown	1027/udp	0.019822
unknown	1028/tcp	0.003421
ms-lsa	1028/udp	0.013443
ms-lsa	1029/tcp	0.003801	# solid-mux | Solid Mux Server
solid-mux	1029/udp	0.014536	# Solid Mux Server
iad1	1030/tcp	0.002860	# BBN IAD
iad1	1030/udp	0.008007	# BBN IAD
iad2	1031/tcp	0.002221	# BBN IAD
iad2	1031/udp	0.006639	# BBN IAD
iad3	1032/tcp	0.001719	# BBN IAD
iad3	1032/udp	0.006705	# BBN IAD
netinfo	1033/tcp	0.001342	# netinfo-local | Netinfo is apparently on many OS X boxes. | local netinfo port
netinfo-local	1033/udp	0.003964	# local netinfo port
zincite-a	1034/tcp	0.001064	# activesync | Zincite.A backdoor | ActiveSync Notifications
activesync-notify	1034/udp	0.005173	# Windows Mobile device ActiveSync Notifications
multidropper	1035/tcp	0.001216	# mxxrlogin | A Multidropper Adware, or PhoneFree | MX-XR RPC
mxxrlogin	1035/udp	0.001982	# MX-XR RPC
nsstp	1036/tcp	0.001216	# Nebula Secure Segment Transfer Protocol
nsstp	1036/udp	0.004295	# Nebula Secure Segment Transfer Protocol
ams	1037/tcp	0.001216
ams	1037/udp	0.002313
mtqp	1038/tcp	0.002053	# Message Tracking Query Protocol
mtqp	1038/udp	0.004295	# Message Tracking Query Protocol
sbl	1039/tcp	0.002129	# Streamlined Blackhole
sbl	1039/udp	0.004295	# Streamlined Blackhole
netsaint	1040/tcp	0.001342	# netarx | Netsaint status daemon | Netarx Netcare
netarx	1040/udp	0.001982	# Netarx Netcare
danf-ak2	1041/tcp	0.002433	# AK2 Product
danf-ak2	1041/udp	0.004625	# AK2 Product
afrog	1042/tcp	0.000988	# Subnet Roaming
afrog	1042/udp	0.001982	# Subnet Roaming
boinc	1043/tcp	0.000841	# boinc-client | BOINC Client Control or Microsoft IIS | BOINC Client Control
boinc	1043/udp	0.003493	# BOINC Client Control
dcutility	1044/tcp	0.002205	# Dev Consortium Utility
dcutility	1044/udp	0.003304	# Dev Consortium Utility
fpitp	1045/tcp	0.000380	# Fingerprint Image Transfer Protocol
fpitp	1045/udp	0.004625	# Fingerprint Image Transfer Protocol
wfremotertm	1046/tcp	0.000380	# WebFilter Remote Monitor
wfremotertm	1046/udp	0.001652	# WebFilter Remote Monitor
neod1	1047/tcp	0.000760	# Sun's NEO Object Request Broker
neod1	1047/udp	0.002973	# Sun's NEO Object Request Broker
neod2	1048/tcp	0.002357	# Sun's NEO Object Request Broker
neod2	1048/udp	0.002313	# Sun's NEO Object Request Broker
td-postman	1049/tcp	0.002357	# Tobit David Postman VPMN
td-postman	1049/udp	0.003304	# Tobit David Postman VPMN
java-or-OTGfileshare	1050/tcp	0.001669	# cma | J2EE nameserver, also OTG, also called Disk/Application extender. Could also be MiniCommand backdoor OTGlicenseserv | CORBA Management Agent
cma	1050/udp	0.001652	# CORBA Management Agent
optima-vnet	1051/tcp	0.000760	# Optima VNET
optima-vnet	1051/udp	0.001321
ddt	1052/tcp	0.000760	# Dynamic DNS tools | Dynamic DNS Tools
ddt	1052/udp	0.000991	# Dynamic DNS tools
remote-as	1053/tcp	0.002357	# Remote Assistant (RA)
remote-as	1053/udp	0.001652	# Remote Assistant (RA)
brvread	1054/tcp	0.002357
brvread	1054/udp	0.002643
ansyslmd	1055/tcp	0.000760	# ANSYS - License Manager
ansyslmd	1055/udp	0.001652
vfo	1056/tcp	0.002357
vfo	1056/udp	0.002973
startron	1057/tcp	0.000380
startron	1057/udp	0.001652
nim	1058/tcp	0.001380
nim	1058/udp	0.001466
nimreg	1059/tcp	0.001342
nimreg	1059/udp	0.001647
polestar	1060/tcp	0.000760
polestar	1060/udp	0.001652
kiosk	1061/tcp	0.000380
kiosk	1061/udp	0.000991
veracity	1062/tcp	0.000760
veracity	1062/udp	0.000991
kyoceranetdev	1063/tcp	0.000380
kyoceranetdev	1063/udp	0.000661
jstel	1064/tcp	0.002357
jstel	1064/udp	0.001982
syscomlan	1065/tcp	0.002357
syscomlan	1065/udp	0.002313
fpo-fns	1066/tcp	0.001901
fpo-fns	1066/udp	0.002643
instl_boots	1067/tcp	0.000728	# instl-boots | Installation Bootstrap Proto. Serv.
instl_boots	1067/udp	0.001516	# Installation Bootstrap Proto. Serv.
instl_bootc	1068/tcp	0.000941	# instl-bootc | Installation Bootstrap Proto. Cli.
instl_bootc	1068/udp	0.004778	# Installation Bootstrap Proto. Cli.
cognex-insight	1069/tcp	0.001901
cognex-insight	1069/udp	0.001982
gmrupdateserv	1070/tcp	0.000380
gmrupdateserv	1070/udp	0.001321
bsquare-voip	1071/tcp	0.002205
bsquare-voip	1071/udp	0.000330
cardax	1072/tcp	0.000380
cardax	1072/udp	0.001321
bridgecontrol	1073/tcp	0.000380	# Bridge Control
bridgecontrol	1073/udp	0.000000	# Bridge Control
warmspotMgmt	1074/tcp	0.001216	# Warmspot Management Protocol
warmspotMgmt	1074/udp	0.000661	# Warmspot Management Protocol
rdrmshc	1075/tcp	0.000380
rdrmshc	1075/udp	0.000330
sns_credit	1076/tcp	0.000213	# dab-sti-c | Shared Network Services (SNS) for Canadian credit card authorizations | DAB STI-C
dab-sti-c	1076/udp	0.000661	# DAB STI-C
imgames	1077/tcp	0.000380
imgames	1077/udp	0.000661
avocent-proxy	1078/tcp	0.000380	# Avocent Proxy Protocol
avocent-proxy	1078/udp	0.000661	# Avocent Proxy Protocol
asprovatalk	1079/tcp	0.000380
asprovatalk	1079/udp	0.000661
socks	1080/tcp	0.001518
socks	1080/udp	0.002685
pvuniwien	1081/tcp	0.000380
pvuniwien	1081/udp	0.001652
amt-esd-prot	1082/tcp	0.000380
amt-esd-prot	1082/udp	0.000330
ansoft-lm-1	1083/tcp	0.000427	# Anasoft License Manager
ansoft-lm-1	1083/udp	0.001236	# Anasoft License Manager
ansoft-lm-2	1084/tcp	0.000263	# Anasoft License Manager
ansoft-lm-2	1084/udp	0.000626	# Anasoft License Manager
webobjects	1085/tcp	0.000380	# Web Objects
webobjects	1085/udp	0.000661	# Web Objects
cplscrambler-lg	1086/tcp	0.000456	# CPL Scrambler Logging
cplscrambler-lg	1086/udp	0.000330	# CPL Scrambler Logging
cplscrambler-in	1087/tcp	0.000304	# CPL Scrambler Internal
cplscrambler-in	1087/udp	0.001321	# CPL Scrambler Internal
cplscrambler-al	1088/tcp	0.000456	# CPL Scrambler Alarm Log
cplscrambler-al	1088/udp	0.001321	# CPL Scrambler Alarm Log
ff-annunc	1089/tcp	0.000304	# FF Annunciation
ff-annunc	1089/udp	0.000661	# FF Annunciation
ff-fms	1090/tcp	0.000228	# FF Fieldbus Message Specification
ff-fms	1090/udp	0.002313	# FF Fieldbus Message Specification
ff-sm	1091/tcp	0.000228	# FF System Management
ff-sm	1091/udp	0.000000	# FF System Management
obrpd	1092/tcp	0.000152	# Open Business Reporting Protocol
obrpd	1092/udp	0.000330	# Open Business Reporting Protocol
proofd	1093/tcp	0.000380
proofd	1093/udp	0.000330
rootd	1094/tcp	0.000380
rootd	1094/udp	0.000330
nicelink	1095/tcp	0.000152
nicelink	1095/udp	0.000661
cnrprotocol	1096/tcp	0.000380	# Common Name Resolution Protocol
cnrprotocol	1096/udp	0.000000	# Common Name Resolution Protocol
sunclustermgr	1097/tcp	0.000456	# Sun Cluster Manager
sunclustermgr	1097/udp	0.000000	# Sun Cluster Manager
rmiactivation	1098/tcp	0.000380	# RMI Activation
rmiactivation	1098/udp	0.000991	# RMI Activation
rmiregistry	1099/tcp	0.000380	# RMI Registry
rmiregistry	1099/udp	0.000661	# RMI Registry
mctp	1100/tcp	0.000380
mctp	1100/udp	0.001652
pt2-discover	1101/tcp	0.000076
pt2-discover	1101/udp	0.001321
adobeserver-1	1102/tcp	0.000152	# ADOBE SERVER 1
adobeserver-1	1102/udp	0.000661	# ADOBE SERVER 1
xaudio	1103/tcp	0.000151	# adobeserver-2 | Xaserver	# X Audio Server | ADOBE SERVER 2
adobeserver-2	1103/udp	0.000661	# ADOBE SERVER 2
xrl	1104/tcp	0.000380
xrl	1104/udp	0.000330
ftranhc	1105/tcp	0.000152
ftranhc	1105/udp	0.001652
isoipsigport-1	1106/tcp	0.000380
isoipsigport-1	1106/udp	0.000661
isoipsigport-2	1107/tcp	0.000380
isoipsigport-2	1107/udp	0.000330
ratio-adp	1108/tcp	0.000380
ratio-adp	1108/udp	0.000330
kpop	1109/tcp	0.000151	# Pop with Kerberos
nfsd-status	1110/tcp	0.005809	# nfsd-keepalive | webadmstart | Cluster status info | Start web admin server | Client status info
nfsd-keepalive	1110/udp	0.000939	# Client status info
lmsocialserver	1111/tcp	0.001140	# LM Social Server
lmsocialserver	1111/udp	0.000000	# LM Social Server
msql	1112/tcp	0.000276	# icp | mini-sql server | Intelligent Communication Protocol
icp	1112/udp	0.000330	# Intelligent Communication Protocol
ltp-deepspace	1113/tcp	0.000152	# Licklider Transmission Protocol
ltp-deepspace	1113/udp	0.000991	# Licklider Transmission Protocol
mini-sql	1114/tcp	0.000228	# Mini SQL
mini-sql	1114/udp	0.000330	# Mini SQL
ardus-trns	1115/tcp	0.000000	# ARDUS Transfer
ardus-trns	1115/udp	0.000000	# ARDUS Transfer
ardus-cntl	1116/tcp	0.000076	# ARDUS Control
ardus-cntl	1116/udp	0.000661	# ARDUS Control
ardus-mtrns	1117/tcp	0.000228	# ARDUS Multicast Transfer
ardus-mtrns	1117/udp	0.000330	# ARDUS Multicast Transfer
sacred	1118/tcp	0.000076
sacred	1118/udp	0.000000
bnetgame	1119/tcp	0.000228	# Battle.net Chat/Game Protocol
bnetgame	1119/udp	0.000330	# Battle.net Chat/Game Protocol
bnetfile	1120/tcp	0.000000	# Battle.net File Transfer Protocol
bnetfile	1120/udp	0.000330	# Battle.net File Transfer Protocol
rmpp	1121/tcp	0.000152	# Datalode RMPP
rmpp	1121/udp	0.000000	# Datalode RMPP
availant-mgr	1122/tcp	0.000228
availant-mgr	1122/udp	0.000661
murray	1123/tcp	0.000152
murray	1123/udp	0.000000
hpvmmcontrol	1124/tcp	0.000304	# HP VMM Control
hpvmmcontrol	1124/udp	0.001652	# HP VMM Control
hpvmmagent	1125/tcp	0.000076	# HP VMM Agent
hpvmmagent	1125/udp	0.000330	# HP VMM Agent
hpvmmdata	1126/tcp	0.000152	# HP VMM Agent
hpvmmdata	1126/udp	0.000000	# HP VMM Agent
supfiledbg	1127/tcp	0.000088	# kwdb-commn | SUP debugging | KWDB Remote Communication
kwdb-commn	1127/udp	0.000000	# KWDB Remote Communication
saphostctrl	1128/tcp	0.000076	# SAPHostControl over SOAP/HTTP
saphostctrl	1128/udp	0.000000	# SAPHostControl over SOAP/HTTP
saphostctrls	1129/tcp	0.000000	# SAPHostControl over SOAP/HTTPS
saphostctrls	1129/udp	0.000330	# SAPHostControl over SOAP/HTTPS
casp	1130/tcp	0.000152	# CAC App Service Protocol
casp	1130/udp	0.000330	# CAC App Service Protocol
caspssl	1131/tcp	0.000228	# CAC App Service Protocol Encripted
caspssl	1131/udp	0.000330	# CAC App Service Protocol Encripted
kvm-via-ip	1132/tcp	0.000152	# KVM-via-IP Management Service
kvm-via-ip	1132/udp	0.000000	# KVM-via-IP Management Service
dfn	1133/tcp	0.000000	# Data Flow Network
dfn	1133/udp	0.000330	# Data Flow Network
aplx	1134/tcp	0.000076	# MicroAPL APLX
aplx	1134/udp	0.000000	# MicroAPL APLX
omnivision	1135/tcp	0.000076	# OmniVision Communication Service
omnivision	1135/udp	0.000000	# OmniVision Communication Service
hhb-gateway	1136/tcp	0.000076	# HHB Gateway Control
hhb-gateway	1136/udp	0.000330	# HHB Gateway Control
trim	1137/tcp	0.000152	# TRIM Workgroup Service
trim	1137/udp	0.000330	# TRIM Workgroup Service
encrypted_admin	1138/tcp	0.000228	# encrypted-admin | encrypted admin requests
encrypted_admin	1138/udp	0.000000	# encrypted admin requests
cce3x	1139/tcp	0.000063	# evm | ClearCommerce Engine 3.x ( www.clearcommerce.com) | Enterprise Virtual Manager
evm	1139/udp	0.000661	# Enterprise Virtual Manager
autonoc	1140/tcp	0.000000	# AutoNOC Network Operations Protocol
autonoc	1140/udp	0.000000	# AutoNOC Network Operations Protocol
mxomss	1141/tcp	0.000152	# User Message Service
mxomss	1141/udp	0.000000	# User Message Service
edtools	1142/tcp	0.000000	# User Discovery Service
edtools	1142/udp	0.000000	# User Discovery Service
imyx	1143/tcp	0.000076	# Infomatryx Exchange
imyx	1143/udp	0.000661	# Infomatryx Exchange
fuscript	1144/tcp	0.000076	# Fusion Script
fuscript	1144/udp	0.000330	# Fusion Script
x9-icue	1145/tcp	0.000152	# X9 iCue Show Control
x9-icue	1145/udp	0.000330	# X9 iCue Show Control
audit-transfer	1146/tcp	0.000000	# audit transfer
audit-transfer	1146/udp	0.000330	# audit transfer
capioverlan	1147/tcp	0.000152
capioverlan	1147/udp	0.000330
elfiq-repl	1148/tcp	0.000380	# Elfiq Replication Service
elfiq-repl	1148/udp	0.000661	# Elfiq Replication Service
bvtsonar	1149/tcp	0.000152	# BVT Sonar Service | BlueView Sonar Service
bvtsonar	1149/udp	0.000330	# BVT Sonar Service
blaze	1150/tcp	0.000076	# Blaze File Server
blaze	1150/udp	0.000000	# Blaze File Server
unizensus	1151/tcp	0.000228	# Unizensus Login Server
unizensus	1151/udp	0.000330	# Unizensus Login Server
winpoplanmess	1152/tcp	0.000304	# Winpopup LAN Messenger
winpoplanmess	1152/udp	0.000000	# Winpopup LAN Messenger
c1222-acse	1153/tcp	0.000076	# ANSI C12.22 Port
c1222-acse	1153/udp	0.000000	# ANSI C12.22 Port
resacommunity	1154/tcp	0.000152	# Community Service
resacommunity	1154/udp	0.000000	# Community Service
nfa	1155/tcp	0.000000	# Network File Access
nfa	1155/udp	0.000890	# Network File Access
iascontrol-oms	1156/tcp	0.000076	# iasControl OMS
iascontrol-oms	1156/udp	0.000000	# iasControl OMS
iascontrol	1157/tcp	0.000076	# Oracle iASControl
iascontrol	1157/udp	0.000000	# Oracle iASControl
lsnr	1158/tcp	0.000138	# dbcontrol-oms | Oracle DB listener | dbControl OMS
dbcontrol-oms	1158/udp	0.000330	# dbControl OMS
oracle-oms	1159/tcp	0.000076	# Oracle OMS
oracle-oms	1159/udp	0.000000	# Oracle OMS
olsv	1160/tcp	0.000000	# DB Lite Mult-User Server
olsv	1160/udp	0.000000	# DB Lite Mult-User Server
health-polling	1161/tcp	0.000000	# Health Polling
health-polling	1161/udp	0.000000	# Health Polling
health-trap	1162/tcp	0.000076	# Health Trap
health-trap	1162/udp	0.000330	# Health Trap
sddp	1163/tcp	0.000152	# SmartDialer Data Protocol
sddp	1163/udp	0.000991	# SmartDialer Data Protocol
qsm-proxy	1164/tcp	0.000152	# QSM Proxy Service
qsm-proxy	1164/udp	0.000330	# QSM Proxy Service
qsm-gui	1165/tcp	0.000152	# QSM GUI Service
qsm-gui	1165/udp	0.000000	# QSM GUI Service
qsm-remote	1166/tcp	0.000152	# QSM RemoteExec
qsm-remote	1166/udp	0.000330	# QSM RemoteExec
cisco-ipsla	1167/sctp	0.000000	# Cisco IP SLAs Control Protocol
cisco-ipsla	1167/tcp	0.000076	# Cisco IP SLAs Control Protocol
cisco-ipsla	1167/udp	0.000593	# Cisco IP SLAs Control Protocol
vchat	1168/tcp	0.000076	# VChat Conference Service
vchat	1168/udp	0.000330	# VChat Conference Service
tripwire	1169/tcp	0.000380
tripwire	1169/udp	0.000330
atc-lm	1170/tcp	0.000000	# AT+C License Manager
atc-lm	1170/udp	0.000330	# AT+C License Manager
atc-appserver	1171/tcp	0.000000	# AT+C FmiApplicationServer
atc-appserver	1171/udp	0.000000	# AT+C FmiApplicationServer
dnap	1172/tcp	0.000000	# DNA Protocol
dnap	1172/udp	0.000000	# DNA Protocol
d-cinema-rrp	1173/tcp	0.000076	# D-Cinema Request-Response
d-cinema-rrp	1173/udp	0.000330	# D-Cinema Request-Response
fnet-remote-ui	1174/tcp	0.000152	# FlashNet Remote Admin
fnet-remote-ui	1174/udp	0.000000	# FlashNet Remote Admin
dossier	1175/tcp	0.000228	# Dossier Server
dossier	1175/udp	0.000661	# Dossier Server
indigo-server	1176/tcp	0.000076	# Indigo Home Server
indigo-server	1176/udp	0.000000	# Indigo Home Server
dkmessenger	1177/tcp	0.000000	# DKMessenger Protocol
dkmessenger	1177/udp	0.000000	# DKMessenger Protocol
skkserv	1178/tcp	0.000050	# sgi-storman | SKK (kanji input) | SGI Storage Manager
sgi-storman	1178/udp	0.000000	# SGI Storage Manager
b2n	1179/tcp	0.000076	# Backup To Neighbor
b2n	1179/udp	0.000000	# Backup To Neighbor
mc-client	1180/tcp	0.000076	# Millicent Client Proxy
mc-client	1180/udp	0.000000	# Millicent Client Proxy
3comnetman	1181/tcp	0.000000	# 3Com Net Management
3comnetman	1181/udp	0.000000	# 3Com Net Management
accelenet	1182/tcp	0.000076	# accelenet-data | AcceleNet Control | AcceleNet Data
accelenet-data	1182/udp	0.000000	# AcceleNet Data
llsurfup-http	1183/tcp	0.000304	# LL Surfup HTTP
llsurfup-http	1183/udp	0.000000	# LL Surfup HTTP
llsurfup-https	1184/tcp	0.000076	# LL Surfup HTTPS
llsurfup-https	1184/udp	0.000000	# LL Surfup HTTPS
catchpole	1185/tcp	0.000152	# Catchpole port
catchpole	1185/udp	0.000330	# Catchpole port
mysql-cluster	1186/tcp	0.000304	# MySQL Cluster Manager
mysql-cluster	1186/udp	0.000000	# MySQL Cluster Manager
alias	1187/tcp	0.000152	# Alias Service
alias	1187/udp	0.000000	# Alias Service
hp-webadmin	1188/tcp	0.000076	# HP Web Admin
hp-webadmin	1188/udp	0.000330	# HP Web Admin
unet	1189/tcp	0.000000	# Unet Connection
unet	1189/udp	0.000330	# Unet Connection
commlinx-avl	1190/tcp	0.000076	# CommLinx GPS / AVL System
commlinx-avl	1190/udp	0.000000	# CommLinx GPS / AVL System
gpfs	1191/tcp	0.000076	# General Parallel File System
gpfs	1191/udp	0.000661	# General Parallel File System
caids-sensor	1192/tcp	0.000152	# caids sensors channel
caids-sensor	1192/udp	0.000000	# caids sensors channel
fiveacross	1193/tcp	0.000000	# Five Across Server
fiveacross	1193/udp	0.000330	# Five Across Server
openvpn	1194/tcp	0.000076
openvpn	1194/udp	0.000330
rsf-1	1195/tcp	0.000076	# RSF-1 clustering
rsf-1	1195/udp	0.000000	# RSF-1 clustering
netmagic	1196/tcp	0.000076	# Network Magic
netmagic	1196/udp	0.000000	# Network Magic
carrius-rshell	1197/tcp	0.000000	# Carrius Remote Access
carrius-rshell	1197/udp	0.000000	# Carrius Remote Access
cajo-discovery	1198/tcp	0.000152	# cajo reference discovery
cajo-discovery	1198/udp	0.000330	# cajo reference discovery
dmidi	1199/tcp	0.000228
dmidi	1199/udp	0.000000
scol	1200/tcp	0.000076
scol	1200/udp	0.001321
nucleus-sand	1201/tcp	0.000228	# Nucleus Sand Database Server
nucleus-sand	1201/udp	0.000000	# Nucleus Sand Database Server
caiccipc	1202/tcp	0.000000
caiccipc	1202/udp	0.000000
ssslic-mgr	1203/tcp	0.000000	# License Validation
ssslic-mgr	1203/udp	0.000661	# License Validation
ssslog-mgr	1204/tcp	0.000076	# Log Request Listener
ssslog-mgr	1204/udp	0.000000	# Log Request Listener
accord-mgc	1205/tcp	0.000000
accord-mgc	1205/udp	0.000000
anthony-data	1206/tcp	0.000000	# Anthony Data
anthony-data	1206/udp	0.000661	# Anthony Data
metasage	1207/tcp	0.000076
metasage	1207/udp	0.000330
seagull-ais	1208/tcp	0.000076	# SEAGULL AIS
seagull-ais	1208/udp	0.000000	# SEAGULL AIS
ipcd3	1209/tcp	0.000076
ipcd3	1209/udp	0.000000
eoss	1210/tcp	0.000076
eoss	1210/udp	0.000000
groove-dpp	1211/tcp	0.000076	# Groove DPP
groove-dpp	1211/udp	0.000000	# Groove DPP
lupa	1212/tcp	0.000125
lupa	1212/udp	0.000544
mpc-lifenet	1213/tcp	0.000152	# MPC LIFENET | Medtronic/Physio-Control LIFENET
mpc-lifenet	1213/udp	0.000000	# MPC LIFENET
fasttrack	1214/tcp	0.000050	# kazaa | Kazaa File Sharing | KAZAA
fasttrack	1214/udp	0.001796	# Kazaa File Sharing
scanstat-1	1215/tcp	0.000076	# scanSTAT 1.0
scanstat-1	1215/udp	0.000661	# scanSTAT 1.0
etebac5	1216/tcp	0.000152	# ETEBAC 5
etebac5	1216/udp	0.000330	# ETEBAC 5
hpss-ndapi	1217/tcp	0.000152	# HPSS NonDCE Gateway
hpss-ndapi	1217/udp	0.000000	# HPSS NonDCE Gateway
aeroflight-ads	1218/tcp	0.001064	# AeroFlight ADs
aeroflight-ads	1218/udp	0.000000	# AeroFlight ADs
aeroflight-ret	1219/tcp	0.000000
aeroflight-ret	1219/udp	0.000000
quicktime	1220/tcp	0.000151	# qt-serveradmin | Apple Darwin and QuickTime Streaming Administration Servers | QT SERVER ADMIN
qt-serveradmin	1220/udp	0.000000	# QT SERVER ADMIN
sweetware-apps	1221/tcp	0.000076	# SweetWARE Apps
sweetware-apps	1221/udp	0.000000	# SweetWARE Apps
nerv	1222/tcp	0.000138	# SNI R&D network
nerv	1222/udp	0.000346	# SNI R&D network
tgp	1223/tcp	0.000076	# TrulyGlobal Protocol
tgp	1223/udp	0.000000	# TrulyGlobal Protocol
vpnz	1224/tcp	0.000000
vpnz	1224/udp	0.000330
slinkysearch	1225/tcp	0.000000
slinkysearch	1225/udp	0.000330
stgxfws	1226/tcp	0.000000
stgxfws	1226/udp	0.000330
dns2go	1227/tcp	0.000000
dns2go	1227/udp	0.000330
florence	1228/tcp	0.000076
florence	1228/udp	0.000000
zented	1229/tcp	0.000076	# ZENworks Tiered Electronic Distribution
zented	1229/udp	0.000330	# ZENworks Tiered Electronic Distribution
periscope	1230/tcp	0.000000
periscope	1230/udp	0.000000
menandmice-lpm	1231/tcp	0.000000
menandmice-lpm	1231/udp	0.000330
first-defense	1232/tcp	0.000000	# Remote systems monitoring
univ-appserver	1233/tcp	0.000152	# Universal App Server
univ-appserver	1233/udp	0.000330	# Universal App Server
hotline	1234/tcp	0.001217	# search-agent | Infoseek Search Agent
search-agent	1234/udp	0.001652	# Infoseek Search Agent
mosaicsyssvc1	1235/tcp	0.000000
mosaicsyssvc1	1235/udp	0.000000
bvcontrol	1236/tcp	0.000152
bvcontrol	1236/udp	0.000000
tsdos390	1237/tcp	0.000000
tsdos390	1237/udp	0.000991
hacl-qs	1238/tcp	0.000000
hacl-qs	1238/udp	0.000000
nmsd	1239/tcp	0.000076
nmsd	1239/udp	0.000000
instantia	1240/tcp	0.000076
instantia	1240/udp	0.000000
nessus	1241/tcp	0.000113	# Nessus or remote message server
nessus	1241/udp	0.000330
nmasoverip	1242/tcp	0.000000	# NMAS over IP
nmasoverip	1242/udp	0.000000	# NMAS over IP
serialgateway	1243/tcp	0.000076
serialgateway	1243/udp	0.000000
isbconference1	1244/tcp	0.000152
isbconference1	1244/udp	0.000000
isbconference2	1245/tcp	0.000000
isbconference2	1245/udp	0.000000
payrouter	1246/tcp	0.000000
payrouter	1246/udp	0.000000
visionpyramid	1247/tcp	0.000304
visionpyramid	1247/udp	0.000000
hermes	1248/tcp	0.000477
hermes	1248/udp	0.000412
mesavistaco	1249/tcp	0.000076	# Mesa Vista Co
mesavistaco	1249/udp	0.000330	# Mesa Vista Co
swldy-sias	1250/tcp	0.000076
swldy-sias	1250/udp	0.000000
servergraph	1251/tcp	0.000076
servergraph	1251/udp	0.000661
bspne-pcc	1252/tcp	0.000000
bspne-pcc	1252/udp	0.000000
q55-pcc	1253/tcp	0.000000
q55-pcc	1253/udp	0.000330
de-noc	1254/tcp	0.000000
de-noc	1254/udp	0.000000
de-cache-query	1255/tcp	0.000000
de-cache-query	1255/udp	0.000330
de-server	1256/tcp	0.000000
de-server	1256/udp	0.000661
shockwave2	1257/tcp	0.000000	# Shockwave 2
shockwave2	1257/udp	0.000661	# Shockwave 2
opennl	1258/tcp	0.000000	# Open Network Library
opennl	1258/udp	0.000000	# Open Network Library
opennl-voice	1259/tcp	0.000152	# Open Network Library Voice
opennl-voice	1259/udp	0.000330	# Open Network Library Voice
ibm-ssd	1260/tcp	0.000000
ibm-ssd	1260/udp	0.000330
mpshrsv	1261/tcp	0.000076
mpshrsv	1261/udp	0.000000
qnts-orb	1262/tcp	0.000076
qnts-orb	1262/udp	0.000000
dka	1263/tcp	0.000000
dka	1263/udp	0.000000
prat	1264/tcp	0.000076
prat	1264/udp	0.000330
dssiapi	1265/tcp	0.000000
dssiapi	1265/udp	0.000000
dellpwrappks	1266/tcp	0.000000
dellpwrappks	1266/udp	0.000000
epc	1267/tcp	0.000000	# eTrust Policy Compliance
epc	1267/udp	0.000000	# eTrust Policy Compliance
propel-msgsys	1268/tcp	0.000076
propel-msgsys	1268/udp	0.000000
watilapp	1269/tcp	0.000000
watilapp	1269/udp	0.000330
ssserver	1270/tcp	0.000138	# opsmgr | Sun StorEdge Configuration Service | Microsoft Operations Manager
opsmgr	1270/udp	0.000000	# Microsoft Operations Manager
excw	1271/tcp	0.000228
excw	1271/udp	0.000000
cspmlockmgr	1272/tcp	0.000380
cspmlockmgr	1272/udp	0.000000
emc-gateway	1273/tcp	0.000000
emc-gateway	1273/udp	0.000000
t1distproc	1274/tcp	0.000000
t1distproc	1274/udp	0.000000
ivcollector	1275/tcp	0.000000
ivcollector	1275/udp	0.000000
ivmanager	1276/tcp	0.000076
ivmanager	1276/udp	0.000000
miva-mqs	1277/tcp	0.000152	# mqs
miva-mqs	1277/udp	0.000000	# mqs
dellwebadmin-1	1278/tcp	0.000000	# Dell Web Admin 1
dellwebadmin-1	1278/udp	0.000000	# Dell Web Admin 1
dellwebadmin-2	1279/tcp	0.000076	# Dell Web Admin 2
dellwebadmin-2	1279/udp	0.000330	# Dell Web Admin 2
pictrography	1280/tcp	0.000000
pictrography	1280/udp	0.000000
healthd	1281/tcp	0.000000
healthd	1281/udp	0.000000
emperion	1282/tcp	0.000076
emperion	1282/udp	0.000000
productinfo	1283/tcp	0.000000	# Product Information
productinfo	1283/udp	0.000000	# Product Information
iee-qfx	1284/tcp	0.000000
iee-qfx	1284/udp	0.000000
neoiface	1285/tcp	0.000000
neoiface	1285/udp	0.000000
netuitive	1286/tcp	0.000000
netuitive	1286/udp	0.000991
routematch	1287/tcp	0.000152	# RouteMatch Com
routematch	1287/udp	0.000991	# RouteMatch Com
navbuddy	1288/tcp	0.000000
navbuddy	1288/udp	0.000000
jwalkserver	1289/tcp	0.000000
jwalkserver	1289/udp	0.000000
winjaserver	1290/tcp	0.000076
winjaserver	1290/udp	0.000000
seagulllms	1291/tcp	0.000076
seagulllms	1291/udp	0.000330
dsdn	1292/tcp	0.000000
dsdn	1292/udp	0.000000
pkt-krb-ipsec	1293/tcp	0.000000
pkt-krb-ipsec	1293/udp	0.000000
cmmdriver	1294/tcp	0.000000
cmmdriver	1294/udp	0.000330
ehtp	1295/tcp	0.000000	# End-by-Hop Transmission Protocol
ehtp	1295/udp	0.000330	# End-by-Hop Transmission Protocol
dproxy	1296/tcp	0.000304
dproxy	1296/udp	0.000000
sdproxy	1297/tcp	0.000076
sdproxy	1297/udp	0.000330
lpcp	1298/tcp	0.000000
lpcp	1298/udp	0.000000
hp-sci	1299/tcp	0.000076
hp-sci	1299/udp	0.000330
h323hostcallsc	1300/tcp	0.000152	# H323 Host Call Secure | H.323 Secure Call Control Signalling
h323hostcallsc	1300/udp	0.000330	# H323 Host Call Secure
ci3-software-1	1301/tcp	0.000152
ci3-software-1	1301/udp	0.000330
ci3-software-2	1302/tcp	0.000076
ci3-software-2	1302/udp	0.000661
sftsrv	1303/tcp	0.000076
sftsrv	1303/udp	0.000000
boomerang	1304/tcp	0.000000
boomerang	1304/udp	0.000000
pe-mike	1305/tcp	0.000076
pe-mike	1305/udp	0.000000
re-conn-proto	1306/tcp	0.000076
re-conn-proto	1306/udp	0.000000
pacmand	1307/tcp	0.000076
pacmand	1307/udp	0.000000
odsi	1308/tcp	0.000076	# Optical Domain Service Interconnect (ODSI)
odsi	1308/udp	0.000000	# Optical Domain Service Interconnect (ODSI)
jtag-server	1309/tcp	0.000152	# JTAG server
jtag-server	1309/udp	0.000000	# JTAG server
husky	1310/tcp	0.000380
husky	1310/udp	0.000330
rxmon	1311/tcp	0.000760
rxmon	1311/udp	0.000000
sti-envision	1312/tcp	0.000000	# STI Envision
sti-envision	1312/udp	0.000000	# STI Envision
bmc_patroldb	1313/tcp	0.000000	# bmc-patroldb
bmc_patroldb	1313/udp	0.000000
pdps	1314/tcp	0.000076	# Photoscript Distributed Printing System
pdps	1314/udp	0.000330	# Photoscript Distributed Printing System
els	1315/tcp	0.000076	# E.L.S., Event Listener Service
els	1315/udp	0.000330	# E.L.S., Event Listener Service
exbit-escp	1316/tcp	0.000076
exbit-escp	1316/udp	0.000000
vrts-ipcserver	1317/tcp	0.000076
vrts-ipcserver	1317/udp	0.000330
krb5gatekeeper	1318/tcp	0.000076
krb5gatekeeper	1318/udp	0.000000
amx-icsp	1319/tcp	0.000076
amx-icsp	1319/udp	0.000000
amx-axbnet	1320/tcp	0.000000
amx-axbnet	1320/udp	0.000000
pip	1321/tcp	0.000076
pip	1321/udp	0.000000
novation	1322/tcp	0.000152
novation	1322/udp	0.000000
brcd	1323/tcp	0.000000
brcd	1323/udp	0.000000
delta-mcp	1324/tcp	0.000076
delta-mcp	1324/udp	0.000000
dx-instrument	1325/tcp	0.000000
dx-instrument	1325/udp	0.000330
wimsic	1326/tcp	0.000000
wimsic	1326/udp	0.000000
ultrex	1327/tcp	0.000076
ultrex	1327/udp	0.000330
ewall	1328/tcp	0.000152
ewall	1328/udp	0.000000
netdb-export	1329/tcp	0.000000
netdb-export	1329/udp	0.000000
streetperfect	1330/tcp	0.000076
streetperfect	1330/udp	0.000000
intersan	1331/tcp	0.000076
intersan	1331/udp	0.000000
pcia-rxp-b	1332/tcp	0.000000	# PCIA RXP-B
pcia-rxp-b	1332/udp	0.000000	# PCIA RXP-B
passwrd-policy	1333/tcp	0.000000	# Password Policy
passwrd-policy	1333/udp	0.000000	# Password Policy
writesrv	1334/tcp	0.000304
writesrv	1334/udp	0.000991
digital-notary	1335/tcp	0.000000	# Digital Notary Protocol
digital-notary	1335/udp	0.000000	# Digital Notary Protocol
ischat	1336/tcp	0.000076	# Instant Service Chat
ischat	1336/udp	0.000330	# Instant Service Chat
waste	1337/tcp	0.000088	# menandmice-dns | Nullsoft WASTE encrypted P2P app | menandmice DNS
menandmice-dns	1337/udp	0.000661	# menandmice DNS
wmc-log-svc	1338/tcp	0.000000	# WMC-log-svr
wmc-log-svc	1338/udp	0.000330	# WMC-log-svr
kjtsiteserver	1339/tcp	0.000076
kjtsiteserver	1339/udp	0.000000
naap	1340/tcp	0.000076
naap	1340/udp	0.000000
qubes	1341/tcp	0.000000
qubes	1341/udp	0.000000
esbroker	1342/tcp	0.000000
esbroker	1342/udp	0.000330
re101	1343/tcp	0.000000
re101	1343/udp	0.000000
icap	1344/tcp	0.000000
icap	1344/udp	0.000330
vpjp	1345/tcp	0.000000
vpjp	1345/udp	0.000991
alta-ana-lm	1346/tcp	0.000050	# Alta Analytics License Manager
alta-ana-lm	1346/udp	0.001928	# Alta Analytics License Manager
bbn-mmc	1347/tcp	0.000151	# multi media conferencing
bbn-mmc	1347/udp	0.000692	# multi media conferencing
bbn-mmx	1348/tcp	0.000038	# multi media conferencing
bbn-mmx	1348/udp	0.000988	# multi media conferencing
sbook	1349/tcp	0.000050	# Registration Network Protocol
sbook	1349/udp	0.000873	# Registration Network Protocol
editbench	1350/tcp	0.000113	# Registration Network Protocol
editbench	1350/udp	0.000577	# Registration Network Protocol
equationbuilder	1351/tcp	0.000113	# Digital Tool Works (MIT)
equationbuilder	1351/udp	0.000544	# Digital Tool Works (MIT)
lotusnotes	1352/tcp	0.001154	# lotusnote | Lotus Note
lotusnotes	1352/udp	0.000610	# Lotus Note
relief	1353/tcp	0.000100	# Relief Consulting
relief	1353/udp	0.000708	# Relief Consulting
rightbrain	1354/tcp	0.000038	# XSIP-network | RightBrain Software | Five Across XSIP Network
rightbrain	1354/udp	0.000544	# RightBrain Software
intuitive-edge	1355/tcp	0.000025	# Intuitive Edge
intuitive-edge	1355/udp	0.000527	# Intuitive Edge
cuillamartin	1356/tcp	0.000050	# CuillaMartin Company
cuillamartin	1356/udp	0.000461	# CuillaMartin Company
pegboard	1357/tcp	0.000100	# Electronic PegBoard
pegboard	1357/udp	0.000708	# Electronic PegBoard
connlcli	1358/tcp	0.000063
connlcli	1358/udp	0.000577
ftsrv	1359/tcp	0.000063
ftsrv	1359/udp	0.000824
mimer	1360/tcp	0.000013
mimer	1360/udp	0.000478
linx	1361/tcp	0.000013
linx	1361/udp	0.000610
timeflies	1362/tcp	0.000025
timeflies	1362/udp	0.000494
ndm-requester	1363/tcp	0.000013	# Network DataMover Requester
ndm-requester	1363/udp	0.000494	# Network DataMover Requester
ndm-server	1364/tcp	0.000063	# Network DataMover Server
ndm-server	1364/udp	0.000824	# Network DataMover Server
adapt-sna	1365/tcp	0.000025	# Network Software Associates
adapt-sna	1365/udp	0.000643	# Network Software Associates
netware-csp	1366/tcp	0.000063	# Novell NetWare Comm Service Platform
netware-csp	1366/udp	0.000923	# Novell NetWare Comm Service Platform
dcs	1367/tcp	0.000013
dcs	1367/udp	0.000560
screencast	1368/tcp	0.000025
screencast	1368/udp	0.000379
gv-us	1369/tcp	0.000038	# GlobalView to Unix Shell
gv-us	1369/udp	0.000461	# GlobalView to Unix Shell
us-gv	1370/tcp	0.000050	# Unix Shell to GlobalView
us-gv	1370/udp	0.000725	# Unix Shell to GlobalView
fc-cli	1371/tcp	0.000013	# Fujitsu Config Protocol
fc-cli	1371/udp	0.000692	# Fujitsu Config Protocol
fc-ser	1372/tcp	0.000038	# Fujitsu Config Protocol
fc-ser	1372/udp	0.000708	# Fujitsu Config Protocol
chromagrafx	1373/tcp	0.000038
chromagrafx	1373/udp	0.000428
molly	1374/tcp	0.000013	# EPI Software Systems
molly	1374/udp	0.000461	# EPI Software Systems
bytex	1375/tcp	0.000000
bytex	1375/udp	0.000494
ibm-pps	1376/tcp	0.000025	# IBM Person to Person Software
ibm-pps	1376/udp	0.000577	# IBM Person to Person Software
cichlid	1377/tcp	0.000000	# Cichlid License Manager
cichlid	1377/udp	0.000593	# Cichlid License Manager
elan	1378/tcp	0.000000	# Elan License Manager
elan	1378/udp	0.000560	# Elan License Manager
dbreporter	1379/tcp	0.000038	# Integrity Solutions
dbreporter	1379/udp	0.000560	# Integrity Solutions
telesis-licman	1380/tcp	0.000000	# Telesis Network License Manager
telesis-licman	1380/udp	0.000610	# Telesis Network License Manager
apple-licman	1381/tcp	0.000038	# Apple Network License Manager
apple-licman	1381/udp	0.000560	# Apple Network License Manager
udt_os	1382/tcp	0.000000	# udt-os
udt_os	1382/udp	0.000000
gwha	1383/tcp	0.000013	# GW Hannaway Network License Manager
gwha	1383/udp	0.000659	# GW Hannaway Network License Manager
os-licman	1384/tcp	0.000050	# Objective Solutions License Manager
os-licman	1384/udp	0.000428	# Objective Solutions License Manager
atex_elmd	1385/tcp	0.000050	# atex-elmd | Atex Publishing License Manager
atex_elmd	1385/udp	0.000280	# Atex Publishing License Manager
checksum	1386/tcp	0.000025	# CheckSum License Manager
checksum	1386/udp	0.000511	# CheckSum License Manager
cadsi-lm	1387/tcp	0.000038	# Computer Aided Design Software Inc LM
cadsi-lm	1387/udp	0.000577	# Computer Aided Design Software Inc LM
objective-dbc	1388/tcp	0.000050	# Objective Solutions DataBase Cache
objective-dbc	1388/udp	0.000741	# Objective Solutions DataBase Cache
iclpv-dm	1389/tcp	0.000050	# Document Manager
iclpv-dm	1389/udp	0.000923	# Document Manager
iclpv-sc	1390/tcp	0.000025	# Storage Controller
iclpv-sc	1390/udp	0.000511	# Storage Controller
iclpv-sas	1391/tcp	0.000013	# Storage Access Server
iclpv-sas	1391/udp	0.000659	# Storage Access Server
iclpv-pm	1392/tcp	0.000000	# Print Manager
iclpv-pm	1392/udp	0.000659	# Print Manager
iclpv-nls	1393/tcp	0.000025	# Network Log Server
iclpv-nls	1393/udp	0.000725	# Network Log Server
iclpv-nlc	1394/tcp	0.000025	# Network Log Client
iclpv-nlc	1394/udp	0.000445	# Network Log Client
iclpv-wsm	1395/tcp	0.000013	# PC Workstation Manager software
iclpv-wsm	1395/udp	0.000675	# PC Workstation Manager software
dvl-activemail	1396/tcp	0.000013	# DVL Active Mail
dvl-activemail	1396/udp	0.000577	# DVL Active Mail
audio-activmail	1397/tcp	0.000025	# Audio Active Mail
audio-activmail	1397/udp	0.000527	# Audio Active Mail
video-activmail	1398/tcp	0.000025	# Video Active Mail
video-activmail	1398/udp	0.000774	# Video Active Mail
cadkey-licman	1399/tcp	0.000050	# Cadkey License Manager
cadkey-licman	1399/udp	0.000643	# Cadkey License Manager
cadkey-tablet	1400/tcp	0.000050	# Cadkey Tablet Daemon
cadkey-tablet	1400/udp	0.001219	# Cadkey Tablet Daemon
goldleaf-licman	1401/tcp	0.000038	# Goldleaf License Manager
goldleaf-licman	1401/udp	0.000494	# Goldleaf License Manager
prm-sm-np	1402/tcp	0.000050	# Prospero Resource Manager
prm-sm-np	1402/udp	0.000659	# Prospero Resource Manager
prm-nm-np	1403/tcp	0.000038	# Prospero Resource Manager
prm-nm-np	1403/udp	0.000527	# Prospero Resource Manager
igi-lm	1404/tcp	0.000050	# Infinite Graphics License Manager
igi-lm	1404/udp	0.000494	# Infinite Graphics License Manager
ibm-res	1405/tcp	0.000038	# IBM Remote Execution Starter
ibm-res	1405/udp	0.000445	# IBM Remote Execution Starter
netlabs-lm	1406/tcp	0.000000	# NetLabs License Manager
netlabs-lm	1406/udp	0.000643	# NetLabs License Manager
dbsa-lm	1407/tcp	0.000013	# tibet-server | DBSA License Manager | TIBET Data Server
dbsa-lm	1407/udp	0.000478	# DBSA License Manager
sophia-lm	1408/tcp	0.000013	# Sophia License Manager
sophia-lm	1408/udp	0.000478	# Sophia License Manager
here-lm	1409/tcp	0.000025	# Here License Manager
here-lm	1409/udp	0.000395	# Here License Manager
hiq	1410/tcp	0.000025	# HiQ License Manager
hiq	1410/udp	0.000643	# HiQ License Manager
af	1411/tcp	0.000013	# AudioFile
af	1411/udp	0.000544	# AudioFile
innosys	1412/tcp	0.000038
innosys	1412/udp	0.000890
innosys-acl	1413/tcp	0.000088
innosys-acl	1413/udp	0.000577
ibm-mqseries	1414/tcp	0.000088	# IBM MQSeries
ibm-mqseries	1414/udp	0.000988	# IBM MQSeries
dbstar	1415/tcp	0.000000
dbstar	1415/udp	0.000659
novell-lu6.2	1416/tcp	0.000013	# novell-lu6-2 | Novell LU6.2
novell-lu6.2	1416/udp	0.000577	# Novell LU6.2
timbuktu-srv1	1417/tcp	0.000201	# Timbuktu Service 1 Port
timbuktu-srv1	1417/udp	0.000610	# Timbuktu Service 1 Port
timbuktu-srv2	1418/tcp	0.000013	# Timbuktu Service 2 Port
timbuktu-srv2	1418/udp	0.000478	# Timbuktu Service 2 Port
timbuktu-srv3	1419/tcp	0.000013	# Timbuktu Service 3 Port
timbuktu-srv3	1419/udp	0.004267	# Timbuktu Service 3 Port
timbuktu-srv4	1420/tcp	0.000063	# Timbuktu Service 4 Port
timbuktu-srv4	1420/udp	0.000741	# Timbuktu Service 4 Port
gandalf-lm	1421/tcp	0.000000	# Gandalf License Manager
gandalf-lm	1421/udp	0.000577	# Gandalf License Manager
autodesk-lm	1422/tcp	0.000025	# Autodesk License Manager
autodesk-lm	1422/udp	0.000906	# Autodesk License Manager
essbase	1423/tcp	0.000013	# Essbase Arbor Software
essbase	1423/udp	0.000544	# Essbase Arbor Software
hybrid	1424/tcp	0.000025	# Hybrid Encryption Protocol
hybrid	1424/udp	0.000527	# Hybrid Encryption Protocol
zion-lm	1425/tcp	0.000000	# Zion Software License Manager
zion-lm	1425/udp	0.000511	# Zion Software License Manager
sas-1	1426/tcp	0.000025	# sais | Satellite-data Acquisition System 1
sas-1	1426/udp	0.000445	# Satellite-data Acquisition System 1
mloadd	1427/tcp	0.000013	# mloadd monitoring tool
mloadd	1427/udp	0.000659	# mloadd monitoring tool
informatik-lm	1428/tcp	0.000000	# Informatik License Manager
informatik-lm	1428/udp	0.000659	# Informatik License Manager
nms	1429/tcp	0.000013	# Hypercom NMS
nms	1429/udp	0.000593	# Hypercom NMS
tpdu	1430/tcp	0.000013	# Hypercom TPDU
tpdu	1430/udp	0.000478	# Hypercom TPDU
rgtp	1431/tcp	0.000000	# Reverse Gossip Transport
rgtp	1431/udp	0.000461	# Reverse Gossip Transport
blueberry-lm	1432/tcp	0.000025	# Blueberry Software License Manager
blueberry-lm	1432/udp	0.000840	# Blueberry Software License Manager
ms-sql-s	1433/tcp	0.007929	# Microsoft-SQL-Server
ms-sql-s	1433/udp	0.036821	# Microsoft-SQL-Server
ms-sql-m	1434/tcp	0.000201	# Microsoft-SQL-Monitor
ms-sql-m	1434/udp	0.293184	# Microsoft-SQL-Monitor
ibm-cics	1435/tcp	0.000038	# IBM CICS
ibm-cics	1435/udp	0.000774
sas-2	1436/tcp	0.000025	# saism | Satellite-data Acquisition System 2
sas-2	1436/udp	0.000478	# Satellite-data Acquisition System 2
tabula	1437/tcp	0.000025
tabula	1437/udp	0.000610
eicon-server	1438/tcp	0.000025	# Eicon Security Agent/Server
eicon-server	1438/udp	0.000758	# Eicon Security Agent/Server
eicon-x25	1439/tcp	0.000025	# Eicon X25/SNA Gateway
eicon-x25	1439/udp	0.000297	# Eicon X25/SNA Gateway
eicon-slp	1440/tcp	0.000013	# Eicon Service Location Protocol
eicon-slp	1440/udp	0.000725	# Eicon Service Location Protocol
cadis-1	1441/tcp	0.000075	# Cadis License Management
cadis-1	1441/udp	0.000857	# Cadis License Management
cadis-2	1442/tcp	0.000025	# Cadis License Management
cadis-2	1442/udp	0.000346	# Cadis License Management
ies-lm	1443/tcp	0.000238	# Integrated Engineering Software
ies-lm	1443/udp	0.000395	# Integrated Engineering Software
marcam-lm	1444/tcp	0.000075	# Marcam License Management
marcam-lm	1444/udp	0.000379	# Marcam License Management
proxima-lm	1445/tcp	0.000050	# Proxima License Manager
proxima-lm	1445/udp	0.000692	# Proxima License Manager
ora-lm	1446/tcp	0.000025	# Optical Research Associates License Manager
ora-lm	1446/udp	0.000478	# Optical Research Associates License Manager
apri-lm	1447/tcp	0.000000	# Applied Parallel Research LM
apri-lm	1447/udp	0.000478	# Applied Parallel Research LM
oc-lm	1448/tcp	0.000013	# OpenConnect License Manager
oc-lm	1448/udp	0.000626	# OpenConnect License Manager
peport	1449/tcp	0.000013
peport	1449/udp	0.000379
dwf	1450/tcp	0.000000	# Tandem Distributed Workbench Facility
dwf	1450/udp	0.000478	# Tandem Distributed Workbench Facility
infoman	1451/tcp	0.000013	# IBM Information Management
infoman	1451/udp	0.000461	# IBM Information Management
gtegsc-lm	1452/tcp	0.000000	# GTE Government Systems License Man
gtegsc-lm	1452/udp	0.000445	# GTE Government Systems License Man
genie-lm	1453/tcp	0.000013	# Genie License Manager
genie-lm	1453/udp	0.000692	# Genie License Manager
interhdl_elmd	1454/tcp	0.000025	# interhdl-elmd | interHDL License Manager
interhdl_elmd	1454/udp	0.000379	# interHDL License Manager
esl-lm	1455/tcp	0.000176	# ESL License Manager
esl-lm	1455/udp	0.001417	# ESL License Manager
dca	1456/tcp	0.000025
dca	1456/udp	0.000511
valisys-lm	1457/tcp	0.000013	# Valisys License Manager
valisys-lm	1457/udp	0.001334	# Valisys License Manager
nrcabq-lm	1458/tcp	0.000013	# Nichols Research Corp.
nrcabq-lm	1458/udp	0.000643	# Nichols Research Corp.
proshare1	1459/tcp	0.000013	# Proshare Notebook Application
proshare1	1459/udp	0.000610	# Proshare Notebook Application
proshare2	1460/tcp	0.000000	# Proshare Notebook Application
proshare2	1460/udp	0.000610	# Proshare Notebook Application
ibm_wrless_lan	1461/tcp	0.000188	# ibm-wrless-lan | IBM Wireless LAN
ibm_wrless_lan	1461/udp	0.000643	# IBM Wireless LAN
world-lm	1462/tcp	0.000013	# World License Manager
world-lm	1462/udp	0.000445	# World License Manager
nucleus	1463/tcp	0.000000
nucleus	1463/udp	0.000297
msl_lmd	1464/tcp	0.000013	# msl-lmd | MSL License Manager
msl_lmd	1464/udp	0.000362	# MSL License Manager
pipes	1465/tcp	0.000050	# Pipes Platform
pipes	1465/udp	0.000741
oceansoft-lm	1466/tcp	0.000038	# Ocean Software License Manager
oceansoft-lm	1466/udp	0.000395	# Ocean Software License Manager
csdmbase	1467/tcp	0.000038
csdmbase	1467/udp	0.000873
csdm	1468/tcp	0.000000
csdm	1468/udp	0.000577
aal-lm	1469/tcp	0.000013	# Active Analysis Limited License Manager
aal-lm	1469/udp	0.000873	# Active Analysis Limited License Manager
uaiact	1470/tcp	0.000013	# Universal Analytics
uaiact	1470/udp	0.000362	# Universal Analytics
csdmbase	1471/tcp	0.000000
csdmbase	1471/udp	0.000445
csdm	1472/tcp	0.000025
csdm	1472/udp	0.000379
openmath	1473/tcp	0.000013
openmath	1473/udp	0.000560
telefinder	1474/tcp	0.000050
telefinder	1474/udp	0.000461
taligent-lm	1475/tcp	0.000038	# Taligent License Manager
taligent-lm	1475/udp	0.000461	# Taligent License Manager
clvm-cfg	1476/tcp	0.000038
clvm-cfg	1476/udp	0.000692
ms-sna-server	1477/tcp	0.000000
ms-sna-server	1477/udp	0.000527
ms-sna-base	1478/tcp	0.000000
ms-sna-base	1478/udp	0.000577
dberegister	1479/tcp	0.000025
dberegister	1479/udp	0.000511
pacerforum	1480/tcp	0.000013
pacerforum	1480/udp	0.000527
airs	1481/tcp	0.000000
airs	1481/udp	0.000758
miteksys-lm	1482/tcp	0.000013	# Miteksys License Manager
miteksys-lm	1482/udp	0.000708	# Miteksys License Manager
afs	1483/tcp	0.000025	# AFS License Manager
afs	1483/udp	0.000956	# AFS License Manager
confluent	1484/tcp	0.000050	# Confluent License Manager
confluent	1484/udp	0.001549	# Confluent License Manager
lansource	1485/tcp	0.000000
lansource	1485/udp	0.002323
nms_topo_serv	1486/tcp	0.000038	# nms-topo-serv
nms_topo_serv	1486/udp	0.000626
localinfosrvr	1487/tcp	0.000000
localinfosrvr	1487/udp	0.000428
docstor	1488/tcp	0.000013
docstor	1488/udp	0.000544
dmdocbroker	1489/tcp	0.000000
dmdocbroker	1489/udp	0.000428
insitu-conf	1490/tcp	0.000000
insitu-conf	1490/udp	0.000577
anynetgateway	1491/tcp	0.000013
anynetgateway	1491/udp	0.000972
stone-design-1	1492/tcp	0.000075
stone-design-1	1492/udp	0.000478
netmap_lm	1493/tcp	0.000025	# netmap-lm
netmap_lm	1493/udp	0.000395
citrix-ica	1494/tcp	0.001255	# ica
citrix-ica	1494/udp	0.000494
cvc	1495/tcp	0.000075
cvc	1495/udp	0.000527
liberty-lm	1496/tcp	0.000038
liberty-lm	1496/udp	0.000412
rfx-lm	1497/tcp	0.000038
rfx-lm	1497/udp	0.000329
watcom-sql	1498/tcp	0.000025	# sybase-sqlany | Sybase SQL Any
watcom-sql	1498/udp	0.000758
fhc	1499/tcp	0.000025	# Federico Heinz Consultora
fhc	1499/udp	0.000461	# Federico Heinz Consultora
vlsi-lm	1500/tcp	0.000627	# VLSI License Manager
vlsi-lm	1500/udp	0.000461	# VLSI License Manager
sas-3	1501/tcp	0.000602	# saiscm | Satellite-data Acquisition System 3
sas-3	1501/udp	0.000725	# Satellite-data Acquisition System 3
shivadiscovery	1502/tcp	0.000013	# Shiva
shivadiscovery	1502/udp	0.000626	# Shiva
imtc-mcs	1503/tcp	0.000640	# Databeam
imtc-mcs	1503/udp	0.000675	# Databeam
evb-elm	1504/tcp	0.000000	# EVB Software Engineering License Manager
evb-elm	1504/udp	0.000428	# EVB Software Engineering License Manager
funkproxy	1505/tcp	0.000013	# Funk Software, Inc.
funkproxy	1505/udp	0.000675	# Funk Software, Inc.
utcd	1506/tcp	0.000000	# Universal Time daemon (utcd)
utcd	1506/udp	0.000544	# Universal Time daemon (utcd)
symplex	1507/tcp	0.000075
symplex	1507/udp	0.000840
diagmond	1508/tcp	0.000013
diagmond	1508/udp	0.000478
robcad-lm	1509/tcp	0.000013	# Robcad, Ltd. License Manager
robcad-lm	1509/udp	0.000593	# Robcad, Ltd. License Manager
mvx-lm	1510/tcp	0.000025	# Midland Valley Exploration Ltd. Lic. Man.
mvx-lm	1510/udp	0.000511	# Midland Valley Exploration Ltd. Lic. Man.
3l-l1	1511/tcp	0.000025
3l-l1	1511/udp	0.000577
wins	1512/tcp	0.000000	# Microsoft's Windows Internet Name Service
wins	1512/udp	0.000791	# Microsoft's Windows Internet Name Service
fujitsu-dtc	1513/tcp	0.000025	# Fujitsu Systems Business of America, Inc
fujitsu-dtc	1513/udp	0.000807	# Fujitsu Systems Business of America, Inc
fujitsu-dtcns	1514/tcp	0.000000	# Fujitsu Systems Business of America, Inc
fujitsu-dtcns	1514/udp	0.001120	# Fujitsu Systems Business of America, Inc
ifor-protocol	1515/tcp	0.000038
ifor-protocol	1515/udp	0.000758
vpad	1516/tcp	0.000113	# Virtual Places Audio data
vpad	1516/udp	0.000593	# Virtual Places Audio data
vpac	1517/tcp	0.000050	# Virtual Places Audio control
vpac	1517/udp	0.000428	# Virtual Places Audio control
vpvd	1518/tcp	0.000013	# Virtual Places Video data
vpvd	1518/udp	0.000758	# Virtual Places Video data
vpvc	1519/tcp	0.000025	# Virtual Places Video control
vpvc	1519/udp	0.000593	# Virtual Places Video control
atm-zip-office	1520/tcp	0.000000	# atm zip office
atm-zip-office	1520/udp	0.000428	# atm zip office
oracle	1521/tcp	0.001568	# ncube-lm | Oracle Database | nCube License Manager
ncube-lm	1521/udp	0.000873	# nCube License Manager
rna-lm	1522/tcp	0.000100	# ricardo-lm | Ricardo North America License Manager
rna-lm	1522/udp	0.000461	# Ricardo North America License Manager
cichild-lm	1523/tcp	0.000050	# cichild
cichild-lm	1523/udp	0.000610
ingreslock	1524/tcp	0.000276	# ingres
ingreslock	1524/udp	0.001647	# ingres
orasrv	1525/tcp	0.000088	# prospero-np | oracle or Prospero Directory Service non-priv | oracle | Prospero Directory Service non-priv
oracle	1525/udp	0.000461
pdap-np	1526/tcp	0.000113	# Prospero Data Access Prot non-priv
pdap-np	1526/udp	0.000478	# Prospero Data Access Prot non-priv
tlisrv	1527/tcp	0.000038	# oracle
tlisrv	1527/udp	0.000758	# oracle
mciautoreg	1528/tcp	0.000025	# norp | ngr-t | NGR transport protocol for mobile ad-hoc networks | Not Only a Routeing Protocol
mciautoreg	1528/udp	0.000445
support	1529/tcp	0.000025	# coauthor | prmsd gnatsd	# cygnus bug tracker | oracle
coauthor	1529/udp	0.000544	# oracle
rap-service	1530/tcp	0.000000
rap-service	1530/udp	0.000675
rap-listen	1531/tcp	0.000025
rap-listen	1531/udp	0.000857
miroconnect	1532/tcp	0.000013
miroconnect	1532/udp	0.000708
virtual-places	1533/tcp	0.000238	# Virtual Places Software
virtual-places	1533/udp	0.000428	# Virtual Places Software
micromuse-lm	1534/tcp	0.000000
micromuse-lm	1534/udp	0.000461
ampr-info	1535/tcp	0.000038
ampr-info	1535/udp	0.000610
ampr-inter	1536/tcp	0.000000
ampr-inter	1536/udp	0.000593
sdsc-lm	1537/tcp	0.000025	# isi-lm
sdsc-lm	1537/udp	0.000807
3ds-lm	1538/tcp	0.000025
3ds-lm	1538/udp	0.000346
intellistor-lm	1539/tcp	0.000038	# Intellistor License Manager
intellistor-lm	1539/udp	0.000412	# Intellistor License Manager
rds	1540/tcp	0.000013
rds	1540/udp	0.000428
rds2	1541/tcp	0.000013
rds2	1541/udp	0.000395
gridgen-elmd	1542/tcp	0.000013
gridgen-elmd	1542/udp	0.000461
simba-cs	1543/tcp	0.000013
simba-cs	1543/udp	0.000461
aspeclmd	1544/tcp	0.000025
aspeclmd	1544/udp	0.000511
vistium-share	1545/tcp	0.000025
vistium-share	1545/udp	0.000544
abbaccuray	1546/tcp	0.000000
abbaccuray	1546/udp	0.000560
laplink	1547/tcp	0.000113
laplink	1547/udp	0.000544
axon-lm	1548/tcp	0.000025	# Axon License Manager
axon-lm	1548/udp	0.000708	# Axon License Manager
shivahose	1549/tcp	0.000025	# shivasound | Shiva Hose | Shiva Sound
shivasound	1549/udp	0.000610	# Shiva Sound
3m-image-lm	1550/tcp	0.000125	# Image Storage license manager 3M Company
3m-image-lm	1550/udp	0.000362	# Image Storage license manager 3M Company
hecmtl-db	1551/tcp	0.000050
hecmtl-db	1551/udp	0.000675
pciarray	1552/tcp	0.000050
pciarray	1552/udp	0.000478
sna-cs	1553/tcp	0.000000
sna-cs	1553/udp	0.000000
caci-lm	1554/tcp	0.000000	# CACI Products Company License Manager
caci-lm	1554/udp	0.000000	# CACI Products Company License Manager
livelan	1555/tcp	0.000000
livelan	1555/udp	0.000330
veritas_pbx	1556/tcp	0.000152	# veritas-pbx | VERITAS Private Branch Exchange
veritas_pbx	1556/udp	0.000000	# VERITAS Private Branch Exchange
arbortext-lm	1557/tcp	0.000000	# ArborText License Manager
arbortext-lm	1557/udp	0.000000	# ArborText License Manager
xingmpeg	1558/tcp	0.000076
xingmpeg	1558/udp	0.000000
web2host	1559/tcp	0.000076
web2host	1559/udp	0.000330
asci-val	1560/tcp	0.000076	# ASCI-RemoteSHADOW
asci-val	1560/udp	0.000000	# ASCI-RemoteSHADOW
facilityview	1561/tcp	0.000000
facilityview	1561/udp	0.000000
pconnectmgr	1562/tcp	0.000000
pconnectmgr	1562/udp	0.000000
cadabra-lm	1563/tcp	0.000000	# Cadabra License Manager
cadabra-lm	1563/udp	0.000000	# Cadabra License Manager
pay-per-view	1564/tcp	0.000000
pay-per-view	1564/udp	0.000000
winddlb	1565/tcp	0.000076	# WinDD
winddlb	1565/udp	0.000000	# WinDD
corelvideo	1566/tcp	0.000076
corelvideo	1566/udp	0.000000
jlicelmd	1567/tcp	0.000000
jlicelmd	1567/udp	0.000000
tsspmap	1568/tcp	0.000000
tsspmap	1568/udp	0.000000
ets	1569/tcp	0.000076
ets	1569/udp	0.000000
orbixd	1570/tcp	0.000000
orbixd	1570/udp	0.000000
rdb-dbs-disp	1571/tcp	0.000000	# Oracle Remote Data Base
rdb-dbs-disp	1571/udp	0.000000	# Oracle Remote Data Base
chip-lm	1572/tcp	0.000000	# Chipcom License Manager
chip-lm	1572/udp	0.000330	# Chipcom License Manager
itscomm-ns	1573/tcp	0.000000
itscomm-ns	1573/udp	0.000000
mvel-lm	1574/tcp	0.000000
mvel-lm	1574/udp	0.000000
oraclenames	1575/tcp	0.000000
oraclenames	1575/udp	0.000000
moldflow-lm	1576/tcp	0.000000	# Moldflow License Manager
moldflow-lm	1576/udp	0.000330	# Moldflow License Manager
hypercube-lm	1577/tcp	0.000000
hypercube-lm	1577/udp	0.000000
jacobus-lm	1578/tcp	0.000000	# Jacobus License Manager
jacobus-lm	1578/udp	0.000000	# Jacobus License Manager
ioc-sea-lm	1579/tcp	0.000000
ioc-sea-lm	1579/udp	0.000330
tn-tl-r1	1580/tcp	0.000304	# tn-tl-r2
tn-tl-r2	1580/udp	0.000000
mil-2045-47001	1581/tcp	0.000000
mil-2045-47001	1581/udp	0.000000
msims	1582/tcp	0.000000
msims	1582/udp	0.000000
simbaexpress	1583/tcp	0.000152
simbaexpress	1583/udp	0.000000
tn-tl-fd2	1584/tcp	0.000076
tn-tl-fd2	1584/udp	0.000000
intv	1585/tcp	0.000000
intv	1585/udp	0.000661
ibm-abtact	1586/tcp	0.000000
ibm-abtact	1586/udp	0.000000
pra_elmd	1587/tcp	0.000000	# pra-elmd
pra_elmd	1587/udp	0.000330
triquest-lm	1588/tcp	0.000000
triquest-lm	1588/udp	0.000000
vqp	1589/tcp	0.000000
vqp	1589/udp	0.000330
gemini-lm	1590/tcp	0.000000
gemini-lm	1590/udp	0.000000
ncpm-pm	1591/tcp	0.000000
ncpm-pm	1591/udp	0.000000
commonspace	1592/tcp	0.000076
commonspace	1592/udp	0.000000
mainsoft-lm	1593/tcp	0.000000
mainsoft-lm	1593/udp	0.000000
sixtrak	1594/tcp	0.000152
sixtrak	1594/udp	0.000000
radio	1595/tcp	0.000000
radio	1595/udp	0.000000
radio-sm	1596/tcp	0.000000	# radio-bc
radio-bc	1596/udp	0.000330
orbplus-iiop	1597/tcp	0.000000
orbplus-iiop	1597/udp	0.000330
picknfs	1598/tcp	0.000076
picknfs	1598/udp	0.000000
simbaservices	1599/tcp	0.000000
simbaservices	1599/udp	0.000330
issd	1600/tcp	0.000263
issd	1600/udp	0.000807
aas	1601/tcp	0.000000
aas	1601/udp	0.000000
inspect	1602/tcp	0.000000
inspect	1602/udp	0.000000
picodbc	1603/tcp	0.000000	# pickodbc
picodbc	1603/udp	0.000000	# pickodbc
icabrowser	1604/tcp	0.000000
icabrowser	1604/udp	0.000000
slp	1605/tcp	0.000076	# Salutation Manager (Salutation Protocol)
slp	1605/udp	0.000330	# Salutation Manager (Salutation Protocol)
slm-api	1606/tcp	0.000000	# Salutation Manager (SLM-API)
slm-api	1606/udp	0.000330	# Salutation Manager (SLM-API)
stt	1607/tcp	0.000076
stt	1607/udp	0.000000
smart-lm	1608/tcp	0.000000	# Smart Corp. License Manager
smart-lm	1608/udp	0.000330	# Smart Corp. License Manager
isysg-lm	1609/tcp	0.000000
isysg-lm	1609/udp	0.000000
taurus-wh	1610/tcp	0.000000
taurus-wh	1610/udp	0.000330
ill	1611/tcp	0.000000	# Inter Library Loan
ill	1611/udp	0.000000	# Inter Library Loan
netbill-trans	1612/tcp	0.000000	# NetBill Transaction Server
netbill-trans	1612/udp	0.000000	# NetBill Transaction Server
netbill-keyrep	1613/tcp	0.000000	# NetBill Key Repository
netbill-keyrep	1613/udp	0.000000	# NetBill Key Repository
netbill-cred	1614/tcp	0.000000	# NetBill Credential Server
netbill-cred	1614/udp	0.000000	# NetBill Credential Server
netbill-auth	1615/tcp	0.000076	# NetBill Authorization Server
netbill-auth	1615/udp	0.000000	# NetBill Authorization Server
netbill-prod	1616/tcp	0.000000	# NetBill Product Server
netbill-prod	1616/udp	0.000330	# NetBill Product Server
nimrod-agent	1617/tcp	0.000000	# Nimrod Inter-Agent Communication
nimrod-agent	1617/udp	0.000000	# Nimrod Inter-Agent Communication
skytelnet	1618/tcp	0.000000
skytelnet	1618/udp	0.000330
xs-openstorage	1619/tcp	0.000000
xs-openstorage	1619/udp	0.000000
faxportwinport	1620/tcp	0.000076
faxportwinport	1620/udp	0.000661
softdataphone	1621/tcp	0.000000
softdataphone	1621/udp	0.000330
ontime	1622/tcp	0.000076
ontime	1622/udp	0.000991
jaleosnd	1623/tcp	0.000000
jaleosnd	1623/udp	0.000330
udp-sr-port	1624/tcp	0.000000
udp-sr-port	1624/udp	0.000000
svs-omagent	1625/tcp	0.000000
svs-omagent	1625/udp	0.000000
shockwave	1626/tcp	0.000000
shockwave	1626/udp	0.000330
t128-gateway	1627/tcp	0.000000	# T.128 Gateway
t128-gateway	1627/udp	0.000000	# T.128 Gateway
lontalk-norm	1628/tcp	0.000000	# LonTalk normal
lontalk-norm	1628/udp	0.000330	# LonTalk normal
lontalk-urgnt	1629/tcp	0.000000	# LonTalk urgent
lontalk-urgnt	1629/udp	0.000000	# LonTalk urgent
oraclenet8cman	1630/tcp	0.000000	# Oracle Net8 Cman
oraclenet8cman	1630/udp	0.000000	# Oracle Net8 Cman
visitview	1631/tcp	0.000000	# Visit view
visitview	1631/udp	0.000330	# Visit view
pammratc	1632/tcp	0.000076
pammratc	1632/udp	0.000000
pammrpc	1633/tcp	0.000000
pammrpc	1633/udp	0.000330
loaprobe	1634/tcp	0.000000	# Log On America Probe
loaprobe	1634/udp	0.000000	# Log On America Probe
edb-server1	1635/tcp	0.000076	# EDB Server 1
edb-server1	1635/udp	0.000000	# EDB Server 1
isdc	1636/tcp	0.000000	# ISP shared public data control
isdc	1636/udp	0.000000	# ISP shared public data control
islc	1637/tcp	0.000000	# ISP shared local data control
islc	1637/udp	0.000000	# ISP shared local data control
ismc	1638/tcp	0.000076	# ISP shared management control
ismc	1638/udp	0.000000	# ISP shared management control
cert-initiator	1639/tcp	0.000000
cert-initiator	1639/udp	0.000330
cert-responder	1640/tcp	0.000000
cert-responder	1640/udp	0.000330
invision	1641/tcp	0.000152
invision	1641/udp	0.000000
isis-am	1642/tcp	0.000000
isis-am	1642/udp	0.000000
isis-ambc	1643/tcp	0.000000
isis-ambc	1643/udp	0.000000
saiseh	1644/tcp	0.000000	# Satellite-data Acquisition System 4
sightline	1645/tcp	0.000076
radius	1645/udp	0.023180	# radius authentication
sa-msg-port	1646/tcp	0.000000
radacct	1646/udp	0.023196	# radius accounting
rsap	1647/tcp	0.000000
rsap	1647/udp	0.000330
concurrent-lm	1648/tcp	0.000000
concurrent-lm	1648/udp	0.000000
kermit	1649/tcp	0.000000
kermit	1649/udp	0.000000
nkd	1650/tcp	0.000038	# nkdn
nkd	1650/udp	0.000774
shiva_confsrvr	1651/tcp	0.000050	# shiva-confsrvr
shiva_confsrvr	1651/udp	0.000593
xnmp	1652/tcp	0.000063
xnmp	1652/udp	0.000593
alphatech-lm	1653/tcp	0.000000
alphatech-lm	1653/udp	0.000000
stargatealerts	1654/tcp	0.000000
stargatealerts	1654/udp	0.000000
dec-mbadmin	1655/tcp	0.000000
dec-mbadmin	1655/udp	0.000000
dec-mbadmin-h	1656/tcp	0.000000
dec-mbadmin-h	1656/udp	0.000000
fujitsu-mmpdc	1657/tcp	0.000000
fujitsu-mmpdc	1657/udp	0.000000
sixnetudr	1658/tcp	0.000152
sixnetudr	1658/udp	0.000000
sg-lm	1659/tcp	0.000000	# Silicon Grail License Manager
sg-lm	1659/udp	0.000000	# Silicon Grail License Manager
skip-mc-gikreq	1660/tcp	0.000000
skip-mc-gikreq	1660/udp	0.000000
netview-aix-1	1661/tcp	0.000025
netview-aix-1	1661/udp	0.000445
netview-aix-2	1662/tcp	0.000025
netview-aix-2	1662/udp	0.000807
netview-aix-3	1663/tcp	0.000063
netview-aix-3	1663/udp	0.000527
netview-aix-4	1664/tcp	0.000038
netview-aix-4	1664/udp	0.000939
netview-aix-5	1665/tcp	0.000000
netview-aix-5	1665/udp	0.000362
netview-aix-6	1666/tcp	0.000577
netview-aix-6	1666/udp	0.001186
netview-aix-7	1667/tcp	0.000025
netview-aix-7	1667/udp	0.000445
netview-aix-8	1668/tcp	0.000038
netview-aix-8	1668/udp	0.000428
netview-aix-9	1669/tcp	0.000000
netview-aix-9	1669/udp	0.000412
netview-aix-10	1670/tcp	0.000013
netview-aix-10	1670/udp	0.000675
netview-aix-11	1671/tcp	0.000013
netview-aix-11	1671/udp	0.000659
netview-aix-12	1672/tcp	0.000013
netview-aix-12	1672/udp	0.000824
proshare-mc-1	1673/tcp	0.000000	# Intel Proshare Multicast
proshare-mc-1	1673/udp	0.000000	# Intel Proshare Multicast
proshare-mc-2	1674/tcp	0.000000	# Intel Proshare Multicast
proshare-mc-2	1674/udp	0.000000	# Intel Proshare Multicast
pdp	1675/tcp	0.000000	# Pacific Data Products
pdp	1675/udp	0.000000	# Pacific Data Products
netcomm1	1676/tcp	0.000000	# netcomm2
netcomm2	1676/udp	0.000000
groupwise	1677/tcp	0.000076
groupwise	1677/udp	0.000330
prolink	1678/tcp	0.000000
prolink	1678/udp	0.000330
darcorp-lm	1679/tcp	0.000000
darcorp-lm	1679/udp	0.000000
CarbonCopy	1680/tcp	0.000063	# microcom-sbp
microcom-sbp	1680/udp	0.000330
sd-elmd	1681/tcp	0.000000
sd-elmd	1681/udp	0.000000
lanyon-lantern	1682/tcp	0.000000
lanyon-lantern	1682/udp	0.000000
ncpm-hip	1683/tcp	0.000076
ncpm-hip	1683/udp	0.000000
snaresecure	1684/tcp	0.000000
snaresecure	1684/udp	0.000000
n2nremote	1685/tcp	0.000000
n2nremote	1685/udp	0.000661
cvmon	1686/tcp	0.000000
cvmon	1686/udp	0.000000
nsjtp-ctrl	1687/tcp	0.000380
nsjtp-ctrl	1687/udp	0.000330
nsjtp-data	1688/tcp	0.000152
nsjtp-data	1688/udp	0.000330
firefox	1689/tcp	0.000000
firefox	1689/udp	0.000000
ng-umds	1690/tcp	0.000000
ng-umds	1690/udp	0.000000
empire-empuma	1691/tcp	0.000076
empire-empuma	1691/udp	0.000000
sstsys-lm	1692/tcp	0.000000
sstsys-lm	1692/udp	0.000000
rrirtr	1693/tcp	0.000000
rrirtr	1693/udp	0.000000
rrimwm	1694/tcp	0.000076
rrimwm	1694/udp	0.000000
rrilwm	1695/tcp	0.000000
rrilwm	1695/udp	0.000661
rrifmm	1696/tcp	0.000000
rrifmm	1696/udp	0.000330
rrisat	1697/tcp	0.000000
rrisat	1697/udp	0.000000
rsvp-encap-1	1698/tcp	0.000000	# RSVP-ENCAPSULATION-1
rsvp-encap-1	1698/udp	0.000000	# RSVP-ENCAPSULATION-1
rsvp-encap-2	1699/tcp	0.000076	# RSVP-ENCAPSULATION-2
rsvp-encap-2	1699/udp	0.000330	# RSVP-ENCAPSULATION-2
mps-raft	1700/tcp	0.000836
mps-raft	1700/udp	0.000000
l2f	1701/tcp	0.000076	# l2tp
L2TP	1701/udp	0.076163
deskshare	1702/tcp	0.000000
deskshare	1702/udp	0.000000
hb-engine	1703/tcp	0.000076
hb-engine	1703/udp	0.000000
bcs-broker	1704/tcp	0.000000
bcs-broker	1704/udp	0.000000
slingshot	1705/tcp	0.000000
slingshot	1705/udp	0.000000
jetform	1706/tcp	0.000000
jetform	1706/udp	0.000000
vdmplay	1707/tcp	0.000076
vdmplay	1707/udp	0.000000
gat-lmd	1708/tcp	0.000076
gat-lmd	1708/udp	0.000000
centra	1709/tcp	0.000076
centra	1709/udp	0.000000
impera	1710/tcp	0.000000
impera	1710/udp	0.000000
pptconference	1711/tcp	0.000076
pptconference	1711/udp	0.000330
registrar	1712/tcp	0.000076	# resource monitoring service
registrar	1712/udp	0.000330	# resource monitoring service
conferencetalk	1713/tcp	0.000076
conferencetalk	1713/udp	0.000000
sesi-lm	1714/tcp	0.000000
sesi-lm	1714/udp	0.000000
houdini-lm	1715/tcp	0.000076
houdini-lm	1715/udp	0.000000
xmsg	1716/tcp	0.000000
xmsg	1716/udp	0.000000
fj-hdnet	1717/tcp	0.000912
fj-hdnet	1717/udp	0.000000
h323gatedisc	1718/tcp	0.000380	# H.323 Multicast Gatekeeper Discover
h225gatedisc	1718/udp	0.012554	# H.225 gatekeeper discovery
h323gatestat	1719/tcp	0.000152	# H.323 Unicast Gatekeeper Signaling
h323gatestat	1719/udp	0.018500	# H.323 Gatestat
h323q931	1720/tcp	0.014277	# h323hostcall | Interactive media | H.323 Call Control Signalling | H.323 Call Control
h323hostcall	1720/udp	0.000000
caicci	1721/tcp	0.000152
caicci	1721/udp	0.000000
hks-lm	1722/tcp	0.000076	# HKS License Manager
hks-lm	1722/udp	0.000000	# HKS License Manager
pptp	1723/tcp	0.032468	# Point-to-point tunnelling protocol
pptp	1723/udp	0.000000
csbphone	1724/tcp	0.000000	# csbphonemaster
csbphone	1724/udp	0.000330
iden-ralp	1725/tcp	0.000000
iden-ralp	1725/udp	0.000000
iberiagames	1726/tcp	0.000000
iberiagames	1726/udp	0.000330
winddx	1727/tcp	0.000000
winddx	1727/udp	0.000000
telindus	1728/tcp	0.000000
telindus	1728/udp	0.000000
citynl	1729/tcp	0.000000	# CityNL License Management
citynl	1729/udp	0.000330	# CityNL License Management
roketz	1730/tcp	0.000076
roketz	1730/udp	0.000330
msiccp	1731/tcp	0.000000
msiccp	1731/udp	0.000000
proxim	1732/tcp	0.000000
proxim	1732/udp	0.000000
siipat	1733/tcp	0.000000	# SIMS - SIIPAT Protocol for Alarm Transmission
siipat	1733/udp	0.000330	# SIMS - SIIPAT Protocol for Alarm Transmission
cambertx-lm	1734/tcp	0.000000	# Camber Corporation License Management
cambertx-lm	1734/udp	0.000000	# Camber Corporation License Management
privatechat	1735/tcp	0.000076
privatechat	1735/udp	0.000000
street-stream	1736/tcp	0.000076
street-stream	1736/udp	0.000000
ultimad	1737/tcp	0.000000
ultimad	1737/udp	0.000000
gamegen1	1738/tcp	0.000000
gamegen1	1738/udp	0.000661
webaccess	1739/tcp	0.000000
webaccess	1739/udp	0.000000
encore	1740/tcp	0.000000
encore	1740/udp	0.000330
cisco-net-mgmt	1741/tcp	0.000000
cisco-net-mgmt	1741/udp	0.000000
3Com-nsd	1742/tcp	0.000000
3Com-nsd	1742/udp	0.000000
cinegrfx-lm	1743/tcp	0.000000	# Cinema Graphics License Manager
cinegrfx-lm	1743/udp	0.000330	# Cinema Graphics License Manager
ncpm-ft	1744/tcp	0.000000
ncpm-ft	1744/udp	0.000000
remote-winsock	1745/tcp	0.000076
remote-winsock	1745/udp	0.000000
ftrapid-1	1746/tcp	0.000000
ftrapid-1	1746/udp	0.000000
ftrapid-2	1747/tcp	0.000000
ftrapid-2	1747/udp	0.000000
oracle-em1	1748/tcp	0.000000
oracle-em1	1748/udp	0.000000
aspen-services	1749/tcp	0.000000
aspen-services	1749/udp	0.000000
sslp	1750/tcp	0.000076	# Simple Socket Library's PortMaster
sslp	1750/udp	0.000000	# Simple Socket Library's PortMaster
swiftnet	1751/tcp	0.000000
swiftnet	1751/udp	0.000000
lofr-lm	1752/tcp	0.000076	# Leap of Faith Research License Manager
lofr-lm	1752/udp	0.000000	# Leap of Faith Research License Manager
predatar-comms	1753/tcp	0.000076	# Predatar Comms Service
unknown	1753/udp	0.000661
oracle-em2	1754/tcp	0.000000
oracle-em2	1754/udp	0.000000
wms	1755/tcp	0.003350	# Windows media service | ms-streaming
ms-streaming	1755/udp	0.000661
capfast-lmd	1756/tcp	0.000000
capfast-lmd	1756/udp	0.000000
cnhrp	1757/tcp	0.000000
cnhrp	1757/udp	0.000000
tftp-mcast	1758/tcp	0.000000
tftp-mcast	1758/udp	0.000000
spss-lm	1759/tcp	0.000000	# SPSS License Manager
spss-lm	1759/udp	0.000000	# SPSS License Manager
www-ldap-gw	1760/tcp	0.000000
www-ldap-gw	1760/udp	0.000000
landesk-rc	1761/tcp	0.001756	# LANDesk Remote Control | cft-0
cft-0	1761/udp	0.002313
landesk-rc	1762/tcp	0.000038	# LANDesk Remote Control | cft-1
cft-1	1762/udp	0.000000
landesk-rc	1763/tcp	0.000025	# LANDesk Remote Control | cft-2
cft-2	1763/udp	0.000000
landesk-rc	1764/tcp	0.000000	# LANDesk Remote Control | cft-3
cft-3	1764/udp	0.000000
cft-4	1765/tcp	0.000000
cft-4	1765/udp	0.000000
cft-5	1766/tcp	0.000000
cft-5	1766/udp	0.000330
cft-6	1767/tcp	0.000000
cft-6	1767/udp	0.000330
cft-7	1768/tcp	0.000000
cft-7	1768/udp	0.000000
bmc-net-adm	1769/tcp	0.000000
bmc-net-adm	1769/udp	0.000000
bmc-net-svc	1770/tcp	0.000000
bmc-net-svc	1770/udp	0.000000
vaultbase	1771/tcp	0.000000
vaultbase	1771/udp	0.000000
essweb-gw	1772/tcp	0.000000	# EssWeb Gateway
essweb-gw	1772/udp	0.000000	# EssWeb Gateway
kmscontrol	1773/tcp	0.000000
kmscontrol	1773/udp	0.000330
global-dtserv	1774/tcp	0.000000
global-dtserv	1774/udp	0.000000
vdab	1775/tcp	0.000000	# data interchange between visual processing containers
femis	1776/tcp	0.000000	# Federal Emergency Management Information System
femis	1776/udp	0.000000	# Federal Emergency Management Information System
powerguardian	1777/tcp	0.000000
powerguardian	1777/udp	0.000000
prodigy-intrnet	1778/tcp	0.000000	# prodigy-internet
prodigy-intrnet	1778/udp	0.000000	# prodigy-internet
pharmasoft	1779/tcp	0.000000
pharmasoft	1779/udp	0.000330
dpkeyserv	1780/tcp	0.000000
dpkeyserv	1780/udp	0.000000
answersoft-lm	1781/tcp	0.000000
answersoft-lm	1781/udp	0.000000
hp-hcip	1782/tcp	0.000304
hp-hcip	1782/udp	0.004625
unknown	1783/tcp	0.000380
finle-lm	1784/tcp	0.000000	# Finle License Manager
finle-lm	1784/udp	0.000000	# Finle License Manager
windlm	1785/tcp	0.000000	# Wind River Systems License Manager
windlm	1785/udp	0.000000	# Wind River Systems License Manager
funk-logger	1786/tcp	0.000000
funk-logger	1786/udp	0.000330
funk-license	1787/tcp	0.000000
funk-license	1787/udp	0.000000
psmond	1788/tcp	0.000000
psmond	1788/udp	0.000000
hello	1789/tcp	0.000000
hello	1789/udp	0.000000
nmsp	1790/tcp	0.000000	# Narrative Media Streaming Protocol
nmsp	1790/udp	0.000000	# Narrative Media Streaming Protocol
ea1	1791/tcp	0.000076
ea1	1791/udp	0.000000
ibm-dt-2	1792/tcp	0.000076
ibm-dt-2	1792/udp	0.000661
rsc-robot	1793/tcp	0.000000
rsc-robot	1793/udp	0.000000
cera-bcm	1794/tcp	0.000000
cera-bcm	1794/udp	0.000000
dpi-proxy	1795/tcp	0.000000
dpi-proxy	1795/udp	0.000000
vocaltec-admin	1796/tcp	0.000000	# Vocaltec Server Administration
vocaltec-admin	1796/udp	0.000330	# Vocaltec Server Administration
uma	1797/tcp	0.000000
uma	1797/udp	0.000000
etp	1798/tcp	0.000000	# Event Transfer Protocol
etp	1798/udp	0.000000	# Event Transfer Protocol
netrisk	1799/tcp	0.000076
netrisk	1799/udp	0.000000
ansys-lm	1800/tcp	0.000076	# ANSYS-License manager
ansys-lm	1800/udp	0.000330	# ANSYS-License manager
msmq	1801/tcp	0.002585	# Microsoft Message Queuing | Microsoft Message Que
msmq	1801/udp	0.000000	# Microsoft Message Que
concomp1	1802/tcp	0.000000
concomp1	1802/udp	0.000000
hp-hcip-gwy	1803/tcp	0.000000
hp-hcip-gwy	1803/udp	0.000661
enl	1804/tcp	0.000000
enl	1804/udp	0.001652
enl-name	1805/tcp	0.000152
enl-name	1805/udp	0.000000
musiconline	1806/tcp	0.000076
musiconline	1806/udp	0.000000
fhsp	1807/tcp	0.000076	# Fujitsu Hot Standby Protocol
fhsp	1807/udp	0.000000	# Fujitsu Hot Standby Protocol
oracle-vp2	1808/tcp	0.000076
oracle-vp2	1808/udp	0.000000
oracle-vp1	1809/tcp	0.000000
oracle-vp1	1809/udp	0.000000
jerand-lm	1810/tcp	0.000000	# Jerand License Manager
jerand-lm	1810/udp	0.000000	# Jerand License Manager
scientia-sdb	1811/tcp	0.000076
scientia-sdb	1811/udp	0.000000
radius	1812/sctp	0.000000	# RADIUS authentication protocol (RFC 2138)
radius	1812/tcp	0.000152
radius	1812/udp	0.053839	# RADIUS authentication protocol (RFC 2138)
radacct	1813/sctp	0.000000	# radius-acct | RADIUS accounting protocol (RFC 2139) | RADIUS Accounting
radius-acct	1813/tcp	0.000000	# RADIUS Accounting
radacct	1813/udp	0.010429	# RADIUS accounting protocol (RFC 2139)
tdp-suite	1814/tcp	0.000000	# TDP Suite
tdp-suite	1814/udp	0.000330	# TDP Suite
mmpft	1815/tcp	0.000000
mmpft	1815/udp	0.000330
harp	1816/tcp	0.000000
harp	1816/udp	0.000000
rkb-oscs	1817/tcp	0.000000
rkb-oscs	1817/udp	0.000000
etftp	1818/tcp	0.000000	# Enhanced Trivial File Transfer Protocol
etftp	1818/udp	0.000330	# Enhanced Trivial File Transfer Protocol
plato-lm	1819/tcp	0.000000	# Plato License Manager
plato-lm	1819/udp	0.000000	# Plato License Manager
mcagent	1820/tcp	0.000000
mcagent	1820/udp	0.000000
donnyworld	1821/tcp	0.000000
donnyworld	1821/udp	0.000000
es-elmd	1822/tcp	0.000000
es-elmd	1822/udp	0.000330
unisys-lm	1823/tcp	0.000076	# Unisys Natural Language License Manager
unisys-lm	1823/udp	0.000000	# Unisys Natural Language License Manager
metrics-pas	1824/tcp	0.000000
metrics-pas	1824/udp	0.000330
direcpc-video	1825/tcp	0.000076	# DirecPC Video
direcpc-video	1825/udp	0.000000	# DirecPC Video
ardt	1826/tcp	0.000000
ardt	1826/udp	0.000330
pcm	1827/tcp	0.000025	# asi | PCM Agent (AutoSecure Policy Compliance Manager | ASI
asi	1827/udp	0.000330
itm-mcell-u	1828/tcp	0.000000
itm-mcell-u	1828/udp	0.000000
optika-emedia	1829/tcp	0.000000	# Optika eMedia
optika-emedia	1829/udp	0.000000	# Optika eMedia
net8-cman	1830/tcp	0.000000	# Oracle Net8 CMan Admin
net8-cman	1830/udp	0.000000	# Oracle Net8 CMan Admin
myrtle	1831/tcp	0.000000
myrtle	1831/udp	0.000000
tht-treasure	1832/tcp	0.000000	# ThoughtTreasure
tht-treasure	1832/udp	0.000000	# ThoughtTreasure
udpradio	1833/tcp	0.000000
udpradio	1833/udp	0.000000
ardusuni	1834/tcp	0.000000	# ARDUS Unicast
ardusuni	1834/udp	0.000661	# ARDUS Unicast
ardusmul	1835/tcp	0.000076	# ARDUS Multicast
ardusmul	1835/udp	0.000330	# ARDUS Multicast
ste-smsc	1836/tcp	0.000000
ste-smsc	1836/udp	0.000000
csoft1	1837/tcp	0.000000
csoft1	1837/udp	0.000000
talnet	1838/tcp	0.000000
talnet	1838/udp	0.000000
netopia-vo1	1839/tcp	0.000152
netopia-vo1	1839/udp	0.000000
netopia-vo2	1840/tcp	0.000380
netopia-vo2	1840/udp	0.000330
netopia-vo3	1841/tcp	0.000000
netopia-vo3	1841/udp	0.000330
netopia-vo4	1842/tcp	0.000000
netopia-vo4	1842/udp	0.000000
netopia-vo5	1843/tcp	0.000000
netopia-vo5	1843/udp	0.000000
direcpc-dll	1844/tcp	0.000000
direcpc-dll	1844/udp	0.000000
altalink	1845/tcp	0.000000
altalink	1845/udp	0.000000
tunstall-pnc	1846/tcp	0.000000	# Tunstall PNC
tunstall-pnc	1846/udp	0.000000	# Tunstall PNC
slp-notify	1847/tcp	0.000000	# SLP Notification
slp-notify	1847/udp	0.000000	# SLP Notification
fjdocdist	1848/tcp	0.000000
fjdocdist	1848/udp	0.000000
alpha-sms	1849/tcp	0.000000
alpha-sms	1849/udp	0.000000
gsi	1850/tcp	0.000000
gsi	1850/udp	0.000000
ctcd	1851/tcp	0.000000
ctcd	1851/udp	0.000000
virtual-time	1852/tcp	0.000000	# Virtual Time
virtual-time	1852/udp	0.000000	# Virtual Time
vids-avtp	1853/tcp	0.000000
vids-avtp	1853/udp	0.000000
buddy-draw	1854/tcp	0.000000	# Buddy Draw
buddy-draw	1854/udp	0.000000	# Buddy Draw
fiorano-rtrsvc	1855/tcp	0.000000	# Fiorano RtrSvc
fiorano-rtrsvc	1855/udp	0.000000	# Fiorano RtrSvc
fiorano-msgsvc	1856/tcp	0.000000	# Fiorano MsgSvc
fiorano-msgsvc	1856/udp	0.000330	# Fiorano MsgSvc
datacaptor	1857/tcp	0.000000
datacaptor	1857/udp	0.000000
privateark	1858/tcp	0.000076
privateark	1858/udp	0.000000
gammafetchsvr	1859/tcp	0.000000	# Gamma Fetcher Server
gammafetchsvr	1859/udp	0.000000	# Gamma Fetcher Server
sunscalar-svc	1860/tcp	0.000000	# SunSCALAR Services
sunscalar-svc	1860/udp	0.000000	# SunSCALAR Services
lecroy-vicp	1861/tcp	0.000076	# LeCroy VICP
lecroy-vicp	1861/udp	0.000661	# LeCroy VICP
mysql-cm-agent	1862/tcp	0.000228	# MySQL Cluster Manager Agent
mysql-cm-agent	1862/udp	0.000991	# MySQL Cluster Manager Agent
msnp	1863/tcp	0.000684	# MSN Messenger
msnp	1863/udp	0.000000	# MSN Messenger
paradym-31	1864/tcp	0.000684	# paradym-31port | Paradym 31 Port
paradym-31	1864/udp	0.000000
entp	1865/tcp	0.000000
entp	1865/udp	0.000000
swrmi	1866/tcp	0.000000
swrmi	1866/udp	0.000000
udrive	1867/tcp	0.000000
udrive	1867/udp	0.000000
viziblebrowser	1868/tcp	0.000000
viziblebrowser	1868/udp	0.000000
transact	1869/tcp	0.000000
transact	1869/udp	0.000000
sunscalar-dns	1870/tcp	0.000000	# SunSCALAR DNS Service
sunscalar-dns	1870/udp	0.000000	# SunSCALAR DNS Service
canocentral0	1871/tcp	0.000076	# Cano Central 0
canocentral0	1871/udp	0.000330	# Cano Central 0
canocentral1	1872/tcp	0.000000	# Cano Central 1
canocentral1	1872/udp	0.000000	# Cano Central 1
fjmpjps	1873/tcp	0.000000
fjmpjps	1873/udp	0.000330
fjswapsnp	1874/tcp	0.000000
fjswapsnp	1874/udp	0.000000
westell-stats	1875/tcp	0.000152	# westell stats
westell-stats	1875/udp	0.000330	# westell stats
ewcappsrv	1876/tcp	0.000000
ewcappsrv	1876/udp	0.000000
hp-webqosdb	1877/tcp	0.000000
hp-webqosdb	1877/udp	0.000000
drmsmc	1878/tcp	0.000000
drmsmc	1878/udp	0.000000
nettgain-nms	1879/tcp	0.000000	# NettGain NMS
nettgain-nms	1879/udp	0.000000	# NettGain NMS
vsat-control	1880/tcp	0.000000	# Gilat VSAT Control
vsat-control	1880/udp	0.000000	# Gilat VSAT Control
ibm-mqseries2	1881/tcp	0.000000	# IBM WebSphere MQ Everyplace
ibm-mqseries2	1881/udp	0.000000	# IBM WebSphere MQ Everyplace
ecsqdmn	1882/tcp	0.000000	# CA eTrust Common Services
ecsqdmn	1882/udp	0.000000	# CA eTrust Common Services
mqtt	1883/tcp	0.000076	# Message Queuing Telemetry Transport Protocol
ibm-mqisdp	1883/udp	0.000330	# IBM MQSeries SCADA
idmaps	1884/tcp	0.000000	# Internet Distance Map Svc
idmaps	1884/udp	0.000661	# Internet Distance Map Svc
vrtstrapserver	1885/tcp	0.000000	# Veritas Trap Server
vrtstrapserver	1885/udp	0.003304	# Veritas Trap Server
leoip	1886/tcp	0.000000	# Leonardo over IP
leoip	1886/udp	0.002973	# Leonardo over IP
filex-lport	1887/tcp	0.000000	# FileX Listening Port
filex-lport	1887/udp	0.000000	# FileX Listening Port
ncconfig	1888/tcp	0.000000	# NC Config Port
ncconfig	1888/udp	0.000330	# NC Config Port
unify-adapter	1889/tcp	0.000000	# Unify Web Adapter Service
unify-adapter	1889/udp	0.000000	# Unify Web Adapter Service
wilkenlistener	1890/tcp	0.000000
wilkenlistener	1890/udp	0.000000
childkey-notif	1891/tcp	0.000000	# ChildKey Notification
childkey-notif	1891/udp	0.000330	# ChildKey Notification
childkey-ctrl	1892/tcp	0.000000	# ChildKey Control
childkey-ctrl	1892/udp	0.000000	# ChildKey Control
elad	1893/tcp	0.000000	# ELAD Protocol
elad	1893/udp	0.000000	# ELAD Protocol
o2server-port	1894/tcp	0.000000	# O2Server Port
o2server-port	1894/udp	0.000000	# O2Server Port
unknown	1895/udp	0.000330
b-novative-ls	1896/tcp	0.000000	# b-novative license server
b-novative-ls	1896/udp	0.000000	# b-novative license server
metaagent	1897/tcp	0.000000
metaagent	1897/udp	0.000000
cymtec-port	1898/tcp	0.000000	# Cymtec secure management
cymtec-port	1898/udp	0.000330	# Cymtec secure management
mc2studios	1899/tcp	0.000000
mc2studios	1899/udp	0.000000
upnp	1900/tcp	0.003977	# ssdp | Universal PnP | SSDP
upnp	1900/udp	0.136543	# Universal PnP
fjicl-tep-a	1901/tcp	0.000076	# Fujitsu ICL Terminal Emulator Program A
fjicl-tep-a	1901/udp	0.001982	# Fujitsu ICL Terminal Emulator Program A
fjicl-tep-b	1902/tcp	0.000000	# Fujitsu ICL Terminal Emulator Program B
fjicl-tep-b	1902/udp	0.000000	# Fujitsu ICL Terminal Emulator Program B
linkname	1903/tcp	0.000000	# Local Link Name Resolution
linkname	1903/udp	0.000000	# Local Link Name Resolution
fjicl-tep-c	1904/tcp	0.000000	# Fujitsu ICL Terminal Emulator Program C
fjicl-tep-c	1904/udp	0.000000	# Fujitsu ICL Terminal Emulator Program C
sugp	1905/tcp	0.000000	# Secure UP.Link Gateway Protocol
sugp	1905/udp	0.000000	# Secure UP.Link Gateway Protocol
tpmd	1906/tcp	0.000000	# TPortMapperReq
tpmd	1906/udp	0.000330	# TPortMapperReq
intrastar	1907/tcp	0.000000
intrastar	1907/udp	0.000000
dawn	1908/tcp	0.000000
dawn	1908/udp	0.000000
global-wlink	1909/tcp	0.000000	# Global World Link
global-wlink	1909/udp	0.000661	# Global World Link
ultrabac	1910/tcp	0.000000	# UltraBac Software communications port
ultrabac	1910/udp	0.000000	# UltraBac Software communications port
mtp	1911/tcp	0.000076	# Starlight Networks Multimedia Transport Protocol
mtp	1911/udp	0.000000	# Starlight Networks Multimedia Transport Protocol
rhp-iibp	1912/tcp	0.000076
rhp-iibp	1912/udp	0.000330
armadp	1913/tcp	0.000000
armadp	1913/udp	0.000000
elm-momentum	1914/tcp	0.000152
elm-momentum	1914/udp	0.000000
facelink	1915/tcp	0.000000
facelink	1915/udp	0.000000
persona	1916/tcp	0.000000	# Persoft Persona
persona	1916/udp	0.000000	# Persoft Persona
noagent	1917/tcp	0.000000
noagent	1917/udp	0.000000
can-nds	1918/tcp	0.000076	# IBM Tivole Directory Service - NDS
can-nds	1918/udp	0.000000	# IBM Tivole Directory Service - NDS
can-dch	1919/tcp	0.000000	# IBM Tivoli Directory Service - DCH
can-dch	1919/udp	0.000000	# IBM Tivoli Directory Service - DCH
can-ferret	1920/tcp	0.000000	# IBM Tivoli Directory Service - FERRET
can-ferret	1920/udp	0.000000	# IBM Tivoli Directory Service - FERRET
noadmin	1921/tcp	0.000000
noadmin	1921/udp	0.000661
tapestry	1922/tcp	0.000000
tapestry	1922/udp	0.000330
spice	1923/tcp	0.000000
spice	1923/udp	0.000000
xiip	1924/tcp	0.000076
xiip	1924/udp	0.000000
discovery-port	1925/tcp	0.000000	# Surrogate Discovery Port
discovery-port	1925/udp	0.000000	# Surrogate Discovery Port
egs	1926/tcp	0.000000	# Evolution Game Server
egs	1926/udp	0.000000	# Evolution Game Server
videte-cipc	1927/tcp	0.000076	# Videte CIPC Port
videte-cipc	1927/udp	0.000000	# Videte CIPC Port
emsd-port	1928/tcp	0.000000	# Expnd Maui Srvr Dscovr
emsd-port	1928/udp	0.000000	# Expnd Maui Srvr Dscovr
bandwiz-system	1929/tcp	0.000000	# Bandwiz System - Server
bandwiz-system	1929/udp	0.000000	# Bandwiz System - Server
driveappserver	1930/tcp	0.000000	# Drive AppServer
driveappserver	1930/udp	0.000000	# Drive AppServer
amdsched	1931/tcp	0.000000	# AMD SCHED
amdsched	1931/udp	0.000330	# AMD SCHED
ctt-broker	1932/tcp	0.000000	# CTT Broker
ctt-broker	1932/udp	0.000000	# CTT Broker
xmapi	1933/tcp	0.000000	# IBM LM MT Agent
xmapi	1933/udp	0.000000	# IBM LM MT Agent
xaapi	1934/tcp	0.000000	# IBM LM Appl Agent
xaapi	1934/udp	0.000000	# IBM LM Appl Agent
rtmp	1935/tcp	0.001179	# macromedia-fcs | Macromedia FlasComm Server | Macromedia Flash Communications Server MX | Macromedia Flash Communications server MX
macromedia-fcs	1935/udp	0.000000	# Macromedia Flash Communications server MX
jetcmeserver	1936/tcp	0.000000	# JetCmeServer Server Port
jetcmeserver	1936/udp	0.000000	# JetCmeServer Server Port
jwserver	1937/tcp	0.000000	# JetVWay Server Port
jwserver	1937/udp	0.000000	# JetVWay Server Port
jwclient	1938/tcp	0.000000	# JetVWay Client Port
jwclient	1938/udp	0.000000	# JetVWay Client Port
jvserver	1939/tcp	0.000000	# JetVision Server Port
jvserver	1939/udp	0.000000	# JetVision Server Port
jvclient	1940/tcp	0.000000	# JetVision Client Port
jvclient	1940/udp	0.000000	# JetVision Client Port
dic-aida	1941/tcp	0.000000
dic-aida	1941/udp	0.000000
res	1942/tcp	0.000000	# Real Enterprise Service
res	1942/udp	0.000000	# Real Enterprise Service
beeyond-media	1943/tcp	0.000000	# Beeyond Media
beeyond-media	1943/udp	0.000000	# Beeyond Media
close-combat	1944/tcp	0.000000
close-combat	1944/udp	0.000000
dialogic-elmd	1945/tcp	0.000000
dialogic-elmd	1945/udp	0.000000
tekpls	1946/tcp	0.000000
tekpls	1946/udp	0.000000
sentinelsrm	1947/tcp	0.000380
sentinelsrm	1947/udp	0.000330
eye2eye	1948/tcp	0.000000
eye2eye	1948/udp	0.000000
ismaeasdaqlive	1949/tcp	0.000000	# ISMA Easdaq Live
ismaeasdaqlive	1949/udp	0.000000	# ISMA Easdaq Live
ismaeasdaqtest	1950/tcp	0.000000	# ISMA Easdaq Test
ismaeasdaqtest	1950/udp	0.000330	# ISMA Easdaq Test
bcs-lmserver	1951/tcp	0.000000
bcs-lmserver	1951/udp	0.000000
mpnjsc	1952/tcp	0.000000
mpnjsc	1952/udp	0.000000
rapidbase	1953/tcp	0.000000	# Rapid Base
rapidbase	1953/udp	0.000000	# Rapid Base
abr-api	1954/tcp	0.000076	# ABR-API (diskbridge)
abr-api	1954/udp	0.000000	# ABR-API (diskbridge)
abr-secure	1955/tcp	0.000000	# ABR-Secure Data (diskbridge)
abr-secure	1955/udp	0.000000	# ABR-Secure Data (diskbridge)
vrtl-vmf-ds	1956/tcp	0.000000	# Vertel VMF DS
vrtl-vmf-ds	1956/udp	0.000000	# Vertel VMF DS
unix-status	1957/tcp	0.000000
unix-status	1957/udp	0.000330
dxadmind	1958/tcp	0.000076	# CA Administration Daemon
dxadmind	1958/udp	0.000330	# CA Administration Daemon
simp-all	1959/tcp	0.000000	# SIMP Channel
simp-all	1959/udp	0.000330	# SIMP Channel
nasmanager	1960/tcp	0.000000	# Merit DAC NASmanager
nasmanager	1960/udp	0.000000	# Merit DAC NASmanager
bts-appserver	1961/tcp	0.000000	# BTS APPSERVER
bts-appserver	1961/udp	0.000000	# BTS APPSERVER
biap-mp	1962/tcp	0.000000
biap-mp	1962/udp	0.000330
webmachine	1963/tcp	0.000000
webmachine	1963/udp	0.000000
solid-e-engine	1964/tcp	0.000000	# SOLID E ENGINE
solid-e-engine	1964/udp	0.000000	# SOLID E ENGINE
tivoli-npm	1965/tcp	0.000000	# Tivoli NPM
tivoli-npm	1965/udp	0.000000	# Tivoli NPM
slush	1966/tcp	0.000000
slush	1966/udp	0.000330
sns-quote	1967/tcp	0.000000	# SNS Quote
sns-quote	1967/udp	0.000000	# SNS Quote
lipsinc	1968/tcp	0.000000
lipsinc	1968/udp	0.000330
lipsinc1	1969/tcp	0.000000	# LIPSinc 1
lipsinc1	1969/udp	0.000000	# LIPSinc 1
netop-rc	1970/tcp	0.000000	# NetOp Remote Control
netop-rc	1970/udp	0.000000	# NetOp Remote Control
netop-school	1971/tcp	0.000152	# NetOp School
netop-school	1971/udp	0.000000	# NetOp School
intersys-cache	1972/tcp	0.000152	# Cache
intersys-cache	1972/udp	0.000000	# Cache
dlsrap	1973/tcp	0.000076	# Data Link Switching Remote Access Protocol
dlsrap	1973/udp	0.000000	# Data Link Switching Remote Access Protocol
drp	1974/tcp	0.000152
drp	1974/udp	0.000000
tcoflashagent	1975/tcp	0.000076	# TCO Flash Agent
tcoflashagent	1975/udp	0.000000	# TCO Flash Agent
tcoregagent	1976/tcp	0.000076	# TCO Reg Agent
tcoregagent	1976/udp	0.000000	# TCO Reg Agent
tcoaddressbook	1977/tcp	0.000000	# TCO Address Book
tcoaddressbook	1977/udp	0.000000	# TCO Address Book
unisql	1978/tcp	0.000000
unisql	1978/udp	0.000000
unisql-java	1979/tcp	0.000000	# UniSQL Java
unisql-java	1979/udp	0.000000	# UniSQL Java
pearldoc-xact	1980/tcp	0.000000	# PearlDoc XACT
pearldoc-xact	1980/udp	0.000000	# PearlDoc XACT
p2pq	1981/tcp	0.000076
p2pq	1981/udp	0.000330
estamp	1982/tcp	0.000000	# Evidentiary Timestamp
estamp	1982/udp	0.000000	# Evidentiary Timestamp
lhtp	1983/tcp	0.000000	# Loophole Test Protocol
lhtp	1983/udp	0.000000	# Loophole Test Protocol
bigbrother	1984/tcp	0.000201	# bb | Big Brother monitoring server - www.bb4.com | BB
bb	1984/udp	0.000330
hsrp	1985/tcp	0.000000	# Hot Standby Router Protocol
hsrp	1985/udp	0.000000	# Hot Standby Router Protocol
licensedaemon	1986/tcp	0.000025	# cisco license management
licensedaemon	1986/udp	0.000544	# cisco license management
tr-rsrb-p1	1987/tcp	0.000013	# cisco RSRB Priority 1 port
tr-rsrb-p1	1987/udp	0.000675	# cisco RSRB Priority 1 port
tr-rsrb-p2	1988/tcp	0.000050	# cisco RSRB Priority 2 port
tr-rsrb-p2	1988/udp	0.000428	# cisco RSRB Priority 2 port
tr-rsrb-p3	1989/tcp	0.000075	# mshnet | cisco RSRB Priority 3 port | MHSnet system
tr-rsrb-p3	1989/udp	0.000313	# cisco RSRB Priority 3 port
stun-p1	1990/tcp	0.000025	# cisco STUN Priority 1 port
stun-p1	1990/udp	0.000494	# cisco STUN Priority 1 port
stun-p2	1991/tcp	0.000050	# cisco STUN Priority 2 port
stun-p2	1991/udp	0.000428	# cisco STUN Priority 2 port
stun-p3	1992/tcp	0.000025	# ipsendmsg | cisco STUN Priority 3 port | IPsendmsg
stun-p3	1992/udp	0.000478	# cisco STUN Priority 3 port
snmp-tcp-port	1993/tcp	0.000013	# cisco SNMP TCP port
snmp-tcp-port	1993/udp	0.001779	# cisco SNMP TCP port
stun-port	1994/tcp	0.000025	# cisco serial tunnel port
stun-port	1994/udp	0.000313	# cisco serial tunnel port
perf-port	1995/tcp	0.000038	# cisco perf port
perf-port	1995/udp	0.000577	# cisco perf port
tr-rsrb-port	1996/tcp	0.000038	# cisco Remote SRB port
tr-rsrb-port	1996/udp	0.000626	# cisco Remote SRB port
gdp-port	1997/tcp	0.000038	# cisco Gateway Discovery Protocol
gdp-port	1997/udp	0.000494	# cisco Gateway Discovery Protocol
x25-svc-port	1998/tcp	0.001731	# cisco X.25 service (XOT)
x25-svc-port	1998/udp	0.000610	# cisco X.25 service (XOT)
tcp-id-port	1999/tcp	0.000364	# cisco identification port
tcp-id-port	1999/udp	0.000923	# cisco identification port
cisco-sccp	2000/tcp	0.010112	# cisco SCCP (Skinny Client Control Protocol) | Cisco SCCP | Cisco SCCp
cisco-sccp	2000/udp	0.011697	# cisco SCCP (Skinny Client Control Protocol)
dc	2001/tcp	0.007339	# wizard | or nfr20 web queries | curry
wizard	2001/udp	0.001186	# curry
globe	2002/tcp	0.001744
globe	2002/udp	0.003740
finger	2003/tcp	0.001179	# brutus | GNU finger (cfingerd) | Brutus Server
brutus	2003/udp	0.000000	# Brutus Server
mailbox	2004/tcp	0.001016	# emce | CCWS mm conf
emce	2004/udp	0.000988	# CCWS mm conf
deslogin	2005/tcp	0.001731	# oracle | berknet | encrypted symmetric telnet/login
oracle	2005/udp	0.000494
invokator	2006/tcp	0.001066	# raid-cd | raid
raid-cc	2006/udp	0.000675	# raid
dectalk	2007/tcp	0.000878	# raid-am
raid-am	2007/udp	0.000593
conf	2008/tcp	0.000903	# terminaldb
terminaldb	2008/udp	0.000593
news	2009/tcp	0.000841	# whosockami
whosockami	2009/udp	0.000511
search	2010/tcp	0.000803	# pipe_server | pipe-server | Or nfr411
pipe_server	2010/udp	0.000560	# Also used by NFR
raid-cc	2011/tcp	0.000113	# servserv | raid
servserv	2011/udp	0.000445
ttyinfo	2012/tcp	0.000151	# raid-ac
raid-ac	2012/udp	0.000873
raid-am	2013/tcp	0.000176	# raid-cd
raid-cd	2013/udp	0.000659
troff	2014/tcp	0.000050	# raid-sf
raid-sf	2014/udp	0.000478
cypress	2015/tcp	0.000038	# raid-cs
raid-cs	2015/udp	0.000362
bootserver	2016/tcp	0.000013
bootserver	2016/udp	0.000379
cypress-stat	2017/tcp	0.000000	# bootclient
bootclient	2017/udp	0.000346
terminaldb	2018/tcp	0.000050	# rellpack
rellpack	2018/udp	0.000972
whosockami	2019/tcp	0.000013	# about
about	2019/udp	0.000791
xinupageserver	2020/tcp	0.000364
xinupageserver	2020/udp	0.000577
servexec	2021/tcp	0.000289	# xinuexpansion1
xinuexpansion1	2021/udp	0.000478
down	2022/tcp	0.000226	# xinuexpansion2
xinuexpansion2	2022/udp	0.000593
xinuexpansion3	2023/tcp	0.000025
xinuexpansion3	2023/udp	0.000231
xinuexpansion4	2024/tcp	0.000050
xinuexpansion4	2024/udp	0.000511
ellpack	2025/tcp	0.000100	# xribs
xribs	2025/udp	0.000494
scrabble	2026/tcp	0.000038
scrabble	2026/udp	0.000824
shadowserver	2027/tcp	0.000025
shadowserver	2027/udp	0.000395
submitserver	2028/tcp	0.000013
submitserver	2028/udp	0.000445
hsrpv6	2029/tcp	0.000000	# Hot Standby Router Protocol IPv6
hsrpv6	2029/udp	0.000000	# Hot Standby Router Protocol IPv6
device2	2030/tcp	0.000514
device2	2030/udp	0.000412
mobrien-chat	2031/tcp	0.000076
mobrien-chat	2031/udp	0.000000
blackboard	2032/tcp	0.000000
blackboard	2032/udp	0.000840
glogger	2033/tcp	0.000339
glogger	2033/udp	0.000560
scoremgr	2034/tcp	0.000238
scoremgr	2034/udp	0.000544
imsldoc	2035/tcp	0.000188
imsldoc	2035/udp	0.000527
e-dpnet	2036/tcp	0.000000	# Ethernet WS DP network
e-dpnet	2036/udp	0.000330	# Ethernet WS DP network
applus	2037/tcp	0.000000	# APplus Application Server
applus	2037/udp	0.000000	# APplus Application Server
objectmanager	2038/tcp	0.000201
objectmanager	2038/udp	0.000626
prizma	2039/tcp	0.000000	# Prizma Monitoring Service
prizma	2039/udp	0.000000	# Prizma Monitoring Service
lam	2040/tcp	0.000276
lam	2040/udp	0.000725
interbase	2041/tcp	0.000213
interbase	2041/udp	0.000428
isis	2042/tcp	0.000163
isis	2042/udp	0.000379
isis-bcast	2043/tcp	0.000176
isis-bcast	2043/udp	0.000494
rimsl	2044/tcp	0.000138
rimsl	2044/udp	0.000560
cdfunc	2045/tcp	0.000163
cdfunc	2045/udp	0.000857
sdfunc	2046/tcp	0.000188
sdfunc	2046/udp	0.000511
dls	2047/tcp	0.000176
dls	2047/udp	0.000478
dls-monitor	2048/tcp	0.000263
dls-monitor	2048/udp	0.021549
nfs	2049/sctp	0.000000	# shilp | Network File System | Network File System - Sun Microsystems
nfs	2049/tcp	0.006110	# networked file system
nfs	2049/udp	0.044531	# networked file system
av-emb-config	2050/tcp	0.000000	# Avaya EMB Config Port
av-emb-config	2050/udp	0.000000	# Avaya EMB Config Port
epnsdp	2051/tcp	0.000000
epnsdp	2051/udp	0.002643
clearvisn	2052/tcp	0.000000	# clearVisn Services Port
clearvisn	2052/udp	0.000000	# clearVisn Services Port
knetd	2053/tcp	0.000025	# lot105-ds-upd | Lot105 DSuper Updates
lot105-ds-upd	2053/udp	0.000991	# Lot105 DSuper Updates
weblogin	2054/tcp	0.000000	# Weblogin Port
weblogin	2054/udp	0.000661	# Weblogin Port
iop	2055/tcp	0.000000	# Iliad-Odyssey Protocol
iop	2055/udp	0.000661	# Iliad-Odyssey Protocol
omnisky	2056/tcp	0.000000	# OmniSky Port
omnisky	2056/udp	0.000000	# OmniSky Port
rich-cp	2057/tcp	0.000000	# Rich Content Protocol
rich-cp	2057/udp	0.000000	# Rich Content Protocol
newwavesearch	2058/tcp	0.000000	# NewWaveSearchables RMI
newwavesearch	2058/udp	0.000661	# NewWaveSearchables RMI
bmc-messaging	2059/tcp	0.000000	# BMC Messaging Service
bmc-messaging	2059/udp	0.000330	# BMC Messaging Service
teleniumdaemon	2060/tcp	0.000000	# Telenium Daemon IF
teleniumdaemon	2060/udp	0.000661	# Telenium Daemon IF
netmount	2061/tcp	0.000000
netmount	2061/udp	0.000661
icg-swp	2062/tcp	0.000076	# ICG SWP Port
icg-swp	2062/udp	0.000661	# ICG SWP Port
icg-bridge	2063/tcp	0.000000	# ICG Bridge Port
icg-bridge	2063/udp	0.000000	# ICG Bridge Port
dnet-keyproxy	2064/tcp	0.000038	# icg-iprelay | A closed-source client for solving the RSA cryptographic challenge. This is the keyblock proxy port. | ICG IP Relay Port
icg-iprelay	2064/udp	0.000000	# ICG IP Relay Port
dlsrpn	2065/tcp	0.000815	# Data Link Switch Read Port Number
dlsrpn	2065/udp	0.000511	# Data Link Switch Read Port Number
aura	2066/tcp	0.000000	# AVM USB Remote Architecture
aura	2066/udp	0.000000	# AVM USB Remote Architecture
dlswpn	2067/tcp	0.000113	# Data Link Switch Write Port Number
dlswpn	2067/udp	0.001005	# Data Link Switch Write Port Number
avocentkvm	2068/tcp	0.000201	# avauthsrvprtcl | Avocent KVM Server | Avocent AuthSrv Protocol
avauthsrvprtcl	2068/udp	0.000000	# Avocent AuthSrv Protocol
event-port	2069/tcp	0.000076	# HTTP Event Port
event-port	2069/udp	0.000000	# HTTP Event Port
ah-esp-encap	2070/tcp	0.000076	# AH and ESP Encapsulated in UDP packet
ah-esp-encap	2070/udp	0.000330	# AH and ESP Encapsulated in UDP packet
acp-port	2071/tcp	0.000000	# Axon Control Protocol
acp-port	2071/udp	0.000000	# Axon Control Protocol
msync	2072/tcp	0.000000	# GlobeCast mSync
msync	2072/udp	0.000000	# GlobeCast mSync
gxs-data-port	2073/tcp	0.000000	# DataReel Database Socket
gxs-data-port	2073/udp	0.000000	# DataReel Database Socket
vrtl-vmf-sa	2074/tcp	0.000000	# Vertel VMF SA
vrtl-vmf-sa	2074/udp	0.000000	# Vertel VMF SA
newlixengine	2075/tcp	0.000000	# Newlix ServerWare Engine
newlixengine	2075/udp	0.000330	# Newlix ServerWare Engine
newlixconfig	2076/tcp	0.000000	# Newlix JSPConfig
newlixconfig	2076/udp	0.000330	# Newlix JSPConfig
tsrmagt	2077/tcp	0.000000	# Old Tivoli Storage Manager
tsrmagt	2077/udp	0.000330	# Old Tivoli Storage Manager
tpcsrvr	2078/tcp	0.000000	# IBM Total Productivity Center Server
tpcsrvr	2078/udp	0.000661	# IBM Total Productivity Center Server
idware-router	2079/tcp	0.000000	# IDWARE Router Port
idware-router	2079/udp	0.000000	# IDWARE Router Port
autodesk-nlm	2080/tcp	0.000076	# Autodesk NLM (FLEXlm)
autodesk-nlm	2080/udp	0.000330	# Autodesk NLM (FLEXlm)
kme-trap-port	2081/tcp	0.000076	# KME PRINTER TRAP PORT
kme-trap-port	2081/udp	0.000000	# KME PRINTER TRAP PORT
infowave	2082/tcp	0.000076	# Infowave Mobility Server
infowave	2082/udp	0.000330	# Infowave Mobiltiy Server
radsec	2083/tcp	0.000076	# Secure Radius Service
radsec	2083/udp	0.000661	# Secure Radius Service
sunclustergeo	2084/tcp	0.000000	# SunCluster Geographic
sunclustergeo	2084/udp	0.000000	# SunCluster Geographic
ada-cip	2085/tcp	0.000000	# ADA Control
ada-cip	2085/udp	0.000000	# ADA Control
gnunet	2086/tcp	0.000076
gnunet	2086/udp	0.000330
eli	2087/tcp	0.000076	# ELI - Event Logging Integration
eli	2087/udp	0.000000	# ELI - Event Logging Integration
ip-blf	2088/tcp	0.000000	# IP Busy Lamp Field
ip-blf	2088/udp	0.000000	# IP Busy Lamp Field
sep	2089/tcp	0.000000	# Security Encapsulation Protocol - SEP
sep	2089/udp	0.000000	# Security Encapsulation Protocol - SEP
lrp	2090/tcp	0.000000	# Load Report Protocol
lrp	2090/udp	0.000000	# Load Report Protocol
prp	2091/tcp	0.000000
prp	2091/udp	0.000000
descent3	2092/tcp	0.000000	# Descent 3
descent3	2092/udp	0.000000	# Descent 3
nbx-cc	2093/tcp	0.000000	# NBX CC
nbx-cc	2093/udp	0.000330	# NBX CC
nbx-au	2094/tcp	0.000000	# NBX AU
nbx-au	2094/udp	0.000000	# NBX AU
nbx-ser	2095/tcp	0.000076	# NBX SER
nbx-ser	2095/udp	0.000000	# NBX SER
nbx-dir	2096/tcp	0.000076	# NBX DIR
nbx-dir	2096/udp	0.000000	# NBX DIR
jetformpreview	2097/tcp	0.000000	# Jet Form Preview
jetformpreview	2097/udp	0.000000	# Jet Form Preview
dialog-port	2098/tcp	0.000000	# Dialog Port
dialog-port	2098/udp	0.000000	# Dialog Port
h2250-annex-g	2099/tcp	0.000152	# H.225.0 Annex G | H.225.0 Annex G Signalling
h2250-annex-g	2099/udp	0.000000	# H.225.0 Annex G
amiganetfs	2100/tcp	0.000380	# Amiga Network Filesystem
amiganetfs	2100/udp	0.000000	# Amiga Network Filesystem
rtcm-sc104	2101/tcp	0.000076
rtcm-sc104	2101/udp	0.000991
zephyr-srv	2102/tcp	0.000000	# Zephyr server
zephyr-srv	2102/udp	0.000330	# Zephyr server
zephyr-clt	2103/tcp	0.002661	# Zephyr serv-hm connection
zephyr-clt	2103/udp	0.000758	# Zephyr serv-hm connection
zephyr-hm	2104/tcp	0.000076	# Zephyr hostmanager
zephyr-hm	2104/udp	0.000478	# Zephyr hostmanager
eklogin	2105/tcp	0.002120	# minipay | Kerberos (v4) encrypted rlogin | MiniPay
eklogin	2105/udp	0.000544	# Kerberos (v4) encrypted rlogin
ekshell	2106/tcp	0.000238	# mzap | Kerberos (v4) encrypted rshell | MZAP
ekshell	2106/udp	0.000972	# Kerberos (v4) encrypted rshell
msmq-mgmt	2107/tcp	0.002737	# bintec-admin | Microsoft Message Queuing (IANA calls this bintec-admin) | BinTec Admin
bintec-admin	2107/udp	0.000000	# BinTec Admin
rkinit	2108/tcp	0.000013	# comcam | Kerberos (v4) remote initialization | Comcam
rkinit	2108/udp	0.000593	# Kerberos (v4) remote initialization
ergolight	2109/tcp	0.000000
ergolight	2109/udp	0.000000
umsp	2110/tcp	0.000000
umsp	2110/udp	0.000000
kx	2111/tcp	0.000263	# dsatp | X over kerberos | OPNET Dynamic Sampling Agent Transaction Protocol
dsatp	2111/udp	0.000330
kip	2112/tcp	0.000088	# idonix-metanet | IP over kerberos | Idonix MetaNet
idonix-metanet	2112/udp	0.000000	# Idonix MetaNet
hsl-storm	2113/tcp	0.000000	# HSL StoRM
hsl-storm	2113/udp	0.000000	# HSL StoRM
newheights	2114/tcp	0.000000	# ariascribe | Classical Music Meta-Data Access and Enhancement
newheights	2114/udp	0.000000
kdm	2115/tcp	0.000076	# Key Distribution Manager
kdm	2115/udp	0.000000	# Key Distribution Manager
ccowcmr	2116/tcp	0.000000
ccowcmr	2116/udp	0.000000
mentaclient	2117/tcp	0.000000
mentaclient	2117/udp	0.000000
mentaserver	2118/tcp	0.000000
mentaserver	2118/udp	0.000000
gsigatekeeper	2119/tcp	0.000380
gsigatekeeper	2119/udp	0.000330
kauth	2120/tcp	0.000050	# qencp | Remote kauth | Quick Eagle Networks CP
qencp	2120/udp	0.000000	# Quick Eagle Networks CP
ccproxy-ftp	2121/tcp	0.005834	# scientia-ssdb | CCProxy FTP Proxy | SCIENTIA-SSDB
scientia-ssdb	2121/udp	0.000661
caupc-remote	2122/tcp	0.000000	# CauPC Remote Control
caupc-remote	2122/udp	0.000000	# CauPC Remote Control
gtp-control	2123/tcp	0.000000	# GTP-Control Plane (3GPP)
gtp-control	2123/udp	0.000661	# GTP-Control Plane (3GPP)
elatelink	2124/tcp	0.000076
elatelink	2124/udp	0.000000
lockstep	2125/tcp	0.000000
lockstep	2125/udp	0.000000
pktcable-cops	2126/tcp	0.000304
pktcable-cops	2126/udp	0.000330
index-pc-wb	2127/tcp	0.000000
index-pc-wb	2127/udp	0.000330
net-steward	2128/tcp	0.000000	# Net Steward Control
net-steward	2128/udp	0.000000	# Net Steward Control
cs-live	2129/tcp	0.000000	# cs-live.com
cs-live	2129/udp	0.000661	# cs-live.com
xds	2130/tcp	0.000000
xds	2130/udp	0.000000
avantageb2b	2131/tcp	0.000000
avantageb2b	2131/udp	0.000330
solera-epmap	2132/tcp	0.000000	# SoleraTec End Point Map
solera-epmap	2132/udp	0.000000	# SoleraTec End Point Map
zymed-zpp	2133/tcp	0.000000
zymed-zpp	2133/udp	0.000000
avenue	2134/tcp	0.000076
avenue	2134/udp	0.000000
gris	2135/tcp	0.000380	# Grid Resource Information Server
gris	2135/udp	0.000000	# Grid Resource Information Server
appworxsrv	2136/tcp	0.000000
appworxsrv	2136/udp	0.000330
connect	2137/tcp	0.000000
connect	2137/udp	0.000000
unbind-cluster	2138/tcp	0.000000
unbind-cluster	2138/udp	0.000330
ias-auth	2139/tcp	0.000000
ias-auth	2139/udp	0.000000
ias-reg	2140/tcp	0.000000
ias-reg	2140/udp	0.000661
ias-admind	2141/tcp	0.000000
ias-admind	2141/udp	0.000000
tdmoip	2142/tcp	0.000076	# TDM OVER IP
tdmoip	2142/udp	0.000000	# TDM OVER IP
lv-jc	2143/tcp	0.000000	# Live Vault Job Control
lv-jc	2143/udp	0.000000	# Live Vault Job Control
lv-ffx	2144/tcp	0.000380	# Live Vault Fast Object Transfer
lv-ffx	2144/udp	0.000330	# Live Vault Fast Object Transfer
lv-pici	2145/tcp	0.000000	# Live Vault Remote Diagnostic Console Support
lv-pici	2145/udp	0.000000	# Live Vault Remote Diagnostic Console Support
lv-not	2146/tcp	0.000000	# Live Vault Admin Event Notification
lv-not	2146/udp	0.000000	# Live Vault Admin Event Notification
lv-auth	2147/tcp	0.000000	# Live Vault Authentication
lv-auth	2147/udp	0.000000	# Live Vault Authentication
veritas-ucl	2148/tcp	0.000076	# Veritas Universal Communication Layer | VERITAS UNIVERSAL COMMUNICATION LAYER
veritas-ucl	2148/udp	0.005946	# Veritas Universal Communication Layer
acptsys	2149/tcp	0.000000
acptsys	2149/udp	0.000000
dynamic3d	2150/tcp	0.000076
dynamic3d	2150/udp	0.000000
docent	2151/tcp	0.000000
docent	2151/udp	0.000000
gtp-user	2152/tcp	0.000000	# GTP-User Plane (3GPP)
gtp-user	2152/udp	0.000000	# GTP-User Plane (3GPP)
ctlptc	2153/tcp	0.000000	# Control Protocol
ctlptc	2153/udp	0.000000	# Control Protocol
stdptc	2154/tcp	0.000000	# Standard Protocol
stdptc	2154/udp	0.000000	# Standard Protocol
brdptc	2155/tcp	0.000000	# Bridge Protocol
brdptc	2155/udp	0.000000	# Bridge Protocol
trp	2156/tcp	0.000000	# Talari Reliable Protocol
trp	2156/udp	0.000000	# Talari Reliable Protocol
xnds	2157/tcp	0.000000	# Xerox Network Document Scan Protocol
xnds	2157/udp	0.000000	# Xerox Network Document Scan Protocol
touchnetplus	2158/tcp	0.000000	# TouchNetPlus Service
touchnetplus	2158/udp	0.000661	# TouchNetPlus Service
gdbremote	2159/tcp	0.000000	# GDB Remote Debug Port
gdbremote	2159/udp	0.000000	# GDB Remote Debug Port
apc-2160	2160/tcp	0.000380	# APC 2160
apc-2160	2160/udp	0.001982	# APC 2160
apc-agent	2161/tcp	0.001521	# apc-2161 | American Power Conversion | APC 2161
apc-2161	2161/udp	0.001321	# APC 2161
navisphere	2162/tcp	0.000000
navisphere	2162/udp	0.000330
navisphere-sec	2163/tcp	0.000000	# Navisphere Secure
navisphere-sec	2163/udp	0.000000	# Navisphere Secure
ddns-v3	2164/tcp	0.000000	# Dynamic DNS Version 3
ddns-v3	2164/udp	0.000991	# Dynamic DNS Version 3
x-bone-api	2165/tcp	0.000000	# X-Bone API
x-bone-api	2165/udp	0.000000	# X-Bone API
iwserver	2166/tcp	0.000000
iwserver	2166/udp	0.000000
raw-serial	2167/tcp	0.000000	# Raw Async Serial Link
raw-serial	2167/udp	0.000000	# Raw Async Serial Link
easy-soft-mux	2168/tcp	0.000000	# easy-soft Multiplexer
easy-soft-mux	2168/udp	0.000661	# easy-soft Multiplexer
brain	2169/tcp	0.000000	# Backbone for Academic Information Notification (BRAIN)
brain	2169/udp	0.000330	# Backbone for Academic Information Notification (BRAIN)
eyetv	2170/tcp	0.000152	# EyeTV Server Port
eyetv	2170/udp	0.000330	# EyeTV Server Port
msfw-storage	2171/tcp	0.000000	# MS Firewall Storage
msfw-storage	2171/udp	0.000000	# MS Firewall Storage
msfw-s-storage	2172/tcp	0.000000	# MS Firewall SecureStorage
msfw-s-storage	2172/udp	0.000000	# MS Firewall SecureStorage
msfw-replica	2173/tcp	0.000000	# MS Firewall Replication
msfw-replica	2173/udp	0.000000	# MS Firewall Replication
msfw-array	2174/tcp	0.000000	# MS Firewall Intra Array
msfw-array	2174/udp	0.000000	# MS Firewall Intra Array
airsync	2175/tcp	0.000000	# Microsoft Desktop AirSync Protocol
airsync	2175/udp	0.000000	# Microsoft Desktop AirSync Protocol
rapi	2176/tcp	0.000000	# Microsoft ActiveSync Remote API
rapi	2176/udp	0.000000	# Microsoft ActiveSync Remote API
qwave	2177/tcp	0.000000	# qWAVE Bandwidth Estimate
qwave	2177/udp	0.000000	# qWAVE Bandwidth Estimate
bitspeer	2178/tcp	0.000000	# Peer Services for BITS
bitspeer	2178/udp	0.000000	# Peer Services for BITS
vmrdp	2179/tcp	0.000304	# Microsoft RDP for virtual machines
vmrdp	2179/udp	0.000000	# Microsoft RDP for virtual machines
mc-gt-srv	2180/tcp	0.000000	# Millicent Vendor Gateway Server
mc-gt-srv	2180/udp	0.000000	# Millicent Vendor Gateway Server
eforward	2181/tcp	0.000000
eforward	2181/udp	0.000000
cgn-stat	2182/tcp	0.000000	# CGN status
cgn-stat	2182/udp	0.000330	# CGN status
cgn-config	2183/tcp	0.000000	# Code Green configuration
cgn-config	2183/udp	0.000000	# Code Green configuration
nvd	2184/tcp	0.000000	# NVD User
nvd	2184/udp	0.000000	# NVD User
onbase-dds	2185/tcp	0.000000	# OnBase Distributed Disk Services
onbase-dds	2185/udp	0.000330	# OnBase Distributed Disk Services
gtaua	2186/tcp	0.000000	# Guy-Tek Automated Update Applications
gtaua	2186/udp	0.000000	# Guy-Tek Automated Update Applications
ssmc	2187/tcp	0.000076	# ssmd | Sepehr System Management Control | Sepehr System Management Data
ssmd	2187/udp	0.000000	# Sepehr System Management Data
radware-rpm	2188/tcp	0.000000	# Radware Resource Pool Manager
radware-rpm-s	2189/tcp	0.000000	# Secure Radware Resource Pool Manager
tivoconnect	2190/tcp	0.000380	# TiVoConnect Beacon
tivoconnect	2190/udp	0.000000	# TiVoConnect Beacon
tvbus	2191/tcp	0.000304	# TvBus Messaging
tvbus	2191/udp	0.000330	# TvBus Messaging
asdis	2192/tcp	0.000000	# ASDIS software management
asdis	2192/udp	0.000000	# ASDIS software management
drwcs	2193/tcp	0.000000	# Dr.Web Enterprise Management Service
drwcs	2193/udp	0.000000	# Dr.Web Enterprise Management Service
unknown	2196/tcp	0.000152
mnp-exchange	2197/tcp	0.000076	# MNP data exchange
mnp-exchange	2197/udp	0.000000	# MNP data exchange
onehome-remote	2198/tcp	0.000000	# OneHome Remote Access
onehome-remote	2198/udp	0.000000	# OneHome Remote Access
onehome-help	2199/tcp	0.000000	# OneHome Service Port
onehome-help	2199/udp	0.000000	# OneHome Service Port
ici	2200/tcp	0.000152
ici	2200/udp	0.000330
ats	2201/tcp	0.000100	# Advanced Training System Program
ats	2201/udp	0.000577	# Advanced Training System Program
imtc-map	2202/tcp	0.000000	# Int. Multimedia Teleconferencing Cosortium
imtc-map	2202/udp	0.000000	# Int. Multimedia Teleconferencing Cosortium
b2-runtime	2203/tcp	0.000076	# b2 Runtime Protocol
b2-runtime	2203/udp	0.000000	# b2 Runtime Protocol
b2-license	2204/tcp	0.000000	# b2 License Server
b2-license	2204/udp	0.000000	# b2 License Server
jps	2205/tcp	0.000000	# Java Presentation Server
jps	2205/udp	0.000000	# Java Presentation Server
hpocbus	2206/tcp	0.000000	# HP OpenCall bus
hpocbus	2206/udp	0.000000	# HP OpenCall bus
hpssd	2207/tcp	0.000000	# HP Status and Services
hpssd	2207/udp	0.000000	# HP Status and Services
hpiod	2208/tcp	0.000000	# HP I/O Backend
hpiod	2208/udp	0.000000	# HP I/O Backend
rimf-ps	2209/tcp	0.000000	# HP RIM for Files Portal Service
rimf-ps	2209/udp	0.000000	# HP RIM for Files Portal Service
noaaport	2210/tcp	0.000000	# NOAAPORT Broadcast Network
noaaport	2210/udp	0.000000	# NOAAPORT Broadcast Network
emwin	2211/tcp	0.000000
emwin	2211/udp	0.000000
leecoposserver	2212/tcp	0.000000	# LeeCO POS Server Service
leecoposserver	2212/udp	0.000000	# LeeCO POS Server Service
kali	2213/tcp	0.000000
kali	2213/udp	0.000000
rpi	2214/tcp	0.000000	# RDQ Protocol Interface
rpi	2214/udp	0.000330	# RDQ Protocol Interface
ipcore	2215/tcp	0.000000	# IPCore.co.za GPRS
ipcore	2215/udp	0.000661	# IPCore.co.za GPRS
vtu-comms	2216/tcp	0.000000	# VTU data service
vtu-comms	2216/udp	0.000000	# VTU data service
gotodevice	2217/tcp	0.000000	# GoToDevice Device Management
gotodevice	2217/udp	0.000330	# GoToDevice Device Management
bounzza	2218/tcp	0.000000	# Bounzza IRC Proxy
bounzza	2218/udp	0.000000	# Bounzza IRC Proxy
netiq-ncap	2219/tcp	0.000000	# NetIQ NCAP Protocol
netiq-ncap	2219/udp	0.000000	# NetIQ NCAP Protocol
netiq	2220/tcp	0.000000	# NetIQ End2End
netiq	2220/udp	0.000000	# NetIQ End2End
rockwell-csp1	2221/tcp	0.000000	# ethernet-ip-s | Rockwell CSP1 | EtherNet/IP over TLS | EtherNet/IP over DTLS
rockwell-csp1	2221/udp	0.000330	# Rockwell CSP1
EtherNetIP-1	2222/tcp	0.000608	# EtherNet/IP-1 | EtherNet-IP-1 | EtherNet/IP I/O
msantipiracy	2222/udp	0.047902	# Microsoft Office OS X antipiracy network monitor
rockwell-csp2	2223/tcp	0.000000	# Rockwell CSP2
rockwell-csp2	2223/udp	0.010902	# Rockwell CSP2
efi-mg	2224/tcp	0.000076	# Easy Flexible Internet/Multiplayer Games
efi-mg	2224/udp	0.000000	# Easy Flexible Internet/Multiplayer Games
rcip-itu	2225/sctp	0.000000	# Resource Connection Initiation Protocol
rcip-itu	2225/tcp	0.000000	# Resource Connection Initiation Protocol
rcip-itu	2225/udp	0.000000	# Resource Connection Initiation Protocol
di-drm	2226/tcp	0.000000	# Digital Instinct DRM
di-drm	2226/udp	0.000330	# Digital Instinct DRM
di-msg	2227/tcp	0.000000	# DI Messaging Service
di-msg	2227/udp	0.000000	# DI Messaging Service
ehome-ms	2228/tcp	0.000000	# eHome Message Server
ehome-ms	2228/udp	0.000000	# eHome Message Server
datalens	2229/tcp	0.000000	# DataLens Service
datalens	2229/udp	0.000000	# DataLens Service
queueadm	2230/tcp	0.000000	# MetaSoft Job Queue Administration Service
queueadm	2230/udp	0.000000	# MetaSoft Job Queue Administration Service
wimaxasncp	2231/tcp	0.000000	# WiMAX ASN Control Plane Protocol
wimaxasncp	2231/udp	0.000000	# WiMAX ASN Control Plane Protocol
ivs-video	2232/tcp	0.000151	# IVS Video default
ivs-video	2232/udp	0.000626	# IVS Video default
infocrypt	2233/tcp	0.000000
infocrypt	2233/udp	0.000000
directplay	2234/tcp	0.000000
directplay	2234/udp	0.000000
sercomm-wlink	2235/tcp	0.000000
sercomm-wlink	2235/udp	0.000000
nani	2236/tcp	0.000000
nani	2236/udp	0.000000
optech-port1-lm	2237/tcp	0.000000	# Optech Port1 License Manager
optech-port1-lm	2237/udp	0.000330	# Optech Port1 License Manager
aviva-sna	2238/tcp	0.000000	# AVIVA SNA SERVER
aviva-sna	2238/udp	0.000000	# AVIVA SNA SERVER
imagequery	2239/tcp	0.000000	# Image Query
imagequery	2239/udp	0.000330	# Image Query
recipe	2240/tcp	0.000000
recipe	2240/udp	0.000330
ivsd	2241/tcp	0.000151	# IVS Daemon
ivsd	2241/udp	0.000659	# IVS Daemon
foliocorp	2242/tcp	0.000000	# Folio Remote Server
foliocorp	2242/udp	0.000000	# Folio Remote Server
magicom	2243/tcp	0.000000	# Magicom Protocol
magicom	2243/udp	0.000000	# Magicom Protocol
nmsserver	2244/tcp	0.000000	# NMS Server
nmsserver	2244/udp	0.000330	# NMS Server
hao	2245/tcp	0.000000
hao	2245/udp	0.000330
pc-mta-addrmap	2246/tcp	0.000000	# PacketCable MTA Addr Map
pc-mta-addrmap	2246/udp	0.000330	# PacketCable MTA Addr Map
antidotemgrsvr	2247/tcp	0.000000	# Antidote Deployment Manager Service
antidotemgrsvr	2247/udp	0.000330	# Antidote Deployment Manager Service
ums	2248/tcp	0.000000	# User Management Service
ums	2248/udp	0.000000	# User Management Service
rfmp	2249/tcp	0.000000	# RISO File Manager Protocol
rfmp	2249/udp	0.000330	# RISO File Manager Protocol
remote-collab	2250/tcp	0.000076
remote-collab	2250/udp	0.000000
dif-port	2251/tcp	0.000304	# Distributed Framework Port
dif-port	2251/udp	0.000330	# Distributed Framework Port
njenet-ssl	2252/tcp	0.000000	# NJENET using SSL
njenet-ssl	2252/udp	0.000000	# NJENET using SSL
dtv-chan-req	2253/tcp	0.000076	# DTV Channel Request
dtv-chan-req	2253/udp	0.000000	# DTV Channel Request
seispoc	2254/tcp	0.000000	# Seismic P.O.C. Port
seispoc	2254/udp	0.000000	# Seismic P.O.C. Port
vrtp	2255/tcp	0.000000	# VRTP - ViRtue Transfer Protocol
vrtp	2255/udp	0.000000	# VRTP - ViRtue Transfer Protocol
pcc-mfp	2256/tcp	0.000000	# PCC MFP
pcc-mfp	2256/udp	0.000000	# PCC MFP
simple-tx-rx	2257/tcp	0.000000	# simple text/file transfer
simple-tx-rx	2257/udp	0.000000	# simple text/file transfer
rcts	2258/tcp	0.000000	# Rotorcraft Communications Test System
rcts	2258/udp	0.000330	# Rotorcraft Communications Test System
acd-pm	2259/tcp	0.000000	# bid-serv | Accedian Performance Measurement | BIF identifiers resolution service
acd-pm	2259/udp	0.000000	# Accedian Performance Measurement
apc-2260	2260/tcp	0.000380	# APC 2260
apc-2260	2260/udp	0.000000	# APC 2260
comotionmaster	2261/tcp	0.000076	# CoMotion Master Server
comotionmaster	2261/udp	0.000000	# CoMotion Master Server
comotionback	2262/tcp	0.000076	# CoMotion Backup Server
comotionback	2262/udp	0.000330	# CoMotion Backup Server
ecwcfg	2263/tcp	0.000000	# ECweb Configuration Service
ecwcfg	2263/udp	0.000000	# ECweb Configuration Service
apx500api-1	2264/tcp	0.000000	# Audio Precision Apx500 API Port 1
apx500api-1	2264/udp	0.000330	# Audio Precision Apx500 API Port 1
apx500api-2	2265/tcp	0.000076	# Audio Precision Apx500 API Port 2
apx500api-2	2265/udp	0.000330	# Audio Precision Apx500 API Port 2
mfserver	2266/tcp	0.000000	# M-Files Server | M-files Server
mfserver	2266/udp	0.000330	# M-files Server
ontobroker	2267/tcp	0.000000
ontobroker	2267/udp	0.000000
amt	2268/tcp	0.000000
amt	2268/udp	0.000000
mikey	2269/tcp	0.000076
mikey	2269/udp	0.000330
starschool	2270/tcp	0.000076
starschool	2270/udp	0.000330
mmcals	2271/tcp	0.000076	# Secure Meeting Maker Scheduling
mmcals	2271/udp	0.000000	# Secure Meeting Maker Scheduling
mmcal	2272/tcp	0.000000	# Meeting Maker Scheduling
mmcal	2272/udp	0.000000	# Meeting Maker Scheduling
mysql-im	2273/tcp	0.000000	# MySQL Instance Manager
mysql-im	2273/udp	0.000330	# MySQL Instance Manager
pcttunnell	2274/tcp	0.000000	# PCTTunneller
pcttunnell	2274/udp	0.000000	# PCTTunneller
ibridge-data	2275/tcp	0.000000	# iBridge Conferencing
ibridge-data	2275/udp	0.000000	# iBridge Conferencing
ibridge-mgmt	2276/tcp	0.000000	# iBridge Management
ibridge-mgmt	2276/udp	0.000000	# iBridge Management
bluectrlproxy	2277/tcp	0.000000	# Bt device control proxy
bluectrlproxy	2277/udp	0.000000	# Bt device control proxy
s3db	2278/tcp	0.000000	# Simple Stacked Sequences Database
s3db	2278/udp	0.000000	# Simple Stacked Sequences Database
xmquery	2279/tcp	0.000000
xmquery	2279/udp	0.000330
lnvpoller	2280/tcp	0.000076
lnvpoller	2280/udp	0.000000
lnvconsole	2281/tcp	0.000000
lnvconsole	2281/udp	0.000000
lnvalarm	2282/tcp	0.000000
lnvalarm	2282/udp	0.000000
lnvstatus	2283/tcp	0.000000
lnvstatus	2283/udp	0.000330
lnvmaps	2284/tcp	0.000000
lnvmaps	2284/udp	0.000000
lnvmailmon	2285/tcp	0.000000
lnvmailmon	2285/udp	0.000000
nas-metering	2286/tcp	0.000000
nas-metering	2286/udp	0.000000
dna	2287/tcp	0.000000
dna	2287/udp	0.000000
netml	2288/tcp	0.000152
netml	2288/udp	0.000000
dict-lookup	2289/tcp	0.000000	# Lookup dict server
dict-lookup	2289/udp	0.000000	# Lookup dict server
sonus-logging	2290/tcp	0.000000	# Sonus Logging Services
sonus-logging	2290/udp	0.000000	# Sonus Logging Services
eapsp	2291/tcp	0.000076	# EPSON Advanced Printer Share Protocol
eapsp	2291/udp	0.000000	# EPSON Advanced Printer Share Protocol
mib-streaming	2292/tcp	0.000076	# Sonus Element Management Services
mib-streaming	2292/udp	0.000330	# Sonus Element Management Services
npdbgmngr	2293/tcp	0.000000	# Network Platform Debug Manager
npdbgmngr	2293/udp	0.000000	# Network Platform Debug Manager
konshus-lm	2294/tcp	0.000000	# Konshus License Manager (FLEX)
konshus-lm	2294/udp	0.000000	# Konshus License Manager (FLEX)
advant-lm	2295/tcp	0.000000	# Advant License Manager
advant-lm	2295/udp	0.000000	# Advant License Manager
theta-lm	2296/tcp	0.000000	# Theta License Manager (Rainbow)
theta-lm	2296/udp	0.000000	# Theta License Manager (Rainbow)
d2k-datamover1	2297/tcp	0.000000	# D2K DataMover 1
d2k-datamover1	2297/udp	0.000000	# D2K DataMover 1
d2k-datamover2	2298/tcp	0.000000	# D2K DataMover 2
d2k-datamover2	2298/udp	0.000000	# D2K DataMover 2
pc-telecommute	2299/tcp	0.000000	# PC Telecommute
pc-telecommute	2299/udp	0.000000	# PC Telecommute
cvmmon	2300/tcp	0.000076
cvmmon	2300/udp	0.000000
compaqdiag	2301/tcp	0.001242	# cpq-wbem | Compaq remote diagnostic/management | Compaq HTTP
cpq-wbem	2301/udp	0.000330	# Compaq HTTP
binderysupport	2302/tcp	0.000076	# Bindery Support
binderysupport	2302/udp	0.000661	# Bindery Support
proxy-gateway	2303/tcp	0.000000	# Proxy Gateway
proxy-gateway	2303/udp	0.000000	# Proxy Gateway
attachmate-uts	2304/tcp	0.000076	# Attachmate UTS
attachmate-uts	2304/udp	0.000000	# Attachmate UTS
mt-scaleserver	2305/tcp	0.000000	# MT ScaleServer
mt-scaleserver	2305/udp	0.000000	# MT ScaleServer
tappi-boxnet	2306/tcp	0.000000	# TAPPI BoxNet
tappi-boxnet	2306/udp	0.000000	# TAPPI BoxNet
pehelp	2307/tcp	0.000050
pehelp	2307/udp	0.000659
sdhelp	2308/tcp	0.000000
sdhelp	2308/udp	0.000000
sdserver	2309/tcp	0.000000	# SD Server
sdserver	2309/udp	0.000000	# SD Server
sdclient	2310/tcp	0.000000	# SD Client
sdclient	2310/udp	0.000000	# SD Client
messageservice	2311/tcp	0.000000	# Message Service
messageservice	2311/udp	0.000000	# Message Service
wanscaler	2312/tcp	0.000076	# WANScaler Communication Service
wanscaler	2312/udp	0.000000	# WANScaler Communication Service
iapp	2313/tcp	0.000076	# IAPP (Inter Access Point Protocol)
iapp	2313/udp	0.000000	# IAPP (Inter Access Point Protocol)
cr-websystems	2314/tcp	0.000000	# CR WebSystems
cr-websystems	2314/udp	0.000000	# CR WebSystems
precise-sft	2315/tcp	0.000000	# Precise Sft.
precise-sft	2315/udp	0.000000	# Precise Sft.
sent-lm	2316/tcp	0.000000	# SENT License Manager
sent-lm	2316/udp	0.000000	# SENT License Manager
attachmate-g32	2317/tcp	0.000000	# Attachmate G32
attachmate-g32	2317/udp	0.000330	# Attachmate G32
cadencecontrol	2318/tcp	0.000000	# Cadence Control
cadencecontrol	2318/udp	0.000000	# Cadence Control
infolibria	2319/tcp	0.000000
infolibria	2319/udp	0.000330
siebel-ns	2320/tcp	0.000000	# Siebel NS
siebel-ns	2320/udp	0.000330	# Siebel NS
rdlap	2321/tcp	0.000000
rdlap	2321/udp	0.000000
ofsd	2322/tcp	0.000000
ofsd	2322/udp	0.000000
3d-nfsd	2323/tcp	0.000228
3d-nfsd	2323/udp	0.000000
cosmocall	2324/tcp	0.000000
cosmocall	2324/udp	0.000330
ansysli	2325/tcp	0.000076	# ANSYS Licensing Interconnect
ansysli	2325/udp	0.000000	# ANSYS Licensing Interconnect
idcp	2326/tcp	0.000076
idcp	2326/udp	0.000330
xingcsm	2327/tcp	0.000000
xingcsm	2327/udp	0.000330
netrix-sftm	2328/tcp	0.000000	# Netrix SFTM
netrix-sftm	2328/udp	0.000330	# Netrix SFTM
nvd	2329/tcp	0.000000
nvd	2329/udp	0.000000
tscchat	2330/tcp	0.000076
tscchat	2330/udp	0.000330
agentview	2331/tcp	0.000000
agentview	2331/udp	0.000000
rcc-host	2332/tcp	0.000000	# RCC Host
rcc-host	2332/udp	0.000330	# RCC Host
snapp	2333/tcp	0.000000
snapp	2333/udp	0.000000
ace-client	2334/tcp	0.000000	# ACE Client Auth
ace-client	2334/udp	0.000330	# ACE Client Auth
ace-proxy	2335/tcp	0.000076	# ACE Proxy
ace-proxy	2335/udp	0.000330	# ACE Proxy
appleugcontrol	2336/tcp	0.000000	# Apple UG Control
appleugcontrol	2336/udp	0.000000	# Apple UG Control
ideesrv	2337/tcp	0.000000
ideesrv	2337/udp	0.000000
norton-lambert	2338/tcp	0.000000	# Norton Lambert
norton-lambert	2338/udp	0.000000	# Norton Lambert
3com-webview	2339/tcp	0.000000	# 3Com WebView
3com-webview	2339/udp	0.000000	# 3Com WebView
wrs_registry	2340/tcp	0.000076	# wrs-registry | WRS Registry
wrs_registry	2340/udp	0.000330	# WRS Registry
xiostatus	2341/tcp	0.000000	# XIO Status
xiostatus	2341/udp	0.000000	# XIO Status
manage-exec	2342/tcp	0.000000	# Seagate Manage Exec
manage-exec	2342/udp	0.000330	# Seagate Manage Exec
nati-logos	2343/tcp	0.000000	# nati logos
nati-logos	2343/udp	0.001652	# nati logos
fcmsys	2344/tcp	0.000000
fcmsys	2344/udp	0.000000
dbm	2345/tcp	0.000000
dbm	2345/udp	0.001321
redstorm_join	2346/tcp	0.000000	# redstorm-join | Game Connection Port
redstorm_join	2346/udp	0.000000	# Game Connection Port
redstorm_find	2347/tcp	0.000000	# redstorm-find | Game Announcement and Location
redstorm_find	2347/udp	0.000000	# Game Announcement and Location
redstorm_info	2348/tcp	0.000000	# redstorm-info | Information to query for game status
redstorm_info	2348/udp	0.000000	# Information to query for game status
redstorm_diag	2349/tcp	0.000000	# redstorm-diag | Diagnostics Port
redstorm_diag	2349/udp	0.000000	# Diagnostics Port
psbserver	2350/tcp	0.000000	# Pharos Booking Server
psbserver	2350/udp	0.000000	# Pharos Booking Server
psrserver	2351/tcp	0.000000
psrserver	2351/udp	0.000000
pslserver	2352/tcp	0.000000
pslserver	2352/udp	0.000330
pspserver	2353/tcp	0.000000
pspserver	2353/udp	0.000000
psprserver	2354/tcp	0.000000
psprserver	2354/udp	0.000000
psdbserver	2355/tcp	0.000000
psdbserver	2355/udp	0.000000
gxtelmd	2356/tcp	0.000000	# GXT License Managemant
gxtelmd	2356/udp	0.000000	# GXT License Managemant
unihub-server	2357/tcp	0.000000	# UniHub Server
unihub-server	2357/udp	0.000000	# UniHub Server
futrix	2358/tcp	0.000000
futrix	2358/udp	0.000000
flukeserver	2359/tcp	0.000000
flukeserver	2359/udp	0.000000
nexstorindltd	2360/tcp	0.000000
nexstorindltd	2360/udp	0.000330
tl1	2361/tcp	0.000000
tl1	2361/udp	0.000000
digiman	2362/tcp	0.000000
digiman	2362/udp	0.001321
mediacntrlnfsd	2363/tcp	0.000000	# Media Central NFSD
mediacntrlnfsd	2363/udp	0.000000	# Media Central NFSD
oi-2000	2364/tcp	0.000000
oi-2000	2364/udp	0.000330
dbref	2365/tcp	0.000000
dbref	2365/udp	0.000000
qip-login	2366/tcp	0.000152
qip-login	2366/udp	0.000000
service-ctrl	2367/tcp	0.000000	# Service Control
service-ctrl	2367/udp	0.000000	# Service Control
opentable	2368/tcp	0.000000
opentable	2368/udp	0.000661
bif-p2p	2369/tcp	0.000000	# Blockchain Identifier InFrastructure P2P
unknown	2369/udp	0.000330
l3-hbmon	2370/tcp	0.000000
l3-hbmon	2370/udp	0.000000
worldwire	2371/tcp	0.000076	# rda | hp-rda | Compaq WorldWire Port | HP Remote Device Access | Remote Device Access
worldwire	2371/udp	0.000330	# Compaq WorldWire Port
lanmessenger	2372/tcp	0.000076
lanmessenger	2372/udp	0.000330
remographlm	2373/tcp	0.000000	# Remograph License Manager
hydra	2374/tcp	0.000000	# Hydra RPC
docker	2375/tcp	0.000076	# docker.com | Docker REST API (plain text)
docker	2376/tcp	0.000076	# docker-s | docker.com | Docker REST API (ssl)
swarm	2377/tcp	0.000000	# RPC interface for Docker Swarm
unknown	2377/udp	0.000330
dali	2378/tcp	0.000000	# DALI lighting control
etcd-client	2379/tcp	0.000000	# etcd client communication
unknown	2379/udp	0.000330
etcd-server	2380/tcp	0.000000	# etcd server to server communication
unknown	2380/udp	0.000330
compaq-https	2381/tcp	0.000380	# Compaq HTTPS
compaq-https	2381/udp	0.000000	# Compaq HTTPS
ms-olap3	2382/tcp	0.000152	# Microsoft OLAP
ms-olap3	2382/udp	0.000661	# Microsoft OLAP
ms-olap4	2383/tcp	0.001369	# MS OLAP 4 | Microsoft OLAP
ms-olap4	2383/udp	0.000000	# Microsoft OLAP
sd-request	2384/tcp	0.000000	# sd-capacity | SD-CAPACITY
sd-capacity	2384/udp	0.000000
sd-data	2385/tcp	0.000000
sd-data	2385/udp	0.000000
virtualtape	2386/tcp	0.000000	# Virtual Tape
virtualtape	2386/udp	0.000330	# Virtual Tape
vsamredirector	2387/tcp	0.000000	# VSAM Redirector
vsamredirector	2387/udp	0.000661	# VSAM Redirector
mynahautostart	2388/tcp	0.000000	# MYNAH AutoStart
mynahautostart	2388/udp	0.000000	# MYNAH AutoStart
ovsessionmgr	2389/tcp	0.000000	# OpenView Session Mgr
ovsessionmgr	2389/udp	0.000000	# OpenView Session Mgr
rsmtp	2390/tcp	0.000000
rsmtp	2390/udp	0.000000
3com-net-mgmt	2391/tcp	0.000076	# 3COM Net Management
3com-net-mgmt	2391/udp	0.000000	# 3COM Net Management
tacticalauth	2392/tcp	0.000000	# Tactical Auth
tacticalauth	2392/udp	0.000330	# Tactical Auth
ms-olap1	2393/tcp	0.000228	# SQL Server Downlevel OLAP Client Support | MS OLAP 1
ms-olap1	2393/udp	0.000000	# MS OLAP 1
ms-olap2	2394/tcp	0.000228	# SQL Server Downlevel OLAP Client Support | MS OLAP 2
ms-olap2	2394/udp	0.000000	# MS OLAP 2
lan900_remote	2395/tcp	0.000000	# lan900-remote | LAN900 Remote
lan900_remote	2395/udp	0.000330	# LAN900 Remote
wusage	2396/tcp	0.000000
wusage	2396/udp	0.000000
ncl	2397/tcp	0.000000
ncl	2397/udp	0.000000
orbiter	2398/tcp	0.000000
orbiter	2398/udp	0.000661
fmpro-fdal	2399/tcp	0.000380	# FileMaker, Inc. - Data Access Layer
fmpro-fdal	2399/udp	0.000000	# FileMaker, Inc. - Data Access Layer
opequus-server	2400/tcp	0.000000	# OpEquus Server
opequus-server	2400/udp	0.000000	# OpEquus Server
cvspserver	2401/tcp	0.001480	# CVS network server
cvspserver	2401/udp	0.000544	# CVS network server
taskmaster2000	2402/tcp	0.000000	# TaskMaster 2000 Server
taskmaster2000	2402/udp	0.000000	# TaskMaster 2000 Server
taskmaster2000	2403/tcp	0.000000	# TaskMaster 2000 Web
taskmaster2000	2403/udp	0.000000	# TaskMaster 2000 Web
iec-104	2404/tcp	0.000000	# IEC 60870-5-104 process control over IP
iec-104	2404/udp	0.000000	# IEC 60870-5-104 process control over IP
trc-netpoll	2405/tcp	0.000000	# TRC Netpoll
trc-netpoll	2405/udp	0.000000	# TRC Netpoll
jediserver	2406/tcp	0.000000
jediserver	2406/udp	0.000330
orion	2407/tcp	0.000000
orion	2407/udp	0.000000
optimanet	2408/tcp	0.000000	# railgun-webaccl | CloudFlare Railgun Web Acceleration Protocol
optimanet	2408/udp	0.000000
sns-protocol	2409/tcp	0.000000	# SNS Protocol
sns-protocol	2409/udp	0.000000	# SNS Protocol
vrts-registry	2410/tcp	0.000000	# VRTS Registry
vrts-registry	2410/udp	0.000000	# VRTS Registry
netwave-ap-mgmt	2411/tcp	0.000000	# Netwave AP Management
netwave-ap-mgmt	2411/udp	0.000000	# Netwave AP Management
cdn	2412/tcp	0.000000
cdn	2412/udp	0.000330
orion-rmi-reg	2413/tcp	0.000000
orion-rmi-reg	2413/udp	0.000000
beeyond	2414/tcp	0.000000
beeyond	2414/udp	0.000000
codima-rtp	2415/tcp	0.000000	# Codima Remote Transaction Protocol
codima-rtp	2415/udp	0.000000	# Codima Remote Transaction Protocol
rmtserver	2416/tcp	0.000000	# RMT Server
rmtserver	2416/udp	0.000000	# RMT Server
composit-server	2417/tcp	0.000000	# Composit Server
composit-server	2417/udp	0.000330	# Composit Server
cas	2418/tcp	0.000076
cas	2418/udp	0.000330
attachmate-s2s	2419/tcp	0.000000	# Attachmate S2S
attachmate-s2s	2419/udp	0.000000	# Attachmate S2S
dslremote-mgmt	2420/tcp	0.000000	# DSL Remote Management
dslremote-mgmt	2420/udp	0.000000	# DSL Remote Management
g-talk	2421/tcp	0.000000
g-talk	2421/udp	0.000000
crmsbits	2422/tcp	0.000000
crmsbits	2422/udp	0.000000
rnrp	2423/tcp	0.000000
rnrp	2423/udp	0.000000
kofax-svr	2424/tcp	0.000000
kofax-svr	2424/udp	0.000000
fjitsuappmgr	2425/tcp	0.000076	# Fujitsu App Manager
fjitsuappmgr	2425/udp	0.000000	# Fujitsu App Manager
vcmp	2426/tcp	0.000000	# VeloCloud MultiPath Protocol
mgcp-gateway	2427/sctp	0.000000	# Media Gateway Control Protocol Gateway
mgcp-gateway	2427/tcp	0.000000	# Media Gateway Control Protocol Gateway
mgcp-gateway	2427/udp	0.000000	# Media Gateway Control Protocol Gateway
ott	2428/tcp	0.000000	# One Way Trip Time
ott	2428/udp	0.000000	# One Way Trip Time
ft-role	2429/tcp	0.000000
ft-role	2429/udp	0.000330
venus	2430/tcp	0.000050
venus	2430/udp	0.000478
venus-se	2431/tcp	0.000025
venus-se	2431/udp	0.000840
codasrv	2432/tcp	0.000025
codasrv	2432/udp	0.000560
codasrv-se	2433/tcp	0.000125
codasrv-se	2433/udp	0.000395
pxc-epmap	2434/tcp	0.000000
pxc-epmap	2434/udp	0.000000
optilogic	2435/tcp	0.000076
optilogic	2435/udp	0.000000
topx	2436/tcp	0.000076	# TOP/X
topx	2436/udp	0.000000	# TOP/X
unicontrol	2437/tcp	0.000000
unicontrol	2437/udp	0.000000
msp	2438/tcp	0.000076
msp	2438/udp	0.000000
sybasedbsynch	2439/tcp	0.000076
sybasedbsynch	2439/udp	0.000000
spearway	2440/tcp	0.000000	# Spearway Lockers
spearway	2440/udp	0.000000	# Spearway Lockers
pvsw-inet	2441/tcp	0.000000	# Pervasive I*net Data Server
pvsw-inet	2441/udp	0.000000	# Pervasive I*net Data Server
netangel	2442/tcp	0.000000
netangel	2442/udp	0.000000
powerclientcsf	2443/tcp	0.000000	# PowerClient Central Storage Facility
powerclientcsf	2443/udp	0.000000	# PowerClient Central Storage Facility
btpp2sectrans	2444/tcp	0.000000	# BT PP2 Sectrans
btpp2sectrans	2444/udp	0.000000	# BT PP2 Sectrans
dtn1	2445/tcp	0.000000
dtn1	2445/udp	0.000330
bues_service	2446/tcp	0.000000	# bues-service
bues_service	2446/udp	0.000000
ovwdb	2447/tcp	0.000000	# OpenView NNM daemon
ovwdb	2447/udp	0.000000	# OpenView NNM daemon
hpppssvr	2448/tcp	0.000000	# hpppsvr
hpppssvr	2448/udp	0.000000	# hpppsvr
ratl	2449/tcp	0.000076
ratl	2449/udp	0.000000
netadmin	2450/tcp	0.000000
netadmin	2450/udp	0.000000
netchat	2451/tcp	0.000000
netchat	2451/udp	0.000000
snifferclient	2452/tcp	0.000000
snifferclient	2452/udp	0.000000
madge-ltd	2453/tcp	0.000000	# madge ltd
madge-ltd	2453/udp	0.000000	# madge ltd
indx-dds	2454/tcp	0.000000
indx-dds	2454/udp	0.000000
wago-io-system	2455/tcp	0.000000
wago-io-system	2455/udp	0.000000
altav-remmgt	2456/tcp	0.000076
altav-remmgt	2456/udp	0.000000
rapido-ip	2457/tcp	0.000000	# Rapido_IP
rapido-ip	2457/udp	0.000330	# Rapido_IP
griffin	2458/tcp	0.000000
griffin	2458/udp	0.000000
community	2459/tcp	0.000000	# xrpl
community	2459/udp	0.000000
ms-theater	2460/tcp	0.000000
ms-theater	2460/udp	0.000000
qadmifoper	2461/tcp	0.000000
qadmifoper	2461/udp	0.000000
qadmifevent	2462/tcp	0.000000
qadmifevent	2462/udp	0.000000
lsi-raid-mgmt	2463/tcp	0.000076	# LSI RAID Management
lsi-raid-mgmt	2463/udp	0.000330	# LSI RAID Management
direcpc-si	2464/tcp	0.000000	# DirecPC SI
direcpc-si	2464/udp	0.000000	# DirecPC SI
lbm	2465/tcp	0.000000	# Load Balance Management
lbm	2465/udp	0.000000	# Load Balance Management
lbf	2466/tcp	0.000000	# Load Balance Forwarding
lbf	2466/udp	0.000000	# Load Balance Forwarding
high-criteria	2467/tcp	0.000000	# High Criteria
high-criteria	2467/udp	0.000000	# High Criteria
qip-msgd	2468/tcp	0.000000	# qip_msgd
qip-msgd	2468/udp	0.000000	# qip_msgd
mti-tcs-comm	2469/tcp	0.000000
mti-tcs-comm	2469/udp	0.000000
taskman-port	2470/tcp	0.000000	# taskman port
taskman-port	2470/udp	0.000000	# taskman port
seaodbc	2471/tcp	0.000000
seaodbc	2471/udp	0.000000
c3	2472/tcp	0.000076
c3	2472/udp	0.000000
aker-cdp	2473/tcp	0.000000
aker-cdp	2473/udp	0.000000
vitalanalysis	2474/tcp	0.000000	# Vital Analysis
vitalanalysis	2474/udp	0.000330	# Vital Analysis
ace-server	2475/tcp	0.000000	# ACE Server
ace-server	2475/udp	0.000000	# ACE Server
ace-svr-prop	2476/tcp	0.000000	# ACE Server Propagation
ace-svr-prop	2476/udp	0.000000	# ACE Server Propagation
ssm-cvs	2477/tcp	0.000000	# SecurSight Certificate Valifation Service
ssm-cvs	2477/udp	0.000000	# SecurSight Certificate Valifation Service
ssm-cssps	2478/tcp	0.000000	# SecurSight Authentication Server (SSL)
ssm-cssps	2478/udp	0.000000	# SecurSight Authentication Server (SSL)
ssm-els	2479/tcp	0.000000	# SecurSight Event Logging Server (SSL)
ssm-els	2479/udp	0.000000	# SecurSight Event Logging Server (SSL)
powerexchange	2480/tcp	0.000000	# Informatica PowerExchange Listener
powerexchange	2480/udp	0.000000	# Informatica PowerExchange Listener
giop	2481/tcp	0.000000	# Oracle GIOP
giop	2481/udp	0.000000	# Oracle GIOP
giop-ssl	2482/tcp	0.000000	# Oracle GIOP SSL
giop-ssl	2482/udp	0.000000	# Oracle GIOP SSL
ttc	2483/tcp	0.000000	# Oracle TTC
ttc	2483/udp	0.000000	# Oracle TTC
ttc-ssl	2484/tcp	0.000000	# Oracle TTC SSL
ttc-ssl	2484/udp	0.000000	# Oracle TTC SSL
netobjects1	2485/tcp	0.000000	# Net Objects1
netobjects1	2485/udp	0.000000	# Net Objects1
netobjects2	2486/tcp	0.000000	# Net Objects2
netobjects2	2486/udp	0.000000	# Net Objects2
pns	2487/tcp	0.000000	# Policy Notice Service
pns	2487/udp	0.000330	# Policy Notice Service
moy-corp	2488/tcp	0.000000	# Moy Corporation
moy-corp	2488/udp	0.000000	# Moy Corporation
tsilb	2489/tcp	0.000000
tsilb	2489/udp	0.000330
qip-qdhcp	2490/tcp	0.000000	# qip_qdhcp
qip-qdhcp	2490/udp	0.000000	# qip_qdhcp
conclave-cpp	2491/tcp	0.000000	# Conclave CPP
conclave-cpp	2491/udp	0.000000	# Conclave CPP
groove	2492/tcp	0.000380
groove	2492/udp	0.000330
talarian-mqs	2493/tcp	0.000000	# Talarian MQS
talarian-mqs	2493/udp	0.000000	# Talarian MQS
bmc-ar	2494/tcp	0.000000	# BMC AR
bmc-ar	2494/udp	0.000330	# BMC AR
fast-rem-serv	2495/tcp	0.000000	# Fast Remote Services
fast-rem-serv	2495/udp	0.000000	# Fast Remote Services
dirgis	2496/tcp	0.000000
dirgis	2496/udp	0.000661
quaddb	2497/tcp	0.000000	# Quad DB
quaddb	2497/udp	0.000000	# Quad DB
odn-castraq	2498/tcp	0.000000
odn-castraq	2498/udp	0.000000
unicontrol	2499/tcp	0.000000
unicontrol	2499/udp	0.000000
rtsserv	2500/tcp	0.000464	# Resource Tracking system server
rtsserv	2500/udp	0.000511	# Resource Tracking system server
rtsclient	2501/tcp	0.000151	# Resource Tracking system client
rtsclient	2501/udp	0.000461	# Resource Tracking system client
kentrox-prot	2502/tcp	0.000000	# Kentrox Protocol
kentrox-prot	2502/udp	0.000000	# Kentrox Protocol
nms-dpnss	2503/tcp	0.000000
nms-dpnss	2503/udp	0.000330
wlbs	2504/tcp	0.000000
wlbs	2504/udp	0.000000
ppcontrol	2505/tcp	0.000076	# PowerPlay Control
ppcontrol	2505/udp	0.000330	# PowerPlay Control
jbroker	2506/tcp	0.000000
jbroker	2506/udp	0.000000
spock	2507/tcp	0.000000
spock	2507/udp	0.000000
jdatastore	2508/tcp	0.000000
jdatastore	2508/udp	0.000000
fjmpss	2509/tcp	0.000000
fjmpss	2509/udp	0.000330
fjappmgrbulk	2510/tcp	0.000000
fjappmgrbulk	2510/udp	0.000330
metastorm	2511/tcp	0.000000
metastorm	2511/udp	0.000000
citrixima	2512/tcp	0.000000	# Citrix IMA
citrixima	2512/udp	0.000330	# Citrix IMA
citrixadmin	2513/tcp	0.000000	# Citrix ADMIN
citrixadmin	2513/udp	0.000000	# Citrix ADMIN
facsys-ntp	2514/tcp	0.000000	# Facsys NTP
facsys-ntp	2514/udp	0.000000	# Facsys NTP
facsys-router	2515/tcp	0.000000	# Facsys Router
facsys-router	2515/udp	0.000330	# Facsys Router
maincontrol	2516/tcp	0.000000	# Main Control
maincontrol	2516/udp	0.000000	# Main Control
call-sig-trans	2517/tcp	0.000000	# H.323 Annex E call signaling transport | H.323 Annex E Call Control Signalling Transport
call-sig-trans	2517/udp	0.000661	# H.323 Annex E call signaling transport
willy	2518/tcp	0.000000
willy	2518/udp	0.000000
globmsgsvc	2519/tcp	0.000000
globmsgsvc	2519/udp	0.000000
pvsw	2520/tcp	0.000000	# Pervasive Listener
pvsw	2520/udp	0.000000	# Pervasive Listener
adaptecmgr	2521/tcp	0.000000	# Adaptec Manager
adaptecmgr	2521/udp	0.000000	# Adaptec Manager
windb	2522/tcp	0.000304
windb	2522/udp	0.000000
qke-llc-v3	2523/tcp	0.000000	# Qke LLC V.3
qke-llc-v3	2523/udp	0.000000	# Qke LLC V.3
optiwave-lm	2524/tcp	0.000000	# Optiwave License Management
optiwave-lm	2524/udp	0.000330	# Optiwave License Management
ms-v-worlds	2525/tcp	0.000456	# MS V-Worlds
ms-v-worlds	2525/udp	0.000000	# MS V-Worlds
ema-sent-lm	2526/tcp	0.000000	# EMA License Manager
ema-sent-lm	2526/udp	0.000000	# EMA License Manager
iqserver	2527/tcp	0.000000	# IQ Server
iqserver	2527/udp	0.000330	# IQ Server
ncr_ccl	2528/tcp	0.000000	# ncr-ccl | NCR CCL
ncr_ccl	2528/udp	0.000661	# NCR CCL
utsftp	2529/tcp	0.000000	# UTS FTP
utsftp	2529/udp	0.000000	# UTS FTP
vrcommerce	2530/tcp	0.000000	# VR Commerce
vrcommerce	2530/udp	0.000000	# VR Commerce
ito-e-gui	2531/tcp	0.000076	# ITO-E GUI
ito-e-gui	2531/udp	0.000000	# ITO-E GUI
ovtopmd	2532/tcp	0.000076
ovtopmd	2532/udp	0.000000
snifferserver	2533/tcp	0.000000
snifferserver	2533/udp	0.000330
combox-web-acc	2534/tcp	0.000000	# Combox Web Access
combox-web-acc	2534/udp	0.000000	# Combox Web Access
madcap	2535/tcp	0.000000
madcap	2535/udp	0.000000
btpp2audctr1	2536/tcp	0.000000
btpp2audctr1	2536/udp	0.000000
upgrade	2537/tcp	0.000000	# Upgrade Protocol
upgrade	2537/udp	0.000000	# Upgrade Protocol
vnwk-prapi	2538/tcp	0.000000
vnwk-prapi	2538/udp	0.000330
vsiadmin	2539/tcp	0.000000	# VSI Admin
vsiadmin	2539/udp	0.000330	# VSI Admin
lonworks	2540/tcp	0.000000
lonworks	2540/udp	0.000000
lonworks2	2541/tcp	0.000000
lonworks2	2541/udp	0.000000
udrawgraph	2542/tcp	0.000000	# uDraw(Graph)
udrawgraph	2542/udp	0.000330	# uDraw(Graph)
reftek	2543/tcp	0.000000
reftek	2543/udp	0.000330
novell-zen	2544/tcp	0.000000	# Management Daemon Refresh
novell-zen	2544/udp	0.000000	# Management Daemon Refresh
sis-emt	2545/tcp	0.000000
sis-emt	2545/udp	0.000000
vytalvaultbrtp	2546/tcp	0.000000
vytalvaultbrtp	2546/udp	0.000330
vytalvaultvsmp	2547/tcp	0.000000
vytalvaultvsmp	2547/udp	0.000000
vytalvaultpipe	2548/tcp	0.000000
vytalvaultpipe	2548/udp	0.000000
ipass	2549/tcp	0.000000
ipass	2549/udp	0.000000
ads	2550/tcp	0.000076
ads	2550/udp	0.000000
isg-uda-server	2551/tcp	0.000076	# ISG UDA Server
isg-uda-server	2551/udp	0.000000	# ISG UDA Server
call-logging	2552/tcp	0.000000	# Call Logging
call-logging	2552/udp	0.000330	# Call Logging
efidiningport	2553/tcp	0.000000
efidiningport	2553/udp	0.000000
vcnet-link-v10	2554/tcp	0.000000	# VCnet-Link v10
vcnet-link-v10	2554/udp	0.000000	# VCnet-Link v10
compaq-wcp	2555/tcp	0.000000	# Compaq WCP
compaq-wcp	2555/udp	0.000330	# Compaq WCP
nicetec-nmsvc	2556/tcp	0.000000
nicetec-nmsvc	2556/udp	0.000000
nicetec-mgmt	2557/tcp	0.000152
nicetec-mgmt	2557/udp	0.000000
pclemultimedia	2558/tcp	0.000076	# PCLE Multi Media
pclemultimedia	2558/udp	0.000000	# PCLE Multi Media
lstp	2559/tcp	0.000000
lstp	2559/udp	0.000330
labrat	2560/tcp	0.000000
labrat	2560/udp	0.000000
mosaixcc	2561/tcp	0.000000
mosaixcc	2561/udp	0.000000
delibo	2562/tcp	0.000000
delibo	2562/udp	0.000000
cti-redwood	2563/tcp	0.000000	# CTI Redwood
cti-redwood	2563/udp	0.000000	# CTI Redwood
hp-3000-telnet	2564/tcp	0.000013	# HP 3000 NS/VT block mode telnet
coord-svr	2565/tcp	0.000000	# Coordinator Server
coord-svr	2565/udp	0.000000	# Coordinator Server
pcs-pcw	2566/tcp	0.000000
pcs-pcw	2566/udp	0.000000
clp	2567/tcp	0.000076	# Cisco Line Protocol
clp	2567/udp	0.000000	# Cisco Line Protocol
spamtrap	2568/tcp	0.000000	# SPAM TRAP
spamtrap	2568/udp	0.000000	# SPAM TRAP
sonuscallsig	2569/tcp	0.000000	# Sonus Call Signal
sonuscallsig	2569/udp	0.000000	# Sonus Call Signal
hs-port	2570/tcp	0.000000	# HS Port
hs-port	2570/udp	0.000000	# HS Port
cecsvc	2571/tcp	0.000000
cecsvc	2571/udp	0.000000
ibp	2572/tcp	0.000000
ibp	2572/udp	0.000000
trustestablish	2573/tcp	0.000000	# Trust Establish
trustestablish	2573/udp	0.000000	# Trust Establish
blockade-bpsp	2574/tcp	0.000000	# Blockade BPSP
blockade-bpsp	2574/udp	0.000000	# Blockade BPSP
hl7	2575/tcp	0.000000
hl7	2575/udp	0.000000
tclprodebugger	2576/tcp	0.000000	# TCL Pro Debugger
tclprodebugger	2576/udp	0.000000	# TCL Pro Debugger
scipticslsrvr	2577/tcp	0.000000	# Scriptics Lsrvr
scipticslsrvr	2577/udp	0.000000	# Scriptics Lsrvr
rvs-isdn-dcp	2578/tcp	0.000000	# RVS ISDN DCP
rvs-isdn-dcp	2578/udp	0.000000	# RVS ISDN DCP
mpfoncl	2579/tcp	0.000000
mpfoncl	2579/udp	0.000000
tributary	2580/tcp	0.000076
tributary	2580/udp	0.000000
argis-te	2581/tcp	0.000000	# ARGIS TE
argis-te	2581/udp	0.000000	# ARGIS TE
argis-ds	2582/tcp	0.000000	# ARGIS DS
argis-ds	2582/udp	0.000330	# ARGIS DS
mon	2583/tcp	0.000076
mon	2583/udp	0.000000
cyaserv	2584/tcp	0.000076
cyaserv	2584/udp	0.000000
netx-server	2585/tcp	0.000000	# NETX Server
netx-server	2585/udp	0.000000	# NETX Server
netx-agent	2586/tcp	0.000000	# NETX Agent
netx-agent	2586/udp	0.000000	# NETX Agent
masc	2587/tcp	0.000000
masc	2587/udp	0.000000
privilege	2588/tcp	0.000000
privilege	2588/udp	0.000000
quartus-tcl	2589/tcp	0.000000	# quartus tcl
quartus-tcl	2589/udp	0.000330	# quartus tcl
idotdist	2590/tcp	0.000000
idotdist	2590/udp	0.000000
maytagshuffle	2591/tcp	0.000000	# Maytag Shuffle
maytagshuffle	2591/udp	0.000000	# Maytag Shuffle
netrek	2592/tcp	0.000000
netrek	2592/udp	0.000330
mns-mail	2593/tcp	0.000000	# MNS Mail Notice Service
mns-mail	2593/udp	0.000000	# MNS Mail Notice Service
dts	2594/tcp	0.000000	# Data Base Server
dts	2594/udp	0.000000	# Data Base Server
worldfusion1	2595/tcp	0.000000	# World Fusion 1
worldfusion1	2595/udp	0.000000	# World Fusion 1
worldfusion2	2596/tcp	0.000000	# World Fusion 2
worldfusion2	2596/udp	0.000000	# World Fusion 2
homesteadglory	2597/tcp	0.000000	# Homestead Glory
homesteadglory	2597/udp	0.000000	# Homestead Glory
citriximaclient	2598/tcp	0.000076	# Citrix MA Client
citriximaclient	2598/udp	0.000000	# Citrix MA Client
snapd	2599/tcp	0.000000	# Snap Discovery
snapd	2599/udp	0.000000	# Snap Discovery
zebrasrv	2600/tcp	0.000088	# hpstgmgr | zebra service | HPSTGMGR
hpstgmgr	2600/udp	0.000330
zebra	2601/tcp	0.002032	# discp-client | zebra vty | discp client
discp-client	2601/udp	0.000000	# discp client
ripd	2602/tcp	0.000790	# discp-server | RIPd vty | discp server
discp-server	2602/udp	0.000000	# discp server
ripngd	2603/tcp	0.000000	# servicemeter | RIPngd vty | Service Meter
servicemeter	2603/udp	0.000330	# Service Meter
ospfd	2604/tcp	0.000765	# nsc-ccs | OSPFd vty | NSC CCS
nsc-ccs	2604/udp	0.000000	# NSC CCS
bgpd	2605/tcp	0.000514	# nsc-posa | BGPd vty | NSC POSA
nsc-posa	2605/udp	0.000000	# NSC POSA
netmon	2606/tcp	0.000076	# Dell Netmon
netmon	2606/udp	0.000000	# Dell Netmon
connection	2607/tcp	0.000380	# Dell Connection
connection	2607/udp	0.000000	# Dell Connection
wag-service	2608/tcp	0.000228	# Wag Service
wag-service	2608/udp	0.000000	# Wag Service
system-monitor	2609/tcp	0.000000	# System Monitor
system-monitor	2609/udp	0.000000	# System Monitor
versa-tek	2610/tcp	0.000000	# VersaTek
versa-tek	2610/udp	0.000000	# VersaTek
lionhead	2611/tcp	0.000000
lionhead	2611/udp	0.000000
qpasa-agent	2612/tcp	0.000000	# Qpasa Agent
qpasa-agent	2612/udp	0.000330	# Qpasa Agent
smntubootstrap	2613/tcp	0.000000
smntubootstrap	2613/udp	0.000330
neveroffline	2614/tcp	0.000000	# Never Offline
neveroffline	2614/udp	0.000000	# Never Offline
firepower	2615/tcp	0.000000
firepower	2615/udp	0.000330
appswitch-emp	2616/tcp	0.000000
appswitch-emp	2616/udp	0.000000
cmadmin	2617/tcp	0.000000	# Clinical Context Managers
cmadmin	2617/udp	0.000000	# Clinical Context Managers
priority-e-com	2618/tcp	0.000000	# Priority E-Com
priority-e-com	2618/udp	0.000330	# Priority E-Com
bruce	2619/tcp	0.000000
bruce	2619/udp	0.000000
lpsrecommender	2620/tcp	0.000000
lpsrecommender	2620/udp	0.000000
miles-apart	2621/tcp	0.000000	# Miles Apart Jukebox Server
miles-apart	2621/udp	0.000000	# Miles Apart Jukebox Server
metricadbc	2622/tcp	0.000076
metricadbc	2622/udp	0.000000
lmdp	2623/tcp	0.000076
lmdp	2623/udp	0.000000
aria	2624/tcp	0.000000
aria	2624/udp	0.000000
blwnkl-port	2625/tcp	0.000000	# Blwnkl Port
blwnkl-port	2625/udp	0.000330	# Blwnkl Port
gbjd816	2626/tcp	0.000000
gbjd816	2626/udp	0.000000
webster	2627/tcp	0.000025	# moshebeeri | Network dictionary | Moshe Beeri
webster	2627/udp	0.000692
dict	2628/tcp	0.000125	# Dictionary service (RFC2229)
dict	2628/udp	0.000000
sitaraserver	2629/tcp	0.000000	# Sitara Server
sitaraserver	2629/udp	0.000330	# Sitara Server
sitaramgmt	2630/tcp	0.000000	# Sitara Management
sitaramgmt	2630/udp	0.000000	# Sitara Management
sitaradir	2631/tcp	0.000076	# Sitara Dir
sitaradir	2631/udp	0.000000	# Sitara Dir
irdg-post	2632/tcp	0.000000	# IRdg Post
irdg-post	2632/udp	0.000000	# IRdg Post
interintelli	2633/tcp	0.000000
interintelli	2633/udp	0.000000
pk-electronics	2634/tcp	0.000000	# PK Electronics
pk-electronics	2634/udp	0.000330	# PK Electronics
backburner	2635/tcp	0.000000	# Back Burner
backburner	2635/udp	0.000330	# Back Burner
solve	2636/tcp	0.000000
solve	2636/udp	0.000000
imdocsvc	2637/tcp	0.000000	# Import Document Service
imdocsvc	2637/udp	0.000000	# Import Document Service
sybase	2638/tcp	0.000251	# sybaseanywhere | Sybase database | Sybase Anywhere
sybaseanywhere	2638/udp	0.000330	# Sybase Anywhere
aminet	2639/tcp	0.000000
aminet	2639/udp	0.000000
sai_sentlm	2640/tcp	0.000000	# ami-control | Sabbagh Associates Licence Manager | Alcorn McBride Inc protocol used for device control
sai_sentlm	2640/udp	0.000000	# Sabbagh Associates Licence Manager
hdl-srv	2641/tcp	0.000000	# HDL Server
hdl-srv	2641/udp	0.000330	# HDL Server
tragic	2642/tcp	0.000000
tragic	2642/udp	0.000000
gte-samp	2643/tcp	0.000000
gte-samp	2643/udp	0.000000
travsoft-ipx-t	2644/tcp	0.000076	# Travsoft IPX Tunnel
travsoft-ipx-t	2644/udp	0.000000	# Travsoft IPX Tunnel
novell-ipx-cmd	2645/tcp	0.000000	# Novell IPX CMD
novell-ipx-cmd	2645/udp	0.000000	# Novell IPX CMD
and-lm	2646/tcp	0.000000	# AND License Manager
and-lm	2646/udp	0.000330	# AND License Manager
syncserver	2647/tcp	0.000000
syncserver	2647/udp	0.000000
upsnotifyprot	2648/tcp	0.000000
upsnotifyprot	2648/udp	0.000000
vpsipport	2649/tcp	0.000000
vpsipport	2649/udp	0.000330
eristwoguns	2650/tcp	0.000000
eristwoguns	2650/udp	0.000000
ebinsite	2651/tcp	0.000000
ebinsite	2651/udp	0.000000
interpathpanel	2652/tcp	0.000000
interpathpanel	2652/udp	0.000000
sonus	2653/tcp	0.000000
sonus	2653/udp	0.000000
corel_vncadmin	2654/tcp	0.000000	# corel-vncadmin | Corel VNC Admin
corel_vncadmin	2654/udp	0.000000	# Corel VNC Admin
unglue	2655/tcp	0.000000	# UNIX Nt Glue
unglue	2655/udp	0.000000	# UNIX Nt Glue
kana	2656/tcp	0.000000
kana	2656/udp	0.000000
sns-dispatcher	2657/tcp	0.000000	# SNS Dispatcher
sns-dispatcher	2657/udp	0.000330	# SNS Dispatcher
sns-admin	2658/tcp	0.000000	# SNS Admin
sns-admin	2658/udp	0.000000	# SNS Admin
sns-query	2659/tcp	0.000000	# SNS Query
sns-query	2659/udp	0.000000	# SNS Query
gcmonitor	2660/tcp	0.000000	# GC Monitor
gcmonitor	2660/udp	0.000000	# GC Monitor
olhost	2661/tcp	0.000000
olhost	2661/udp	0.000000
bintec-capi	2662/tcp	0.000000
bintec-capi	2662/udp	0.000330
bintec-tapi	2663/tcp	0.000000
bintec-tapi	2663/udp	0.000000
patrol-mq-gm	2664/tcp	0.000000	# Patrol for MQ GM
patrol-mq-gm	2664/udp	0.000330	# Patrol for MQ GM
patrol-mq-nm	2665/tcp	0.000000	# Patrol for MQ NM
patrol-mq-nm	2665/udp	0.000000	# Patrol for MQ NM
extensis	2666/tcp	0.000000
extensis	2666/udp	0.000330
alarm-clock-s	2667/tcp	0.000000	# Alarm Clock Server
alarm-clock-s	2667/udp	0.000330	# Alarm Clock Server
alarm-clock-c	2668/tcp	0.000000	# Alarm Clock Client
alarm-clock-c	2668/udp	0.000000	# Alarm Clock Client
toad	2669/tcp	0.000000
toad	2669/udp	0.000000
tve-announce	2670/tcp	0.000000	# TVE Announce
tve-announce	2670/udp	0.000000	# TVE Announce
newlixreg	2671/tcp	0.000000
newlixreg	2671/udp	0.000000
nhserver	2672/tcp	0.000000
nhserver	2672/udp	0.000000
firstcall42	2673/tcp	0.000000	# First Call 42
firstcall42	2673/udp	0.000330	# First Call 42
ewnn	2674/tcp	0.000000
ewnn	2674/udp	0.000000
ttc-etap	2675/tcp	0.000000	# TTC ETAP
ttc-etap	2675/udp	0.000000	# TTC ETAP
simslink	2676/tcp	0.000000
simslink	2676/udp	0.000000
gadgetgate1way	2677/tcp	0.000000	# Gadget Gate 1 Way
gadgetgate1way	2677/udp	0.000330	# Gadget Gate 1 Way
gadgetgate2way	2678/tcp	0.000000	# Gadget Gate 2 Way
gadgetgate2way	2678/udp	0.000330	# Gadget Gate 2 Way
syncserverssl	2679/tcp	0.000000	# Sync Server SSL
syncserverssl	2679/udp	0.000000	# Sync Server SSL
pxc-sapxom	2680/tcp	0.000000
pxc-sapxom	2680/udp	0.000000
mpnjsomb	2681/tcp	0.000000
mpnjsomb	2681/udp	0.000000
ncdloadbalance	2683/tcp	0.000000
ncdloadbalance	2683/udp	0.000000
mpnjsosv	2684/tcp	0.000000
mpnjsosv	2684/udp	0.000000
mpnjsocl	2685/tcp	0.000000
mpnjsocl	2685/udp	0.000000
mpnjsomg	2686/tcp	0.000000
mpnjsomg	2686/udp	0.000000
pq-lic-mgmt	2687/tcp	0.000000
pq-lic-mgmt	2687/udp	0.000000
md-cg-http	2688/tcp	0.000000	# md-cf-http
md-cg-http	2688/udp	0.000000	# md-cf-http
fastlynx	2689/tcp	0.000000
fastlynx	2689/udp	0.000000
hp-nnm-data	2690/tcp	0.000000	# HP NNM Embedded Database
hp-nnm-data	2690/udp	0.000000	# HP NNM Embedded Database
itinternet	2691/tcp	0.000076	# ITInternet ISM Server
itinternet	2691/udp	0.000000	# ITInternet ISM Server
admins-lms	2692/tcp	0.000000	# Admins LMS
admins-lms	2692/udp	0.000330	# Admins LMS
pwrsevent	2694/tcp	0.000000
pwrsevent	2694/udp	0.000000
vspread	2695/tcp	0.000000
vspread	2695/udp	0.000330
unifyadmin	2696/tcp	0.000000	# Unify Admin
unifyadmin	2696/udp	0.000000	# Unify Admin
oce-snmp-trap	2697/tcp	0.000000	# Oce SNMP Trap Port
oce-snmp-trap	2697/udp	0.000000	# Oce SNMP Trap Port
mck-ivpip	2698/tcp	0.000000
mck-ivpip	2698/udp	0.000000
csoft-plusclnt	2699/tcp	0.000000	# Csoft Plus Client
csoft-plusclnt	2699/udp	0.000000	# Csoft Plus Client
tqdata	2700/tcp	0.000076
tqdata	2700/udp	0.000000
sms-rcinfo	2701/tcp	0.000836	# SMS RCINFO
sms-rcinfo	2701/udp	0.000000
sms-xfer	2702/tcp	0.000760	# SMS XFER
sms-xfer	2702/udp	0.000000
sms-chat	2703/tcp	0.000000	# SMS CHAT
sms-chat	2703/udp	0.000000	# SMS CHAT
sms-remctrl	2704/tcp	0.000000	# SMS REMCTRL
sms-remctrl	2704/udp	0.000330	# SMS REMCTRL
sds-admin	2705/tcp	0.000000	# SDS Admin
sds-admin	2705/udp	0.000330	# SDS Admin
ncdmirroring	2706/tcp	0.000076	# NCD Mirroring
ncdmirroring	2706/udp	0.000000	# NCD Mirroring
emcsymapiport	2707/tcp	0.000000
emcsymapiport	2707/udp	0.000000
banyan-net	2708/tcp	0.000000
banyan-net	2708/udp	0.000330
supermon	2709/tcp	0.000000
supermon	2709/udp	0.000330
sso-service	2710/tcp	0.000152	# SSO Service
sso-service	2710/udp	0.000000	# SSO Service
sso-control	2711/tcp	0.000076	# SSO Control
sso-control	2711/udp	0.000000	# SSO Control
aocp	2712/tcp	0.000076	# Axapta Object Communication Protocol
aocp	2712/udp	0.000000	# Axapta Object Communication Protocol
raventbs	2713/tcp	0.000000	# Raven Trinity Broker Service
raventbs	2713/udp	0.000000	# Raven Trinity Broker Service
raventdm	2714/tcp	0.000000	# Raven Trinity Data Mover
raventdm	2714/udp	0.000000	# Raven Trinity Data Mover
hpstgmgr2	2715/tcp	0.000000
hpstgmgr2	2715/udp	0.000000
inova-ip-disco	2716/tcp	0.000000	# Inova IP Disco
inova-ip-disco	2716/udp	0.000000	# Inova IP Disco
pn-requester	2717/tcp	0.003345	# PN REQUESTER
pn-requester	2717/udp	0.000000	# PN REQUESTER
pn-requester2	2718/tcp	0.000380	# PN REQUESTER 2
pn-requester2	2718/udp	0.000000	# PN REQUESTER 2
scan-change	2719/tcp	0.000000	# Scan & Change
scan-change	2719/udp	0.000330	# Scan & Change
wkars	2720/tcp	0.000000
wkars	2720/udp	0.000330
smart-diagnose	2721/tcp	0.000000	# Smart Diagnose
smart-diagnose	2721/udp	0.000000	# Smart Diagnose
proactivesrvr	2722/tcp	0.000000	# Proactive Server
proactivesrvr	2722/udp	0.000000	# Proactive Server
watchdog-nt	2723/tcp	0.000076	# WatchDog NT Protocol
watchdog-nt	2723/udp	0.000000	# WatchDog NT Protocol
qotps	2724/tcp	0.000000
qotps	2724/udp	0.000000
msolap-ptp2	2725/tcp	0.000228	# SQL Analysis Server | MSOLAP PTP2
msolap-ptp2	2725/udp	0.000000	# MSOLAP PTP2
tams	2726/tcp	0.000000
tams	2726/udp	0.000330
mgcp-callagent	2727/tcp	0.000000	# Media Gateway Control Protocol Call Agent
mgcp-callagent	2727/udp	0.000000	# Media Gateway Control Protocol Call Agent
sqdr	2728/tcp	0.000076
sqdr	2728/udp	0.000000
tcim-control	2729/tcp	0.000000	# TCIM Control
tcim-control	2729/udp	0.000000	# TCIM Control
nec-raidplus	2730/tcp	0.000000	# NEC RaidPlus
nec-raidplus	2730/udp	0.000000	# NEC RaidPlus
fyre-messanger	2731/tcp	0.000000	# Fyre Messanger | Fyre Messagner
fyre-messanger	2731/udp	0.000000	# Fyre Messagner
g5m	2732/tcp	0.000000
g5m	2732/udp	0.000000
signet-ctf	2733/tcp	0.000000	# Signet CTF
signet-ctf	2733/udp	0.000000	# Signet CTF
ccs-software	2734/tcp	0.000076	# CCS Software
ccs-software	2734/udp	0.000330	# CCS Software
netiq-mc	2735/tcp	0.000000	# NetIQ Monitor Console
netiq-mc	2735/udp	0.000000	# NetIQ Monitor Console
radwiz-nms-srv	2736/tcp	0.000000	# RADWIZ NMS SRV
radwiz-nms-srv	2736/udp	0.000000	# RADWIZ NMS SRV
srp-feedback	2737/tcp	0.000000	# SRP Feedback
srp-feedback	2737/udp	0.000330	# SRP Feedback
ndl-tcp-ois-gw	2738/tcp	0.000000	# NDL TCP-OSI Gateway
ndl-tcp-ois-gw	2738/udp	0.000000	# NDL TCP-OSI Gateway
tn-timing	2739/tcp	0.000000	# TN Timing
tn-timing	2739/udp	0.000330	# TN Timing
alarm	2740/tcp	0.000000
alarm	2740/udp	0.000000
tsb	2741/tcp	0.000000
tsb	2741/udp	0.000000
tsb2	2742/tcp	0.000000
tsb2	2742/udp	0.000000
murx	2743/tcp	0.000000
murx	2743/udp	0.000000
honyaku	2744/tcp	0.000000
honyaku	2744/udp	0.000000
urbisnet	2745/tcp	0.000000
urbisnet	2745/udp	0.000000
cpudpencap	2746/tcp	0.000000
cpudpencap	2746/udp	0.000000
fjippol-swrly	2747/tcp	0.000000
fjippol-swrly	2747/udp	0.000000
fjippol-polsvr	2748/tcp	0.000000
fjippol-polsvr	2748/udp	0.000000
fjippol-cnsl	2749/tcp	0.000000
fjippol-cnsl	2749/udp	0.000330
fjippol-port1	2750/tcp	0.000000
fjippol-port1	2750/udp	0.000000
fjippol-port2	2751/tcp	0.000000
fjippol-port2	2751/udp	0.000000
rsisysaccess	2752/tcp	0.000000	# RSISYS ACCESS
rsisysaccess	2752/udp	0.000000	# RSISYS ACCESS
de-spot	2753/tcp	0.000000
de-spot	2753/udp	0.000000
apollo-cc	2754/tcp	0.000000	# APOLLO CC
apollo-cc	2754/udp	0.000000	# APOLLO CC
expresspay	2755/tcp	0.000000	# Express Pay
expresspay	2755/udp	0.000000	# Express Pay
simplement-tie	2756/tcp	0.000000
simplement-tie	2756/udp	0.000000
cnrp	2757/tcp	0.000000
cnrp	2757/udp	0.000000
apollo-status	2758/tcp	0.000000	# APOLLO Status
apollo-status	2758/udp	0.000000	# APOLLO Status
apollo-gms	2759/tcp	0.000000	# APOLLO GMS
apollo-gms	2759/udp	0.000000	# APOLLO GMS
sabams	2760/tcp	0.000000	# Saba MS
sabams	2760/udp	0.000000	# Saba MS
dicom-iscl	2761/tcp	0.000000	# DICOM ISCL
dicom-iscl	2761/udp	0.000000	# DICOM ISCL
dicom-tls	2762/tcp	0.000000	# DICOM TLS
dicom-tls	2762/udp	0.000000	# DICOM TLS
desktop-dna	2763/tcp	0.000000	# Desktop DNA
desktop-dna	2763/udp	0.000000	# Desktop DNA
data-insurance	2764/tcp	0.000000	# Data Insurance
data-insurance	2764/udp	0.000000	# Data Insurance
qip-audup	2765/tcp	0.000000
qip-audup	2765/udp	0.000330
listen	2766/tcp	0.000013	# compaq-scp | System V listener port | Compaq SCP
compaq-scp	2766/udp	0.000000	# Compaq SCP
uadtc	2767/tcp	0.000000
uadtc	2767/udp	0.000330
uacs	2768/tcp	0.000000
uacs	2768/udp	0.000000
exce	2769/tcp	0.000000
exce	2769/udp	0.000000
veronica	2770/tcp	0.000000
veronica	2770/udp	0.000000
vergencecm	2771/tcp	0.000000	# Vergence CM
vergencecm	2771/udp	0.000330	# Vergence CM
auris	2772/tcp	0.000000
auris	2772/udp	0.000000
rbakcup1	2773/tcp	0.000000	# RBackup Remote Backup
rbakcup1	2773/udp	0.000330	# RBackup Remote Backup
rbakcup2	2774/tcp	0.000000	# RBackup Remote Backup
rbakcup2	2774/udp	0.000000	# RBackup Remote Backup
smpp	2775/tcp	0.000000
smpp	2775/udp	0.000000
ridgeway1	2776/tcp	0.000000	# Ridgeway Systems & Software
ridgeway1	2776/udp	0.000000	# Ridgeway Systems & Software
ridgeway2	2777/tcp	0.000000	# Ridgeway Systems & Software
ridgeway2	2777/udp	0.000330	# Ridgeway Systems & Software
gwen-sonya	2778/tcp	0.000000
gwen-sonya	2778/udp	0.000000
lbc-sync	2779/tcp	0.000000	# LBC Sync
lbc-sync	2779/udp	0.000000	# LBC Sync
lbc-control	2780/tcp	0.000000	# LBC Control
lbc-control	2780/udp	0.000000	# LBC Control
whosells	2781/tcp	0.000000
whosells	2781/udp	0.000330
everydayrc	2782/tcp	0.000000
everydayrc	2782/udp	0.000000
aises	2783/tcp	0.000000
aises	2783/udp	0.000000
www-dev	2784/tcp	0.000000	# world wide web - development
www-dev	2784/udp	0.000395	# world wide web - development
aic-np	2785/tcp	0.000000
aic-np	2785/udp	0.000000
aic-oncrpc	2786/tcp	0.000000	# aic-oncrpc - Destiny MCD database
aic-oncrpc	2786/udp	0.000000	# aic-oncrpc - Destiny MCD database
piccolo	2787/tcp	0.000000	# piccolo - Cornerstone Software
piccolo	2787/udp	0.000000	# piccolo - Cornerstone Software
fryeserv	2788/tcp	0.000000	# NetWare Loadable Module - Seagate Software
fryeserv	2788/udp	0.000000	# NetWare Loadable Module - Seagate Software
media-agent	2789/tcp	0.000000	# Media Agent
media-agent	2789/udp	0.000330	# Media Agent
plgproxy	2790/tcp	0.000000	# PLG Proxy
plgproxy	2790/udp	0.000000	# PLG Proxy
mtport-regist	2791/tcp	0.000000	# MT Port Registrator
mtport-regist	2791/udp	0.000330	# MT Port Registrator
f5-globalsite	2792/tcp	0.000000
f5-globalsite	2792/udp	0.000000
initlsmsad	2793/tcp	0.000000
initlsmsad	2793/udp	0.000000
livestats	2795/tcp	0.000000
livestats	2795/udp	0.000000
ac-tech	2796/tcp	0.000000
ac-tech	2796/udp	0.000000
esp-encap	2797/tcp	0.000000
esp-encap	2797/udp	0.000330
tmesis-upshot	2798/tcp	0.000000
tmesis-upshot	2798/udp	0.000000
icon-discover	2799/tcp	0.000000	# ICON Discover
icon-discover	2799/udp	0.000000	# ICON Discover
acc-raid	2800/tcp	0.000152	# ACC RAID
acc-raid	2800/udp	0.000000	# ACC RAID
igcp	2801/tcp	0.000000
igcp	2801/udp	0.000330
veritas-tcp1	2802/tcp	0.000000	# veritas-udp1 | Veritas TCP1 | Veritas UDP1
veritas-udp1	2802/udp	0.000000	# Veritas UDP1
btprjctrl	2803/tcp	0.000000
btprjctrl	2803/udp	0.000330
dvr-esm	2804/tcp	0.000076	# March Networks Digital Video Recorders and Enterprise Service Manager products
dvr-esm	2804/udp	0.000330	# March Networks Digital Video Recorders and Enterprise Service Manager products
wta-wsp-s	2805/tcp	0.000000	# WTA WSP-S
wta-wsp-s	2805/udp	0.000000	# WTA WSP-S
cspuni	2806/tcp	0.000076
cspuni	2806/udp	0.000000
cspmulti	2807/tcp	0.000000
cspmulti	2807/udp	0.000000
j-lan-p	2808/tcp	0.000000
j-lan-p	2808/udp	0.000000
corbaloc	2809/tcp	0.000439	# Corba | CORBA LOC
corbaloc	2809/udp	0.000000	# CORBA LOC
netsteward	2810/tcp	0.000000	# Active Net Steward
netsteward	2810/udp	0.000000	# Active Net Steward
gsiftp	2811/tcp	0.000380	# GSI FTP
gsiftp	2811/udp	0.000000	# GSI FTP
atmtcp	2812/tcp	0.000076	# commonly Monit httpd - http://mmonit.com/monit/documentation/monit.html#monit_httpd
atmtcp	2812/udp	0.000000
llm-pass	2813/tcp	0.000000
llm-pass	2813/udp	0.000330
llm-csv	2814/tcp	0.000000
llm-csv	2814/udp	0.000000
lbc-measure	2815/tcp	0.000000	# LBC Measurement
lbc-measure	2815/udp	0.000000	# LBC Measurement
lbc-watchdog	2816/tcp	0.000000	# LBC Watchdog
lbc-watchdog	2816/udp	0.000000	# LBC Watchdog
nmsigport	2817/tcp	0.000000	# NMSig Port
nmsigport	2817/udp	0.000000	# NMSig Port
rmlnk	2818/tcp	0.000000
rmlnk	2818/udp	0.000000
fc-faultnotify	2819/tcp	0.000000	# FC Fault Notification
fc-faultnotify	2819/udp	0.000661	# FC Fault Notification
univision	2820/tcp	0.000000
univision	2820/udp	0.000000
vrts-at-port	2821/tcp	0.000000	# VERITAS Authentication Service
vrts-at-port	2821/udp	0.000661	# VERITAS Authentication Service
ka0wuc	2822/tcp	0.000000
ka0wuc	2822/udp	0.000000
cqg-netlan	2823/tcp	0.000000	# CQG Net/LAN
cqg-netlan	2823/udp	0.000000	# CQG Net/LAN
cqg-netlan-1	2824/tcp	0.000000	# CQG Net/LAN 1 | CQG Net/Lan 1
cqg-netlan-1	2824/udp	0.000330	# CQG Net/Lan 1
slc-systemlog	2826/tcp	0.000000	# slc systemlog
slc-systemlog	2826/udp	0.000330	# slc systemlog
slc-ctrlrloops	2827/tcp	0.000000	# slc ctrlrloops
slc-ctrlrloops	2827/udp	0.000000	# slc ctrlrloops
itm-lm	2828/tcp	0.000000	# ITM License Manager
itm-lm	2828/udp	0.000000	# ITM License Manager
silkp1	2829/tcp	0.000000
silkp1	2829/udp	0.000000
silkp2	2830/tcp	0.000000
silkp2	2830/udp	0.000000
silkp3	2831/tcp	0.000000
silkp3	2831/udp	0.000330
silkp4	2832/tcp	0.000000
silkp4	2832/udp	0.000000
glishd	2833/tcp	0.000000
glishd	2833/udp	0.000000
evtp	2834/tcp	0.000000
evtp	2834/udp	0.000000
evtp-data	2835/tcp	0.000000
evtp-data	2835/udp	0.000000
catalyst	2836/tcp	0.000000
catalyst	2836/udp	0.000000
repliweb	2837/tcp	0.000000
repliweb	2837/udp	0.000330
starbot	2838/tcp	0.000000
starbot	2838/udp	0.000000
nmsigport	2839/tcp	0.000000
nmsigport	2839/udp	0.000000
l3-exprt	2840/tcp	0.000000
l3-exprt	2840/udp	0.000000
l3-ranger	2841/tcp	0.000000
l3-ranger	2841/udp	0.000000
l3-hawk	2842/tcp	0.000000
l3-hawk	2842/udp	0.000000
pdnet	2843/tcp	0.000000
pdnet	2843/udp	0.000000
bpcp-poll	2844/tcp	0.000000	# BPCP POLL
bpcp-poll	2844/udp	0.000000	# BPCP POLL
bpcp-trap	2845/tcp	0.000000	# BPCP TRAP
bpcp-trap	2845/udp	0.000000	# BPCP TRAP
aimpp-hello	2846/tcp	0.000000	# AIMPP Hello
aimpp-hello	2846/udp	0.000000	# AIMPP Hello
aimpp-port-req	2847/tcp	0.000076	# AIMPP Port Req
aimpp-port-req	2847/udp	0.000330	# AIMPP Port Req
amt-blc-port	2848/tcp	0.000000
amt-blc-port	2848/udp	0.000000
fxp	2849/tcp	0.000000
fxp	2849/udp	0.000000
metaconsole	2850/tcp	0.000076
metaconsole	2850/udp	0.000000
webemshttp	2851/tcp	0.000000
webemshttp	2851/udp	0.000000
bears-01	2852/tcp	0.000000
bears-01	2852/udp	0.000000
ispipes	2853/tcp	0.000000
ispipes	2853/udp	0.000000
infomover	2854/tcp	0.000000
infomover	2854/udp	0.000000
msrp	2855/tcp	0.000000	# MSRP over TCP
msrp	2855/udp	0.000330
cesdinv	2856/tcp	0.000000
cesdinv	2856/udp	0.000000
simctlp	2857/tcp	0.000000	# SimCtIP
simctlp	2857/udp	0.000000	# SimCtIP
ecnp	2858/tcp	0.000000
ecnp	2858/udp	0.000000
activememory	2859/tcp	0.000000	# Active Memory
activememory	2859/udp	0.000000	# Active Memory
dialpad-voice1	2860/tcp	0.000000	# Dialpad Voice 1
dialpad-voice1	2860/udp	0.000330	# Dialpad Voice 1
dialpad-voice2	2861/tcp	0.000000	# Dialpad Voice 2
dialpad-voice2	2861/udp	0.000000	# Dialpad Voice 2
ttg-protocol	2862/tcp	0.000000	# TTG Protocol
ttg-protocol	2862/udp	0.000000	# TTG Protocol
sonardata	2863/tcp	0.000000	# Sonar Data
sonardata	2863/udp	0.000991	# Sonar Data
astromed-main	2864/tcp	0.000000	# astronova-main | main 5001 cmd
astromed-main	2864/udp	0.000330	# main 5001 cmd
pit-vpn	2865/tcp	0.000000
pit-vpn	2865/udp	0.000330
iwlistener	2866/tcp	0.000000
iwlistener	2866/udp	0.000000
esps-portal	2867/tcp	0.000000
esps-portal	2867/udp	0.000000
npep-messaging	2868/tcp	0.000000	# NPEP Messaging | Norman Proprietaqry Events Protocol
npep-messaging	2868/udp	0.000000	# NPEP Messaging
icslap	2869/tcp	0.002129	# Universal Plug and Play Device Host, SSDP Discovery Service
icslap	2869/udp	0.000330
daishi	2870/tcp	0.000000
daishi	2870/udp	0.000000
msi-selectplay	2871/tcp	0.000000	# MSI Select Play
msi-selectplay	2871/udp	0.000000	# MSI Select Play
radix	2872/tcp	0.000000
radix	2872/udp	0.000000
psrt	2873/tcp	0.000000	# PubSub Realtime Telemetry Protocol
unknown	2873/udp	0.000330
dxmessagebase1	2874/tcp	0.000000	# DX Message Base Transport Protocol
dxmessagebase1	2874/udp	0.000330	# DX Message Base Transport Protocol
dxmessagebase2	2875/tcp	0.000380	# DX Message Base Transport Protocol
dxmessagebase2	2875/udp	0.000000	# DX Message Base Transport Protocol
sps-tunnel	2876/tcp	0.000000	# SPS Tunnel
sps-tunnel	2876/udp	0.000000	# SPS Tunnel
bluelance	2877/tcp	0.000000
bluelance	2877/udp	0.000330
aap	2878/tcp	0.000000
aap	2878/udp	0.000330
ucentric-ds	2879/tcp	0.000000
ucentric-ds	2879/udp	0.000000
synapse	2880/tcp	0.000000	# Synapse Transport
synapse	2880/udp	0.000330	# Synapse Transport
ndsp	2881/tcp	0.000000
ndsp	2881/udp	0.000330
ndtp	2882/tcp	0.000076
ndtp	2882/udp	0.000000
ndnp	2883/tcp	0.000000
ndnp	2883/udp	0.000330
flashmsg	2884/tcp	0.000000	# Flash Msg
flashmsg	2884/udp	0.000330	# Flash Msg
topflow	2885/tcp	0.000000
topflow	2885/udp	0.000330
responselogic	2886/tcp	0.000000
responselogic	2886/udp	0.000000
aironetddp	2887/tcp	0.000000	# aironet
aironetddp	2887/udp	0.000000	# aironet
spcsdlobby	2888/tcp	0.000076
spcsdlobby	2888/udp	0.000000
rsom	2889/tcp	0.000076
rsom	2889/udp	0.000330
cspclmulti	2890/tcp	0.000000
cspclmulti	2890/udp	0.000000
cinegrfx-elmd	2891/tcp	0.000000	# CINEGRFX-ELMD License Manager
cinegrfx-elmd	2891/udp	0.000000	# CINEGRFX-ELMD License Manager
snifferdata	2892/tcp	0.000000
snifferdata	2892/udp	0.000000
vseconnector	2893/tcp	0.000000
vseconnector	2893/udp	0.000000
abacus-remote	2894/tcp	0.000000
abacus-remote	2894/udp	0.000000
natuslink	2895/tcp	0.000000	# NATUS LINK
natuslink	2895/udp	0.000000	# NATUS LINK
ecovisiong6-1	2896/tcp	0.000000
ecovisiong6-1	2896/udp	0.000000
citrix-rtmp	2897/tcp	0.000000	# Citrix RTMP
citrix-rtmp	2897/udp	0.000000	# Citrix RTMP
appliance-cfg	2898/tcp	0.000076
appliance-cfg	2898/udp	0.000330
powergemplus	2899/tcp	0.000000
powergemplus	2899/udp	0.000000
quicksuite	2900/tcp	0.000000
quicksuite	2900/udp	0.000000
allstorcns	2901/tcp	0.000076
allstorcns	2901/udp	0.000330
netaspi	2902/tcp	0.000076	# NET ASPI
netaspi	2902/udp	0.000000	# NET ASPI
extensisportfolio	2903/tcp	0.000100	# suitcase | Portfolio Server by Extensis Product Group | SUITCASE
suitcase	2903/udp	0.000330
m2ua	2904/sctp	0.000000	# SIGTRAN M2UA
m2ua	2904/tcp	0.000000	# SIGTRAN M2UA
m2ua	2904/udp	0.000330	# SIGTRAN M2UA
m3ua	2905/sctp	0.000000	# SIGTRAN M3UA
m3ua	2905/tcp	0.000000	# SIGTRAN M3UA
m3ua	2905/udp	0.000000	# SIGTRAN M3UA
caller9	2906/tcp	0.000000
caller9	2906/udp	0.000000
webmethods-b2b	2907/tcp	0.000000	# WEBMETHODS B2B
webmethods-b2b	2907/udp	0.000000	# WEBMETHODS B2B
mao	2908/tcp	0.000076
mao	2908/udp	0.000661
funk-dialout	2909/tcp	0.000228	# Funk Dialout
funk-dialout	2909/udp	0.000330	# Funk Dialout
tdaccess	2910/tcp	0.000152
tdaccess	2910/udp	0.000330
blockade	2911/tcp	0.000000
blockade	2911/udp	0.000000
epicon	2912/tcp	0.000000
epicon	2912/udp	0.000000
boosterware	2913/tcp	0.000000	# Booster Ware
boosterware	2913/udp	0.000000	# Booster Ware
gamelobby	2914/tcp	0.000000	# Game Lobby
gamelobby	2914/udp	0.000000	# Game Lobby
tksocket	2915/tcp	0.000000	# TK Socket
tksocket	2915/udp	0.000000	# TK Socket
elvin_server	2916/tcp	0.000000	# elvin-server | Elvin Server
elvin_server	2916/udp	0.000330	# Elvin Server
elvin_client	2917/tcp	0.000000	# elvin-client | Elvin Client
elvin_client	2917/udp	0.000000	# Elvin Client
kastenchasepad	2918/tcp	0.000000	# Kasten Chase Pad
kastenchasepad	2918/udp	0.000000	# Kasten Chase Pad
roboer	2919/tcp	0.000000
roboer	2919/udp	0.000330
roboeda	2920/tcp	0.000152
roboeda	2920/udp	0.000000
cesdcdman	2921/tcp	0.000000	# CESD Contents Delivery Management
cesdcdman	2921/udp	0.000000	# CESD Contents Delivery Management
cesdcdtrn	2922/tcp	0.000000	# CESD Contents Delivery Data Transfer
cesdcdtrn	2922/udp	0.000000	# CESD Contents Delivery Data Transfer
wta-wsp-wtp-s	2923/tcp	0.000000
wta-wsp-wtp-s	2923/udp	0.000000
precise-vip	2924/tcp	0.000000
precise-vip	2924/udp	0.000000
mobile-file-dl	2926/tcp	0.000000
mobile-file-dl	2926/udp	0.000000
unimobilectrl	2927/tcp	0.000000
unimobilectrl	2927/udp	0.000000
redstone-cpss	2928/tcp	0.000000
redstone-cpss	2928/udp	0.000330
amx-webadmin	2929/tcp	0.000000
amx-webadmin	2929/udp	0.000000
amx-weblinx	2930/tcp	0.000076
amx-weblinx	2930/udp	0.000000
circle-x	2931/tcp	0.000000
circle-x	2931/udp	0.000000
incp	2932/tcp	0.000000
incp	2932/udp	0.000330
4-tieropmgw	2933/tcp	0.000000	# 4-TIER OPM GW
4-tieropmgw	2933/udp	0.000000	# 4-TIER OPM GW
4-tieropmcli	2934/tcp	0.000000	# 4-TIER OPM CLI
4-tieropmcli	2934/udp	0.000000	# 4-TIER OPM CLI
qtp	2935/tcp	0.000000
qtp	2935/udp	0.000000
otpatch	2936/tcp	0.000000
otpatch	2936/udp	0.000000
pnaconsult-lm	2937/tcp	0.000000
pnaconsult-lm	2937/udp	0.000000
sm-pas-1	2938/tcp	0.000000
sm-pas-1	2938/udp	0.000000
sm-pas-2	2939/tcp	0.000000
sm-pas-2	2939/udp	0.000000
sm-pas-3	2940/tcp	0.000000
sm-pas-3	2940/udp	0.000330
sm-pas-4	2941/tcp	0.000000
sm-pas-4	2941/udp	0.000000
sm-pas-5	2942/tcp	0.000000
sm-pas-5	2942/udp	0.000000
ttnrepository	2943/tcp	0.000000
ttnrepository	2943/udp	0.000000
megaco-h248	2944/sctp	0.000000	# Megaco H-248 (Text) | Megaco H-248 | Megaco-H.248 text
megaco-h248	2944/tcp	0.000000	# Megaco H-248 (Text)
megaco-h248	2944/udp	0.000330	# Megaco H-248 (Text)
h248-binary	2945/sctp	0.000000	# Megaco H-248 (Binary) | H248 Binary | Megaco/H.248 binary
h248-binary	2945/tcp	0.000000	# Megaco H-248 (Binary)
h248-binary	2945/udp	0.000000	# Megaco H-248 (Binary)
fjsvmpor	2946/tcp	0.000000
fjsvmpor	2946/udp	0.000000
gpsd	2947/tcp	0.000000	# GPS Daemon request/response protocol
gpsd	2947/udp	0.000000	# GPS Daemon request/response protocol
wap-push	2948/tcp	0.000000	# WAP PUSH
wap-push	2948/udp	0.000791	# Windows Mobile devices often have this
wap-pushsecure	2949/tcp	0.000000	# WAP PUSH SECURE
wap-pushsecure	2949/udp	0.000000	# WAP PUSH SECURE
esip	2950/tcp	0.000000
esip	2950/udp	0.000330
ottp	2951/tcp	0.000000
ottp	2951/udp	0.000330
mpfwsas	2952/tcp	0.000000
mpfwsas	2952/udp	0.000000
ovalarmsrv	2953/tcp	0.000000
ovalarmsrv	2953/udp	0.000000
ovalarmsrv-cmd	2954/tcp	0.000000
ovalarmsrv-cmd	2954/udp	0.000000
csnotify	2955/tcp	0.000000
csnotify	2955/udp	0.000000
ovrimosdbman	2956/tcp	0.000000
ovrimosdbman	2956/udp	0.000330
jmact5	2957/tcp	0.000076	# JAMCT5
jmact5	2957/udp	0.000000	# JAMCT5
jmact6	2958/tcp	0.000076	# JAMCT6
jmact6	2958/udp	0.000000	# JAMCT6
rmopagt	2959/tcp	0.000000
rmopagt	2959/udp	0.000000
dfoxserver	2960/tcp	0.000000
dfoxserver	2960/udp	0.000000
boldsoft-lm	2961/tcp	0.000000
boldsoft-lm	2961/udp	0.000000
iph-policy-cli	2962/tcp	0.000000
iph-policy-cli	2962/udp	0.000000
iph-policy-adm	2963/tcp	0.000000
iph-policy-adm	2963/udp	0.000000
bullant-srap	2964/tcp	0.000000	# BULLANT SRAP
bullant-srap	2964/udp	0.000330	# BULLANT SRAP
bullant-rap	2965/tcp	0.000000	# BULLANT RAP
bullant-rap	2965/udp	0.000000	# BULLANT RAP
idp-infotrieve	2966/tcp	0.000000
idp-infotrieve	2966/udp	0.000000
symantec-av	2967/tcp	0.002357	# ssc-agent | Symantec AntiVirus (rtvscan.exe) | SSC-AGENT
symantec-av	2967/udp	0.006425	# Symantec AntiVirus (rtvscan.exe)
enpp	2968/tcp	0.000152
enpp	2968/udp	0.000000
essp	2969/tcp	0.000000
essp	2969/udp	0.000330
index-net	2970/tcp	0.000000
index-net	2970/udp	0.000330
netclip	2971/tcp	0.000000	# NetClip clipboard daemon
netclip	2971/udp	0.000000	# NetClip clipboard daemon
pmsm-webrctl	2972/tcp	0.000000	# PMSM Webrctl
pmsm-webrctl	2972/udp	0.000330	# PMSM Webrctl
svnetworks	2973/tcp	0.000076	# SV Networks
svnetworks	2973/udp	0.000991	# SV Networks
signal	2974/tcp	0.000000
signal	2974/udp	0.000000
fjmpcm	2975/tcp	0.000000	# Fujitsu Configuration Management Service
fjmpcm	2975/udp	0.000000	# Fujitsu Configuration Management Service
cns-srv-port	2976/tcp	0.000000	# CNS Server Port
cns-srv-port	2976/udp	0.000000	# CNS Server Port
ttc-etap-ns	2977/tcp	0.000000	# TTCs Enterprise Test Access Protocol - NS
ttc-etap-ns	2977/udp	0.000000	# TTCs Enterprise Test Access Protocol - NS
ttc-etap-ds	2978/tcp	0.000000	# TTCs Enterprise Test Access Protocol - DS
ttc-etap-ds	2978/udp	0.000000	# TTCs Enterprise Test Access Protocol - DS
h263-video	2979/tcp	0.000000	# H.263 Video Streaming
h263-video	2979/udp	0.000000	# H.263 Video Streaming
wimd	2980/tcp	0.000000	# Instant Messaging Service
wimd	2980/udp	0.000000	# Instant Messaging Service
mylxamport	2981/tcp	0.000000
mylxamport	2981/udp	0.000000
iwb-whiteboard	2982/tcp	0.000000
iwb-whiteboard	2982/udp	0.000000
netplan	2983/tcp	0.000000
netplan	2983/udp	0.000000
hpidsadmin	2984/tcp	0.000076
hpidsadmin	2984/udp	0.000000
hpidsagent	2985/tcp	0.000000
hpidsagent	2985/udp	0.000000
stonefalls	2986/tcp	0.000000
stonefalls	2986/udp	0.000000
identify	2987/tcp	0.000076
identify	2987/udp	0.000330
hippad	2988/tcp	0.000076	# HIPPA Reporting Protocol
hippad	2988/udp	0.000000	# HIPPA Reporting Protocol
zarkov	2989/tcp	0.000000	# ZARKOV Intelligent Agent Communication
zarkov	2989/udp	0.000000	# ZARKOV Intelligent Agent Communication
boscap	2990/tcp	0.000000
boscap	2990/udp	0.000000
wkstn-mon	2991/tcp	0.000076
wkstn-mon	2991/udp	0.000000
avenyo	2992/tcp	0.000000	# Avenyo Server
avenyo	2992/udp	0.000000	# Avenyo Server
veritas-vis1	2993/tcp	0.000000	# VERITAS VIS1
veritas-vis1	2993/udp	0.000000	# VERITAS VIS1
veritas-vis2	2994/tcp	0.000000	# VERITAS VIS2
veritas-vis2	2994/udp	0.000330	# VERITAS VIS2
idrs	2995/tcp	0.000000
idrs	2995/udp	0.000000
vsixml	2996/tcp	0.000000
vsixml	2996/udp	0.000330
rebol	2997/tcp	0.000076
rebol	2997/udp	0.000000
iss-realsec	2998/tcp	0.000351	# realsecure | ISS RealSecure IDS Remote Console Admin port | Real Secure
realsecure	2998/udp	0.000000	# Real Secure
remoteware-un	2999/tcp	0.000000	# RemoteWare Unassigned
remoteware-un	2999/udp	0.000000	# RemoteWare Unassigned
ppp	3000/tcp	0.004115	# remoteware-cl | hbci | User-level ppp daemon, or chili!soft asp | HBCI | RemoteWare Client
hbci	3000/udp	0.000000
nessus	3001/tcp	0.003124	# origo-native | Nessus Security Scanner (www.nessus.org) Daemon or chili!soft asp | OrigoDB Server Native Interface
unknown	3001/udp	0.000991
exlm-agent	3002/tcp	0.000076	# remoteware-srv | EXLM Agent | RemoteWare Server
exlm-agent	3002/udp	0.000661	# EXLM Agent
cgms	3003/tcp	0.000228
cgms	3003/udp	0.000330
csoftragent	3004/tcp	0.000000	# Csoft Agent
csoftragent	3004/udp	0.000000	# Csoft Agent
deslogin	3005/tcp	0.000477	# geniuslm | encrypted symmetric telnet/login | Genius License Manager
geniuslm	3005/udp	0.000330	# Genius License Manager
deslogind	3006/tcp	0.000263	# ii-admin | Instant Internet Admin
ii-admin	3006/udp	0.000000	# Instant Internet Admin
lotusmtap	3007/tcp	0.000152	# Lotus Mail Tracking Agent Protocol
lotusmtap	3007/udp	0.000000	# Lotus Mail Tracking Agent Protocol
midnight-tech	3008/tcp	0.000000	# Midnight Technologies
midnight-tech	3008/udp	0.000000	# Midnight Technologies
pxc-ntfy	3009/tcp	0.000000
pxc-ntfy	3009/udp	0.000000
gw	3010/tcp	0.000000	# ping-pong | Telerate Workstation
ping-pong	3010/udp	0.000000	# Telerate Workstation
trusted-web	3011/tcp	0.000304	# Trusted Web
trusted-web	3011/udp	0.000000	# Trusted Web
twsdss	3012/tcp	0.000000	# Trusted Web Client
twsdss	3012/udp	0.000000	# Trusted Web Client
gilatskysurfer	3013/tcp	0.000152	# Gilat Sky Surfer
gilatskysurfer	3013/udp	0.000000	# Gilat Sky Surfer
broker_service	3014/tcp	0.000076	# broker-service | Broker Service
broker_service	3014/udp	0.000000	# Broker Service
nati-dstp	3015/tcp	0.000000	# NATI DSTP
nati-dstp	3015/udp	0.000000	# NATI DSTP
notify_srvr	3016/tcp	0.000000	# notify-srvr | Notify Server
notify_srvr	3016/udp	0.000000	# Notify Server
event_listener	3017/tcp	0.000380	# event-listener | Event Listener
event_listener	3017/udp	0.000000	# Event Listener
srvc_registry	3018/tcp	0.000000	# srvc-registry | Service Registry
srvc_registry	3018/udp	0.000000	# Service Registry
resource_mgr	3019/tcp	0.000000	# resource-mgr | Resource Manager
resource_mgr	3019/udp	0.000000	# Resource Manager
cifs	3020/tcp	0.000000
cifs	3020/udp	0.000000
agriserver	3021/tcp	0.000000	# AGRI Server
agriserver	3021/udp	0.000000	# AGRI Server
csregagent	3022/tcp	0.000000
csregagent	3022/udp	0.000000
magicnotes	3023/tcp	0.000076
magicnotes	3023/udp	0.000000
nds_sso	3024/tcp	0.000000	# nds-sso
nds_sso	3024/udp	0.000000
slnp	3025/tcp	0.000125	# arepa-raft | SLNP (Simple Library Network Protocol) by Sisis Informationssysteme GmbH | Arepa Raft
arepa-raft	3025/udp	0.000000	# Arepa Raft
agri-gateway	3026/tcp	0.000000	# AGRI Gateway
agri-gateway	3026/udp	0.000000	# AGRI Gateway
LiebDevMgmt_C	3027/tcp	0.000000	# LiebDevMgmt-C
LiebDevMgmt_C	3027/udp	0.000000
LiebDevMgmt_DM	3028/tcp	0.000000	# LiebDevMgmt-DM
LiebDevMgmt_DM	3028/udp	0.000000
LiebDevMgmt_A	3029/tcp	0.000000	# LiebDevMgmt-A
LiebDevMgmt_A	3029/udp	0.000000
arepa-cas	3030/tcp	0.000304	# Arepa Cas
arepa-cas	3030/udp	0.000330	# Arepa Cas
eppc	3031/tcp	0.000380	# Remote AppleEvents/PPC Toolbox
eppc	3031/udp	0.000000	# Remote AppleEvents/PPC Toolbox
redwood-chat	3032/tcp	0.000000	# Redwood Chat
redwood-chat	3032/udp	0.000000	# Redwood Chat
pdb	3033/tcp	0.000000
pdb	3033/udp	0.000000
osmosis-aeea	3034/tcp	0.000000	# Osmosis / Helix (R) AEEA Port
osmosis-aeea	3034/udp	0.000000	# Osmosis / Helix (R) AEEA Port
fjsv-gssagt	3035/tcp	0.000000	# FJSV gssagt
fjsv-gssagt	3035/udp	0.000000	# FJSV gssagt
hagel-dump	3036/tcp	0.000000	# Hagel DUMP
hagel-dump	3036/udp	0.000330	# Hagel DUMP
hp-san-mgmt	3037/tcp	0.000000	# HP SAN Mgmt
hp-san-mgmt	3037/udp	0.000000	# HP SAN Mgmt
santak-ups	3038/tcp	0.000000	# Santak UPS
santak-ups	3038/udp	0.000000	# Santak UPS
cogitate	3039/tcp	0.000000	# Cogitate, Inc.
cogitate	3039/udp	0.000000	# Cogitate, Inc.
tomato-springs	3040/tcp	0.000000	# Tomato Springs
tomato-springs	3040/udp	0.000000	# Tomato Springs
di-traceware	3041/tcp	0.000000
di-traceware	3041/udp	0.000000
journee	3042/tcp	0.000000
journee	3042/udp	0.000000
brp	3043/tcp	0.000000	# Broadcast Routing Protocol
brp	3043/udp	0.000000	# Broadcast Routing Protocol
epp	3044/tcp	0.000000	# EndPoint Protocol
epp	3044/udp	0.000000	# EndPoint Protocol
slnp	3045/tcp	0.000063	# responsenet | SLNP (Simple Library Network Protocol) by Sisis Informationssysteme GmbH | ResponseNet
responsenet	3045/udp	0.000000
di-ase	3046/tcp	0.000000
di-ase	3046/udp	0.000330
hlserver	3047/tcp	0.000000	# Fast Security HL Server
hlserver	3047/udp	0.000000	# Fast Security HL Server
pctrader	3048/tcp	0.000000	# Sierra Net PC Trader
pctrader	3048/udp	0.000661	# Sierra Net PC Trader
cfs	3049/tcp	0.000063	# nsws | cryptographic file system (nfs) (proposed) | NSWS
cfs	3049/udp	0.000675	# cryptographic file system (nfs)
gds_db	3050/tcp	0.000152	# gds-db
gds_db	3050/udp	0.000330
galaxy-server	3051/tcp	0.000000	# Galaxy Server
galaxy-server	3051/udp	0.000000	# Galaxy Server
powerchute	3052/tcp	0.000966	# apc-3052 | APC 3052
apc-3052	3052/udp	0.003304	# APC 3052
dsom-server	3053/tcp	0.000000
dsom-server	3053/udp	0.000000
amt-cnf-prot	3054/tcp	0.000000	# AMT CNF PROT
amt-cnf-prot	3054/udp	0.000661	# AMT CNF PROT
policyserver	3055/tcp	0.000000	# Policy Server
policyserver	3055/udp	0.000000	# Policy Server
cdl-server	3056/tcp	0.000000	# CDL Server
cdl-server	3056/udp	0.000000	# CDL Server
goahead-fldup	3057/tcp	0.000076	# GoAhead FldUp
goahead-fldup	3057/udp	0.000000	# GoAhead FldUp
videobeans	3058/tcp	0.000000
videobeans	3058/udp	0.000000
qsoft	3059/tcp	0.000000
qsoft	3059/udp	0.000000
interserver	3060/tcp	0.000000
interserver	3060/udp	0.000330
cautcpd	3061/tcp	0.000000
cautcpd	3061/udp	0.000330
ncacn-ip-tcp	3062/tcp	0.000076
ncacn-ip-tcp	3062/udp	0.000000
ncadg-ip-udp	3063/tcp	0.000076
ncadg-ip-udp	3063/udp	0.000000
dnet-tstproxy	3064/tcp	0.000063	# rprt | distributed.net (a closed source crypto-cracking project) proxy test port | Remote Port Redirector
rprt	3064/udp	0.000000	# Remote Port Redirector
slinterbase	3065/tcp	0.000000
slinterbase	3065/udp	0.000000
netattachsdmp	3066/tcp	0.000000
netattachsdmp	3066/udp	0.000330
fjhpjp	3067/tcp	0.000000
fjhpjp	3067/udp	0.000330
ls3bcast	3068/tcp	0.000000	# ls3 Broadcast
ls3bcast	3068/udp	0.000000	# ls3 Broadcast
ls3	3069/tcp	0.000000
ls3	3069/udp	0.000000
mgxswitch	3070/tcp	0.000000
mgxswitch	3070/udp	0.000000
csd-mgmt-port	3071/tcp	0.000380	# xplat-replicate | ContinuStor Manager Port | Crossplatform replication protocol
csd-mgmt-port	3071/udp	0.000000	# ContinuStor Manager Port
csd-monitor	3072/tcp	0.000000	# ContinuStor Monitor Port
csd-monitor	3072/udp	0.000000	# ContinuStor Monitor Port
vcrp	3073/tcp	0.000000	# Very simple chatroom prot
vcrp	3073/udp	0.000000	# Very simple chatroom prot
xbox	3074/tcp	0.000000	# Xbox game port
xbox	3074/udp	0.000000	# Xbox game port
orbix-locator	3075/tcp	0.000000	# Orbix 2000 Locator
orbix-locator	3075/udp	0.000330	# Orbix 2000 Locator
orbix-config	3076/tcp	0.000000	# Orbix 2000 Config
orbix-config	3076/udp	0.000330	# Orbix 2000 Config
orbix-loc-ssl	3077/tcp	0.000304	# Orbix 2000 Locator SSL
orbix-loc-ssl	3077/udp	0.000000	# Orbix 2000 Locator SSL
orbix-cfg-ssl	3078/tcp	0.000000	# Orbix 2000 Locator SSL
orbix-cfg-ssl	3078/udp	0.000000	# Orbix 2000 Locator SSL
lv-frontpanel	3079/tcp	0.000000	# LV Front Panel
lv-frontpanel	3079/udp	0.000000	# LV Front Panel
stm_pproc	3080/tcp	0.000076	# stm-pproc
stm_pproc	3080/udp	0.000000
tl1-lv	3081/tcp	0.000000
tl1-lv	3081/udp	0.000000
tl1-raw	3082/tcp	0.000000
tl1-raw	3082/udp	0.000000
tl1-telnet	3083/tcp	0.000000
tl1-telnet	3083/udp	0.000000
itm-mccs	3084/tcp	0.000000
itm-mccs	3084/udp	0.000000
pcihreq	3085/tcp	0.000000
pcihreq	3085/udp	0.000000
sj3	3086/tcp	0.000050	# jdl-dbkitchen | SJ3 (kanji input) | JDL-DBKitchen
jdl-dbkitchen	3086/udp	0.000000
asoki-sma	3087/tcp	0.000000	# Asoki SMA
asoki-sma	3087/udp	0.000000	# Asoki SMA
xdtp	3088/tcp	0.000000	# eXtensible Data Transfer Protocol
xdtp	3088/udp	0.000000	# eXtensible Data Transfer Protocol
ptk-alink	3089/tcp	0.000076	# ParaTek Agent Linking
ptk-alink	3089/udp	0.000000	# ParaTek Agent Linking
stss	3090/tcp	0.000000	# Senforce Session Services
stss	3090/udp	0.000000	# Senforce Session Services
1ci-smcs	3091/tcp	0.000000	# 1Ci Server Management
1ci-smcs	3091/udp	0.000000	# 1Ci Server Management
rapidmq-center	3093/tcp	0.000000	# Jiiva RapidMQ Center
rapidmq-center	3093/udp	0.000000	# Jiiva RapidMQ Center
rapidmq-reg	3094/tcp	0.000000	# Jiiva RapidMQ Registry
rapidmq-reg	3094/udp	0.000661	# Jiiva RapidMQ Registry
panasas	3095/tcp	0.000000	# Panasas rendevous port | Panasas rendezvous port
panasas	3095/udp	0.000000	# Panasas rendevous port
ndl-aps	3096/tcp	0.000000	# Active Print Server Port
ndl-aps	3096/udp	0.000000	# Active Print Server Port
itu-bicc-stc	3097/sctp	0.000000	# ITU-T Q.1902.1/Q.2150.3
umm-port	3098/tcp	0.000000	# Universal Message Manager
umm-port	3098/udp	0.000000	# Universal Message Manager
chmd	3099/tcp	0.000000	# CHIPSY Machine Daemon
chmd	3099/udp	0.000330	# CHIPSY Machine Daemon
opcon-xps	3100/tcp	0.000000	# OpCon/xps
opcon-xps	3100/udp	0.000000	# OpCon/xps
hp-pxpib	3101/tcp	0.000000	# HP PolicyXpert PIB Server
hp-pxpib	3101/udp	0.000000	# HP PolicyXpert PIB Server
sl-mon	3102/tcp	0.000076	# slslavemon | SoftlinK Mon Port | SoftlinK Slave Mon Port
sl-mon	3102/udp	0.000330	# SoftlinK Mon Port
autocuesmi	3103/tcp	0.000076	# Autocue SMI Protocol
autocuesmi	3103/udp	0.000000	# Autocue SMI Protocol
autocuelog	3104/tcp	0.000000	# autocuetime | Autocue Logger Protocol | Autocue Time Service
autocuetime	3104/udp	0.000330	# Autocue Time Service
cardbox	3105/tcp	0.000000
cardbox	3105/udp	0.000000
cardbox-http	3106/tcp	0.000000	# Cardbox HTTP
cardbox-http	3106/udp	0.000000	# Cardbox HTTP
business	3107/tcp	0.000000	# Business protocol
business	3107/udp	0.000000	# Business protocol
geolocate	3108/tcp	0.000000	# Geolocate protocol
geolocate	3108/udp	0.000000	# Geolocate protocol
personnel	3109/tcp	0.000000	# Personnel protocol
personnel	3109/udp	0.000000	# Personnel protocol
sim-control	3110/tcp	0.000000	# simulator control port
sim-control	3110/udp	0.000330	# simulator control port
wsynch	3111/tcp	0.000000	# Web Synchronous Services
wsynch	3111/udp	0.000000	# Web Synchronous Services
ksysguard	3112/tcp	0.000000	# KDE System Guard
ksysguard	3112/udp	0.000000	# KDE System Guard
cs-auth-svr	3113/tcp	0.000000	# CS-Authenticate Svr Port
cs-auth-svr	3113/udp	0.000330	# CS-Authenticate Svr Port
ccmad	3114/tcp	0.000000	# CCM AutoDiscover
ccmad	3114/udp	0.000000	# CCM AutoDiscover
mctet-master	3115/tcp	0.000000	# MCTET Master
mctet-master	3115/udp	0.000000	# MCTET Master
mctet-gateway	3116/tcp	0.000000	# MCTET Gateway
mctet-gateway	3116/udp	0.000000	# MCTET Gateway
mctet-jserv	3117/tcp	0.000000	# MCTET Jserv
mctet-jserv	3117/udp	0.000000	# MCTET Jserv
pkagent	3118/tcp	0.000076
pkagent	3118/udp	0.000000
d2000kernel	3119/tcp	0.000152	# D2000 Kernel Port
d2000kernel	3119/udp	0.000000	# D2000 Kernel Port
d2000webserver	3120/tcp	0.000000	# D2000 Webserver Port
d2000webserver	3120/udp	0.000000	# D2000 Webserver Port
pcmk-remote	3121/tcp	0.000076	# The pacemaker remote (pcmk-remote) service extends high availability functionality outside of the Linux cluster into remote nodes.
vtr-emulator	3122/tcp	0.000000	# MTI VTR Emulator port
vtr-emulator	3122/udp	0.000000	# MTI VTR Emulator port
edix	3123/tcp	0.000000	# EDI Translation Protocol
edix	3123/udp	0.000000	# EDI Translation Protocol
beacon-port	3124/tcp	0.000000	# Beacon Port
beacon-port	3124/udp	0.000000	# Beacon Port
a13-an	3125/tcp	0.000000	# A13-AN Interface
a13-an	3125/udp	0.000000	# A13-AN Interface
ctx-bridge	3127/tcp	0.000000	# CTX Bridge Port
ctx-bridge	3127/udp	0.000000	# CTX Bridge Port
squid-http	3128/tcp	0.004516	# ndl-aas | Active API Server Port
ndl-aas	3128/udp	0.000000	# Active API Server Port
netport-id	3129/tcp	0.000000	# NetPort Discovery Port
netport-id	3129/udp	0.000000	# NetPort Discovery Port
icpv2	3130/tcp	0.000000
squid-ipc	3130/udp	0.006656
netbookmark	3131/tcp	0.000000	# Net Book Mark
netbookmark	3131/udp	0.000330	# Net Book Mark
ms-rule-engine	3132/tcp	0.000000	# Microsoft Business Rule Engine Update Service
ms-rule-engine	3132/udp	0.000000	# Microsoft Business Rule Engine Update Service
prism-deploy	3133/tcp	0.000000	# Prism Deploy User Port
prism-deploy	3133/udp	0.000000	# Prism Deploy User Port
ecp	3134/tcp	0.000000	# Extensible Code Protocol
ecp	3134/udp	0.000000	# Extensible Code Protocol
peerbook-port	3135/tcp	0.000000	# PeerBook Port
peerbook-port	3135/udp	0.000000	# PeerBook Port
grubd	3136/tcp	0.000000	# Grub Server Port
grubd	3136/udp	0.000000	# Grub Server Port
rtnt-1	3137/tcp	0.000000	# rtnt-1 data packets
rtnt-1	3137/udp	0.000000	# rtnt-1 data packets
rtnt-2	3138/tcp	0.000000	# rtnt-2 data packets
rtnt-2	3138/udp	0.000000	# rtnt-2 data packets
incognitorv	3139/tcp	0.000000	# Incognito Rendez-Vous
incognitorv	3139/udp	0.000000	# Incognito Rendez-Vous
ariliamulti	3140/tcp	0.000000	# Arilia Multiplexor
ariliamulti	3140/udp	0.000000	# Arilia Multiplexor
vmodem	3141/tcp	0.000038
vmodem	3141/udp	0.000560
apt-cacher	3142/tcp	0.000000	# rdc-wh-eos | A server which keeps a local cache of Debian/Ubuntu package files | RDC WH EOS
rdc-wh-eos	3142/udp	0.000000	# RDC WH EOS
seaview	3143/tcp	0.000000	# Sea View
seaview	3143/udp	0.000000	# Sea View
tarantella	3144/tcp	0.000000
tarantella	3144/udp	0.000000
csi-lfap	3145/tcp	0.000000
csi-lfap	3145/udp	0.000000
bears-02	3146/tcp	0.000076
bears-02	3146/udp	0.000000
rfio	3147/tcp	0.000000
rfio	3147/udp	0.000330
nm-game-admin	3148/tcp	0.000000	# NetMike Game Administrator
nm-game-admin	3148/udp	0.000330	# NetMike Game Administrator
nm-game-server	3149/tcp	0.000000	# NetMike Game Server
nm-game-server	3149/udp	0.000000	# NetMike Game Server
nm-asses-admin	3150/tcp	0.000000	# NetMike Assessor Administrator
nm-asses-admin	3150/udp	0.000000	# NetMike Assessor Administrator
nm-assessor	3151/tcp	0.000000	# NetMike Assessor
nm-assessor	3151/udp	0.000000	# NetMike Assessor
feitianrockey	3152/tcp	0.000000	# FeiTian Port
feitianrockey	3152/udp	0.000000	# FeiTian Port
s8-client-port	3153/tcp	0.000000	# S8Cargo Client Port
s8-client-port	3153/udp	0.000000	# S8Cargo Client Port
ccmrmi	3154/tcp	0.000000	# ON RMI Registry
ccmrmi	3154/udp	0.000000	# ON RMI Registry
jpegmpeg	3155/tcp	0.000000	# JpegMpeg Port
jpegmpeg	3155/udp	0.000000	# JpegMpeg Port
indura	3156/tcp	0.000000	# Indura Collector
indura	3156/udp	0.000330	# Indura Collector
e3consultants	3157/tcp	0.000000	# lsa-comm | CCC Listener Port | LSA Communicator
e3consultants	3157/udp	0.000000	# CCC Listener Port
stvp	3158/tcp	0.000000	# SmashTV Protocol
stvp	3158/udp	0.000000	# SmashTV Protocol
navegaweb-port	3159/tcp	0.000000	# NavegaWeb Tarification
navegaweb-port	3159/udp	0.000000	# NavegaWeb Tarification
tip-app-server	3160/tcp	0.000000	# TIP Application Server
tip-app-server	3160/udp	0.000330	# TIP Application Server
doc1lm	3161/tcp	0.000000	# DOC1 License Manager
doc1lm	3161/udp	0.000000	# DOC1 License Manager
sflm	3162/tcp	0.000152
sflm	3162/udp	0.000661
res-sap	3163/tcp	0.000000
res-sap	3163/udp	0.000000
imprs	3164/tcp	0.000000
imprs	3164/udp	0.000000
newgenpay	3165/tcp	0.000000	# Newgenpay Engine Service
newgenpay	3165/udp	0.000330	# Newgenpay Engine Service
sossecollector	3166/tcp	0.000000	# Quest Spotlight Out-Of-Process Collector
sossecollector	3166/udp	0.000000	# Quest Spotlight Out-Of-Process Collector
nowcontact	3167/tcp	0.000076	# Now Contact Public Server
nowcontact	3167/udp	0.000000	# Now Contact Public Server
poweronnud	3168/tcp	0.000228	# Now Up-to-Date Public Server
poweronnud	3168/udp	0.000000	# Now Up-to-Date Public Server
serverview-as	3169/tcp	0.000000
serverview-as	3169/udp	0.000330
serverview-asn	3170/tcp	0.000000
serverview-asn	3170/udp	0.000330
serverview-gf	3171/tcp	0.000000
serverview-gf	3171/udp	0.000000
serverview-rm	3172/tcp	0.000000
serverview-rm	3172/udp	0.000000
serverview-icc	3173/tcp	0.000000
serverview-icc	3173/udp	0.000330
armi-server	3174/tcp	0.000000	# ARMI Server
armi-server	3174/udp	0.000000	# ARMI Server
t1-e1-over-ip	3175/tcp	0.000000	# T1_E1_Over_IP
t1-e1-over-ip	3175/udp	0.000000	# T1_E1_Over_IP
ars-master	3176/tcp	0.000000	# ARS Master
ars-master	3176/udp	0.000000	# ARS Master
phonex-port	3177/tcp	0.000000	# Phonex Protocol
phonex-port	3177/udp	0.000000	# Phonex Protocol
radclientport	3178/tcp	0.000000	# Radiance UltraEdge Port
radclientport	3178/udp	0.000000	# Radiance UltraEdge Port
h2gf-w-2m	3179/tcp	0.000000	# H2GF W.2m Handover prot.
h2gf-w-2m	3179/udp	0.000330	# H2GF W.2m Handover prot.
mc-brk-srv	3180/tcp	0.000000	# Millicent Broker Server
mc-brk-srv	3180/udp	0.000000	# Millicent Broker Server
bmcpatrolagent	3181/tcp	0.000000	# BMC Patrol Agent
bmcpatrolagent	3181/udp	0.000000	# BMC Patrol Agent
bmcpatrolrnvu	3182/tcp	0.000000	# BMC Patrol Rendezvous
bmcpatrolrnvu	3182/udp	0.000000	# BMC Patrol Rendezvous
cops-tls	3183/tcp	0.000000	# COPS/TLS
cops-tls	3183/udp	0.000000	# COPS/TLS
apogeex-port	3184/tcp	0.000000	# ApogeeX Port
apogeex-port	3184/udp	0.000000	# ApogeeX Port
smpppd	3185/tcp	0.000000	# SuSE Meta PPPD
smpppd	3185/udp	0.000000	# SuSE Meta PPPD
iiw-port	3186/tcp	0.000000	# IIW Monitor User Port
iiw-port	3186/udp	0.000000	# IIW Monitor User Port
odi-port	3187/tcp	0.000000	# Open Design Listen Port
odi-port	3187/udp	0.000000	# Open Design Listen Port
brcm-comm-port	3188/tcp	0.000000	# Broadcom Port
brcm-comm-port	3188/udp	0.000000	# Broadcom Port
pcle-infex	3189/tcp	0.000000	# Pinnacle Sys InfEx Port
pcle-infex	3189/udp	0.000000	# Pinnacle Sys InfEx Port
csvr-proxy	3190/tcp	0.000076	# ConServR Proxy
csvr-proxy	3190/udp	0.000000	# ConServR Proxy
csvr-sslproxy	3191/tcp	0.000000	# ConServR SSL Proxy
csvr-sslproxy	3191/udp	0.000000	# ConServR SSL Proxy
firemonrcc	3192/tcp	0.000000	# FireMon Revision Control
firemonrcc	3192/udp	0.000000	# FireMon Revision Control
spandataport	3193/tcp	0.000000
spandataport	3193/udp	0.000000
magbind	3194/tcp	0.000000	# Rockstorm MAG protocol
magbind	3194/udp	0.000000	# Rockstorm MAG protocol
ncu-1	3195/tcp	0.000000	# Network Control Unit
ncu-1	3195/udp	0.000000	# Network Control Unit
ncu-2	3196/tcp	0.000000	# Network Control Unit
ncu-2	3196/udp	0.000000	# Network Control Unit
embrace-dp-s	3197/tcp	0.000000	# Embrace Device Protocol Server
embrace-dp-s	3197/udp	0.000000	# Embrace Device Protocol Server
embrace-dp-c	3198/tcp	0.000000	# Embrace Device Protocol Client
embrace-dp-c	3198/udp	0.000000	# Embrace Device Protocol Client
dmod-workspace	3199/tcp	0.000000	# DMOD WorkSpace
dmod-workspace	3199/udp	0.000000	# DMOD WorkSpace
tick-port	3200/tcp	0.000076	# Press-sense Tick Port
tick-port	3200/udp	0.000000	# Press-sense Tick Port
cpq-tasksmart	3201/tcp	0.000000
cpq-tasksmart	3201/udp	0.000330
intraintra	3202/tcp	0.000000
intraintra	3202/udp	0.000000
netwatcher-mon	3203/tcp	0.000000	# Network Watcher Monitor
netwatcher-mon	3203/udp	0.000330	# Network Watcher Monitor
netwatcher-db	3204/tcp	0.000000	# Network Watcher DB Access
netwatcher-db	3204/udp	0.000000	# Network Watcher DB Access
isns	3205/tcp	0.000000	# iSNS Server Port
isns	3205/udp	0.000000	# iSNS Server Port
ironmail	3206/tcp	0.000000	# IronMail POP Proxy
ironmail	3206/udp	0.000000	# IronMail POP Proxy
vx-auth-port	3207/tcp	0.000000	# Veritas Authentication Port
vx-auth-port	3207/udp	0.000000	# Veritas Authentication Port
pfu-prcallback	3208/tcp	0.000000	# PFU PR Callback
pfu-prcallback	3208/udp	0.000000	# PFU PR Callback
netwkpathengine	3209/tcp	0.000000	# HP OpenView Network Path Engine Server
netwkpathengine	3209/udp	0.000000	# HP OpenView Network Path Engine Server
flamenco-proxy	3210/tcp	0.000076	# Flamenco Networks Proxy
flamenco-proxy	3210/udp	0.000000	# Flamenco Networks Proxy
avsecuremgmt	3211/tcp	0.000380	# Avocent Secure Management
avsecuremgmt	3211/udp	0.000000	# Avocent Secure Management
surveyinst	3212/tcp	0.000000	# Survey Instrument
surveyinst	3212/udp	0.000330	# Survey Instrument
neon24x7	3213/tcp	0.000000	# NEON 24X7 Mission Control
neon24x7	3213/udp	0.000000	# NEON 24X7 Mission Control
jmq-daemon-1	3214/tcp	0.000000	# JMQ Daemon Port 1
jmq-daemon-1	3214/udp	0.000000	# JMQ Daemon Port 1
jmq-daemon-2	3215/tcp	0.000000	# JMQ Daemon Port 2
jmq-daemon-2	3215/udp	0.000000	# JMQ Daemon Port 2
ferrari-foam	3216/tcp	0.000000	# Ferrari electronic FOAM
ferrari-foam	3216/udp	0.000000	# Ferrari electronic FOAM
unite	3217/tcp	0.000000	# Unified IP & Telecom Environment
unite	3217/udp	0.000000	# Unified IP & Telecom Environment
smartpackets	3218/tcp	0.000000	# EMC SmartPackets
smartpackets	3218/udp	0.000000	# EMC SmartPackets
wms-messenger	3219/tcp	0.000000	# WMS Messenger
wms-messenger	3219/udp	0.000000	# WMS Messenger
xnm-ssl	3220/tcp	0.000076	# XML NM over SSL
xnm-ssl	3220/udp	0.000000	# XML NM over SSL
xnm-clear-text	3221/tcp	0.000228	# XML NM over TCP
xnm-clear-text	3221/udp	0.000000	# XML NM over TCP
glbp	3222/tcp	0.000000	# Gateway Load Balancing Pr
glbp	3222/udp	0.000000	# Gateway Load Balancing Pr
digivote	3223/tcp	0.000000	# DIGIVOTE (R) Vote-Server
digivote	3223/udp	0.000000	# DIGIVOTE (R) Vote-Server
aes-discovery	3224/tcp	0.000000	# AES Discovery Port
aes-discovery	3224/udp	0.000000	# AES Discovery Port
fcip-port	3225/tcp	0.000000	# FCIP
fcip-port	3225/udp	0.000000	# FCIP
isi-irp	3226/tcp	0.000000	# ISI Industry Software IRP
isi-irp	3226/udp	0.000000	# ISI Industry Software IRP
dwnmshttp	3227/tcp	0.000000	# DiamondWave NMS Server
dwnmshttp	3227/udp	0.000000	# DiamondWave NMS Server
dwmsgserver	3228/tcp	0.000000	# DiamondWave MSG Server
dwmsgserver	3228/udp	0.000330	# DiamondWave MSG Server
global-cd-port	3229/tcp	0.000000	# Global CD Port
global-cd-port	3229/udp	0.000000	# Global CD Port
sftdst-port	3230/tcp	0.000000	# Software Distributor Port
sftdst-port	3230/udp	0.000000	# Software Distributor Port
vidigo	3231/tcp	0.000000	# VidiGo communication (previous was: Delta Solutions Direct)
vidigo	3231/udp	0.000000	# VidiGo communication (previous was: Delta Solutions Direct)
mdtp	3232/tcp	0.000000	# MDT port
mdtp	3232/udp	0.000000	# MDT port
whisker	3233/tcp	0.000000	# WhiskerControl main port
whisker	3233/udp	0.000661	# WhiskerControl main port
alchemy	3234/tcp	0.000000	# Alchemy Server
alchemy	3234/udp	0.000000	# Alchemy Server
mdap-port	3235/tcp	0.000000	# MDAP port | MDAP Port
mdap-port	3235/udp	0.000661	# MDAP Port
apparenet-ts	3236/tcp	0.000000	# appareNet Test Server
apparenet-ts	3236/udp	0.000000	# appareNet Test Server
apparenet-tps	3237/tcp	0.000000	# appareNet Test Packet Sequencer
apparenet-tps	3237/udp	0.000000	# appareNet Test Packet Sequencer
apparenet-as	3238/tcp	0.000000	# appareNet Analysis Server
apparenet-as	3238/udp	0.000000	# appareNet Analysis Server
apparenet-ui	3239/tcp	0.000000	# appareNet User Interface
apparenet-ui	3239/udp	0.000000	# appareNet User Interface
triomotion	3240/tcp	0.000076	# Trio Motion Control Port
triomotion	3240/udp	0.000000	# Trio Motion Control Port
sysorb	3241/tcp	0.000000	# SysOrb Monitoring Server
sysorb	3241/udp	0.000000	# SysOrb Monitoring Server
sdp-id-port	3242/tcp	0.000000	# Session Description ID
sdp-id-port	3242/udp	0.000000	# Session Description ID
timelot	3243/tcp	0.000000	# Timelot Port
timelot	3243/udp	0.000000	# Timelot Port
onesaf	3244/tcp	0.000000
onesaf	3244/udp	0.000000
vieo-fe	3245/tcp	0.000000	# VIEO Fabric Executive
vieo-fe	3245/udp	0.000330	# VIEO Fabric Executive
dvt-system	3246/tcp	0.000000	# DVT SYSTEM PORT
kademlia	3246/udp	0.000857	# Kademlia P2P (mlnet)
dvt-data	3247/tcp	0.000000	# DVT DATA LINK
dvt-data	3247/udp	0.000000	# DVT DATA LINK
procos-lm	3248/tcp	0.000000	# PROCOS LM
procos-lm	3248/udp	0.000000	# PROCOS LM
ssp	3249/tcp	0.000000	# State Sync Protocol
ssp	3249/udp	0.000000	# State Sync Protocol
hicp	3250/tcp	0.000000	# HMS hicp port
hicp	3250/udp	0.000000	# HMS hicp port
sysscanner	3251/tcp	0.000000	# Sys Scanner
sysscanner	3251/udp	0.000000	# Sys Scanner
dhe	3252/tcp	0.000000	# DHE port
dhe	3252/udp	0.000000	# DHE port
pda-data	3253/tcp	0.000000	# PDA Data
pda-data	3253/udp	0.000000	# PDA Data
pda-sys	3254/tcp	0.000000	# PDA System
pda-sys	3254/udp	0.000330	# PDA System
semaphore	3255/tcp	0.000000	# Semaphore Connection Port
semaphore	3255/udp	0.000000	# Semaphore Connection Port
cpqrpm-agent	3256/tcp	0.000000	# Compaq RPM Agent Port
cpqrpm-agent	3256/udp	0.000330	# Compaq RPM Agent Port
cpqrpm-server	3257/tcp	0.000000	# Compaq RPM Server Port
cpqrpm-server	3257/udp	0.000000	# Compaq RPM Server Port
ivecon-port	3258/tcp	0.000000	# Ivecon Server Port
ivecon-port	3258/udp	0.000000	# Ivecon Server Port
epncdp2	3259/tcp	0.000000	# Epson Network Common Devi
epncdp2	3259/udp	0.000000	# Epson Network Common Devi
iscsi	3260/tcp	0.001064	# iscsi-target | iSCSI port
iscsi	3260/udp	0.000000
winshadow	3261/tcp	0.000304
winshadow	3261/udp	0.000000
necp	3262/tcp	0.000000
necp	3262/udp	0.000000
ecolor-imager	3263/tcp	0.000076	# E-Color Enterprise Imager
ecolor-imager	3263/udp	0.000330	# E-Color Enterprise Imager
ccmail	3264/tcp	0.000038	# cc:mail/lotus
ccmail	3264/udp	0.000395	# cc:mail/lotus
altav-tunnel	3265/tcp	0.000000	# Altav Tunnel
altav-tunnel	3265/udp	0.000330	# Altav Tunnel
ns-cfg-server	3266/tcp	0.000000	# NS CFG Server
ns-cfg-server	3266/udp	0.000000	# NS CFG Server
ibm-dial-out	3267/tcp	0.000000	# IBM Dial Out
ibm-dial-out	3267/udp	0.000000	# IBM Dial Out
globalcatLDAP	3268/tcp	0.001229	# msft-gc | Global Catalog LDAP | Microsoft Global Catalog
msft-gc	3268/udp	0.000000	# Microsoft Global Catalog
globalcatLDAPssl	3269/tcp	0.001142	# msft-gc-ssl | Global Catalog LDAP over ssl | Microsoft Global Catalog with LDAP/SSL
msft-gc-ssl	3269/udp	0.000000	# Microsoft Global Catalog with LDAP/SSL
verismart	3270/tcp	0.000000
verismart	3270/udp	0.000000
csoft-prev	3271/tcp	0.000000	# CSoft Prev Port
csoft-prev	3271/udp	0.000000	# CSoft Prev Port
user-manager	3272/tcp	0.000000	# Fujitsu User Manager
user-manager	3272/udp	0.000330	# Fujitsu User Manager
sxmp	3273/tcp	0.000000	# Simple Extensible Multiplexed Protocol
sxmp	3273/udp	0.000330	# Simple Extensible Multiplexed Protocol
ordinox-server	3274/tcp	0.000000	# Ordinox Server
ordinox-server	3274/udp	0.000000	# Ordinox Server
samd	3275/tcp	0.000000
samd	3275/udp	0.000000
maxim-asics	3276/tcp	0.000000	# Maxim ASICs
maxim-asics	3276/udp	0.000000	# Maxim ASICs
awg-proxy	3277/tcp	0.000000	# AWG Proxy
awg-proxy	3277/udp	0.000000	# AWG Proxy
lkcmserver	3278/tcp	0.000000	# LKCM Server
lkcmserver	3278/udp	0.000330	# LKCM Server
admind	3279/tcp	0.000000
admind	3279/udp	0.000330
vs-server	3280/tcp	0.000076	# VS Server
vs-server	3280/udp	0.000000	# VS Server
sysopt	3281/tcp	0.000076
sysopt	3281/udp	0.000000
datusorb	3282/tcp	0.000000
datusorb	3282/udp	0.000000
netassistant	3283/tcp	0.000760	# #ERROR:Apple Remote Desktop (Net Assistant) | Apple Remote Desktop Net Assistant reporting feature | Net Assistant
netassistant	3283/udp	0.066072	# Apple Remote Desktop Net Assistant reporting feature
4talk	3284/tcp	0.000000
4talk	3284/udp	0.000000
plato	3285/tcp	0.000000
plato	3285/udp	0.000000
e-net	3286/tcp	0.000000
e-net	3286/udp	0.000000
directvdata	3287/tcp	0.000000
directvdata	3287/udp	0.000000
cops	3288/tcp	0.000000
cops	3288/udp	0.000000
enpc	3289/tcp	0.000000
enpc	3289/udp	0.000330
caps-lm	3290/tcp	0.000000	# CAPS LOGISTICS TOOLKIT - LM
caps-lm	3290/udp	0.000000	# CAPS LOGISTICS TOOLKIT - LM
sah-lm	3291/tcp	0.000076	# S A Holditch & Associates - LM
sah-lm	3291/udp	0.000330	# S A Holditch & Associates - LM
meetingmaker	3292/tcp	0.000038	# cart-o-rama | Meeting maker time management software | Cart O Rama
cart-o-rama	3292/udp	0.000330	# Cart O Rama
fg-fps	3293/tcp	0.000000
fg-fps	3293/udp	0.000330
fg-gip	3294/tcp	0.000000
fg-gip	3294/udp	0.000000
dyniplookup	3295/tcp	0.000000	# Dynamic IP Lookup
dyniplookup	3295/udp	0.000000	# Dynamic IP Lookup
rib-slm	3296/tcp	0.000000	# Rib License Manager
rib-slm	3296/udp	0.001321	# Rib License Manager
cytel-lm	3297/tcp	0.000000	# Cytel License Manager
cytel-lm	3297/udp	0.000000	# Cytel License Manager
deskview	3298/tcp	0.000000
deskview	3298/udp	0.000000
saprouter	3299/tcp	0.000125	# pdrncs
pdrncs	3299/udp	0.000000
ceph	3300/tcp	0.000380	# Ceph monitor
tarantool	3301/tcp	0.000380	# Tarantool in-memory computing platform
unknown	3301/udp	0.000991
mcs-fastmail	3302/tcp	0.000000	# MCS Fastmail
mcs-fastmail	3302/udp	0.000000	# MCS Fastmail
opsession-clnt	3303/tcp	0.000000	# OP Session Client
opsession-clnt	3303/udp	0.000000	# OP Session Client
opsession-srvr	3304/tcp	0.000152	# OP Session Server
opsession-srvr	3304/udp	0.000661	# OP Session Server
odette-ftp	3305/tcp	0.000000
odette-ftp	3305/udp	0.000330
mysql	3306/tcp	0.045390
mysql	3306/udp	0.000000
opsession-prxy	3307/tcp	0.000152	# OP Session Proxy
opsession-prxy	3307/udp	0.000000	# OP Session Proxy
tns-server	3308/tcp	0.000000	# TNS Server
tns-server	3308/udp	0.000000	# TNS Server
tns-adv	3309/tcp	0.000000	# TNS ADV
tns-adv	3309/udp	0.000000	# TNS ADV
dyna-access	3310/tcp	0.000076	# Dyna Access
dyna-access	3310/udp	0.000000	# Dyna Access
mcns-tel-ret	3311/tcp	0.000076	# MCNS Tel Ret
mcns-tel-ret	3311/udp	0.000000	# MCNS Tel Ret
appman-server	3312/tcp	0.000000	# Application Management Server
appman-server	3312/udp	0.000000	# Application Management Server
uorb	3313/tcp	0.000000	# Unify Object Broker
uorb	3313/udp	0.000000	# Unify Object Broker
uohost	3314/tcp	0.000000	# Unify Object Host
uohost	3314/udp	0.000000	# Unify Object Host
cdid	3315/tcp	0.000000
cdid	3315/udp	0.000330
aicc-cmi	3316/tcp	0.000000	# AICC/CMI
aicc-cmi	3316/udp	0.000000	# AICC/CMI
vsaiport	3317/tcp	0.000000	# VSAI PORT
vsaiport	3317/udp	0.000000	# VSAI PORT
ssrip	3318/tcp	0.000000	# Swith to Swith Routing Information Protocol
ssrip	3318/udp	0.000000	# Swith to Swith Routing Information Protocol
sdt-lmd	3319/tcp	0.000076	# SDT License Manager
sdt-lmd	3319/udp	0.000000	# SDT License Manager
officelink2000	3320/tcp	0.000000	# Office Link 2000
officelink2000	3320/udp	0.000000	# Office Link 2000
vnsstr	3321/tcp	0.000000
vnsstr	3321/udp	0.000330
active-net	3322/tcp	0.000228	# Active Networks
active-net	3322/udp	0.000000	# Active Networks
active-net	3323/tcp	0.000380	# Active Networks
active-net	3323/udp	0.000000	# Active Networks
active-net	3324/tcp	0.000228	# Active Networks
active-net	3324/udp	0.000000	# Active Networks
active-net	3325/tcp	0.000380	# Active Networks
active-net	3325/udp	0.000000	# Active Networks
sftu	3326/tcp	0.000000
sftu	3326/udp	0.000000
bbars	3327/tcp	0.000000
bbars	3327/udp	0.000000
egptlm	3328/tcp	0.000000	# Eaglepoint License Manager
egptlm	3328/udp	0.000000	# Eaglepoint License Manager
hp-device-disc	3329/tcp	0.000000	# HP Device Disc
hp-device-disc	3329/udp	0.000000	# HP Device Disc
mcs-calypsoicf	3330/tcp	0.000000	# MCS Calypso ICF
mcs-calypsoicf	3330/udp	0.000000	# MCS Calypso ICF
mcs-messaging	3331/tcp	0.000000	# MCS Messaging
mcs-messaging	3331/udp	0.000330	# MCS Messaging
mcs-mailsvr	3332/tcp	0.000000	# MCS Mail Server
mcs-mailsvr	3332/udp	0.000000	# MCS Mail Server
dec-notes	3333/tcp	0.000790	# DEC Notes
dec-notes	3333/udp	0.000890	# DEC Notes
directv-web	3334/tcp	0.000076	# Direct TV Webcasting
directv-web	3334/udp	0.000330	# Direct TV Webcasting
directv-soft	3335/tcp	0.000000	# Direct TV Software Updates
directv-soft	3335/udp	0.000330	# Direct TV Software Updates
directv-tick	3336/tcp	0.000000	# Direct TV Tickers
directv-tick	3336/udp	0.000000	# Direct TV Tickers
directv-catlg	3337/tcp	0.000000	# Direct TV Data Catalog
directv-catlg	3337/udp	0.000330	# Direct TV Data Catalog
anet-b	3338/tcp	0.000000	# OMF data b
anet-b	3338/udp	0.000000	# OMF data b
anet-l	3339/tcp	0.000000	# OMF data l
anet-l	3339/udp	0.000330	# OMF data l
anet-m	3340/tcp	0.000000	# OMF data m
anet-m	3340/udp	0.000000	# OMF data m
anet-h	3341/tcp	0.000000	# OMF data h
anet-h	3341/udp	0.000000	# OMF data h
webtie	3342/tcp	0.000000
webtie	3342/udp	0.000000
ms-cluster-net	3343/tcp	0.000000	# MS Cluster Net
ms-cluster-net	3343/udp	0.001321	# MS Cluster Net
bnt-manager	3344/tcp	0.000000	# BNT Manager
bnt-manager	3344/udp	0.000000	# BNT Manager
influence	3345/tcp	0.000000
influence	3345/udp	0.000000
trnsprntproxy	3346/tcp	0.000000	# Trnsprnt Proxy
trnsprntproxy	3346/udp	0.000000	# Trnsprnt Proxy
phoenix-rpc	3347/tcp	0.000000	# Phoenix RPC
phoenix-rpc	3347/udp	0.000000	# Phoenix RPC
pangolin-laser	3348/tcp	0.000000	# Pangolin Laser
pangolin-laser	3348/udp	0.000000	# Pangolin Laser
chevinservices	3349/tcp	0.000000	# Chevin Services
chevinservices	3349/udp	0.000000	# Chevin Services
findviatv	3350/tcp	0.000000
findviatv	3350/udp	0.000000
btrieve	3351/tcp	0.000380	# Btrieve port
btrieve	3351/udp	0.000000	# Btrieve port
ssql	3352/tcp	0.000000	# Scalable SQL
ssql	3352/udp	0.000000	# Scalable SQL
fatpipe	3353/tcp	0.000000
fatpipe	3353/udp	0.000000
suitjd	3354/tcp	0.000000
suitjd	3354/udp	0.000330
ordinox-dbase	3355/tcp	0.000000	# Ordinox Dbase
ordinox-dbase	3355/udp	0.000000	# Ordinox Dbase
upnotifyps	3356/tcp	0.000000
upnotifyps	3356/udp	0.000000
adtech-test	3357/tcp	0.000000	# Adtech Test IP
adtech-test	3357/udp	0.000000	# Adtech Test IP
mpsysrmsvr	3358/tcp	0.000000	# Mp Sys Rmsvr
mpsysrmsvr	3358/udp	0.000000	# Mp Sys Rmsvr
wg-netforce	3359/tcp	0.000000	# WG NetForce
wg-netforce	3359/udp	0.000000	# WG NetForce
kv-server	3360/tcp	0.000000	# KV Server
kv-server	3360/udp	0.000000	# KV Server
kv-agent	3361/tcp	0.000000	# KV Agent
kv-agent	3361/udp	0.000000	# KV Agent
dj-ilm	3362/tcp	0.000076	# DJ ILM
dj-ilm	3362/udp	0.000330	# DJ ILM
nati-vi-server	3363/tcp	0.000076	# NATI Vi Server
nati-vi-server	3363/udp	0.000330	# NATI Vi Server
creativeserver	3364/tcp	0.000000	# Creative Server
creativeserver	3364/udp	0.000661	# Creative Server
contentserver	3365/tcp	0.000076	# Content Server
contentserver	3365/udp	0.000000	# Content Server
creativepartnr	3366/tcp	0.000000	# Creative Partner
creativepartnr	3366/udp	0.000330	# Creative Partner
satvid-datalnk	3367/tcp	0.000380	# Satellite Video Data Link
satvid-datalnk	3367/udp	0.000000	# Satellite Video Data Link
satvid-datalnk	3368/tcp	0.000076	# Satellite Video Data Link
satvid-datalnk	3368/udp	0.000330	# Satellite Video Data Link
satvid-datalnk	3369/tcp	0.000304	# Satellite Video Data Link
satvid-datalnk	3369/udp	0.000000	# Satellite Video Data Link
satvid-datalnk	3370/tcp	0.000304	# Satellite Video Data Link
satvid-datalnk	3370/udp	0.000000	# Satellite Video Data Link
satvid-datalnk	3371/tcp	0.000304	# Satellite Video Data Link
satvid-datalnk	3371/udp	0.000000	# Satellite Video Data Link
msdtc	3372/tcp	0.000339	# tip2 | MS distributed transaction coordinator | TIP 2
tip2	3372/udp	0.000661	# TIP 2
lavenir-lm	3373/tcp	0.000000	# Lavenir License Manager
lavenir-lm	3373/udp	0.000000	# Lavenir License Manager
cluster-disc	3374/tcp	0.000076	# Cluster Disc
cluster-disc	3374/udp	0.000000	# Cluster Disc
vsnm-agent	3375/tcp	0.000000	# VSNM Agent
vsnm-agent	3375/udp	0.000000	# VSNM Agent
cdbroker	3376/tcp	0.000152	# CD Broker
cdbroker	3376/udp	0.000000	# CD Broker
cogsys-lm	3377/tcp	0.000000	# Cogsys Network License Manager
cogsys-lm	3377/udp	0.000000	# Cogsys Network License Manager
wsicopy	3378/tcp	0.000000
wsicopy	3378/udp	0.000000
socorfs	3379/tcp	0.000000
socorfs	3379/udp	0.000000
sns-channels	3380/tcp	0.000000	# SNS Channels
sns-channels	3380/udp	0.000330	# SNS Channels
geneous	3381/tcp	0.000000
geneous	3381/udp	0.000330
fujitsu-neat	3382/tcp	0.000000	# Fujitsu Network Enhanced Antitheft function
fujitsu-neat	3382/udp	0.000000	# Fujitsu Network Enhanced Antitheft function
esp-lm	3383/tcp	0.000000	# Enterprise Software Products License Manager
esp-lm	3383/udp	0.000330	# Enterprise Software Products License Manager
hp-clic	3384/tcp	0.000000	# Cluster Management Services | Hardware Management
hp-clic	3384/udp	0.000330	# Hardware Management
qnxnetman	3385/tcp	0.000000
qnxnetman	3385/udp	0.000000
gprs-data	3386/tcp	0.000000	# gprs-sig | GPRS Data | GPRS SIG
gprs-sig	3386/udp	0.000330	# GPRS SIG
backroomnet	3387/tcp	0.000000	# Back Room Net
backroomnet	3387/udp	0.000000	# Back Room Net
cbserver	3388/tcp	0.000076	# CB Server
cbserver	3388/udp	0.000330	# CB Server
ms-wbt-server	3389/tcp	0.083904	# Microsoft Remote Display Protocol (aka ms-term-serv, microsoft-rdp) | MS WBT Server
ms-wbt-server	3389/udp	0.004955	# Microsoft Remote Display Protocol (aka ms-term-serv, microsoft-rdp)
dsc	3390/tcp	0.000228	# Distributed Service Coordinator
dsc	3390/udp	0.000000	# Distributed Service Coordinator
savant	3391/tcp	0.000000
savant	3391/udp	0.000330
efi-lm	3392/tcp	0.000000	# EFI License Management
efi-lm	3392/udp	0.000330	# EFI License Management
d2k-tapestry1	3393/tcp	0.000000	# D2K Tapestry Client to Server
d2k-tapestry1	3393/udp	0.000000	# D2K Tapestry Client to Server
d2k-tapestry2	3394/tcp	0.000000	# D2K Tapestry Server to Server
d2k-tapestry2	3394/udp	0.000000	# D2K Tapestry Server to Server
dyna-lm	3395/tcp	0.000000	# Dyna License Manager (Elam)
dyna-lm	3395/udp	0.000000	# Dyna License Manager (Elam)
printer_agent	3396/tcp	0.000076	# printer-agent | Printer Agent
printer_agent	3396/udp	0.000661	# Printer Agent
saposs	3397/tcp	0.000038	# cloanto-lm | SAP Oss | Cloanto License Manager
cloanto-lm	3397/udp	0.000000	# Cloanto License Manager
sapcomm	3398/tcp	0.000063	# mercantile | Mercantile
mercantile	3398/udp	0.000000
sapeps	3399/tcp	0.000100	# csms | SAP EPS | CSMS
csms	3399/udp	0.000330
csms2	3400/tcp	0.000152
csms2	3400/udp	0.000000
filecast	3401/tcp	0.000000
squid-snmp	3401/udp	0.002241	# Squid proxy SNMP port
fxaengine-net	3402/tcp	0.000000	# FXa Engine Network Port
fxaengine-net	3402/udp	0.000000	# FXa Engine Network Port
unknown	3403/udp	0.000991
unknown	3404/tcp	0.000380
nokia-ann-ch1	3405/tcp	0.000000	# Nokia Announcement ch 1
nokia-ann-ch1	3405/udp	0.000000	# Nokia Announcement ch 1
nokia-ann-ch2	3406/tcp	0.000000	# Nokia Announcement ch 2
nokia-ann-ch2	3406/udp	0.000330	# Nokia Announcement ch 2
ldap-admin	3407/tcp	0.000000	# LDAP admin server port
ldap-admin	3407/udp	0.000000	# LDAP admin server port
BESApi	3408/tcp	0.000000	# BES Api Port
BESApi	3408/udp	0.000330	# BES Api Port
networklens	3409/tcp	0.000000	# NetworkLens Event Port
networklens	3409/udp	0.000000	# NetworkLens Event Port
networklenss	3410/tcp	0.000152	# NetworkLens SSL Event
networklenss	3410/udp	0.000000	# NetworkLens SSL Event
biolink-auth	3411/tcp	0.000000	# BioLink Authenteon server
biolink-auth	3411/udp	0.000000	# BioLink Authenteon server
xmlblaster	3412/tcp	0.000000
xmlblaster	3412/udp	0.000000
svnet	3413/tcp	0.000000	# SpecView Networking
svnet	3413/udp	0.000000	# SpecView Networking
wip-port	3414/tcp	0.000076	# BroadCloud WIP Port
wip-port	3414/udp	0.000000	# BroadCloud WIP Port
bcinameservice	3415/tcp	0.000076	# BCI Name Service
bcinameservice	3415/udp	0.000000	# BCI Name Service
commandport	3416/tcp	0.000000	# AirMobile IS Command Port
commandport	3416/udp	0.000000	# AirMobile IS Command Port
csvr	3417/tcp	0.000000	# ConServR file translation
csvr	3417/udp	0.000000	# ConServR file translation
rnmap	3418/tcp	0.000000	# Remote nmap
rnmap	3418/udp	0.000000	# Remote nmap
softaudit	3419/tcp	0.000076	# Isogon SoftAudit | ISogon SoftAudit
softaudit	3419/udp	0.000000	# ISogon SoftAudit
ifcp-port	3420/tcp	0.000000	# iFCP User Port
ifcp-port	3420/udp	0.000000	# iFCP User Port
bmap	3421/tcp	0.000013	# Bull Apprise portmapper
bmap	3421/udp	0.000643	# Bull Apprise portmapper
rusb-sys-port	3422/tcp	0.000000	# Remote USB System Port
rusb-sys-port	3422/udp	0.000330	# Remote USB System Port
xtrm	3423/tcp	0.000000	# xTrade Reliable Messaging
xtrm	3423/udp	0.000330	# xTrade Reliable Messaging
xtrms	3424/tcp	0.000000	# xTrade over TLS/SSL
xtrms	3424/udp	0.000000	# xTrade over TLS/SSL
agps-port	3425/tcp	0.000076	# AGPS Access Port
agps-port	3425/udp	0.000000	# AGPS Access Port
arkivio	3426/tcp	0.000000	# Arkivio Storage Protocol
arkivio	3426/udp	0.000000	# Arkivio Storage Protocol
websphere-snmp	3427/tcp	0.000000	# WebSphere SNMP
websphere-snmp	3427/udp	0.000000	# WebSphere SNMP
twcss	3428/tcp	0.000000	# 2Wire CSS
twcss	3428/udp	0.000330	# 2Wire CSS
gcsp	3429/tcp	0.000000	# GCSP user port
gcsp	3429/udp	0.000330	# GCSP user port
ssdispatch	3430/tcp	0.000076	# Scott Studios Dispatch
ssdispatch	3430/udp	0.000000	# Scott Studios Dispatch
ndl-als	3431/tcp	0.000000	# Active License Server Port
ndl-als	3431/udp	0.000000	# Active License Server Port
osdcp	3432/tcp	0.000000	# Secure Device Protocol
osdcp	3432/udp	0.000000	# Secure Device Protocol
alta-smp	3433/tcp	0.000000	# opnet-smp | Altaworks Service Management Platform | OPNET Service Management Platform
alta-smp	3433/udp	0.000000	# Altaworks Service Management Platform
opencm	3434/tcp	0.000000	# OpenCM Server
opencm	3434/udp	0.000000	# OpenCM Server
pacom	3435/tcp	0.000000	# Pacom Security User Port
pacom	3435/udp	0.000000	# Pacom Security User Port
gc-config	3436/tcp	0.000000	# GuardControl Exchange Protocol
gc-config	3436/udp	0.000000	# GuardControl Exchange Protocol
autocueds	3437/tcp	0.000000	# Autocue Directory Service
autocueds	3437/udp	0.000000	# Autocue Directory Service
spiral-admin	3438/tcp	0.000000	# Spiralcraft Admin
spiral-admin	3438/udp	0.000000	# Spiralcraft Admin
hri-port	3439/tcp	0.000076	# HRI Interface Port
hri-port	3439/udp	0.000000	# HRI Interface Port
ans-console	3440/tcp	0.000000	# Net Steward Mgmt Console
ans-console	3440/udp	0.000330	# Net Steward Mgmt Console
connect-client	3441/tcp	0.000000	# OC Connect Client
connect-client	3441/udp	0.000000	# OC Connect Client
connect-server	3442/tcp	0.000000	# OC Connect Server
connect-server	3442/udp	0.000330	# OC Connect Server
ov-nnm-websrv	3443/tcp	0.000076	# OpenView Network Node Manager WEB Server
ov-nnm-websrv	3443/udp	0.000000	# OpenView Network Node Manager WEB Server
denali-server	3444/tcp	0.000000	# Denali Server
denali-server	3444/udp	0.000330	# Denali Server
monp	3445/tcp	0.000000	# Media Object Network | Media Object Network Protocol
monp	3445/udp	0.000000	# Media Object Network
3comfaxrpc	3446/tcp	0.000000	# 3Com FAX RPC port
3comfaxrpc	3446/udp	0.000330	# 3Com FAX RPC port
directnet	3447/tcp	0.000000	# DirectNet IM System
directnet	3447/udp	0.000000	# DirectNet IM System
dnc-port	3448/tcp	0.000000	# Discovery and Net Config
dnc-port	3448/udp	0.000000	# Discovery and Net Config
hotu-chat	3449/tcp	0.000000	# HotU Chat
hotu-chat	3449/udp	0.000330	# HotU Chat
castorproxy	3450/tcp	0.000000
castorproxy	3450/udp	0.000000
asam	3451/tcp	0.000000	# ASAM Services
asam	3451/udp	0.000661	# ASAM Services
sabp-signal	3452/tcp	0.000000	# SABP-Signalling Protocol
sabp-signal	3452/udp	0.000000	# SABP-Signalling Protocol
pscupd	3453/tcp	0.000000	# PSC Update Port | PSC Update
pscupd	3453/udp	0.000661	# PSC Update Port
mira	3454/tcp	0.000000	# Apple Remote Access Protocol
prsvp	3455/tcp	0.000000	# RSVP Port
prsvp	3455/udp	0.000527	# RSVP Port
vat	3456/tcp	0.000100	# VAT default data
IISrpc-or-vat	3456/udp	0.036607	# also VAT default data
vat-control	3457/tcp	0.000025	# VAT default control
vat-control	3457/udp	0.001433	# VAT default control
d3winosfi	3458/tcp	0.000000
d3winosfi	3458/udp	0.000000
integral	3459/tcp	0.000000	# TIP Integral
integral	3459/udp	0.000000	# TIP Integral
edm-manager	3460/tcp	0.000000	# EDM Manger
edm-manager	3460/udp	0.000000	# EDM Manger
edm-stager	3461/tcp	0.000000	# EDM Stager
edm-stager	3461/udp	0.000000	# EDM Stager
track	3462/tcp	0.000000	# edm-std-notify | software distribution | EDM STD Notify
edm-std-notify	3462/udp	0.000330	# EDM STD Notify
edm-adm-notify	3463/tcp	0.000000	# EDM ADM Notify
edm-adm-notify	3463/udp	0.000000	# EDM ADM Notify
edm-mgr-sync	3464/tcp	0.000000	# EDM MGR Sync
edm-mgr-sync	3464/udp	0.000000	# EDM MGR Sync
edm-mgr-cntrl	3465/tcp	0.000000	# EDM MGR Cntrl
edm-mgr-cntrl	3465/udp	0.000000	# EDM MGR Cntrl
workflow	3466/tcp	0.000000
workflow	3466/udp	0.000000
rcst	3467/tcp	0.000000
rcst	3467/udp	0.000330
ttcmremotectrl	3468/tcp	0.000000	# TTCM Remote Controll
ttcmremotectrl	3468/udp	0.000000	# TTCM Remote Controll
pluribus	3469/tcp	0.000000
pluribus	3469/udp	0.000000
jt400	3470/tcp	0.000000
jt400	3470/udp	0.000000
jt400-ssl	3471/tcp	0.000000
jt400-ssl	3471/udp	0.000000
jaugsremotec-1	3472/tcp	0.000000	# JAUGS N-G Remotec 1
jaugsremotec-1	3472/udp	0.000000	# JAUGS N-G Remotec 1
jaugsremotec-2	3473/tcp	0.000000	# JAUGS N-G Remotec 2
jaugsremotec-2	3473/udp	0.000000	# JAUGS N-G Remotec 2
ttntspauto	3474/tcp	0.000000	# TSP Automation
ttntspauto	3474/udp	0.000330	# TSP Automation
genisar-port	3475/tcp	0.000000	# Genisar Comm Port
genisar-port	3475/udp	0.000000	# Genisar Comm Port
nppmp	3476/tcp	0.000532	# NVIDIA Mgmt Protocol
nppmp	3476/udp	0.000000	# NVIDIA Mgmt Protocol
ecomm	3477/tcp	0.000000	# eComm link port
ecomm	3477/udp	0.000661	# eComm link port
stun	3478/tcp	0.000000	# stun-behavior | turn | Session Traversal Utilities for NAT (STUN) port | TURN over TCP | TURN over UDP | STUN Behavior Discovery over TCP | STUN Behavior Discovery over UDP
stun	3478/udp	0.000000	# Session Traversal Utilities for NAT (STUN) port
twrpc	3479/tcp	0.000076	# 2Wire RPC
twrpc	3479/udp	0.000000	# 2Wire RPC
plethora	3480/tcp	0.000000	# Secure Virtual Workspace
plethora	3480/udp	0.000330	# Secure Virtual Workspace
cleanerliverc	3481/tcp	0.000000	# CleanerLive remote ctrl
cleanerliverc	3481/udp	0.000000	# CleanerLive remote ctrl
vulture	3482/tcp	0.000000	# Vulture Monitoring System
vulture	3482/udp	0.000330	# Vulture Monitoring System
slim-devices	3483/tcp	0.000076	# Slim Devices Protocol
slim-devices	3483/udp	0.000000	# Slim Devices Protocol
gbs-stp	3484/tcp	0.000000	# GBS SnapTalk Protocol
gbs-stp	3484/udp	0.000000	# GBS SnapTalk Protocol
celatalk	3485/tcp	0.000076
celatalk	3485/udp	0.000000
ifsf-hb-port	3486/tcp	0.000076	# IFSF Heartbeat Port
ifsf-hb-port	3486/udp	0.000330	# IFSF Heartbeat Port
ltctcp	3487/tcp	0.000000	# ltcudp | LISA TCP Transfer Channel | LISA UDP Transfer Channel
ltcudp	3487/udp	0.000330	# LISA UDP Transfer Channel
fs-rh-srv	3488/tcp	0.000000	# FS Remote Host Server
fs-rh-srv	3488/udp	0.000000	# FS Remote Host Server
dtp-dia	3489/tcp	0.000000	# DTP/DIA
dtp-dia	3489/udp	0.000000	# DTP/DIA
colubris	3490/tcp	0.000000	# Colubris Management Port
colubris	3490/udp	0.000000	# Colubris Management Port
swr-port	3491/tcp	0.000000	# SWR Port
swr-port	3491/udp	0.000000	# SWR Port
tvdumtray-port	3492/tcp	0.000000	# TVDUM Tray Port
tvdumtray-port	3492/udp	0.000000	# TVDUM Tray Port
nut	3493/tcp	0.000304	# Network UPS Tools
nut	3493/udp	0.000000	# Network UPS Tools
ibm3494	3494/tcp	0.000000	# IBM 3494
ibm3494	3494/udp	0.000000	# IBM 3494
seclayer-tcp	3495/tcp	0.000000	# securitylayer over tcp
seclayer-tcp	3495/udp	0.000661	# securitylayer over tcp
seclayer-tls	3496/tcp	0.000000	# securitylayer over tls
seclayer-tls	3496/udp	0.000000	# securitylayer over tls
ipether232port	3497/tcp	0.000076
ipether232port	3497/udp	0.000000
dashpas-port	3498/tcp	0.000000	# DASHPAS user port
dashpas-port	3498/udp	0.000000	# DASHPAS user port
sccip-media	3499/tcp	0.000000	# SccIP Media
sccip-media	3499/udp	0.000330	# SccIP Media
rtmp-port	3500/tcp	0.000000	# RTMP Port
rtmp-port	3500/udp	0.000000	# RTMP Port
isoft-p2p	3501/tcp	0.000000
isoft-p2p	3501/udp	0.000000
avinstalldisc	3502/tcp	0.000000	# Avocent Install Discovery
avinstalldisc	3502/udp	0.000000	# Avocent Install Discovery
lsp-ping	3503/tcp	0.000076	# MPLS LSP-echo Port
lsp-ping	3503/udp	0.000330	# MPLS LSP-echo Port
ironstorm	3504/tcp	0.000000	# IronStorm game server
ironstorm	3504/udp	0.000000	# IronStorm game server
ccmcomm	3505/tcp	0.000076	# CCM communications port
ccmcomm	3505/udp	0.000661	# CCM communications port
apc-3506	3506/tcp	0.000076	# APC 3506
apc-3506	3506/udp	0.000330	# APC 3506
nesh-broker	3507/tcp	0.000000	# Nesh Broker Port
nesh-broker	3507/udp	0.000330	# Nesh Broker Port
interactionweb	3508/tcp	0.000000	# Interaction Web
interactionweb	3508/udp	0.000000	# Interaction Web
vt-ssl	3509/tcp	0.000000	# Virtual Token SSL Port
vt-ssl	3509/udp	0.000000	# Virtual Token SSL Port
xss-port	3510/tcp	0.000000	# XSS Port
xss-port	3510/udp	0.000000	# XSS Port
webmail-2	3511/tcp	0.000076	# WebMail/2
webmail-2	3511/udp	0.000000	# WebMail/2
aztec	3512/tcp	0.000000	# Aztec Distribution Port
aztec	3512/udp	0.000000	# Aztec Distribution Port
arcpd	3513/tcp	0.000076	# Adaptec Remote Protocol
arcpd	3513/udp	0.000330	# Adaptec Remote Protocol
must-p2p	3514/tcp	0.000152	# MUST Peer to Peer
must-p2p	3514/udp	0.000000	# MUST Peer to Peer
must-backplane	3515/tcp	0.000076	# MUST Backplane
must-backplane	3515/udp	0.000000	# MUST Backplane
smartcard-port	3516/tcp	0.000000	# Smartcard Port
smartcard-port	3516/udp	0.000000	# Smartcard Port
802-11-iapp	3517/tcp	0.000228	# IEEE 802.11 WLANs WG IAPP
802-11-iapp	3517/udp	0.000330	# IEEE 802.11 WLANs WG IAPP
artifact-msg	3518/tcp	0.000000	# Artifact Message Server
artifact-msg	3518/udp	0.000000	# Artifact Message Server
nvmsgd	3519/tcp	0.000076	# galileo | Netvion Messenger Port | Netvion Galileo Port
galileo	3519/udp	0.000661	# Netvion Galileo Port
galileolog	3520/tcp	0.000076	# Netvion Galileo Log Port
galileolog	3520/udp	0.000000	# Netvion Galileo Log Port
mc3ss	3521/tcp	0.000000	# Telequip Labs MC3SS
mc3ss	3521/udp	0.000000	# Telequip Labs MC3SS
nssocketport	3522/tcp	0.000000	# DO over NSSocketPort
nssocketport	3522/udp	0.000330	# DO over NSSocketPort
odeumservlink	3523/tcp	0.000000	# Odeum Serverlink
odeumservlink	3523/udp	0.000000	# Odeum Serverlink
ecmport	3524/tcp	0.000000	# ECM Server port
ecmport	3524/udp	0.000000	# ECM Server port
eisport	3525/tcp	0.000000	# EIS Server port
eisport	3525/udp	0.000000	# EIS Server port
starquiz-port	3526/tcp	0.000076	# starQuiz Port
starquiz-port	3526/udp	0.000000	# starQuiz Port
beserver-msg-q	3527/tcp	0.000228	# VERITAS Backup Exec Server
beserver-msg-q	3527/udp	0.000991	# VERITAS Backup Exec Server
jboss-iiop	3528/tcp	0.000000	# JBoss IIOP
jboss-iiop	3528/udp	0.000000	# JBoss IIOP
jboss-iiop-ssl	3529/tcp	0.000000	# JBoss IIOP/SSL
jboss-iiop-ssl	3529/udp	0.000000	# JBoss IIOP/SSL
gf	3530/tcp	0.000076	# Grid Friendly
gf	3530/udp	0.000000	# Grid Friendly
peerenabler	3531/tcp	0.000025	# joltid | P2PNetworking/PeerEnabler protocol | Joltid
peerenabler	3531/udp	0.000890	# P2PNetworking/PeerEnabler protocol
raven-rmp	3532/tcp	0.000076	# Raven Remote Management Control
raven-rmp	3532/udp	0.000000	# Raven Remote Management Control
raven-rdp	3533/tcp	0.000000	# Raven Remote Management Data
raven-rdp	3533/udp	0.000000	# Raven Remote Management Data
urld-port	3534/tcp	0.000000	# URL Daemon Port
urld-port	3534/udp	0.000000	# URL Daemon Port
ms-la	3535/tcp	0.000000
ms-la	3535/udp	0.000000
snac	3536/tcp	0.000000
snac	3536/udp	0.000000
ni-visa-remote	3537/tcp	0.000000	# Remote NI-VISA port
ni-visa-remote	3537/udp	0.000330	# Remote NI-VISA port
ibm-diradm	3538/tcp	0.000000	# IBM Directory Server
ibm-diradm	3538/udp	0.000330	# IBM Directory Server
ibm-diradm-ssl	3539/tcp	0.000000	# IBM Directory Server SSL
ibm-diradm-ssl	3539/udp	0.000000	# IBM Directory Server SSL
pnrp-port	3540/tcp	0.000000	# PNRP User Port
pnrp-port	3540/udp	0.000000	# PNRP User Port
voispeed-port	3541/tcp	0.000000	# VoiSpeed Port
voispeed-port	3541/udp	0.000000	# VoiSpeed Port
hacl-monitor	3542/tcp	0.000000	# HA cluster monitor
hacl-monitor	3542/udp	0.000000	# HA cluster monitor
qftest-lookup	3543/tcp	0.000000	# qftest Lookup Port
qftest-lookup	3543/udp	0.000000	# qftest Lookup Port
teredo	3544/tcp	0.000000	# Teredo Port
teredo	3544/udp	0.000661	# Teredo Port
camac	3545/tcp	0.000000	# CAMAC equipment
camac	3545/udp	0.000000	# CAMAC equipment
unknown	3546/tcp	0.000304
symantec-sim	3547/tcp	0.000000	# Symantec SIM
symantec-sim	3547/udp	0.000000	# Symantec SIM
interworld	3548/tcp	0.000000
interworld	3548/udp	0.000000
tellumat-nms	3549/tcp	0.000000	# Tellumat MDR NMS
tellumat-nms	3549/udp	0.000000	# Tellumat MDR NMS
ssmpp	3550/tcp	0.000000	# Secure SMPP
ssmpp	3550/udp	0.000000	# Secure SMPP
apcupsd	3551/tcp	0.000380	# Apcupsd Information Port
apcupsd	3551/udp	0.000000	# Apcupsd Information Port
taserver	3552/tcp	0.000000	# TeamAgenda Server Port
taserver	3552/udp	0.000000	# TeamAgenda Server Port
rbr-discovery	3553/tcp	0.000000	# Red Box Recorder ADP
rbr-discovery	3553/udp	0.000000	# Red Box Recorder ADP
questnotify	3554/tcp	0.000000	# Quest Notification Server
questnotify	3554/udp	0.000000	# Quest Notification Server
razor	3555/tcp	0.000000	# Vipul's Razor
razor	3555/udp	0.000330	# Vipul's Razor
sky-transport	3556/tcp	0.000000	# Sky Transport Protocol
sky-transport	3556/udp	0.000000	# Sky Transport Protocol
personalos-001	3557/tcp	0.000000	# PersonalOS Comm Port
personalos-001	3557/udp	0.000000	# PersonalOS Comm Port
mcp-port	3558/tcp	0.000000	# MCP user port
mcp-port	3558/udp	0.000000	# MCP user port
cctv-port	3559/tcp	0.000000	# CCTV control port
cctv-port	3559/udp	0.000000	# CCTV control port
iniserve-port	3560/tcp	0.000000	# INIServe port
iniserve-port	3560/udp	0.000000	# INIServe port
bmc-onekey	3561/tcp	0.000000
bmc-onekey	3561/udp	0.000000
sdbproxy	3562/tcp	0.000000
sdbproxy	3562/udp	0.000000
watcomdebug	3563/tcp	0.000000	# Watcom Debug
watcomdebug	3563/udp	0.000000	# Watcom Debug
esimport	3564/tcp	0.000000	# Electromed SIM port
esimport	3564/udp	0.000000	# Electromed SIM port
m2pa	3565/sctp	0.000000
m2pa	3565/tcp	0.000000
quest-data-hub	3566/tcp	0.000000	# Quest Data Hub
oap	3567/tcp	0.000000	# dof-eps | Object Access Protocol | DOF Protocol Stack
oap	3567/udp	0.000000	# Object Access Protocol
oap-s	3568/tcp	0.000000	# dof-tunnel-sec | Object Access Protocol over SSL | DOF Secure Tunnel
oap-s	3568/udp	0.000000	# Object Access Protocol over SSL
mbg-ctrl	3569/tcp	0.000000	# Meinberg Control Service
mbg-ctrl	3569/udp	0.000991	# Meinberg Control Service
mccwebsvr-port	3570/tcp	0.000000	# MCC Web Server Port
mccwebsvr-port	3570/udp	0.000000	# MCC Web Server Port
megardsvr-port	3571/tcp	0.000000	# MegaRAID Server Port
megardsvr-port	3571/udp	0.000330	# MegaRAID Server Port
megaregsvrport	3572/tcp	0.000000	# Registration Server Port
megaregsvrport	3572/udp	0.000000	# Registration Server Port
tag-ups-1	3573/tcp	0.000000	# Advantage Group UPS Suite
tag-ups-1	3573/udp	0.000330	# Advantage Group UPS Suite
dmaf-server	3574/tcp	0.000000	# dmaf-caster | DMAF Server | DMAF Caster
dmaf-caster	3574/udp	0.000991	# DMAF Caster
ccm-port	3575/tcp	0.000000	# Coalsere CCM Port
ccm-port	3575/udp	0.000330	# Coalsere CCM Port
cmc-port	3576/tcp	0.000000	# Coalsere CMC Port
cmc-port	3576/udp	0.000000	# Coalsere CMC Port
config-port	3577/tcp	0.000076	# Configuration Port
config-port	3577/udp	0.000000	# Configuration Port
data-port	3578/tcp	0.000000	# Data Port
data-port	3578/udp	0.000000	# Data Port
ttat3lb	3579/tcp	0.000000	# Tarantella Load Balancing
ttat3lb	3579/udp	0.000000	# Tarantella Load Balancing
nati-svrloc	3580/tcp	0.000380	# NATI-ServiceLocator
nati-svrloc	3580/udp	0.000000	# NATI-ServiceLocator
kfxaclicensing	3581/tcp	0.000000	# Ascent Capture Licensing
kfxaclicensing	3581/udp	0.000000	# Ascent Capture Licensing
press	3582/tcp	0.000000	# PEG PRESS Server
press	3582/udp	0.000000	# PEG PRESS Server
canex-watch	3583/tcp	0.000000	# CANEX Watch System
canex-watch	3583/udp	0.000000	# CANEX Watch System
u-dbap	3584/tcp	0.000000	# U-DBase Access Protocol
u-dbap	3584/udp	0.000000	# U-DBase Access Protocol
emprise-lls	3585/tcp	0.000000	# Emprise License Server
emprise-lls	3585/udp	0.000000	# Emprise License Server
emprise-lsc	3586/tcp	0.000076	# License Server Console
emprise-lsc	3586/udp	0.000000	# License Server Console
p2pgroup	3587/tcp	0.000000	# Peer to Peer Grouping
p2pgroup	3587/udp	0.000000	# Peer to Peer Grouping
sentinel	3588/tcp	0.000000	# Sentinel Server
sentinel	3588/udp	0.000000	# Sentinel Server
isomair	3589/tcp	0.000000
isomair	3589/udp	0.000000
wv-csp-sms	3590/tcp	0.000000	# WV CSP SMS Binding
wv-csp-sms	3590/udp	0.000000	# WV CSP SMS Binding
gtrack-server	3591/tcp	0.000000	# LOCANIS G-TRACK Server
gtrack-server	3591/udp	0.000330	# LOCANIS G-TRACK Server
gtrack-ne	3592/tcp	0.000000	# LOCANIS G-TRACK NE Port
gtrack-ne	3592/udp	0.000000	# LOCANIS G-TRACK NE Port
bpmd	3593/tcp	0.000000	# BP Model Debugger
bpmd	3593/udp	0.000000	# BP Model Debugger
mediaspace	3594/tcp	0.000000
mediaspace	3594/udp	0.000330
shareapp	3595/tcp	0.000000
shareapp	3595/udp	0.000330
iw-mmogame	3596/tcp	0.000000	# Illusion Wireless MMOG
iw-mmogame	3596/udp	0.000000	# Illusion Wireless MMOG
a14	3597/tcp	0.000000	# A14 (AN-to-SC/MM)
a14	3597/udp	0.000000	# A14 (AN-to-SC/MM)
a15	3598/tcp	0.000000	# A15 (AN-to-AN)
a15	3598/udp	0.000000	# A15 (AN-to-AN)
quasar-server	3599/tcp	0.000076	# Quasar Accounting Server
quasar-server	3599/udp	0.000000	# Quasar Accounting Server
trap-daemon	3600/tcp	0.000076	# text relay-answer
trap-daemon	3600/udp	0.000000	# text relay-answer
visinet-gui	3601/tcp	0.000000	# Visinet Gui
visinet-gui	3601/udp	0.000000	# Visinet Gui
infiniswitchcl	3602/tcp	0.000076	# InfiniSwitch Mgr Client
infiniswitchcl	3602/udp	0.000000	# InfiniSwitch Mgr Client
int-rcv-cntrl	3603/tcp	0.000076	# Integrated Rcvr Control
int-rcv-cntrl	3603/udp	0.000330	# Integrated Rcvr Control
bmc-jmx-port	3604/tcp	0.000000	# BMC JMX Port
bmc-jmx-port	3604/udp	0.000000	# BMC JMX Port
comcam-io	3605/tcp	0.000000	# ComCam IO Port
comcam-io	3605/udp	0.000330	# ComCam IO Port
splitlock	3606/tcp	0.000000	# Splitlock Server
splitlock	3606/udp	0.000330	# Splitlock Server
precise-i3	3607/tcp	0.000000	# Precise I3
precise-i3	3607/udp	0.000000	# Precise I3
trendchip-dcp	3608/tcp	0.000000	# Trendchip control protocol
trendchip-dcp	3608/udp	0.000000	# Trendchip control protocol
cpdi-pidas-cm	3609/tcp	0.000000	# CPDI PIDAS Connection Mon
cpdi-pidas-cm	3609/udp	0.000330	# CPDI PIDAS Connection Mon
echonet	3610/tcp	0.000000
echonet	3610/udp	0.000000
six-degrees	3611/tcp	0.000000	# Six Degrees Port
six-degrees	3611/udp	0.000000	# Six Degrees Port
hp-dataprotect	3612/tcp	0.000000	# dataprotector | HP Data Protector | Micro Focus Data Protector
hp-dataprotect	3612/udp	0.000330	# HP Data Protector
alaris-disc	3613/tcp	0.000000	# Alaris Device Discovery
alaris-disc	3613/udp	0.000000	# Alaris Device Discovery
sigma-port	3614/tcp	0.000000	# Invensys Sigma Port | Satchwell Sigma
sigma-port	3614/udp	0.000330	# Invensys Sigma Port
start-network	3615/tcp	0.000000	# Start Messaging Network
start-network	3615/udp	0.000000	# Start Messaging Network
cd3o-protocol	3616/tcp	0.000000	# cd3o Control Protocol
cd3o-protocol	3616/udp	0.000000	# cd3o Control Protocol
sharp-server	3617/tcp	0.000000	# ATI SHARP Logic Engine
sharp-server	3617/udp	0.000000	# ATI SHARP Logic Engine
aairnet-1	3618/tcp	0.000000	# AAIR-Network 1
aairnet-1	3618/udp	0.000000	# AAIR-Network 1
aairnet-2	3619/tcp	0.000000	# AAIR-Network 2
aairnet-2	3619/udp	0.000330	# AAIR-Network 2
ep-pcp	3620/tcp	0.000000	# EPSON Projector Control Port
ep-pcp	3620/udp	0.000330	# EPSON Projector Control Port
ep-nsp	3621/tcp	0.000076	# EPSON Network Screen Port
ep-nsp	3621/udp	0.000000	# EPSON Network Screen Port
ff-lr-port	3622/tcp	0.000076	# FF LAN Redundancy Port
ff-lr-port	3622/udp	0.000000	# FF LAN Redundancy Port
haipe-discover	3623/tcp	0.000000	# HAIPIS Dynamic Discovery
haipe-discover	3623/udp	0.000000	# HAIPIS Dynamic Discovery
dist-upgrade	3624/tcp	0.000000	# Distributed Upgrade Port
dist-upgrade	3624/udp	0.000330	# Distributed Upgrade Port
volley	3625/tcp	0.000000
volley	3625/udp	0.000000
bvcdaemon-port	3626/tcp	0.000000	# bvControl Daemon
bvcdaemon-port	3626/udp	0.000000	# bvControl Daemon
jamserverport	3627/tcp	0.000000	# Jam Server Port
jamserverport	3627/udp	0.000000	# Jam Server Port
ept-machine	3628/tcp	0.000000	# EPT Machine Interface
ept-machine	3628/udp	0.000000	# EPT Machine Interface
escvpnet	3629/tcp	0.000000	# ESC/VP.net
escvpnet	3629/udp	0.000000	# ESC/VP.net
cs-remote-db	3630/tcp	0.000000	# C&S Remote Database Port
cs-remote-db	3630/udp	0.000000	# C&S Remote Database Port
cs-services	3631/tcp	0.000000	# C&S Web Services Port
cs-services	3631/udp	0.000661	# C&S Web Services Port
distccd	3632/tcp	0.000100	# distcc | Distributed compiler daemon | distributed compiler
distcc	3632/udp	0.000000	# distributed compiler
wacp	3633/tcp	0.000000	# Wyrnix AIS port
wacp	3633/udp	0.000000	# Wyrnix AIS port
hlibmgr	3634/tcp	0.000000	# hNTSP Library Manager
hlibmgr	3634/udp	0.000000	# hNTSP Library Manager
sdo	3635/tcp	0.000000	# Simple Distributed Objects
sdo	3635/udp	0.000000	# Simple Distributed Objects
servistaitsm	3636/tcp	0.000076
servistaitsm	3636/udp	0.000000
scservp	3637/tcp	0.000076	# Customer Service Port
scservp	3637/udp	0.000000	# Customer Service Port
ehp-backup	3638/tcp	0.000000	# EHP Backup Protocol
ehp-backup	3638/udp	0.000000	# EHP Backup Protocol
xap-ha	3639/tcp	0.000000	# Extensible Automation
xap-ha	3639/udp	0.000000	# Extensible Automation
netplay-port1	3640/tcp	0.000000	# Netplay Port 1
netplay-port1	3640/udp	0.000000	# Netplay Port 1
netplay-port2	3641/tcp	0.000000	# Netplay Port 2
netplay-port2	3641/udp	0.000000	# Netplay Port 2
juxml-port	3642/tcp	0.000000	# Juxml Replication port
juxml-port	3642/udp	0.000000	# Juxml Replication port
audiojuggler	3643/tcp	0.000000
audiojuggler	3643/udp	0.000330
ssowatch	3644/tcp	0.000000
ssowatch	3644/udp	0.000000
cyc	3645/tcp	0.000000
cyc	3645/udp	0.000000
xss-srv-port	3646/tcp	0.000000	# XSS Server Port
xss-srv-port	3646/udp	0.000000	# XSS Server Port
splitlock-gw	3647/tcp	0.000000	# Splitlock Gateway
splitlock-gw	3647/udp	0.000000	# Splitlock Gateway
fjcp	3648/tcp	0.000000	# Fujitsu Cooperation Port
fjcp	3648/udp	0.000000	# Fujitsu Cooperation Port
nmmp	3649/tcp	0.000000	# Nishioka Miyuki Msg Protocol
nmmp	3649/udp	0.000330	# Nishioka Miyuki Msg Protocol
prismiq-plugin	3650/tcp	0.000000	# PRISMIQ VOD plug-in
prismiq-plugin	3650/udp	0.000330	# PRISMIQ VOD plug-in
xrpc-registry	3651/tcp	0.000000	# XRPC Registry
xrpc-registry	3651/udp	0.000000	# XRPC Registry
vxcrnbuport	3652/tcp	0.000076	# VxCR NBU Default Port
vxcrnbuport	3652/udp	0.000000	# VxCR NBU Default Port
tsp	3653/tcp	0.000076	# Tunnel Setup Protocol
tsp	3653/udp	0.000330	# Tunnel Setup Protocol
vaprtm	3654/tcp	0.000000	# VAP RealTime Messenger
vaprtm	3654/udp	0.000000	# VAP RealTime Messenger
abatemgr	3655/tcp	0.000000	# ActiveBatch Exec Agent
abatemgr	3655/udp	0.000000	# ActiveBatch Exec Agent
abatjss	3656/tcp	0.000076	# ActiveBatch Job Scheduler
abatjss	3656/udp	0.000000	# ActiveBatch Job Scheduler
immedianet-bcn	3657/tcp	0.000000	# ImmediaNet Beacon
immedianet-bcn	3657/udp	0.000000	# ImmediaNet Beacon
ps-ams	3658/tcp	0.000076	# PlayStation AMS (Secure)
ps-ams	3658/udp	0.000000	# PlayStation AMS (Secure)
apple-sasl	3659/tcp	0.000380	# Apple SASL
apple-sasl	3659/udp	0.006277	# Apple SASL
can-nds-ssl	3660/tcp	0.000000	# IBM Tivoli Directory Service using SSL
can-nds-ssl	3660/udp	0.000000	# IBM Tivoli Directory Service using SSL
can-ferret-ssl	3661/tcp	0.000000	# IBM Tivoli Directory Service using SSL
can-ferret-ssl	3661/udp	0.000000	# IBM Tivoli Directory Service using SSL
pserver	3662/tcp	0.000000
pserver	3662/udp	0.000000
dtp	3663/tcp	0.000076	# DIRECWAY Tunnel Protocol
dtp	3663/udp	0.000000	# DIRECWAY Tunnel Protocol
ups-engine	3664/tcp	0.000000	# UPS Engine Port
ups-engine	3664/udp	0.001652	# UPS Engine Port
ent-engine	3665/tcp	0.000000	# Enterprise Engine Port
ent-engine	3665/udp	0.000330	# Enterprise Engine Port
eserver-pap	3666/tcp	0.000000	# IBM eServer PAP | IBM EServer PAP
eserver-pap	3666/udp	0.000000	# IBM EServer PAP
infoexch	3667/tcp	0.000000	# IBM Information Exchange
infoexch	3667/udp	0.000000	# IBM Information Exchange
dell-rm-port	3668/tcp	0.000000	# Dell Remote Management
dell-rm-port	3668/udp	0.000330	# Dell Remote Management
casanswmgmt	3669/tcp	0.000076	# CA SAN Switch Management
casanswmgmt	3669/udp	0.000330	# CA SAN Switch Management
smile	3670/tcp	0.000076	# SMILE TCP/UDP Interface
smile	3670/udp	0.000330	# SMILE TCP/UDP Interface
efcp	3671/tcp	0.000000	# e Field Control (EIBnet)
efcp	3671/udp	0.000330	# e Field Control (EIBnet)
lispworks-orb	3672/tcp	0.000076	# LispWorks ORB
lispworks-orb	3672/udp	0.000330	# LispWorks ORB
mediavault-gui	3673/tcp	0.000000	# Openview Media Vault GUI
mediavault-gui	3673/udp	0.000000	# Openview Media Vault GUI
wininstall-ipc	3674/tcp	0.000000	# WinINSTALL IPC Port
wininstall-ipc	3674/udp	0.000000	# WinINSTALL IPC Port
calltrax	3675/tcp	0.000000	# CallTrax Data Port
calltrax	3675/udp	0.000000	# CallTrax Data Port
va-pacbase	3676/tcp	0.000000	# VisualAge Pacbase server
va-pacbase	3676/udp	0.000000	# VisualAge Pacbase server
roverlog	3677/tcp	0.000000	# RoverLog IPC
roverlog	3677/udp	0.000000	# RoverLog IPC
ipr-dglt	3678/tcp	0.000000	# DataGuardianLT
ipr-dglt	3678/udp	0.000000	# DataGuardianLT
newton-dock	3679/tcp	0.000000	# #ERROR:Escale (Newton Dock) | Newton Dock
newton-dock	3679/udp	0.000000	# Newton Dock
npds-tracker	3680/tcp	0.000076	# NPDS Tracker
npds-tracker	3680/udp	0.000000	# NPDS Tracker
bts-x73	3681/tcp	0.000076	# BTS X73 Port
bts-x73	3681/udp	0.000000	# BTS X73 Port
cas-mapi	3682/tcp	0.000000	# EMC SmartPackets-MAPI
cas-mapi	3682/udp	0.000000	# EMC SmartPackets-MAPI
bmc-ea	3683/tcp	0.000076	# BMC EDV/EA
bmc-ea	3683/udp	0.000330	# BMC EDV/EA
faxstfx-port	3684/tcp	0.000152	# FAXstfX
faxstfx-port	3684/udp	0.000000	# FAXstfX
dsx-agent	3685/tcp	0.000000	# DS Expert Agent
dsx-agent	3685/udp	0.000000	# DS Expert Agent
tnmpv2	3686/tcp	0.000000	# Trivial Network Management
tnmpv2	3686/udp	0.000000	# Trivial Network Management
simple-push	3687/tcp	0.000000
simple-push	3687/udp	0.000000
simple-push-s	3688/tcp	0.000000	# simple-push Secure
simple-push-s	3688/udp	0.000000	# simple-push Secure
rendezvous	3689/tcp	0.002283	# daap | Rendezvous Zeroconf (used by Apple/iTunes) | Digital Audio Access Protocol (iTunes)
daap	3689/udp	0.000330	# Digital Audio Access Protocol
svn	3690/tcp	0.001597	# Subversion
svn	3690/udp	0.000000	# Subversion
magaya-network	3691/tcp	0.000000	# Magaya Network Port
magaya-network	3691/udp	0.000000	# Magaya Network Port
intelsync	3692/tcp	0.000000	# Brimstone IntelSync
intelsync	3692/udp	0.000330	# Brimstone IntelSync
easl	3693/tcp	0.000000	# Emergency Automatic Structure Lockdown System
bmc-data-coll	3695/tcp	0.000000	# BMC Data Collection
bmc-data-coll	3695/udp	0.000000	# BMC Data Collection
telnetcpcd	3696/tcp	0.000000	# Telnet Com Port Control
telnetcpcd	3696/udp	0.000000	# Telnet Com Port Control
nw-license	3697/tcp	0.000152	# NavisWorks License System | NavisWorks Licnese System
nw-license	3697/udp	0.000330	# NavisWorks Licnese System
sagectlpanel	3698/tcp	0.000000
sagectlpanel	3698/udp	0.000330
kpn-icw	3699/tcp	0.000000	# Internet Call Waiting
kpn-icw	3699/udp	0.000000	# Internet Call Waiting
lrs-paging	3700/tcp	0.000152	# LRS NetPage
lrs-paging	3700/udp	0.000330	# LRS NetPage
netcelera	3701/tcp	0.000000
netcelera	3701/udp	0.000000
ws-discovery	3702/tcp	0.000000	# Web Service Discovery
ws-discovery	3702/udp	0.001982	# Web Service Discovery
adobeserver-3	3703/tcp	0.002357	# Adobe Server 3
adobeserver-3	3703/udp	0.009580	# Adobe Server 3
adobeserver-4	3704/tcp	0.000000	# Adobe Server 4
adobeserver-4	3704/udp	0.000000	# Adobe Server 4
adobeserver-5	3705/tcp	0.000000	# Adobe Server 5
adobeserver-5	3705/udp	0.000000	# Adobe Server 5
rt-event	3706/tcp	0.000000	# Real-Time Event Port
rt-event	3706/udp	0.000000	# Real-Time Event Port
rt-event-s	3707/tcp	0.000000	# Real-Time Event Secure Port
rt-event-s	3707/udp	0.000000	# Real-Time Event Secure Port
sun-as-iiops	3708/tcp	0.000000	# Sun App Svr - Naming
sun-as-iiops	3708/udp	0.000000	# Sun App Svr - Naming
ca-idms	3709/tcp	0.000000	# CA-IDMS Server
ca-idms	3709/udp	0.000330	# CA-IDMS Server
portgate-auth	3710/tcp	0.000000	# PortGate Authentication
portgate-auth	3710/udp	0.000330	# PortGate Authentication
edb-server2	3711/tcp	0.000000	# EBD Server 2
edb-server2	3711/udp	0.000000	# EBD Server 2
sentinel-ent	3712/tcp	0.000076	# Sentinel Enterprise
sentinel-ent	3712/udp	0.000000	# Sentinel Enterprise
tftps	3713/tcp	0.000000	# TFTP over TLS
tftps	3713/udp	0.000000	# TFTP over TLS
delos-dms	3714/tcp	0.000000	# DELOS Direct Messaging
delos-dms	3714/udp	0.000000	# DELOS Direct Messaging
anoto-rendezv	3715/tcp	0.000000	# Anoto Rendezvous Port
anoto-rendezv	3715/udp	0.000000	# Anoto Rendezvous Port
wv-csp-sms-cir	3716/tcp	0.000000	# WV CSP SMS CIR Channel
wv-csp-sms-cir	3716/udp	0.000000	# WV CSP SMS CIR Channel
wv-csp-udp-cir	3717/tcp	0.000000	# WV CSP UDP/IP CIR Channel
wv-csp-udp-cir	3717/udp	0.000000	# WV CSP UDP/IP CIR Channel
opus-services	3718/tcp	0.000000	# OPUS Server Port
opus-services	3718/udp	0.000000	# OPUS Server Port
itelserverport	3719/tcp	0.000000	# iTel Server Port
itelserverport	3719/udp	0.000000	# iTel Server Port
ufastro-instr	3720/tcp	0.000000	# UF Astro. Instr. Services
ufastro-instr	3720/udp	0.000000	# UF Astro. Instr. Services
xsync	3721/tcp	0.000000
xsync	3721/udp	0.000000
xserveraid	3722/tcp	0.000000	# Xserve RAID
xserveraid	3722/udp	0.000000	# Xserve RAID
sychrond	3723/tcp	0.000000	# Sychron Service Daemon
sychrond	3723/udp	0.000000	# Sychron Service Daemon
blizwow	3724/tcp	0.000000	# World of Warcraft
blizwow	3724/udp	0.000000	# World of Warcraft
na-er-tip	3725/tcp	0.000000	# Netia NA-ER Port
na-er-tip	3725/udp	0.000330	# Netia NA-ER Port
array-manager	3726/tcp	0.000000	# Xyratex Array Manager | Xyartex Array Manager
array-manager	3726/udp	0.000000	# Xyartex Array Manager
e-mdu	3727/tcp	0.000000	# Ericsson Mobile Data Unit
e-mdu	3727/udp	0.000000	# Ericsson Mobile Data Unit
e-woa	3728/tcp	0.000076	# Ericsson Web on Air
e-woa	3728/udp	0.000000	# Ericsson Web on Air
fksp-audit	3729/tcp	0.000000	# Fireking Audit Port
fksp-audit	3729/udp	0.000000	# Fireking Audit Port
client-ctrl	3730/tcp	0.000000	# Client Control
client-ctrl	3730/udp	0.000000	# Client Control
smap	3731/tcp	0.000152	# Service Manager
smap	3731/udp	0.000000	# Service Manager
m-wnn	3732/tcp	0.000000	# Mobile Wnn
m-wnn	3732/udp	0.000000	# Mobile Wnn
multip-msg	3733/tcp	0.000000	# Multipuesto Msg Port
multip-msg	3733/udp	0.000000	# Multipuesto Msg Port
synel-data	3734/tcp	0.000000	# Synel Data Collection Port
synel-data	3734/udp	0.000330	# Synel Data Collection Port
pwdis	3735/tcp	0.000000	# Password Distribution
pwdis	3735/udp	0.000000	# Password Distribution
rs-rmi	3736/tcp	0.000000	# RealSpace RMI
rs-rmi	3736/udp	0.000000	# RealSpace RMI
xpanel	3737/tcp	0.000304	# XPanel Daemon
versatalk	3738/tcp	0.000000	# versaTalk Server Port
versatalk	3738/udp	0.000000	# versaTalk Server Port
launchbird-lm	3739/tcp	0.000000	# Launchbird LicenseManager
launchbird-lm	3739/udp	0.000000	# Launchbird LicenseManager
heartbeat	3740/tcp	0.000000	# Heartbeat Protocol
heartbeat	3740/udp	0.000000	# Heartbeat Protocol
wysdma	3741/tcp	0.000000	# WysDM Agent
wysdma	3741/udp	0.000000	# WysDM Agent
cst-port	3742/tcp	0.000076	# CST - Configuration & Service Tracker
cst-port	3742/udp	0.000000	# CST - Configuration & Service Tracker
ipcs-command	3743/tcp	0.000000	# IP Control Systems Ltd.
ipcs-command	3743/udp	0.000000	# IP Control Systems Ltd.
sasg	3744/tcp	0.000000
sasg	3744/udp	0.000330
gw-call-port	3745/tcp	0.000000	# GWRTC Call Port
gw-call-port	3745/udp	0.000000	# GWRTC Call Port
linktest	3746/tcp	0.000000	# LXPRO.COM LinkTest
linktest	3746/udp	0.000000	# LXPRO.COM LinkTest
linktest-s	3747/tcp	0.000000	# LXPRO.COM LinkTest SSL
linktest-s	3747/udp	0.000000	# LXPRO.COM LinkTest SSL
webdata	3748/tcp	0.000000
webdata	3748/udp	0.000000
cimtrak	3749/tcp	0.000076
cimtrak	3749/udp	0.000000
cbos-ip-port	3750/tcp	0.000000	# CBOS/IP ncapsalation port | CBOS/IP ncapsalatoin port
cbos-ip-port	3750/udp	0.000000	# CBOS/IP ncapsalatoin port
gprs-cube	3751/tcp	0.000000	# CommLinx GPRS Cube
gprs-cube	3751/udp	0.000330	# CommLinx GPRS Cube
vipremoteagent	3752/tcp	0.000000	# Vigil-IP RemoteAgent
vipremoteagent	3752/udp	0.000000	# Vigil-IP RemoteAgent
nattyserver	3753/tcp	0.000000	# NattyServer Port
nattyserver	3753/udp	0.000000	# NattyServer Port
timestenbroker	3754/tcp	0.000000	# TimesTen Broker Port
timestenbroker	3754/udp	0.000000	# TimesTen Broker Port
sas-remote-hlp	3755/tcp	0.000000	# SAS Remote Help Server
sas-remote-hlp	3755/udp	0.000000	# SAS Remote Help Server
canon-capt	3756/tcp	0.000000	# Canon CAPT Port
canon-capt	3756/udp	0.000000	# Canon CAPT Port
grf-port	3757/tcp	0.000000	# GRF Server Port
grf-port	3757/udp	0.000000	# GRF Server Port
apw-registry	3758/tcp	0.000000	# apw RMI registry
apw-registry	3758/udp	0.000000	# apw RMI registry
exapt-lmgr	3759/tcp	0.000000	# Exapt License Manager
exapt-lmgr	3759/udp	0.000000	# Exapt License Manager
adtempusclient	3760/tcp	0.000000	# adTempus Client | adTEmpus Client
adtempusclient	3760/udp	0.000000	# adTEmpus Client
gsakmp	3761/tcp	0.000000	# gsakmp port
gsakmp	3761/udp	0.000000	# gsakmp port
gbs-smp	3762/tcp	0.000000	# GBS SnapMail Protocol
gbs-smp	3762/udp	0.000000	# GBS SnapMail Protocol
xo-wave	3763/tcp	0.000000	# XO Wave Control Port
xo-wave	3763/udp	0.000000	# XO Wave Control Port
mni-prot-rout	3764/tcp	0.000000	# MNI Protected Routing
mni-prot-rout	3764/udp	0.000000	# MNI Protected Routing
rtraceroute	3765/tcp	0.000076	# Remote Traceroute
rtraceroute	3765/udp	0.000000	# Remote Traceroute
sitewatch-s	3766/tcp	0.000380	# SSL e-watch sitewatch server
listmgr-port	3767/tcp	0.000000	# ListMGR Port
listmgr-port	3767/udp	0.000000	# ListMGR Port
rblcheckd	3768/tcp	0.000000	# rblcheckd server daemon
rblcheckd	3768/udp	0.000000	# rblcheckd server daemon
haipe-otnk	3769/tcp	0.000000	# HAIPE Network Keying
haipe-otnk	3769/udp	0.000330	# HAIPE Network Keying
cindycollab	3770/tcp	0.000000	# Cinderella Collaboration
cindycollab	3770/udp	0.000000	# Cinderella Collaboration
paging-port	3771/tcp	0.000000	# RTP Paging Port
paging-port	3771/udp	0.000330	# RTP Paging Port
ctp	3772/tcp	0.000000	# Chantry Tunnel Protocol
ctp	3772/udp	0.000000	# Chantry Tunnel Protocol
ctdhercules	3773/tcp	0.000000
ctdhercules	3773/udp	0.000000
zicom	3774/tcp	0.000000
zicom	3774/udp	0.000330
ispmmgr	3775/tcp	0.000000	# ISPM Manager Port
ispmmgr	3775/udp	0.000000	# ISPM Manager Port
dvcprov-port	3776/tcp	0.000000	# Device Provisioning Port
dvcprov-port	3776/udp	0.000330	# Device Provisioning Port
jibe-eb	3777/tcp	0.000000	# Jibe EdgeBurst
jibe-eb	3777/udp	0.000000	# Jibe EdgeBurst
c-h-it-port	3778/tcp	0.000000	# Cutler-Hammer IT Port
c-h-it-port	3778/udp	0.000000	# Cutler-Hammer IT Port
cognima	3779/tcp	0.000000	# Cognima Replication
cognima	3779/udp	0.000000	# Cognima Replication
nnp	3780/tcp	0.000000	# Nuzzler Network Protocol
nnp	3780/udp	0.000000	# Nuzzler Network Protocol
abcvoice-port	3781/tcp	0.000000	# ABCvoice server port
abcvoice-port	3781/udp	0.000000	# ABCvoice server port
iso-tp0s	3782/tcp	0.000000	# Secure ISO TP0 port
iso-tp0s	3782/udp	0.000000	# Secure ISO TP0 port
bim-pem	3783/tcp	0.000000	# Impact Mgr./PEM Gateway
bim-pem	3783/udp	0.000330	# Impact Mgr./PEM Gateway
bfd-control	3784/tcp	0.000380	# BFD Control Protocol
bfd-control	3784/udp	0.000661	# BFD Control Protocol
bfd-echo	3785/tcp	0.000000	# BFD Echo Protocol
bfd-echo	3785/udp	0.000000	# BFD Echo Protocol
upstriggervsw	3786/tcp	0.000000	# VSW Upstrigger port
upstriggervsw	3786/udp	0.000000	# VSW Upstrigger port
fintrx	3787/tcp	0.000076
fintrx	3787/udp	0.000000
isrp-port	3788/tcp	0.000076	# SPACEWAY Routing port
isrp-port	3788/udp	0.000330	# SPACEWAY Routing port
remotedeploy	3789/tcp	0.000000	# RemoteDeploy Administration Port [July 2003]
remotedeploy	3789/udp	0.000000	# RemoteDeploy Administration Port [July 2003]
quickbooksrds	3790/tcp	0.000076	# QuickBooks RDS
quickbooksrds	3790/udp	0.000000	# QuickBooks RDS
tvnetworkvideo	3791/tcp	0.000000	# TV NetworkVideo Data port
tvnetworkvideo	3791/udp	0.000000	# TV NetworkVideo Data port
sitewatch	3792/tcp	0.000152	# e-Watch Corporation SiteWatch
sitewatch	3792/udp	0.000000	# e-Watch Corporation SiteWatch
dcsoftware	3793/tcp	0.000076	# DataCore Software
dcsoftware	3793/udp	0.000000	# DataCore Software
jaus	3794/tcp	0.000000	# JAUS Robots
jaus	3794/udp	0.000000	# JAUS Robots
myblast	3795/tcp	0.000076	# myBLAST Mekentosj port
myblast	3795/udp	0.000000	# myBLAST Mekentosj port
spw-dialer	3796/tcp	0.000076	# Spaceway Dialer
spw-dialer	3796/udp	0.000330	# Spaceway Dialer
idps	3797/tcp	0.000000
idps	3797/udp	0.000000
minilock	3798/tcp	0.000076
minilock	3798/udp	0.000000
radius-dynauth	3799/tcp	0.000076	# RADIUS Dynamic Authorization
radius-dynauth	3799/udp	0.000330	# RADIUS Dynamic Authorization
pwgpsi	3800/tcp	0.000228	# Print Services Interface
pwgpsi	3800/udp	0.000000	# Print Services Interface
ibm-mgr	3801/tcp	0.000380	# ibm manager service
ibm-mgr	3801/udp	0.000000	# ibm manager service
vhd	3802/tcp	0.000000
vhd	3802/udp	0.000000
soniqsync	3803/tcp	0.000076
soniqsync	3803/udp	0.000000
iqnet-port	3804/tcp	0.000000	# Harman IQNet Port
iqnet-port	3804/udp	0.000000	# Harman IQNet Port
tcpdataserver	3805/tcp	0.000000	# ThorGuard Server Port
tcpdataserver	3805/udp	0.000000	# ThorGuard Server Port
wsmlb	3806/tcp	0.000076	# Remote System Manager
wsmlb	3806/udp	0.000000	# Remote System Manager
spugna	3807/tcp	0.000000	# SpuGNA Communication Port
spugna	3807/udp	0.000000	# SpuGNA Communication Port
sun-as-iiops-ca	3808/tcp	0.000152	# Sun App Svr-IIOPClntAuth
sun-as-iiops-ca	3808/udp	0.000000	# Sun App Svr-IIOPClntAuth
apocd	3809/tcp	0.000228	# Java Desktop System Configuration Agent
apocd	3809/udp	0.000000	# Java Desktop System Configuration Agent
wlanauth	3810/tcp	0.000076	# WLAN AS server
wlanauth	3810/udp	0.000000	# WLAN AS server
amp	3811/tcp	0.000076
amp	3811/udp	0.000000
neto-wol-server	3812/tcp	0.000076	# netO WOL Server
neto-wol-server	3812/udp	0.000000	# netO WOL Server
rap-ip	3813/tcp	0.000076	# Rhapsody Interface Protocol
rap-ip	3813/udp	0.000330	# Rhapsody Interface Protocol
neto-dcs	3814/tcp	0.000228	# netO DCS
neto-dcs	3814/udp	0.000000	# netO DCS
lansurveyorxml	3815/tcp	0.000000	# LANsurveyor XML
lansurveyorxml	3815/udp	0.000330	# LANsurveyor XML
sunlps-http	3816/tcp	0.000000	# Sun Local Patch Server
sunlps-http	3816/udp	0.000000	# Sun Local Patch Server
tapeware	3817/tcp	0.000076	# Yosemite Tech Tapeware
tapeware	3817/udp	0.000000	# Yosemite Tech Tapeware
crinis-hb	3818/tcp	0.000000	# Crinis Heartbeat
crinis-hb	3818/udp	0.000000	# Crinis Heartbeat
epl-slp	3819/tcp	0.000000	# EPL Sequ Layer Protocol
epl-slp	3819/udp	0.000000	# EPL Sequ Layer Protocol
scp	3820/tcp	0.000152	# Siemens AuD SCP
scp	3820/udp	0.000000	# Siemens AuD SCP
pmcp	3821/tcp	0.000000	# ATSC PMCP Standard
pmcp	3821/udp	0.000000	# ATSC PMCP Standard
acp-discovery	3822/tcp	0.000000	# Compute Pool Discovery
acp-discovery	3822/udp	0.000000	# Compute Pool Discovery
acp-conduit	3823/tcp	0.000076	# Compute Pool Conduit
acp-conduit	3823/udp	0.000000	# Compute Pool Conduit
acp-policy	3824/tcp	0.000152	# Compute Pool Policy
acp-policy	3824/udp	0.000000	# Compute Pool Policy
ffserver	3825/tcp	0.000076	# Antera FlowFusion Process Simulation
ffserver	3825/udp	0.000000	# Antera FlowFusion Process Simulation
wormux	3826/tcp	0.000228	# warmux | Wormux server | WarMUX game server
wormux	3826/udp	0.000000	# Wormux server
netmpi	3827/tcp	0.000380	# Netadmin Systems MPI service
netmpi	3827/udp	0.000000	# Netadmin Systems MPI service
neteh	3828/tcp	0.000304	# Netadmin Systems Event Handler
neteh	3828/udp	0.000000	# Netadmin Systems Event Handler
neteh-ext	3829/tcp	0.000000	# Netadmin Systems Event Handler External
neteh-ext	3829/udp	0.000000	# Netadmin Systems Event Handler External
cernsysmgmtagt	3830/tcp	0.000076	# Cerner System Management Agent
cernsysmgmtagt	3830/udp	0.000000	# Cerner System Management Agent
dvapps	3831/tcp	0.000076	# Docsvault Application Service
dvapps	3831/udp	0.000000	# Docsvault Application Service
xxnetserver	3832/tcp	0.000000
xxnetserver	3832/udp	0.000000
aipn-auth	3833/tcp	0.000000	# AIPN LS Authentication
aipn-auth	3833/udp	0.000000	# AIPN LS Authentication
spectardata	3834/tcp	0.000000	# Spectar Data Stream Service
spectardata	3834/udp	0.000000	# Spectar Data Stream Service
spectardb	3835/tcp	0.000000	# Spectar Database Rights Service
spectardb	3835/udp	0.000000	# Spectar Database Rights Service
markem-dcp	3836/tcp	0.000000	# MARKEM NEXTGEN DCP
markem-dcp	3836/udp	0.000000	# MARKEM NEXTGEN DCP
mkm-discovery	3837/tcp	0.000076	# MARKEM Auto-Discovery
mkm-discovery	3837/udp	0.000330	# MARKEM Auto-Discovery
sos	3838/tcp	0.000000	# Scito Object Server
sos	3838/udp	0.000000	# Scito Object Server
amx-rms	3839/tcp	0.000076	# AMX Resource Management Suite
amx-rms	3839/udp	0.000000	# AMX Resource Management Suite
flirtmitmir	3840/tcp	0.000000	# www.FlirtMitMir.de
flirtmitmir	3840/udp	0.000000	# www.FlirtMitMir.de
zfirm-shiprush3	3841/tcp	0.000000	# shiprush-db-svr | Z-Firm ShipRush v3 | ShipRush Database Server
zfirm-shiprush3	3841/udp	0.000330	# Z-Firm ShipRush v3
nhci	3842/tcp	0.000076	# NHCI status port
nhci	3842/udp	0.000000	# NHCI status port
quest-agent	3843/tcp	0.000000	# Quest Common Agent
quest-agent	3843/udp	0.000000	# Quest Common Agent
rnm	3844/tcp	0.000000
rnm	3844/udp	0.000000
v-one-spp	3845/tcp	0.000000	# V-ONE Single Port Proxy
v-one-spp	3845/udp	0.000000	# V-ONE Single Port Proxy
an-pcp	3846/tcp	0.000152	# Astare Network PCP
an-pcp	3846/udp	0.000000	# Astare Network PCP
msfw-control	3847/tcp	0.000076	# MS Firewall Control
msfw-control	3847/udp	0.000000	# MS Firewall Control
item	3848/tcp	0.000152	# IT Environmental Monitor
item	3848/udp	0.000330	# IT Environmental Monitor
spw-dnspreload	3849/tcp	0.000152	# SPACEWAY DNS Preload | SPACEWAY DNS Prelaod
spw-dnspreload	3849/udp	0.000000	# SPACEWAY DNS Prelaod
qtms-bootstrap	3850/tcp	0.000076	# QTMS Bootstrap Protocol
qtms-bootstrap	3850/udp	0.000330	# QTMS Bootstrap Protocol
spectraport	3851/tcp	0.000304	# SpectraTalk Port
spectraport	3851/udp	0.000000	# SpectraTalk Port
sse-app-config	3852/tcp	0.000152	# SSE App Configuration
sse-app-config	3852/udp	0.000000	# SSE App Configuration
sscan	3853/tcp	0.000152	# SONY scanning protocol
sscan	3853/udp	0.000000	# SONY scanning protocol
stryker-com	3854/tcp	0.000000	# Stryker Comm Port
stryker-com	3854/udp	0.000000	# Stryker Comm Port
opentrac	3855/tcp	0.000000
opentrac	3855/udp	0.000000
informer	3856/tcp	0.000076
informer	3856/udp	0.000000
trap-port	3857/tcp	0.000000	# Trap Port
trap-port	3857/udp	0.000000	# Trap Port
trap-port-mom	3858/tcp	0.000000	# Trap Port MOM
trap-port-mom	3858/udp	0.000000	# Trap Port MOM
nav-port	3859/tcp	0.000152	# Navini Port
nav-port	3859/udp	0.000000	# Navini Port
sasp	3860/tcp	0.000076	# Server/Application State Protocol (SASP)
sasp	3860/udp	0.000000	# Server/Application State Protocol (SASP)
winshadow-hd	3861/tcp	0.000000	# winShadow Host Discovery
winshadow-hd	3861/udp	0.000000	# winShadow Host Discovery
giga-pocket	3862/tcp	0.000000
giga-pocket	3862/udp	0.000000
asap-sctp	3863/sctp	0.000000	# asap-udp | asap-tcp | RSerPool ASAP (SCTP) | asap tcp port | asap udp port | asap sctp
asap-tcp	3863/tcp	0.000152	# RSerPool ASAP (TCP)
asap-tcp	3863/udp	0.000000	# RSerPool ASAP (UDP)
asap-sctp-tls	3864/sctp	0.000000	# asap-tcp-tls | RSerPool ASAP/TLS (SCTP) | asap/tls tcp port | asap-sctp/tls
asap-tcp-tls	3864/tcp	0.000000	# RSerPool ASAP/TLS (TCP)
xpl	3865/tcp	0.000000	# xpl automation protocol
xpl	3865/udp	0.000000	# xpl automation protocol
dzdaemon	3866/tcp	0.000000	# Sun SDViz DZDAEMON Port
dzdaemon	3866/udp	0.000000	# Sun SDViz DZDAEMON Port
dzoglserver	3867/tcp	0.000000	# Sun SDViz DZOGLSERVER Port
dzoglserver	3867/udp	0.000000	# Sun SDViz DZOGLSERVER Port
diameter	3868/sctp	0.000000
diameter	3868/tcp	0.000076
ovsam-mgmt	3869/tcp	0.000228	# hp OVSAM MgmtServer Disco
ovsam-mgmt	3869/udp	0.000330	# hp OVSAM MgmtServer Disco
ovsam-d-agent	3870/tcp	0.000152	# hp OVSAM HostAgent Disco
ovsam-d-agent	3870/udp	0.000330	# hp OVSAM HostAgent Disco
avocent-adsap	3871/tcp	0.000304	# Avocent DS Authorization
avocent-adsap	3871/udp	0.000000	# Avocent DS Authorization
oem-agent	3872/tcp	0.000152	# OEM Agent
oem-agent	3872/udp	0.000330	# OEM Agent
fagordnc	3873/tcp	0.000000
fagordnc	3873/udp	0.000000
sixxsconfig	3874/tcp	0.000000	# SixXS Configuration
sixxsconfig	3874/udp	0.000000	# SixXS Configuration
pnbscada	3875/tcp	0.000000
pnbscada	3875/udp	0.000000
dl_agent	3876/tcp	0.000076	# dl-agent | DirectoryLockdown Agent
dl_agent	3876/udp	0.000000	# DirectoryLockdown Agent
xmpcr-interface	3877/tcp	0.000000	# XMPCR Interface Port
xmpcr-interface	3877/udp	0.000000	# XMPCR Interface Port
fotogcad	3878/tcp	0.000228	# FotoG CAD interface
fotogcad	3878/udp	0.000000	# FotoG CAD interface
appss-lm	3879/tcp	0.000076	# appss license manager
appss-lm	3879/udp	0.000000	# appss license manager
igrs	3880/tcp	0.000304
igrs	3880/udp	0.000000
idac	3881/tcp	0.000000	# Data Acquisition and Control
idac	3881/udp	0.000000	# Data Acquisition and Control
msdts1	3882/tcp	0.000076	# DTS Service Port
msdts1	3882/udp	0.000330	# DTS Service Port
vrpn	3883/tcp	0.000000	# VR Peripheral Network
vrpn	3883/udp	0.000000	# VR Peripheral Network
softrack-meter	3884/tcp	0.000000	# SofTrack Metering
softrack-meter	3884/udp	0.000330	# SofTrack Metering
topflow-ssl	3885/tcp	0.000000	# TopFlow SSL
topflow-ssl	3885/udp	0.000330	# TopFlow SSL
nei-management	3886/tcp	0.000000	# NEI management port
nei-management	3886/udp	0.000000	# NEI management port
ciphire-data	3887/tcp	0.000000	# Ciphire Data Transport
ciphire-data	3887/udp	0.000000	# Ciphire Data Transport
ciphire-serv	3888/tcp	0.000152	# Ciphire Services
ciphire-serv	3888/udp	0.000000	# Ciphire Services
dandv-tester	3889/tcp	0.000228	# D and V Tester Control Port
dandv-tester	3889/udp	0.000000	# D and V Tester Control Port
ndsconnect	3890/tcp	0.000076	# Niche Data Server Connect
ndsconnect	3890/udp	0.000000	# Niche Data Server Connect
rtc-pm-port	3891/tcp	0.000000	# Oracle RTC-PM port
rtc-pm-port	3891/udp	0.000000	# Oracle RTC-PM port
pcc-image-port	3892/tcp	0.000000
pcc-image-port	3892/udp	0.000000
cgi-starapi	3893/tcp	0.000000	# CGI StarAPI Server
cgi-starapi	3893/udp	0.000000	# CGI StarAPI Server
syam-agent	3894/tcp	0.000000	# SyAM Agent Port
syam-agent	3894/udp	0.000000	# SyAM Agent Port
syam-smc	3895/tcp	0.000000	# SyAm SMC Service Port
syam-smc	3895/udp	0.000000	# SyAm SMC Service Port
sdo-tls	3896/tcp	0.000000	# Simple Distributed Objects over TLS
sdo-tls	3896/udp	0.000000	# Simple Distributed Objects over TLS
sdo-ssh	3897/tcp	0.000076	# Simple Distributed Objects over SSH
sdo-ssh	3897/udp	0.000000	# Simple Distributed Objects over SSH
senip	3898/tcp	0.000000	# IAS, Inc. SmartEye NET Internet Protocol
senip	3898/udp	0.000000	# IAS, Inc. SmartEye NET Internet Protocol
itv-control	3899/tcp	0.000076	# ITV Port
itv-control	3899/udp	0.000000	# ITV Port
udt_os	3900/tcp	0.000050	# udt-os | Unidata UDT OS
udt_os	3900/udp	0.000264	# Unidata UDT OS
nimsh	3901/tcp	0.000076	# NIM Service Handler
nimsh	3901/udp	0.000000	# NIM Service Handler
nimaux	3902/tcp	0.000076	# NIMsh Auxiliary Port
nimaux	3902/udp	0.000000	# NIMsh Auxiliary Port
charsetmgr	3903/tcp	0.000000
charsetmgr	3903/udp	0.000000
omnilink-port	3904/tcp	0.000076	# Arnet Omnilink Port
omnilink-port	3904/udp	0.000330	# Arnet Omnilink Port
mupdate	3905/tcp	0.000228	# Mailbox Update (MUPDATE) protocol
mupdate	3905/udp	0.000000	# Mailbox Update (MUPDATE) protocol
topovista-data	3906/tcp	0.000076	# TopoVista elevation data
topovista-data	3906/udp	0.000000	# TopoVista elevation data
imoguia-port	3907/tcp	0.000152	# Imoguia Port
imoguia-port	3907/udp	0.000330	# Imoguia Port
hppronetman	3908/tcp	0.000076	# HP Procurve NetManagement
hppronetman	3908/udp	0.000000	# HP Procurve NetManagement
surfcontrolcpa	3909/tcp	0.000076	# SurfControl CPA
surfcontrolcpa	3909/udp	0.000000	# SurfControl CPA
prnrequest	3910/tcp	0.000000	# Printer Request Port
prnrequest	3910/udp	0.000661	# Printer Request Port
prnstatus	3911/tcp	0.000076	# Printer Status Port
prnstatus	3911/udp	0.000000	# Printer Status Port
gbmt-stars	3912/tcp	0.000000	# Global Maintech Stars
gbmt-stars	3912/udp	0.000000	# Global Maintech Stars
listcrt-port	3913/tcp	0.000076	# ListCREATOR Port
listcrt-port	3913/udp	0.000000	# ListCREATOR Port
listcrt-port-2	3914/tcp	0.000228	# ListCREATOR Port 2
listcrt-port-2	3914/udp	0.000000	# ListCREATOR Port 2
agcat	3915/tcp	0.000076	# Auto-Graphics Cataloging
agcat	3915/udp	0.000000	# Auto-Graphics Cataloging
wysdmc	3916/tcp	0.000152	# WysDM Controller
wysdmc	3916/udp	0.000000	# WysDM Controller
aftmux	3917/tcp	0.000000	# AFT multiplex port | AFT multiples port
aftmux	3917/udp	0.000000	# AFT multiples port
pktcablemmcops	3918/tcp	0.000304	# PacketCableMultimediaCOPS
pktcablemmcops	3918/udp	0.000000	# PacketCableMultimediaCOPS
hyperip	3919/tcp	0.000076
hyperip	3919/udp	0.000000
exasoftport1	3920/tcp	0.000228	# Exasoft IP Port
exasoftport1	3920/udp	0.000000	# Exasoft IP Port
herodotus-net	3921/tcp	0.000000	# Herodotus Net
herodotus-net	3921/udp	0.000000	# Herodotus Net
sor-update	3922/tcp	0.000076	# Soronti Update Port
sor-update	3922/udp	0.000000	# Soronti Update Port
symb-sb-port	3923/tcp	0.000076	# Symbian Service Broker
symb-sb-port	3923/udp	0.000000	# Symbian Service Broker
mpl-gprs-port	3924/tcp	0.000000	# MPL_GPRS_PORT | MPL_GPRS_Port
mpl-gprs-port	3924/udp	0.000000	# MPL_GPRS_Port
zmp	3925/tcp	0.000000	# Zoran Media Port
zmp	3925/udp	0.000000	# Zoran Media Port
winport	3926/tcp	0.000000
winport	3926/udp	0.000000
natdataservice	3927/tcp	0.000000	# ScsTsr
natdataservice	3927/udp	0.000000	# ScsTsr
netboot-pxe	3928/tcp	0.000076	# PXE NetBoot Manager
netboot-pxe	3928/udp	0.000000	# PXE NetBoot Manager
smauth-port	3929/tcp	0.000152	# AMS Port
smauth-port	3929/udp	0.000000	# AMS Port
syam-webserver	3930/tcp	0.000076	# Syam Web Server Port
syam-webserver	3930/udp	0.000000	# Syam Web Server Port
msr-plugin-port	3931/tcp	0.000152	# MSR Plugin Port
msr-plugin-port	3931/udp	0.000000	# MSR Plugin Port
dyn-site	3932/tcp	0.000000	# Dynamic Site System
dyn-site	3932/udp	0.000000	# Dynamic Site System
plbserve-port	3933/tcp	0.000000	# PL/B App Server User Port
plbserve-port	3933/udp	0.000000	# PL/B App Server User Port
sunfm-port	3934/tcp	0.000000	# PL/B File Manager Port
sunfm-port	3934/udp	0.000000	# PL/B File Manager Port
sdp-portmapper	3935/tcp	0.000076	# SDP Port Mapper Protocol
sdp-portmapper	3935/udp	0.000000	# SDP Port Mapper Protocol
mailprox	3936/tcp	0.000076
mailprox	3936/udp	0.000000
dvbservdsc	3937/tcp	0.000076	# DVB Service Discovery
dvbservdsc	3937/udp	0.000000	# DVB Service Discovery
dbcontrol_agent	3938/tcp	0.000000	# dbcontrol-agent | Oracle dbControl Agent po | Oracel dbControl Agent po
dbcontrol_agent	3938/udp	0.000000	# Oracel dbControl Agent po
aamp	3939/tcp	0.000000	# Anti-virus Application Management Port
aamp	3939/udp	0.000000	# Anti-virus Application Management Port
xecp-node	3940/tcp	0.000076	# XeCP Node Service
xecp-node	3940/udp	0.000000	# XeCP Node Service
homeportal-web	3941/tcp	0.000152	# Home Portal Web Server
homeportal-web	3941/udp	0.000000	# Home Portal Web Server
srdp	3942/tcp	0.000000	# satellite distribution
srdp	3942/udp	0.000000	# satellite distribution
tig	3943/tcp	0.000076	# TetraNode Ip Gateway
tig	3943/udp	0.000000	# TetraNode Ip Gateway
sops	3944/tcp	0.000152	# S-Ops Management
sops	3944/udp	0.000330	# S-Ops Management
emcads	3945/tcp	0.000228	# EMCADS Server Port
emcads	3945/udp	0.000000	# EMCADS Server Port
backupedge	3946/tcp	0.000076	# BackupEDGE Server
backupedge	3946/udp	0.000000	# BackupEDGE Server
ccp	3947/tcp	0.000000	# Connect and Control Protocol for Consumer, Commercial, and Industrial Electronic Devices
ccp	3947/udp	0.000661	# Connect and Control Protocol for Consumer, Commercial, and Industrial Electronic Devices
apdap	3948/tcp	0.000076	# Anton Paar Device Administration Protocol
apdap	3948/udp	0.000000	# Anton Paar Device Administration Protocol
drip	3949/tcp	0.000076	# Dynamic Routing Information Protocol
drip	3949/udp	0.000000	# Dynamic Routing Information Protocol
namemunge	3950/tcp	0.000000	# Name Munging
namemunge	3950/udp	0.000330	# Name Munging
pwgippfax	3951/tcp	0.000000	# PWG IPP Facsimile
pwgippfax	3951/udp	0.000000	# PWG IPP Facsimile
i3-sessionmgr	3952/tcp	0.000076	# I3 Session Manager
i3-sessionmgr	3952/udp	0.000000	# I3 Session Manager
xmlink-connect	3953/tcp	0.000000	# Eydeas XMLink Connect
xmlink-connect	3953/udp	0.000330	# Eydeas XMLink Connect
adrep	3954/tcp	0.000000	# AD Replication RPC
adrep	3954/udp	0.000000	# AD Replication RPC
p2pcommunity	3955/tcp	0.000000
p2pcommunity	3955/udp	0.000330
gvcp	3956/tcp	0.000076	# GigE Vision Control
gvcp	3956/udp	0.000000	# GigE Vision Control
mqe-broker	3957/tcp	0.000152	# MQEnterprise Broker
mqe-broker	3957/udp	0.000000	# MQEnterprise Broker
mqe-agent	3958/tcp	0.000000	# MQEnterprise Agent
mqe-agent	3958/udp	0.000000	# MQEnterprise Agent
treehopper	3959/tcp	0.000000	# Tree Hopper Networking
treehopper	3959/udp	0.000000	# Tree Hopper Networking
bess	3960/tcp	0.000000	# Bess Peer Assessment
bess	3960/udp	0.000000	# Bess Peer Assessment
proaxess	3961/tcp	0.000076	# ProAxess Server
proaxess	3961/udp	0.000000	# ProAxess Server
sbi-agent	3962/tcp	0.000076	# SBI Agent Protocol
sbi-agent	3962/udp	0.000000	# SBI Agent Protocol
thrp	3963/tcp	0.000152	# Teran Hybrid Routing Protocol
thrp	3963/udp	0.000000	# Teran Hybrid Routing Protocol
sasggprs	3964/tcp	0.000076	# SASG GPRS
sasggprs	3964/udp	0.000000	# SASG GPRS
ati-ip-to-ncpe	3965/tcp	0.000000	# Avanti IP to NCPE API
ati-ip-to-ncpe	3965/udp	0.000000	# Avanti IP to NCPE API
bflckmgr	3966/tcp	0.000000	# BuildForge Lock Manager
bflckmgr	3966/udp	0.000000	# BuildForge Lock Manager
ppsms	3967/tcp	0.000076	# PPS Message Service
ppsms	3967/udp	0.000000	# PPS Message Service
ianywhere-dbns	3968/tcp	0.000152	# iAnywhere DBNS
ianywhere-dbns	3968/udp	0.000000	# iAnywhere DBNS
landmarks	3969/tcp	0.000152	# Landmark Messages
landmarks	3969/udp	0.000000	# Landmark Messages
lanrevagent	3970/tcp	0.000000	# LANrev Agent
lanrevagent	3970/udp	0.000330	# LANrev Agent
lanrevserver	3971/tcp	0.000228	# LANrev Server
lanrevserver	3971/udp	0.000330	# LANrev Server
iconp	3972/tcp	0.000152	# ict-control Protocol
iconp	3972/udp	0.000000	# ict-control Protocol
progistics	3973/tcp	0.000000	# ConnectShip Progistics
progistics	3973/udp	0.000000	# ConnectShip Progistics
citysearch	3974/tcp	0.000000	# xk22 | Remote Applicant Tracking Service
citysearch	3974/udp	0.000330	# Remote Applicant Tracking Service
airshot	3975/tcp	0.000076	# Air Shot
airshot	3975/udp	0.000000	# Air Shot
opswagent	3976/tcp	0.000000	# Opsware Agent | Server Automation Agent
opswagent	3976/udp	0.000330	# Opsware Agent
opswmanager	3977/tcp	0.000000	# Opsware Manager
opswmanager	3977/udp	0.000000	# Opsware Manager
secure-cfg-svr	3978/tcp	0.000000	# Secured Configuration Server
secure-cfg-svr	3978/udp	0.000661	# Secured Configuration Server
smwan	3979/tcp	0.000076	# Smith Micro Wide Area Network Service
smwan	3979/udp	0.000000	# Smith Micro Wide Area Network Service
acms	3980/tcp	0.000076	# Aircraft Cabin Management System
acms	3980/udp	0.000000	# Aircraft Cabin Management System
starfish	3981/tcp	0.000152	# Starfish System Admin
starfish	3981/udp	0.000000	# Starfish System Admin
eis	3982/tcp	0.000076	# ESRI Image Server
eis	3982/udp	0.000000	# ESRI Image Server
eisp	3983/tcp	0.000076	# ESRI Image Service
eisp	3983/udp	0.000000	# ESRI Image Service
mapper-nodemgr	3984/tcp	0.000013	# MAPPER network node manager
mapper-nodemgr	3984/udp	0.000527	# MAPPER network node manager
mapper-mapethd	3985/tcp	0.000075	# MAPPER TCP/IP server
mapper-mapethd	3985/udp	0.000758	# MAPPER TCP/IP server
mapper-ws_ethd	3986/tcp	0.003977	# mapper-ws-ethd | MAPPER workstation server
mapper-ws_ethd	3986/udp	0.000544	# MAPPER workstation server
centerline	3987/tcp	0.000000
centerline	3987/udp	0.000000
dcs-config	3988/tcp	0.000000	# DCS Configuration Port
dcs-config	3988/udp	0.000330	# DCS Configuration Port
bv-queryengine	3989/tcp	0.000076	# BindView-Query Engine
bv-queryengine	3989/udp	0.000000	# BindView-Query Engine
bv-is	3990/tcp	0.000152	# BindView-IS
bv-is	3990/udp	0.000000	# BindView-IS
bv-smcsrv	3991/tcp	0.000076	# BindView-SMCServer
bv-smcsrv	3991/udp	0.000000	# BindView-SMCServer
bv-ds	3992/tcp	0.000076	# BindView-DirectoryServer
bv-ds	3992/udp	0.000330	# BindView-DirectoryServer
bv-agent	3993/tcp	0.000152	# BindView-Agent
bv-agent	3993/udp	0.000000	# BindView-Agent
unknown	3994/tcp	0.000152
unknown	3994/udp	0.000330
iss-mgmt-ssl	3995/tcp	0.000304	# ISS Management Svcs SSL
iss-mgmt-ssl	3995/udp	0.000000	# ISS Management Svcs SSL
abcsoftware	3996/tcp	0.000076	# abcsoftware-01
remoteanything	3996/udp	0.000478	# neoworx remote-anything daemon
agentsease-db	3997/tcp	0.000076	# aes_db
remoteanything	3997/udp	0.000544	# neoworx remote-anything daemon
dnx	3998/tcp	0.000380	# Distributed Nagios Executor Service
remoteanything	3998/udp	0.000610	# neoworx remote-anything reserved
remoteanything	3999/tcp	0.000088	# nvcnet | neoworx remote-anything file browser | Norman distributes scanning service
nvcnet	3999/udp	0.000330	# Norman distributes scanning service
remoteanything	4000/tcp	0.001794	# terabase | neoworx remote-anything remote control | Terabase
icq	4000/udp	0.006392	# AOL ICQ instant messaging clent-server communication
newoak	4001/tcp	0.002129
newoak	4001/udp	0.000000
mlchat-proxy	4002/tcp	0.000765	# mlnet - MLChat P2P chat proxy | pxc-spvr-ft
pxc-spvr-ft	4002/udp	0.000330
pxc-splr-ft	4003/tcp	0.000380
pxc-splr-ft	4003/udp	0.000000
pxc-roid	4004/tcp	0.000228
pxc-roid	4004/udp	0.000000
pxc-pin	4005/tcp	0.000228
pxc-pin	4005/udp	0.000330
pxc-spvr	4006/tcp	0.000304
pxc-spvr	4006/udp	0.000330
pxc-splr	4007/tcp	0.000076
pxc-splr	4007/udp	0.000000
netcheque	4008/tcp	0.000075	# NetCheque accounting
netcheque	4008/udp	0.001367	# NetCheque accounting
chimera-hwm	4009/tcp	0.000152	# Chimera HWM
chimera-hwm	4009/udp	0.000000	# Chimera HWM
samsung-unidex	4010/tcp	0.000076	# Samsung Unidex
samsung-unidex	4010/udp	0.000330	# Samsung Unidex
altserviceboot	4011/tcp	0.000000	# Alternate Service Boot
altserviceboot	4011/udp	0.000000	# Alternate Service Boot
pda-gate	4012/tcp	0.000000	# PDA Gate
pda-gate	4012/udp	0.000330	# PDA Gate
acl-manager	4013/tcp	0.000000	# ACL Manager
acl-manager	4013/udp	0.000000	# ACL Manager
taiclock	4014/tcp	0.000000
taiclock	4014/udp	0.000000
talarian-mcast1	4015/tcp	0.000000	# Talarian Mcast
talarian-mcast1	4015/udp	0.000330	# Talarian Mcast
talarian-mcast2	4016/tcp	0.000076	# Talarian Mcast
talarian-mcast2	4016/udp	0.000330	# Talarian Mcast
talarian-mcast3	4017/tcp	0.000000	# Talarian Mcast
talarian-mcast3	4017/udp	0.000330	# Talarian Mcast
talarian-mcast4	4018/tcp	0.000000	# Talarian Mcast
talarian-mcast4	4018/udp	0.000000	# Talarian Mcast
talarian-mcast5	4019/tcp	0.000000	# Talarian Mcast
talarian-mcast5	4019/udp	0.000000	# Talarian Mcast
trap	4020/tcp	0.000076	# TRAP Port
trap	4020/udp	0.000000	# TRAP Port
nexus-portal	4021/tcp	0.000000	# Nexus Portal
nexus-portal	4021/udp	0.000330	# Nexus Portal
dnox	4022/tcp	0.000076
dnox	4022/udp	0.000000
esnm-zoning	4023/tcp	0.000000	# ESNM Zoning Port
esnm-zoning	4023/udp	0.000000	# ESNM Zoning Port
tnp1-port	4024/tcp	0.000076	# TNP1 User Port
tnp1-port	4024/udp	0.000000	# TNP1 User Port
partimage	4025/tcp	0.000076	# Partition Image Port
partimage	4025/udp	0.000000	# Partition Image Port
as-debug	4026/tcp	0.000000	# Graphical Debug Server
as-debug	4026/udp	0.000330	# Graphical Debug Server
bxp	4027/tcp	0.000000	# bitxpress
bxp	4027/udp	0.000000	# bitxpress
dtserver-port	4028/tcp	0.000000	# DTServer Port
dtserver-port	4028/udp	0.000000	# DTServer Port
ip-qsig	4029/tcp	0.000076	# IP Q signaling protocol
ip-qsig	4029/udp	0.000000	# IP Q signaling protocol
jdmn-port	4030/tcp	0.000000	# Accell/JSP Daemon Port
jdmn-port	4030/udp	0.000330	# Accell/JSP Daemon Port
suucp	4031/tcp	0.000000	# UUCP over SSL
suucp	4031/udp	0.000000	# UUCP over SSL
vrts-auth-port	4032/tcp	0.000000	# VERITAS Authorization Service
vrts-auth-port	4032/udp	0.000000	# VERITAS Authorization Service
sanavigator	4033/tcp	0.000000	# SANavigator Peer Port
sanavigator	4033/udp	0.000330	# SANavigator Peer Port
ubxd	4034/tcp	0.000000	# Ubiquinox Daemon
ubxd	4034/udp	0.000000	# Ubiquinox Daemon
wap-push-http	4035/tcp	0.000076	# WAP Push OTA-HTTP port
wap-push-http	4035/udp	0.000000	# WAP Push OTA-HTTP port
wap-push-https	4036/tcp	0.000076	# WAP Push OTA-HTTP secure
wap-push-https	4036/udp	0.000000	# WAP Push OTA-HTTP secure
ravehd	4037/tcp	0.000000	# RaveHD network control
ravehd	4037/udp	0.000000	# RaveHD network control
fazzt-ptp	4038/tcp	0.000000	# Fazzt Point-To-Point
fazzt-ptp	4038/udp	0.000000	# Fazzt Point-To-Point
fazzt-admin	4039/tcp	0.000076	# Fazzt Administration
fazzt-admin	4039/udp	0.000991	# Fazzt Administration
yo-main	4040/tcp	0.000152	# Yo.net main service
yo-main	4040/udp	0.000000	# Yo.net main service
houston	4041/tcp	0.000000	# Rocketeer-Houston
houston	4041/udp	0.000000	# Rocketeer-Houston
ldxp	4042/tcp	0.000000
ldxp	4042/udp	0.000330
nirp	4043/tcp	0.000000	# Neighbour Identity Resolution
nirp	4043/udp	0.000000	# Neighbour Identity Resolution
ltp	4044/tcp	0.000000	# Location Tracking Protocol
ltp	4044/udp	0.000000	# Location Tracking Protocol
lockd	4045/tcp	0.001468	# npp | Network Paging Protocol
lockd	4045/udp	0.006656	# NFS lock daemon/manager
acp-proto	4046/tcp	0.000000	# Accounting Protocol
acp-proto	4046/udp	0.000661	# Accounting Protocol
ctp-state	4047/tcp	0.000000	# Context Transfer Protocol
ctp-state	4047/udp	0.000991	# Context Transfer Protocol
unknown	4048/udp	0.000330
wafs	4049/tcp	0.000000	# Wide Area File Services
wafs	4049/udp	0.000661	# Wide Area File Services
cisco-wafs	4050/tcp	0.000000	# Wide Area File Services
cisco-wafs	4050/udp	0.000000	# Wide Area File Services
cppdp	4051/tcp	0.000000	# Cisco Peer to Peer Distribution Protocol
cppdp	4051/udp	0.000330	# Cisco Peer to Peer Distribution Protocol
interact	4052/tcp	0.000000	# VoiceConnect Interact
interact	4052/udp	0.000000	# VoiceConnect Interact
ccu-comm-1	4053/tcp	0.000000	# CosmoCall Universe Communications Port 1
ccu-comm-1	4053/udp	0.000000	# CosmoCall Universe Communications Port 1
ccu-comm-2	4054/tcp	0.000000	# CosmoCall Universe Communications Port 2
ccu-comm-2	4054/udp	0.000000	# CosmoCall Universe Communications Port 2
ccu-comm-3	4055/tcp	0.000000	# CosmoCall Universe Communications Port 3
ccu-comm-3	4055/udp	0.000000	# CosmoCall Universe Communications Port 3
lms	4056/tcp	0.000076	# Location Message Service
lms	4056/udp	0.000000	# Location Message Service
wfm	4057/tcp	0.000000	# Servigistics WFM server
wfm	4057/udp	0.000000	# Servigistics WFM server
kingfisher	4058/tcp	0.000076	# Kingfisher protocol
kingfisher	4058/udp	0.000000	# Kingfisher protocol
dlms-cosem	4059/tcp	0.000000	# DLMS/COSEM
dlms-cosem	4059/udp	0.000000	# DLMS/COSEM
dsmeter_iatc	4060/tcp	0.000000	# dsmeter-iatc | DSMETER Inter-Agent Transfer Channel
dsmeter_iatc	4060/udp	0.000000	# DSMETER Inter-Agent Transfer Channel
ice-location	4061/tcp	0.000000	# Ice Location Service (TCP)
ice-location	4061/udp	0.000661	# Ice Location Service (TCP)
ice-slocation	4062/tcp	0.000000	# Ice Location Service (SSL)
ice-slocation	4062/udp	0.000000	# Ice Location Service (SSL)
ice-router	4063/tcp	0.000000	# Ice Firewall Traversal Service (TCP)
ice-router	4063/udp	0.000000	# Ice Firewall Traversal Service (TCP)
ice-srouter	4064/tcp	0.000000	# Ice Firewall Traversal Service (SSL)
ice-srouter	4064/udp	0.000000	# Ice Firewall Traversal Service (SSL)
avanti_cdp	4065/tcp	0.000076	# avanti-cdp | Avanti Common Data
avanti_cdp	4065/udp	0.000000	# Avanti Common Data
pmas	4066/tcp	0.000000	# Performance Measurement and Analysis
pmas	4066/udp	0.000000	# Performance Measurement and Analysis
idp	4067/tcp	0.000000	# Information Distribution Protocol
idp	4067/udp	0.000330	# Information Distribution Protocol
ipfltbcst	4068/tcp	0.000000	# IP Fleet Broadcast
ipfltbcst	4068/udp	0.000000	# IP Fleet Broadcast
minger	4069/tcp	0.000000	# Minger Email Address Validation Service
minger	4069/udp	0.000330	# Minger Email Address Validation Service
tripe	4070/tcp	0.000000	# Trivial IP Encryption (TrIPE)
tripe	4070/udp	0.000000	# Trivial IP Encryption (TrIPE)
aibkup	4071/tcp	0.000000	# Automatically Incremental Backup
aibkup	4071/udp	0.000330	# Automatically Incremental Backup
zieto-sock	4072/tcp	0.000000	# Zieto Socket Communications
zieto-sock	4072/udp	0.000000	# Zieto Socket Communications
iRAPP	4073/tcp	0.000000	# iRAPP Server Protocol | Interactive Remote Application Pairing Protocol
iRAPP	4073/udp	0.000330	# iRAPP Server Protocol
cequint-cityid	4074/tcp	0.000000	# Cequint City ID UI trigger
cequint-cityid	4074/udp	0.000000	# Cequint City ID UI trigger
perimlan	4075/tcp	0.000000	# ISC Alarm Message Service
perimlan	4075/udp	0.000000	# ISC Alarm Message Service
seraph	4076/tcp	0.000000	# Seraph DCS
seraph	4076/udp	0.000000	# Seraph DCS
ascomalarm	4077/tcp	0.000000	# Ascom IP Alarming
ascomalarm	4077/udp	0.000330	# Ascom IP Alarming
cssp	4078/tcp	0.000000	# Coordinated Security Service Protocol
santools	4079/tcp	0.000000	# SANtools Diagnostic Server
santools	4079/udp	0.000330	# SANtools Diagnostic Server
lorica-in	4080/tcp	0.000152	# Lorica inside facing
lorica-in	4080/udp	0.000000	# Lorica inside facing
lorica-in-sec	4081/tcp	0.000000	# Lorica inside facing (SSL)
lorica-in-sec	4081/udp	0.000330	# Lorica inside facing (SSL)
lorica-out	4082/tcp	0.000000	# Lorica outside facing
lorica-out	4082/udp	0.000330	# Lorica outside facing
lorica-out-sec	4083/tcp	0.000000	# Lorica outside facing (SSL)
lorica-out-sec	4083/udp	0.000000	# Lorica outside facing (SSL)
fortisphere-vm	4084/tcp	0.000000	# Fortisphere VM Service
fortisphere-vm	4084/udp	0.000000	# Fortisphere VM Service
ezmessagesrv	4085/tcp	0.000000	# EZNews Newsroom Message Service
ftsync	4086/tcp	0.000000	# Firewall/NAT state table synchronization
ftsync	4086/udp	0.000000	# Firewall/NAT state table synchronization
applusservice	4087/tcp	0.000076	# APplus Service
npsp	4088/tcp	0.000000	# Noah Printing Service Protocol
opencore	4089/tcp	0.000000	# OpenCORE Remote Control Service
opencore	4089/udp	0.000000	# OpenCORE Remote Control Service
omasgport	4090/tcp	0.000076	# OMA BCAST Service Guide
omasgport	4090/udp	0.000000	# OMA BCAST Service Guide
ewinstaller	4091/tcp	0.000000	# EminentWare Installer
ewinstaller	4091/udp	0.000000	# EminentWare Installer
ewdgs	4092/tcp	0.000000	# EminentWare DGS
ewdgs	4092/udp	0.000000	# EminentWare DGS
pvxpluscs	4093/tcp	0.000000	# Pvx Plus CS Host
pvxpluscs	4093/udp	0.000330	# Pvx Plus CS Host
sysrqd	4094/tcp	0.000000	# sysrq daemon
sysrqd	4094/udp	0.000000	# sysrq daemon
xtgui	4095/tcp	0.000000	# xtgui information service
xtgui	4095/udp	0.000000	# xtgui information service
bre	4096/tcp	0.000152	# BRE (Bridge Relay Element)
bre	4096/udp	0.000330	# BRE (Bridge Relay Element)
patrolview	4097/tcp	0.000000	# Patrol View
patrolview	4097/udp	0.000330	# Patrol View
drmsfsd	4098/tcp	0.000000
drmsfsd	4098/udp	0.000000
dpcp	4099/tcp	0.000000
dpcp	4099/udp	0.000000
igo-incognito	4100/tcp	0.000076	# IGo Incognito Data Port
igo-incognito	4100/udp	0.000000	# IGo Incognito Data Port
brlp-0	4101/tcp	0.000076	# Braille protocol
brlp-0	4101/udp	0.000000	# Braille protocol
brlp-1	4102/tcp	0.000000	# Braille protocol
brlp-1	4102/udp	0.000000	# Braille protocol
brlp-2	4103/tcp	0.000000	# Braille protocol
brlp-2	4103/udp	0.000330	# Braille protocol
brlp-3	4104/tcp	0.000000	# Braille protocol
brlp-3	4104/udp	0.000000	# Braille protocol
shofarplayer	4105/tcp	0.000000	# shofar | Shofar
shofarplayer	4105/udp	0.000000
synchronite	4106/tcp	0.000000
synchronite	4106/udp	0.000000
j-ac	4107/tcp	0.000000	# JDL Accounting LAN Service
j-ac	4107/udp	0.000000	# JDL Accounting LAN Service
accel	4108/tcp	0.000000
accel	4108/udp	0.000000
izm	4109/tcp	0.000000	# Instantiated Zero-control Messaging
izm	4109/udp	0.000330	# Instantiated Zero-control Messaging
g2tag	4110/tcp	0.000000	# G2 RFID Tag Telemetry Data
g2tag	4110/udp	0.000000	# G2 RFID Tag Telemetry Data
xgrid	4111/tcp	0.000304
xgrid	4111/udp	0.000000
apple-vpns-rp	4112/tcp	0.000076	# Apple VPN Server Reporting Protocol
apple-vpns-rp	4112/udp	0.000330	# Apple VPN Server Reporting Protocol
aipn-reg	4113/tcp	0.000076	# AIPN LS Registration
aipn-reg	4113/udp	0.000000	# AIPN LS Registration
jomamqmonitor	4114/tcp	0.000000
jomamqmonitor	4114/udp	0.000000
cds	4115/tcp	0.000000	# CDS Transfer Agent
cds	4115/udp	0.000000	# CDS Transfer Agent
smartcard-tls	4116/tcp	0.000000
smartcard-tls	4116/udp	0.000000
hillrserv	4117/tcp	0.000000	# Hillr Connection Manager
hillrserv	4117/udp	0.000000	# Hillr Connection Manager
netscript	4118/tcp	0.000076	# Netadmin Systems NETscript service
netscript	4118/udp	0.000000	# Netadmin Systems NETscript service
assuria-slm	4119/tcp	0.000076	# Assuria Log Manager
assuria-slm	4119/udp	0.000000	# Assuria Log Manager
minirem	4120/tcp	0.000076	# MiniRem Remote Telemetry and Control
e-builder	4121/tcp	0.000076	# e-Builder Application Communication
e-builder	4121/udp	0.000000	# e-Builder Application Communication
fprams	4122/tcp	0.000000	# Fiber Patrol Alarm Service
fprams	4122/udp	0.000000	# Fiber Patrol Alarm Service
z-wave	4123/tcp	0.000000	# Zensys Z-Wave Control Protocol | Z-Wave Protocol
z-wave	4123/udp	0.000000	# Zensys Z-Wave Control Protocol
tigv2	4124/tcp	0.000000	# Rohill TetraNode Ip Gateway v2
tigv2	4124/udp	0.000000	# Rohill TetraNode Ip Gateway v2
rww	4125/tcp	0.000188	# opsview-envoy | Microsoft Remote Web Workplace on Small Business Server | Opsview Envoy
opsview-envoy	4125/udp	0.000000	# Opsview Envoy
ddrepl	4126/tcp	0.000380	# Data Domain Replication Service
ddrepl	4126/udp	0.000000	# Data Domain Replication Service
unikeypro	4127/tcp	0.000000	# NetUniKeyServer
unikeypro	4127/udp	0.000330	# NetUniKeyServer
nufw	4128/tcp	0.000000	# NuFW decision delegation protocol
nufw	4128/udp	0.000330	# NuFW decision delegation protocol
nuauth	4129/tcp	0.000380	# NuFW authentication protocol
nuauth	4129/udp	0.000000	# NuFW authentication protocol
fronet	4130/tcp	0.000000	# FRONET message protocol
fronet	4130/udp	0.000000	# FRONET message protocol
stars	4131/tcp	0.000000	# Global Maintech Stars
stars	4131/udp	0.000000	# Global Maintech Stars
nuts_dem	4132/tcp	0.000025	# nuts-dem | NUTS Daemon
nuts_dem	4132/udp	0.000692	# NUTS Daemon
nuts_bootp	4133/tcp	0.000013	# nuts-bootp | NUTS Bootp Server
nuts_bootp	4133/udp	0.000692	# NUTS Bootp Server
nifty-hmi	4134/tcp	0.000000	# NIFTY-Serve HMI protocol
nifty-hmi	4134/udp	0.000000	# NIFTY-Serve HMI protocol
cl-db-attach	4135/tcp	0.000076	# Classic Line Database Server Attach
cl-db-attach	4135/udp	0.000330	# Classic Line Database Server Attach
cl-db-request	4136/tcp	0.000000	# Classic Line Database Server Request
cl-db-request	4136/udp	0.000000	# Classic Line Database Server Request
cl-db-remote	4137/tcp	0.000000	# Classic Line Database Server Remote
cl-db-remote	4137/udp	0.000000	# Classic Line Database Server Remote
nettest	4138/tcp	0.000000
nettest	4138/udp	0.000000
thrtx	4139/tcp	0.000000	# Imperfect Networks Server
thrtx	4139/udp	0.000000	# Imperfect Networks Server
cedros_fds	4140/tcp	0.000000	# cedros-fds | Cedros Fraud Detection System
cedros_fds	4140/udp	0.000330	# Cedros Fraud Detection System
oirtgsvc	4141/tcp	0.000076	# Workflow Server
oirtgsvc	4141/udp	0.000000	# Workflow Server
oidocsvc	4142/tcp	0.000000	# Document Server
oidocsvc	4142/udp	0.000000	# Document Server
oidsr	4143/tcp	0.000152	# Document Replication
oidsr	4143/udp	0.000000	# Document Replication
wincim	4144/tcp	0.000025	# pc windows compuserve.com protocol
vvr-control	4145/tcp	0.000000	# VVR Control
vvr-control	4145/udp	0.000000	# VVR Control
tgcconnect	4146/tcp	0.000000	# TGCConnect Beacon
tgcconnect	4146/udp	0.000000	# TGCConnect Beacon
vrxpservman	4147/tcp	0.000152	# Multum Service Manager
vrxpservman	4147/udp	0.000000	# Multum Service Manager
hhb-handheld	4148/tcp	0.000000	# HHB Handheld Client
hhb-handheld	4148/udp	0.000000	# HHB Handheld Client
agslb	4149/tcp	0.000000	# A10 GSLB Service
agslb	4149/udp	0.000000	# A10 GSLB Service
PowerAlert-nsa	4150/tcp	0.000000	# PowerAlert Network Shutdown Agent
PowerAlert-nsa	4150/udp	0.000000	# PowerAlert Network Shutdown Agent
menandmice_noh	4151/tcp	0.000000	# menandmice-noh | Men & Mice Remote Control
menandmice_noh	4151/udp	0.000000	# Men & Mice Remote Control
idig_mux	4152/tcp	0.000000	# idig-mux | iDigTech Multiplex
idig_mux	4152/udp	0.000000	# iDigTech Multiplex
mbl-battd	4153/tcp	0.000000	# MBL Remote Battery Monitoring
mbl-battd	4153/udp	0.000000	# MBL Remote Battery Monitoring
atlinks	4154/tcp	0.000000	# atlinks device discovery
atlinks	4154/udp	0.000000	# atlinks device discovery
bzr	4155/tcp	0.000000	# Bazaar version control system
bzr	4155/udp	0.000000	# Bazaar version control system
stat-results	4156/tcp	0.000000	# STAT Results
stat-results	4156/udp	0.000000	# STAT Results
stat-scanner	4157/tcp	0.000000	# STAT Scanner Control
stat-scanner	4157/udp	0.000330	# STAT Scanner Control
stat-cc	4158/tcp	0.000076	# STAT Command Center
stat-cc	4158/udp	0.000330	# STAT Command Center
nss	4159/tcp	0.000000	# Network Security Service
nss	4159/udp	0.000330	# Network Security Service
jini-discovery	4160/tcp	0.000000	# Jini Discovery
jini-discovery	4160/udp	0.000330	# Jini Discovery
omscontact	4161/tcp	0.000076	# OMS Contact
omscontact	4161/udp	0.000000	# OMS Contact
omstopology	4162/tcp	0.000000	# OMS Topology
omstopology	4162/udp	0.000000	# OMS Topology
silverpeakpeer	4163/tcp	0.000000	# Silver Peak Peer Protocol
silverpeakpeer	4163/udp	0.000000	# Silver Peak Peer Protocol
silverpeakcomm	4164/tcp	0.000152	# Silver Peak Communication Protocol
silverpeakcomm	4164/udp	0.000330	# Silver Peak Communication Protocol
altcp	4165/tcp	0.000000	# ArcLink over Ethernet
altcp	4165/udp	0.000330	# ArcLink over Ethernet
joost	4166/tcp	0.000000	# Joost Peer to Peer Protocol
joost	4166/udp	0.000330	# Joost Peer to Peer Protocol
ddgn	4167/tcp	0.000000	# DeskDirect Global Network
ddgn	4167/udp	0.000000	# DeskDirect Global Network
pslicser	4168/tcp	0.000000	# PrintSoft License Server
pslicser	4168/udp	0.000000	# PrintSoft License Server
iadt	4169/tcp	0.000000	# iadt-disc | Automation Drive Interface Transport | Internet ADT Discovery Protocol
iadt-disc	4169/udp	0.000000	# Internet ADT Discovery Protocol
d-cinema-csp	4170/tcp	0.000000	# SMPTE Content Synchonization Protocol
ml-svnet	4171/tcp	0.000000	# Maxlogic Supervisor Communication
unknown	4171/udp	0.000330
pcoip	4172/tcp	0.000000	# PC over IP
pcoip	4172/udp	0.000000	# PC over IP
mma-discovery	4173/tcp	0.000000	# MMA Device Discovery
unknown	4173/udp	0.000330
smcluster	4174/tcp	0.000076	# sm-disc | StorMagic Cluster Services | StorMagic Discovery
bccp	4175/tcp	0.000000	# Brocade Cluster Communication Protocol
unknown	4175/udp	0.000661
tl-ipcproxy	4176/tcp	0.000000	# Translattice Cluster IPC Proxy
wello	4177/tcp	0.000000	# Wello P2P pubsub service
wello	4177/udp	0.000000	# Wello P2P pubsub service
storman	4178/tcp	0.000000
storman	4178/udp	0.000000
MaxumSP	4179/tcp	0.000000	# Maxum Services
MaxumSP	4179/udp	0.000330	# Maxum Services
httpx	4180/tcp	0.000000
httpx	4180/udp	0.000000
macbak	4181/tcp	0.000000
macbak	4181/udp	0.000000
pcptcpservice	4182/tcp	0.000000	# Production Company Pro TCP Service
pcptcpservice	4182/udp	0.000000	# Production Company Pro TCP Service
gmmp	4183/tcp	0.000000	# cyborgnet | General Metaverse Messaging Protocol | CyborgNet communications protocol
gmmp	4183/udp	0.000000	# General Metaverse Messaging Protocol
universe_suite	4184/tcp	0.000000	# universe-suite | UNIVERSE SUITE MESSAGE SERVICE
universe_suite	4184/udp	0.000000	# UNIVERSE SUITE MESSAGE SERVICE
wcpp	4185/tcp	0.000000	# Woven Control Plane Protocol
wcpp	4185/udp	0.000000	# Woven Control Plane Protocol
boxbackupstore	4186/tcp	0.000000	# Box Backup Store Service
csc_proxy	4187/tcp	0.000000	# csc-proxy | Cascade Proxy
vatata	4188/tcp	0.000000	# Vatata Peer to Peer Protocol
vatata	4188/udp	0.000000	# Vatata Peer to Peer Protocol
pcep	4189/tcp	0.000000	# Path Computation Element Communication Protocol
sieve	4190/tcp	0.000076	# ManageSieve Protocol
dsmipv6	4191/tcp	0.000000	# Dual Stack MIPv6 NAT Traversal
dsmipv6	4191/udp	0.000330	# Dual Stack MIPv6 NAT Traversal
azeti	4192/tcp	0.000076	# azeti-bd | Azeti Agent Service | azeti blinddate
azeti-bd	4192/udp	0.000000	# azeti blinddate
pvxplusio	4193/tcp	0.000000	# PxPlus remote file srvr
spdm	4194/tcp	0.000000	# Security Protocol and Data Model
unknown	4194/udp	0.000330
aws-wsp	4195/tcp	0.000000	# AWS protocol for cloud remoting solution
unknown	4195/udp	0.000330
hctl	4197/tcp	0.000000	# Harman HControl Protocol
unknown	4197/udp	0.000330
unknown	4198/udp	0.000661
eims-admin	4199/tcp	0.000063	# Eudora Internet Mail Service (EIMS) admin | EIMS ADMIN
eims-admin	4199/udp	0.000000	# EIMS ADMIN
vrml-multi-use	4200/tcp	0.000152	# VRML Multi User Systems
vrml-multi-use	4200/udp	0.000330	# VRML Multi User Systems
vrml-multi-use	4201/tcp	0.000000	# VRML Multi User Systems
vrml-multi-use	4201/udp	0.000000	# VRML Multi User Systems
vrml-multi-use	4202/tcp	0.000000	# VRML Multi User Systems
vrml-multi-use	4202/udp	0.000330	# VRML Multi User Systems
vrml-multi-use	4203/tcp	0.000000	# VRML Multi User Systems
vrml-multi-use	4203/udp	0.000000	# VRML Multi User Systems
vrml-multi-use	4204/tcp	0.000000	# VRML Multi User Systems
vrml-multi-use	4204/udp	0.000000	# VRML Multi User Systems
vrml-multi-use	4205/tcp	0.000000	# VRML Multi User Systems
vrml-multi-use	4205/udp	0.000000	# VRML Multi User Systems
vrml-multi-use	4206/tcp	0.000076	# VRML Multi User Systems
vrml-multi-use	4206/udp	0.000000	# VRML Multi User Systems
vrml-multi-use	4207/tcp	0.000000	# VRML Multi User Systems
vrml-multi-use	4207/udp	0.000330	# VRML Multi User Systems
vrml-multi-use	4208/tcp	0.000000	# VRML Multi User Systems
vrml-multi-use	4208/udp	0.000330	# VRML Multi User Systems
vrml-multi-use	4209/tcp	0.000000	# VRML Multi User Systems
vrml-multi-use	4209/udp	0.000000	# VRML Multi User Systems
vrml-multi-use	4210/tcp	0.000000	# VRML Multi User Systems
vrml-multi-use	4210/udp	0.000000	# VRML Multi User Systems
vrml-multi-use	4211/tcp	0.000000	# VRML Multi User Systems
vrml-multi-use	4211/udp	0.000000	# VRML Multi User Systems
vrml-multi-use	4212/tcp	0.000000	# VRML Multi User Systems
vrml-multi-use	4212/udp	0.000000	# VRML Multi User Systems
vrml-multi-use	4213/tcp	0.000000	# VRML Multi User Systems
vrml-multi-use	4213/udp	0.000000	# VRML Multi User Systems
vrml-multi-use	4214/tcp	0.000000	# VRML Multi User Systems
vrml-multi-use	4214/udp	0.000000	# VRML Multi User Systems
vrml-multi-use	4215/tcp	0.000000	# VRML Multi User Systems
vrml-multi-use	4215/udp	0.000000	# VRML Multi User Systems
vrml-multi-use	4216/tcp	0.000000	# VRML Multi User Systems
vrml-multi-use	4216/udp	0.000000	# VRML Multi User Systems
vrml-multi-use	4217/tcp	0.000000	# VRML Multi User Systems
vrml-multi-use	4217/udp	0.000000	# VRML Multi User Systems
vrml-multi-use	4218/tcp	0.000000	# VRML Multi User Systems
vrml-multi-use	4218/udp	0.000000	# VRML Multi User Systems
vrml-multi-use	4219/tcp	0.000000	# VRML Multi User Systems
vrml-multi-use	4219/udp	0.000000	# VRML Multi User Systems
vrml-multi-use	4220/tcp	0.000076	# VRML Multi User Systems
vrml-multi-use	4220/udp	0.000000	# VRML Multi User Systems
vrml-multi-use	4221/tcp	0.000000	# VRML Multi User Systems
vrml-multi-use	4221/udp	0.000000	# VRML Multi User Systems
vrml-multi-use	4222/tcp	0.000000	# VRML Multi User Systems
vrml-multi-use	4222/udp	0.000000	# VRML Multi User Systems
vrml-multi-use	4223/tcp	0.000000	# VRML Multi User Systems
vrml-multi-use	4223/udp	0.000000	# VRML Multi User Systems
xtell	4224/tcp	0.000226	# Xtell messenging server
vrml-multi-use	4224/udp	0.000330	# VRML Multi User Systems
vrml-multi-use	4225/tcp	0.000000	# VRML Multi User Systems
vrml-multi-use	4225/udp	0.000330	# VRML Multi User Systems
vrml-multi-use	4226/tcp	0.000000	# VRML Multi User Systems
vrml-multi-use	4226/udp	0.000000	# VRML Multi User Systems
vrml-multi-use	4227/tcp	0.000000	# VRML Multi User Systems
vrml-multi-use	4227/udp	0.000000	# VRML Multi User Systems
vrml-multi-use	4228/tcp	0.000000	# VRML Multi User Systems
vrml-multi-use	4228/udp	0.000000	# VRML Multi User Systems
vrml-multi-use	4229/tcp	0.000000	# VRML Multi User Systems
vrml-multi-use	4229/udp	0.000000	# VRML Multi User Systems
vrml-multi-use	4230/tcp	0.000000	# VRML Multi User Systems
vrml-multi-use	4230/udp	0.000000	# VRML Multi User Systems
vrml-multi-use	4231/tcp	0.000000	# VRML Multi User Systems
vrml-multi-use	4231/udp	0.000000	# VRML Multi User Systems
vrml-multi-use	4232/tcp	0.000000	# VRML Multi User Systems
vrml-multi-use	4232/udp	0.000661	# VRML Multi User Systems
vrml-multi-use	4233/tcp	0.000000	# VRML Multi User Systems
vrml-multi-use	4233/udp	0.000000	# VRML Multi User Systems
vrml-multi-use	4234/tcp	0.000076	# VRML Multi User Systems
vrml-multi-use	4234/udp	0.000000	# VRML Multi User Systems
vrml-multi-use	4235/tcp	0.000000	# VRML Multi User Systems
vrml-multi-use	4235/udp	0.000000	# VRML Multi User Systems
vrml-multi-use	4236/tcp	0.000000	# VRML Multi User Systems
vrml-multi-use	4236/udp	0.000000	# VRML Multi User Systems
vrml-multi-use	4237/tcp	0.000000	# VRML Multi User Systems
vrml-multi-use	4237/udp	0.000000	# VRML Multi User Systems
vrml-multi-use	4238/tcp	0.000000	# VRML Multi User Systems
vrml-multi-use	4238/udp	0.000000	# VRML Multi User Systems
vrml-multi-use	4239/tcp	0.000000	# VRML Multi User Systems
vrml-multi-use	4239/udp	0.000000	# VRML Multi User Systems
vrml-multi-use	4240/tcp	0.000000	# VRML Multi User Systems
vrml-multi-use	4240/udp	0.000000	# VRML Multi User Systems
vrml-multi-use	4241/tcp	0.000000	# VRML Multi User Systems
vrml-multi-use	4241/udp	0.000000	# VRML Multi User Systems
vrml-multi-use	4242/tcp	0.000456	# VRML Multi User Systems or CrashPlan http://support.code42.com/CrashPlan/Latest/Configuring/Network#Networking_FAQs
vrml-multi-use	4242/udp	0.000000	# VRML Multi User Systems
vrml-multi-use	4243/tcp	0.000076	# VRML Multi User Systems or CrashPlan http://support.code42.com/CrashPlan/Latest/Configuring/Network#Networking_FAQs
vrml-multi-use	4243/udp	0.000000	# VRML Multi User Systems
vrml-multi-use	4244/tcp	0.000000	# VRML Multi User Systems
vrml-multi-use	4244/udp	0.000000	# VRML Multi User Systems
vrml-multi-use	4245/tcp	0.000000	# VRML Multi User Systems
vrml-multi-use	4245/udp	0.000000	# VRML Multi User Systems
vrml-multi-use	4246/tcp	0.000000	# VRML Multi User Systems
vrml-multi-use	4246/udp	0.000000	# VRML Multi User Systems
vrml-multi-use	4247/tcp	0.000000	# VRML Multi User Systems
vrml-multi-use	4247/udp	0.000330	# VRML Multi User Systems
vrml-multi-use	4248/tcp	0.000000	# VRML Multi User Systems
vrml-multi-use	4248/udp	0.000000	# VRML Multi User Systems
vrml-multi-use	4249/tcp	0.000000	# VRML Multi User Systems
vrml-multi-use	4249/udp	0.000000	# VRML Multi User Systems
vrml-multi-use	4250/tcp	0.000000	# VRML Multi User Systems
vrml-multi-use	4250/udp	0.000000	# VRML Multi User Systems
vrml-multi-use	4251/tcp	0.000000	# VRML Multi User Systems
vrml-multi-use	4251/udp	0.000000	# VRML Multi User Systems
vrml-multi-use	4252/tcp	0.000152	# VRML Multi User Systems
vrml-multi-use	4252/udp	0.000000	# VRML Multi User Systems
vrml-multi-use	4253/tcp	0.000000	# VRML Multi User Systems
vrml-multi-use	4253/udp	0.000000	# VRML Multi User Systems
vrml-multi-use	4254/tcp	0.000000	# VRML Multi User Systems
vrml-multi-use	4254/udp	0.000000	# VRML Multi User Systems
vrml-multi-use	4255/tcp	0.000000	# VRML Multi User Systems
vrml-multi-use	4255/udp	0.000000	# VRML Multi User Systems
vrml-multi-use	4256/tcp	0.000000	# VRML Multi User Systems
vrml-multi-use	4256/udp	0.000000	# VRML Multi User Systems
vrml-multi-use	4257/tcp	0.000000	# VRML Multi User Systems
vrml-multi-use	4257/udp	0.000000	# VRML Multi User Systems
vrml-multi-use	4258/tcp	0.000000	# VRML Multi User Systems
vrml-multi-use	4258/udp	0.000000	# VRML Multi User Systems
vrml-multi-use	4259/tcp	0.000000	# VRML Multi User Systems
vrml-multi-use	4259/udp	0.000000	# VRML Multi User Systems
vrml-multi-use	4260/tcp	0.000000	# VRML Multi User Systems
vrml-multi-use	4260/udp	0.000330	# VRML Multi User Systems
vrml-multi-use	4261/tcp	0.000000	# VRML Multi User Systems
vrml-multi-use	4261/udp	0.000000	# VRML Multi User Systems
vrml-multi-use	4262/tcp	0.000076	# VRML Multi User Systems
vrml-multi-use	4262/udp	0.000661	# VRML Multi User Systems
vrml-multi-use	4263/tcp	0.000000	# VRML Multi User Systems
vrml-multi-use	4263/udp	0.000000	# VRML Multi User Systems
vrml-multi-use	4264/tcp	0.000000	# VRML Multi User Systems
vrml-multi-use	4264/udp	0.000000	# VRML Multi User Systems
vrml-multi-use	4265/tcp	0.000000	# VRML Multi User Systems
vrml-multi-use	4265/udp	0.000000	# VRML Multi User Systems
vrml-multi-use	4266/tcp	0.000000	# VRML Multi User Systems
vrml-multi-use	4266/udp	0.000000	# VRML Multi User Systems
vrml-multi-use	4267/tcp	0.000000	# VRML Multi User Systems
vrml-multi-use	4267/udp	0.000000	# VRML Multi User Systems
vrml-multi-use	4268/tcp	0.000000	# VRML Multi User Systems
vrml-multi-use	4268/udp	0.000000	# VRML Multi User Systems
vrml-multi-use	4269/tcp	0.000000	# VRML Multi User Systems
vrml-multi-use	4269/udp	0.000000	# VRML Multi User Systems
vrml-multi-use	4270/tcp	0.000000	# VRML Multi User Systems
vrml-multi-use	4270/udp	0.000000	# VRML Multi User Systems
vrml-multi-use	4271/tcp	0.000000	# VRML Multi User Systems
vrml-multi-use	4271/udp	0.000000	# VRML Multi User Systems
vrml-multi-use	4272/tcp	0.000000	# VRML Multi User Systems
vrml-multi-use	4272/udp	0.000000	# VRML Multi User Systems
vrml-multi-use	4273/tcp	0.000000	# VRML Multi User Systems
vrml-multi-use	4273/udp	0.000000	# VRML Multi User Systems
vrml-multi-use	4274/tcp	0.000000	# VRML Multi User Systems
vrml-multi-use	4274/udp	0.000330	# VRML Multi User Systems
vrml-multi-use	4275/tcp	0.000000	# VRML Multi User Systems
vrml-multi-use	4275/udp	0.000000	# VRML Multi User Systems
vrml-multi-use	4276/tcp	0.000000	# VRML Multi User Systems
vrml-multi-use	4276/udp	0.000000	# VRML Multi User Systems
vrml-multi-use	4277/tcp	0.000000	# VRML Multi User Systems
vrml-multi-use	4277/udp	0.000000	# VRML Multi User Systems
vrml-multi-use	4278/tcp	0.000000	# VRML Multi User Systems
vrml-multi-use	4278/udp	0.000000	# VRML Multi User Systems
vrml-multi-use	4279/tcp	0.000228	# VRML Multi User Systems
vrml-multi-use	4279/udp	0.000330	# VRML Multi User Systems
vrml-multi-use	4280/tcp	0.000000	# VRML Multi User Systems
vrml-multi-use	4280/udp	0.000000	# VRML Multi User Systems
vrml-multi-use	4281/tcp	0.000000	# VRML Multi User Systems
vrml-multi-use	4281/udp	0.000000	# VRML Multi User Systems
vrml-multi-use	4282/tcp	0.000000	# VRML Multi User Systems
vrml-multi-use	4282/udp	0.000330	# VRML Multi User Systems
vrml-multi-use	4283/tcp	0.000000	# VRML Multi User Systems
vrml-multi-use	4283/udp	0.000000	# VRML Multi User Systems
vrml-multi-use	4284/tcp	0.000000	# VRML Multi User Systems
vrml-multi-use	4284/udp	0.000000	# VRML Multi User Systems
vrml-multi-use	4285/tcp	0.000000	# VRML Multi User Systems
vrml-multi-use	4285/udp	0.000330	# VRML Multi User Systems
vrml-multi-use	4286/tcp	0.000000	# VRML Multi User Systems
vrml-multi-use	4286/udp	0.000000	# VRML Multi User Systems
vrml-multi-use	4287/tcp	0.000000	# VRML Multi User Systems
vrml-multi-use	4287/udp	0.000000	# VRML Multi User Systems
vrml-multi-use	4288/tcp	0.000000	# VRML Multi User Systems
vrml-multi-use	4288/udp	0.000000	# VRML Multi User Systems
vrml-multi-use	4289/tcp	0.000000	# VRML Multi User Systems
vrml-multi-use	4289/udp	0.000000	# VRML Multi User Systems
vrml-multi-use	4290/tcp	0.000000	# VRML Multi User Systems
vrml-multi-use	4290/udp	0.000000	# VRML Multi User Systems
vrml-multi-use	4291/tcp	0.000000	# VRML Multi User Systems
vrml-multi-use	4291/udp	0.000000	# VRML Multi User Systems
vrml-multi-use	4292/tcp	0.000000	# VRML Multi User Systems
vrml-multi-use	4292/udp	0.000000	# VRML Multi User Systems
vrml-multi-use	4293/tcp	0.000000	# VRML Multi User Systems
vrml-multi-use	4293/udp	0.000330	# VRML Multi User Systems
vrml-multi-use	4294/tcp	0.000076	# VRML Multi User Systems
vrml-multi-use	4294/udp	0.000000	# VRML Multi User Systems
vrml-multi-use	4295/tcp	0.000000	# VRML Multi User Systems
vrml-multi-use	4295/udp	0.000000	# VRML Multi User Systems
vrml-multi-use	4296/tcp	0.000000	# VRML Multi User Systems
vrml-multi-use	4296/udp	0.000000	# VRML Multi User Systems
vrml-multi-use	4297/tcp	0.000076	# VRML Multi User Systems
vrml-multi-use	4297/udp	0.000000	# VRML Multi User Systems
vrml-multi-use	4298/tcp	0.000076	# VRML Multi User Systems
vrml-multi-use	4298/udp	0.000000	# VRML Multi User Systems
vrml-multi-use	4299/tcp	0.000000	# VRML Multi User Systems
vrml-multi-use	4299/udp	0.000330	# VRML Multi User Systems
corelccam	4300/tcp	0.000076	# Corel CCam
corelccam	4300/udp	0.000000	# Corel CCam
d-data	4301/tcp	0.000000	# Diagnostic Data
d-data	4301/udp	0.000330	# Diagnostic Data
d-data-control	4302/tcp	0.000076	# Diagnostic Data Control
d-data-control	4302/udp	0.000000	# Diagnostic Data Control
srcp	4303/tcp	0.000000	# Simple Railroad Command Protocol
srcp	4303/udp	0.000000	# Simple Railroad Command Protocol
owserver	4304/tcp	0.000000	# One-Wire Filesystem Server
owserver	4304/udp	0.000000	# One-Wire Filesystem Server
batman	4305/tcp	0.000000	# better approach to mobile ad-hoc networking
batman	4305/udp	0.000000	# better approach to mobile ad-hoc networking
pinghgl	4306/tcp	0.000000	# Hellgate London
pinghgl	4306/udp	0.000000	# Hellgate London
visicron-vs	4307/tcp	0.000000	# trueconf | Visicron Videoconference Service | TrueConf Videoconference Service
visicron-vs	4307/udp	0.000000	# Visicron Videoconference Service
compx-lockview	4308/tcp	0.000000
compx-lockview	4308/udp	0.000330
dserver	4309/tcp	0.000000	# Exsequi Appliance Discovery
dserver	4309/udp	0.000000	# Exsequi Appliance Discovery
mirrtex	4310/tcp	0.000000	# Mir-RT exchange service
mirrtex	4310/udp	0.000000	# Mir-RT exchange service
p6ssmc	4311/tcp	0.000000	# P6R Secure Server Management Console
pscl-mgt	4312/tcp	0.000000	# Parascale Membership Manager
perrla	4313/tcp	0.000000	# PERRLA User Services
choiceview-agt	4314/tcp	0.000000	# ChoiceView Agent
choiceview-clt	4316/tcp	0.000000	# ChoiceView Client
opentelemetry	4317/tcp	0.000000	# OpenTelemetry Protocol
unknown	4318/udp	0.000330
fox-skytale	4319/tcp	0.000000	# Fox SkyTale encrypted communication
fdt-rcatp	4320/tcp	0.000000	# FDT Remote Categorization Protocol
fdt-rcatp	4320/udp	0.000000	# FDT Remote Categorization Protocol
rwhois	4321/tcp	0.000276	# Remote Who Is
rwhois	4321/udp	0.001021	# Remote Who Is
trim-event	4322/tcp	0.000000	# TRIM Event Service
trim-event	4322/udp	0.000000	# TRIM Event Service
trim-ice	4323/tcp	0.000000	# TRIM ICE Service
trim-ice	4323/udp	0.000000	# TRIM ICE Service
balour	4324/tcp	0.000000	# Balour Game Server
balour	4324/udp	0.000000	# Balour Game Server
geognosisman	4325/tcp	0.000076	# geognosisadmin | Cadcorp GeognoSIS Manager Service | Cadcorp GeognoSIS Administrator
geognosisman	4325/udp	0.000000	# Cadcorp GeognoSIS Manager Service
geognosis	4326/tcp	0.000000	# Cadcorp GeognoSIS Service | Cadcorp GeognoSIS
geognosis	4326/udp	0.000000	# Cadcorp GeognoSIS Service
jaxer-web	4327/tcp	0.000000	# Jaxer Web Protocol
jaxer-web	4327/udp	0.000000	# Jaxer Web Protocol
jaxer-manager	4328/tcp	0.000076	# Jaxer Manager Command Protocol
jaxer-manager	4328/udp	0.000330	# Jaxer Manager Command Protocol
publiqare-sync	4329/tcp	0.000000	# PubliQare Distributed Environment Synchronisation Engine
unknown	4329/udp	0.000330
dey-sapi	4330/tcp	0.000000	# DEY Storage Administration REST API
ktickets-rest	4331/tcp	0.000000	# ktickets REST API for event management and ticketing systems (embedded POS devices)
unknown	4331/udp	0.000330
getty-focus	4332/tcp	0.000000	# Getty Images FOCUS service
msql	4333/tcp	0.000113	# ahsp | mini-sql server | ArrowHead Service Protocol (AHSP)
netconf-ch-ssh	4334/tcp	0.000000	# NETCONF Call Home (SSH)
netconf-ch-tls	4335/tcp	0.000000	# NETCONF Call Home (TLS)
restconf-ch-tls	4336/tcp	0.000000	# RESTCONF Call Home (TLS)
unknown	4336/udp	0.000330
unknown	4337/udp	0.000330
gaia	4340/tcp	0.000000	# Gaia Connector Protocol
gaia	4340/udp	0.000000	# Gaia Connector Protocol
lisp-data	4341/tcp	0.000000	# LISP Data Packets
lisp-data	4341/udp	0.000330	# LISP Data Packets
lisp-cons	4342/tcp	0.000076	# lisp-control | LISP-CONS Control | LISP Control Packets
lisp-control	4342/udp	0.000000	# LISP Data-Triggered Control
unicall	4343/tcp	0.000201
unicall	4343/udp	0.000511
vinainstall	4344/tcp	0.000000
vinainstall	4344/udp	0.000330
m4-network-as	4345/tcp	0.000000	# Macro 4 Network AS
m4-network-as	4345/udp	0.000000	# Macro 4 Network AS
elanlm	4346/tcp	0.000000	# ELAN LM
elanlm	4346/udp	0.000000	# ELAN LM
lansurveyor	4347/tcp	0.000000	# LAN Surveyor
lansurveyor	4347/udp	0.000000	# LAN Surveyor
itose	4348/tcp	0.000000
itose	4348/udp	0.000000
fsportmap	4349/tcp	0.000000	# File System Port Map
fsportmap	4349/udp	0.000000	# File System Port Map
net-device	4350/tcp	0.000000	# Net Device
net-device	4350/udp	0.000000	# Net Device
plcy-net-svcs	4351/tcp	0.000000	# PLCY Net Services
plcy-net-svcs	4351/udp	0.000000	# PLCY Net Services
pjlink	4352/tcp	0.000000	# Projector Link
pjlink	4352/udp	0.000000	# Projector Link
f5-iquery	4353/tcp	0.000000	# F5 iQuery
f5-iquery	4353/udp	0.000000	# F5 iQuery
qsnet-trans	4354/tcp	0.000000	# QSNet Transmitter
qsnet-trans	4354/udp	0.000330	# QSNet Transmitter
qsnet-workst	4355/tcp	0.000076	# QSNet Workstation
qsnet-workst	4355/udp	0.000330	# QSNet Workstation
qsnet-assist	4356/tcp	0.000076	# QSNet Assistant
qsnet-assist	4356/udp	0.000000	# QSNet Assistant
qsnet-cond	4357/tcp	0.000076	# QSNet Conductor
qsnet-cond	4357/udp	0.000330	# QSNet Conductor
qsnet-nucl	4358/tcp	0.000076	# QSNet Nucleus
qsnet-nucl	4358/udp	0.000330	# QSNet Nucleus
omabcastltkm	4359/tcp	0.000000	# OMA BCAST Long-Term Key Messages
omabcastltkm	4359/udp	0.000330	# OMA BCAST Long-Term Key Messages
matrix_vnet	4360/tcp	0.000000	# matrix-vnet | Matrix VNet Communication Protocol
nacnl	4361/tcp	0.000000	# NavCom Discovery and Control Port
nacnl	4361/udp	0.000661	# NavCom Discovery and Control Port
afore-vdp-disc	4362/tcp	0.000000	# AFORE vNode Discovery protocol
unknown	4362/udp	0.000661
shadowstream	4366/tcp	0.000000	# ShadowStream System
wxbrief	4368/tcp	0.000000	# WeatherBrief Direct
wxbrief	4368/udp	0.000000	# WeatherBrief Direct
epmd	4369/tcp	0.000076	# Erlang Port Mapper Daemon
epmd	4369/udp	0.000330	# Erlang Port Mapper Daemon
elpro_tunnel	4370/tcp	0.000000	# elpro-tunnel | ELPRO V2 Protocol Tunnel
elpro_tunnel	4370/udp	0.000330	# ELPRO V2 Protocol Tunnel
l2c-control	4371/tcp	0.000000	# l2c-disc | LAN2CAN Control | LAN2CAN Discovery
l2c-disc	4371/udp	0.000000	# LAN2CAN Discovery
l2c-data	4372/tcp	0.000000	# LAN2CAN Data
l2c-data	4372/udp	0.000000	# LAN2CAN Data
remctl	4373/tcp	0.000000	# Remote Authenticated Command Service
remctl	4373/udp	0.000000	# Remote Authenticated Command Service
psi-ptt	4374/tcp	0.000076	# PSI Push-to-Talk Protocol
tolteces	4375/tcp	0.000076	# Toltec EasyShare
tolteces	4375/udp	0.000000	# Toltec EasyShare
bip	4376/tcp	0.000076	# BioAPI Interworking
bip	4376/udp	0.000000	# BioAPI Interworking
cp-spxsvr	4377/tcp	0.000000	# Cambridge Pixel SPx Server
cp-spxsvr	4377/udp	0.000000	# Cambridge Pixel SPx Server
cp-spxdpy	4378/tcp	0.000000	# Cambridge Pixel SPx Display
cp-spxdpy	4378/udp	0.000661	# Cambridge Pixel SPx Display
ctdb	4379/tcp	0.000000
ctdb	4379/udp	0.000000
unknown	4380/udp	0.000330
unknown	4384/tcp	0.000076
unknown	4386/udp	0.000330
unknown	4387/udp	0.000330
unknown	4388/tcp	0.000076
xandros-cms	4389/tcp	0.000000	# Xandros Community Management Service
xandros-cms	4389/udp	0.000000	# Xandros Community Management Service
wiegand	4390/tcp	0.000000	# Physical Access Control
wiegand	4390/udp	0.000000	# Physical Access Control
apwi-imserver	4391/tcp	0.000000	# American Printware IMServer Protocol
unknown	4391/udp	0.000330
apwi-rxserver	4392/tcp	0.000000	# American Printware RXServer Protocol
apwi-rxspooler	4393/tcp	0.000000	# American Printware RXSpooler Protocol
apwi-disc	4394/tcp	0.000000	# American Printware Discovery
apwi-disc	4394/udp	0.000330	# American Printware Discovery
omnivisionesx	4395/tcp	0.000000	# OmniVision communication for Virtual environments
omnivisionesx	4395/udp	0.000000	# OmniVision communication for Virtual environments
fly	4396/tcp	0.000000	# Fly Object Space
ds-srv	4400/tcp	0.000000	# ASIGRA Services
ds-srv	4400/udp	0.000000	# ASIGRA Services
ds-srvr	4401/tcp	0.000076	# ASIGRA Televaulting DS-System Service
ds-srvr	4401/udp	0.000661	# ASIGRA Televaulting DS-System Service
ds-clnt	4402/tcp	0.000000	# ASIGRA Televaulting DS-Client Service
ds-clnt	4402/udp	0.000000	# ASIGRA Televaulting DS-Client Service
ds-user	4403/tcp	0.000000	# ASIGRA Televaulting DS-Client Monitoring/Management
ds-user	4403/udp	0.000000	# ASIGRA Televaulting DS-Client Monitoring/Management
ds-admin	4404/tcp	0.000000	# ASIGRA Televaulting DS-System Monitoring/Management
ds-admin	4404/udp	0.000661	# ASIGRA Televaulting DS-System Monitoring/Management
ds-mail	4405/tcp	0.000000	# ASIGRA Televaulting Message Level Restore service
ds-mail	4405/udp	0.000000	# ASIGRA Televaulting Message Level Restore service
ds-slp	4406/tcp	0.000000	# ASIGRA Televaulting DS-Sleeper Service
ds-slp	4406/udp	0.000000	# ASIGRA Televaulting DS-Sleeper Service
nacagent	4407/tcp	0.000076	# Network Access Control Agent
slscc	4408/tcp	0.000000	# SLS Technology Control Centre
unknown	4408/udp	0.000661
netcabinet-com	4409/tcp	0.000000	# Net-Cabinet comunication
itwo-server	4410/tcp	0.000000	# RIB iTWO Application Server
found	4411/tcp	0.000000	# Found Messaging Protocol
unknown	4411/udp	0.000330
smallchat	4412/tcp	0.000000
avi-nms	4413/tcp	0.000000	# avi-nms-disc | AVI Systems NMS
unknown	4413/udp	0.000330
updog	4414/tcp	0.000076	# Updog Monitoring and Status Framework
brcd-vr-req	4415/tcp	0.000076	# Brocade Virtual Router Request
pjj-player	4416/tcp	0.000000	# pjj-player-disc | PJJ Media Player | PJJ Media Player discovery
workflowdir	4417/tcp	0.000000	# Workflow Director Communication
axysbridge	4418/tcp	0.000076	# AXYS communication protocol
cbp	4419/tcp	0.000000	# Colnod Binary Protocol
nvm-express	4420/tcp	0.000000	# nvme | NVM Express over Fabrics storage access
scaleft	4421/tcp	0.000000	# Multi-Platform Remote Management for Cloud Infrastructure
tsepisp	4422/tcp	0.000000	# TSEP Installation Service Protocol
thingkit	4423/tcp	0.000000	# thingkit secure mesh
unknown	4423/udp	0.000330
netrockey6	4425/tcp	0.000000	# NetROCKEY6 SMART Plus Service
netrockey6	4425/udp	0.000000	# NetROCKEY6 SMART Plus Service
beacon-port-2	4426/tcp	0.000000	# SMARTS Beacon Port
beacon-port-2	4426/udp	0.000000	# SMARTS Beacon Port
drizzle	4427/tcp	0.000000	# Drizzle database server
omviserver	4428/tcp	0.000000	# OMV-Investigation Server-Client
unknown	4428/udp	0.000330
omviagent	4429/tcp	0.000000	# OMV Investigation Agent-Server
rsqlserver	4430/tcp	0.000152	# REAL SQL Server
rsqlserver	4430/udp	0.000330	# REAL SQL Server
wspipe	4431/tcp	0.000000	# adWISE Pipe
l-acoustics	4432/tcp	0.000000	# L-ACOUSTICS management
vop	4433/tcp	0.000076	# Versile Object Protocol
unknown	4435/udp	0.000330
unknown	4440/udp	0.000330
netblox	4441/tcp	0.000000	# Netblox Protocol
netblox	4441/udp	0.000000	# Netblox Protocol
saris	4442/tcp	0.000076
saris	4442/udp	0.000000
pharos	4443/tcp	0.000760
pharos	4443/udp	0.000000
krb524	4444/tcp	0.001041	# nv-video | Kerberos 5 to 4 ticket xlator | NV Video default
krb524	4444/udp	0.016343
upnotifyp	4445/tcp	0.000228
upnotifyp	4445/udp	0.000000
n1-fwp	4446/tcp	0.000304
n1-fwp	4446/udp	0.000000
n1-rmgmt	4447/tcp	0.000076
n1-rmgmt	4447/udp	0.000661
asc-slmd	4448/tcp	0.000000	# ASC Licence Manager
asc-slmd	4448/udp	0.000000	# ASC Licence Manager
privatewire	4449/tcp	0.000380
privatewire	4449/udp	0.000000
camp	4450/tcp	0.000000	# Common ASCII Messaging Protocol
camp	4450/udp	0.000000
ctisystemmsg	4451/tcp	0.000000	# CTI System Msg
ctisystemmsg	4451/udp	0.000000	# CTI System Msg
ctiprogramload	4452/tcp	0.000000	# CTI Program Load
ctiprogramload	4452/udp	0.000000	# CTI Program Load
nssalertmgr	4453/tcp	0.000000	# NSS Alert Manager
nssalertmgr	4453/udp	0.000000	# NSS Alert Manager
nssagentmgr	4454/tcp	0.000076	# NSS Agent Manager
nssagentmgr	4454/udp	0.000000	# NSS Agent Manager
prchat-user	4455/tcp	0.000000	# PR Chat User
prchat-user	4455/udp	0.000000	# PR Chat User
prchat-server	4456/tcp	0.000000	# PR Chat Server
prchat-server	4456/udp	0.000000	# PR Chat Server
prRegister	4457/tcp	0.000000	# PR Register
prRegister	4457/udp	0.000000	# PR Register
mcp	4458/tcp	0.000000	# Matrix Configuration Protocol
mcp	4458/udp	0.000000	# Matrix Configuration Protocol
unknown	4459/udp	0.000330
ntske	4460/tcp	0.000000	# Network Time Security Key Establishment
unknown	4462/udp	0.000330
unknown	4464/tcp	0.000076
unknown	4468/udp	0.000330
unknown	4471/tcp	0.000076
unknown	4476/tcp	0.000076
proxy-plus	4480/tcp	0.000038	# Proxy+ HTTP proxy port
unknown	4483/udp	0.000330
hpssmgmt	4484/tcp	0.000000	# hpssmgmt service
hpssmgmt	4484/udp	0.000000	# hpssmgmt service
assyst-dr	4485/tcp	0.000000	# Assyst Data Repository Service
icms	4486/tcp	0.000000	# Integrated Client Message Service
icms	4486/udp	0.000000	# Integrated Client Message Service
prex-tcp	4487/tcp	0.000000	# Protocol for Remote Execution over TCP
awacs-ice	4488/tcp	0.000000	# Apple Wide Area Connectivity Service ICE Bootstrap
awacs-ice	4488/udp	0.000000	# Apple Wide Area Connectivity Service ICE Bootstrap
unknown	4491/udp	0.000330
unknown	4497/udp	0.000330
unknown	4499/udp	0.000330
sae-urn	4500/tcp	0.000038	# ipsec-nat-t | IPsec NAT-Traversal
nat-t-ike	4500/udp	0.124467	# IKE Nat Traversal negotiation (RFC3947)
unknown	4501/udp	0.000330
a25-fap-fgw	4502/tcp	0.000000	# A25 (FAP-FGW)
unknown	4506/udp	0.000330
unknown	4507/udp	0.000330
unknown	4508/udp	0.000330
unknown	4512/udp	0.000330
unknown	4516/tcp	0.000076
unknown	4517/tcp	0.000076
unknown	4523/udp	0.000330
unknown	4524/udp	0.000330
unknown	4530/tcp	0.000076
unknown	4533/udp	0.000330
armagetronad	4534/tcp	0.000076	# Armagetron Advanced Game Server
ehs	4535/tcp	0.000000	# Event Heap Server
ehs	4535/udp	0.000000	# Event Heap Server
ehs-ssl	4536/tcp	0.000000	# Event Heap Server SSL
ehs-ssl	4536/udp	0.000661	# Event Heap Server SSL
wssauthsvc	4537/tcp	0.000000	# WSS Security Service
wssauthsvc	4537/udp	0.000330	# WSS Security Service
swx-gate	4538/tcp	0.000000	# Software Data Exchange Gateway
swx-gate	4538/udp	0.000000	# Software Data Exchange Gateway
unknown	4540/udp	0.000330
unknown	4541/udp	0.000330
worldscores	4545/tcp	0.000076
worldscores	4545/udp	0.000000
sf-lm	4546/tcp	0.000000	# SF License Manager (Sentinel)
sf-lm	4546/udp	0.000000	# SF License Manager (Sentinel)
lanner-lm	4547/tcp	0.000000	# Lanner License Manager
lanner-lm	4547/udp	0.000000	# Lanner License Manager
synchromesh	4548/tcp	0.000000
synchromesh	4548/udp	0.000000
aegate	4549/tcp	0.000000	# Aegate PMR Service
aegate	4549/udp	0.000330	# Aegate PMR Service
gds-adppiw-db	4550/tcp	0.000228	# Perman I Interbase Server
gds-adppiw-db	4550/udp	0.000000	# Perman I Interbase Server
ieee-mih	4551/tcp	0.000000	# MIH Services
ieee-mih	4551/udp	0.000330	# MIH Services
menandmice-mon	4552/tcp	0.000000	# Men and Mice Monitoring
menandmice-mon	4552/udp	0.000330	# Men and Mice Monitoring
icshostsvc	4553/tcp	0.000000	# ICS host services
unknown	4553/udp	0.000330
msfrs	4554/tcp	0.000000	# MS FRS Replication
msfrs	4554/udp	0.000330	# MS FRS Replication
rsip	4555/tcp	0.000152	# RSIP Port
rsip	4555/udp	0.000000	# RSIP Port
dtn-bundle-tcp	4556/tcp	0.000000	# dtn-bundle | DTN Bundle TCP CL Protocol | DTN Bundle UDP CL Protocol | DTN Bundle DCCP CL Protocol
dtn-bundle-udp	4556/udp	0.000000	# DTN Bundle UDP CL Protocol
fax	4557/tcp	0.000050	# mtcevrunqss | FlexFax FAX transmission service | Marathon everRun Quorum Service Server
mtcevrunqss	4557/udp	0.000000	# Marathon everRun Quorum Service Server
mtcevrunqman	4558/tcp	0.000076	# Marathon everRun Quorum Service Manager
mtcevrunqman	4558/udp	0.000000	# Marathon everRun Quorum Service Manager
hylafax	4559/tcp	0.000151	# HylaFAX client-server protocol
hylafax	4559/udp	0.000000
unknown	4560/udp	0.000330
unknown	4562/udp	0.000330
amahi-anywhere	4563/tcp	0.000000	# Amahi Anywhere
unknown	4563/udp	0.000330
unknown	4565/udp	0.000661
kwtc	4566/tcp	0.000000	# Kids Watch Time Control Service
kwtc	4566/udp	0.000000	# Kids Watch Time Control Service
tram	4567/tcp	0.000228
tram	4567/udp	0.000000
bmc-reporting	4568/tcp	0.000000	# BMC Reporting
bmc-reporting	4568/udp	0.000000	# BMC Reporting
iax	4569/tcp	0.000000	# Inter-Asterisk eXchange
iax	4569/udp	0.000000	# Inter-Asterisk eXchange
deploymentmap	4570/tcp	0.000076	# Service to distribute and update within a site deployment information for Oracle Communications Suite
unknown	4571/udp	0.000330
cardifftec-back	4573/tcp	0.000000	# A port for communication between a server and client for a custom backup system
unknown	4579/udp	0.000330
unknown	4585/udp	0.000330
unknown	4586/udp	0.000330
unknown	4587/udp	0.000330
unknown	4588/udp	0.000330
rid	4590/tcp	0.000000	# RID over HTTP/TLS
l3t-at-an	4591/tcp	0.000000	# HRPD L3T (AT-AN)
l3t-at-an	4591/udp	0.000000	# HRPD L3T (AT-AN)
hrpd-ith-at-an	4592/tcp	0.000000	# HRPD-ITH (AT-AN)
hrpd-ith-at-an	4592/udp	0.000000	# HRPD-ITH (AT-AN)
ipt-anri-anri	4593/tcp	0.000000	# IPT (ANRI-ANRI)
ipt-anri-anri	4593/udp	0.000661	# IPT (ANRI-ANRI)
ias-session	4594/tcp	0.000000	# IAS-Session (ANRI-ANRI)
ias-session	4594/udp	0.000000	# IAS-Session (ANRI-ANRI)
ias-paging	4595/tcp	0.000000	# IAS-Paging (ANRI-ANRI)
ias-paging	4595/udp	0.000000	# IAS-Paging (ANRI-ANRI)
ias-neighbor	4596/tcp	0.000000	# IAS-Neighbor (ANRI-ANRI)
ias-neighbor	4596/udp	0.000330	# IAS-Neighbor (ANRI-ANRI)
a21-an-1xbs	4597/tcp	0.000000	# A21 (AN-1xBS)
a21-an-1xbs	4597/udp	0.000000	# A21 (AN-1xBS)
a16-an-an	4598/tcp	0.000000	# A16 (AN-AN)
a16-an-an	4598/udp	0.000000	# A16 (AN-AN)
a17-an-an	4599/tcp	0.000076	# A17 (AN-AN)
a17-an-an	4599/udp	0.000000	# A17 (AN-AN)
piranha1	4600/tcp	0.000152
piranha1	4600/udp	0.000000
piranha2	4601/tcp	0.000076
piranha2	4601/udp	0.000000
mtsserver	4602/tcp	0.000076	# EAX MTS Server
menandmice-upg	4603/tcp	0.000000	# Men & Mice Upgrade Agent
irp	4604/tcp	0.000000	# Identity Registration Protocol
sixchat	4605/tcp	0.000000	# Direct End to End Secure Chat Protocol
sixid	4606/tcp	0.000076	# Secure ID to IP registration and lookup
unknown	4609/tcp	0.000076
unknown	4610/udp	0.000330
unknown	4611/udp	0.000330
ventoso	4621/tcp	0.000000	# Bidirectional single port remote radio VOIP and Control stream
unknown	4622/udp	0.000330
unknown	4629/udp	0.000330
unknown	4634/udp	0.000330
unknown	4644/tcp	0.000076
dots-signal	4646/tcp	0.000000	# Distributed Denial-of-Service Open Threat Signaling (DOTS) Signal Channel | Distributed Denial-of-Service Open Threat Signaling (DOTS) Signal Channel Protocol. The service name is used to construct the SRV service names "_dots-signal._udp" and "_dots-signal._tcp" for discovering DOTS servers used to establish DOTS signal channel.
unknown	4646/udp	0.000330
unknown	4649/tcp	0.000076
playsta2-app	4658/tcp	0.000152	# PlayStation2 App Port
playsta2-app	4658/udp	0.000000	# PlayStation2 App Port
playsta2-lob	4659/tcp	0.000000	# PlayStation2 Lobby Port
playsta2-lob	4659/udp	0.000330	# PlayStation2 Lobby Port
mosmig	4660/tcp	0.000050	# OpenMOSix MIGrates local processes | smaclmgr
smaclmgr	4660/udp	0.000000
kar2ouche	4661/tcp	0.000000	# Kar2ouche Peer location service
kar2ouche	4661/udp	0.000000	# Kar2ouche Peer location service
edonkey	4662/tcp	0.000828	# oms | eDonkey file sharing (Donkey) | OrbitNet Message Service
oms	4662/udp	0.000000	# OrbitNet Message Service
noteit	4663/tcp	0.000000	# Note It! Message Service
noteit	4663/udp	0.000330	# Note It! Message Service
ems	4664/tcp	0.000000	# Rimage Messaging Server
ems	4664/udp	0.000000	# Rimage Messaging Server
contclientms	4665/tcp	0.000076	# Container Client Message Service
contclientms	4665/udp	0.000000	# Container Client Message Service
eportcomm	4666/tcp	0.000000	# E-Port Message Service
edonkey	4666/udp	0.001450	# eDonkey file sharing (Donkey)
mmacomm	4667/tcp	0.000000	# MMA Comm Services
mmacomm	4667/udp	0.000000	# MMA Comm Services
mmaeds	4668/tcp	0.000000	# MMA EDS Service
mmaeds	4668/udp	0.000000	# MMA EDS Service
eportcommdata	4669/tcp	0.000000	# E-Port Data Service
eportcommdata	4669/udp	0.000000	# E-Port Data Service
light	4670/tcp	0.000000	# Light packets transfer protocol
light	4670/udp	0.000000	# Light packets transfer protocol
acter	4671/tcp	0.000000	# Bull RSF action server
acter	4671/udp	0.000000	# Bull RSF action server
rfa	4672/tcp	0.000013	# remote file access server
rfa	4672/udp	0.006227	# remote file access server
cxws	4673/tcp	0.000000	# CXWS Operations
cxws	4673/udp	0.000330	# CXWS Operations
appiq-mgmt	4674/tcp	0.000000	# AppIQ Agent Management
appiq-mgmt	4674/udp	0.000000	# AppIQ Agent Management
dhct-status	4675/tcp	0.000000	# BIAP Device Status
dhct-status	4675/udp	0.000000	# BIAP Device Status
dhct-alerts	4676/tcp	0.000000	# BIAP Generic Alert
dhct-alerts	4676/udp	0.000000	# BIAP Generic Alert
bcs	4677/tcp	0.000000	# Business Continuity Servi
bcs	4677/udp	0.000000	# Business Continuity Servi
traversal	4678/tcp	0.000000	# boundary traversal
traversal	4678/udp	0.000000	# boundary traversal
mgesupervision	4679/tcp	0.000000	# MGE UPS Supervision
mgesupervision	4679/udp	0.000000	# MGE UPS Supervision
mgemanagement	4680/tcp	0.000000	# MGE UPS Management
mgemanagement	4680/udp	0.000000	# MGE UPS Management
parliant	4681/tcp	0.000000	# Parliant Telephony System
parliant	4681/udp	0.000000	# Parliant Telephony System
finisar	4682/tcp	0.000000
finisar	4682/udp	0.000000
spike	4683/tcp	0.000000	# Spike Clipboard Service
spike	4683/udp	0.000000	# Spike Clipboard Service
rfid-rp1	4684/tcp	0.000000	# RFID Reader Protocol 1.0
rfid-rp1	4684/udp	0.000000	# RFID Reader Protocol 1.0
autopac	4685/tcp	0.000000	# Autopac Protocol
autopac	4685/udp	0.000000	# Autopac Protocol
msp-os	4686/tcp	0.000000	# Manina Service Protocol
msp-os	4686/udp	0.000000	# Manina Service Protocol
nst	4687/tcp	0.000076	# Network Scanner Tool FTP
nst	4687/udp	0.000000	# Network Scanner Tool FTP
mobile-p2p	4688/tcp	0.000000	# Mobile P2P Service
mobile-p2p	4688/udp	0.000000	# Mobile P2P Service
altovacentral	4689/tcp	0.000076	# Altova DatabaseCentral
altovacentral	4689/udp	0.000000	# Altova DatabaseCentral
prelude	4690/tcp	0.000000	# Prelude IDS message proto
prelude	4690/udp	0.000000	# Prelude IDS message proto
mtn	4691/tcp	0.000000	# monotone Netsync Protocol
mtn	4691/udp	0.000991	# monotone Netsync Protocol
conspiracy	4692/tcp	0.000000	# Conspiracy messaging
conspiracy	4692/udp	0.000661	# Conspiracy messaging
unknown	4693/udp	0.000330
unknown	4695/udp	0.000661
netxms-agent	4700/tcp	0.000076	# NetXMS Agent
netxms-agent	4700/udp	0.000000	# NetXMS Agent
netxms-mgmt	4701/tcp	0.000000	# NetXMS Management
netxms-mgmt	4701/udp	0.000330	# NetXMS Management
netxms-sync	4702/tcp	0.000000	# NetXMS Server Synchronization
netxms-sync	4702/udp	0.000330	# NetXMS Server Synchronization
npqes-test	4703/tcp	0.000000	# Network Performance Quality Evaluation System Test Service
assuria-ins	4704/tcp	0.000000	# Assuria Insider
unknown	4706/udp	0.000330
unknown	4709/udp	0.000330
trinity-dist	4711/tcp	0.000000	# Trinity Trust Network Node Communication
unknown	4712/tcp	0.000076
pulseaudio	4713/tcp	0.000076	# Pulse Audio UNIX sound framework
unknown	4713/udp	0.000330
truckstar	4725/tcp	0.000000	# TruckStar Service
truckstar	4725/udp	0.000000	# TruckStar Service
a26-fap-fgw	4726/tcp	0.000000	# A26 (FAP-FGW)
a26-fap-fgw	4726/udp	0.000330	# A26 (FAP-FGW)
fcis	4727/tcp	0.000000	# fcis-disc | F-Link Client Information Service | F-Link Client Information Service Discovery
fcis-disc	4727/udp	0.000000	# F-Link Client Information Service Discovery
capmux	4728/tcp	0.000000	# CA Port Multiplexer
capmux	4728/udp	0.000000	# CA Port Multiplexer
gsmtap	4729/tcp	0.000000	# GSM Interface Tap
gsmtap	4729/udp	0.000000	# GSM Interface Tap
gearman	4730/tcp	0.000000	# Gearman Job Queue System
gearman	4730/udp	0.000000	# Gearman Job Queue System
remcap	4731/tcp	0.000000	# Remote Capture Protocol
ohmtrigger	4732/tcp	0.000000	# OHM server trigger
ohmtrigger	4732/udp	0.000000	# OHM server trigger
resorcs	4733/tcp	0.000000	# RES Orchestration Catalog Services
unknown	4734/udp	0.000330
ipdr-sp	4737/tcp	0.000000	# IPDR/SP
ipdr-sp	4737/udp	0.000000	# IPDR/SP
solera-lpn	4738/tcp	0.000000	# SoleraTec Locator
solera-lpn	4738/udp	0.000000	# SoleraTec Locator
ipfix	4739/sctp	0.000000	# IP Flow Info Export
ipfix	4739/tcp	0.000000	# IP Flow Info Export
ipfix	4739/udp	0.000000	# IP Flow Info Export
ipfixs	4740/sctp	0.000000	# IP Flow Info Export over DTLS | ipfix protocol over TLS | ipfix protocol over DTLS
ipfixs	4740/tcp	0.000000	# IP Flow Info Export over TLS
ipfixs	4740/udp	0.000000	# IP Flow Info Export over DTLS
lumimgrd	4741/tcp	0.000000	# Luminizer Manager
lumimgrd	4741/udp	0.000330	# Luminizer Manager
sicct	4742/tcp	0.000000	# sicct-sdp | SICCT Service Discovery Protocol
sicct-sdp	4742/udp	0.000000	# SICCT Service Discovery Protocol
openhpid	4743/tcp	0.000000	# openhpi HPI service
openhpid	4743/udp	0.000330	# openhpi HPI service
ifsp	4744/tcp	0.000000	# Internet File Synchronization Protocol
ifsp	4744/udp	0.000000	# Internet File Synchronization Protocol
fmp	4745/tcp	0.000076	# Funambol Mobile Push
fmp	4745/udp	0.000330	# Funambol Mobile Push
intelliadm-disc	4746/tcp	0.000000	# IntelliAdmin Discovery
unknown	4746/udp	0.000330
buschtrommel	4747/tcp	0.000000	# peer-to-peer file exchange protocol
profilemac	4749/tcp	0.000000	# Profile for Mac
profilemac	4749/udp	0.000000	# Profile for Mac
ssad	4750/tcp	0.000000	# Simple Service Auto Discovery
ssad	4750/udp	0.000000	# Simple Service Auto Discovery
spocp	4751/tcp	0.000000	# Simple Policy Control Protocol
spocp	4751/udp	0.000000	# Simple Policy Control Protocol
snap	4752/tcp	0.000000	# Simple Network Audio Protocol
snap	4752/udp	0.000330	# Simple Network Audio Protocol
simon	4753/tcp	0.000000	# simon-disc | Simple Invocation of Methods Over Network (SIMON) | Simple Invocation of Methods Over Network (SIMON) Discovery
gre-in-udp	4754/tcp	0.000000	# GRE-in-UDP Encapsulation
gre-udp-dtls	4755/tcp	0.000000	# GRE-in-UDP Encapsulation with DTLS
RDCenter	4756/tcp	0.000000	# Reticle Decision Center
unknown	4757/udp	0.000330
unknown	4760/tcp	0.000076
unknown	4761/udp	0.000330
unknown	4767/tcp	0.000076
unknown	4769/udp	0.000330
unknown	4770/tcp	0.000076
unknown	4771/tcp	0.000076
unknown	4773/udp	0.000330
converge	4774/tcp	0.000000	# Converge RPC
unknown	4777/udp	0.000330
unknown	4778/tcp	0.000076
unknown	4778/udp	0.000991
unknown	4783/udp	0.000330
bfd-multi-ctl	4784/tcp	0.000000	# BFD Multihop Control
bfd-multi-ctl	4784/udp	0.000330	# BFD Multihop Control
cncp	4785/tcp	0.000000	# Cisco Nexus Control Protocol
cncp	4785/udp	0.000000	# Cisco Nexus Control Protocol
smart-install	4786/tcp	0.000000	# Smart Install Service
sia-ctrl-plane	4787/tcp	0.000000	# Service Insertion Architecture (SIA) Control-Plane
xmcp	4788/tcp	0.000000	# eXtensible Messaging Client Protocol
vxlan	4789/tcp	0.000000	# Virtual eXtensible Local Area Network (VXLAN)
vxlan-gpe	4790/tcp	0.000000	# Generic Protocol Extension for Virtual eXtensible Local Area Network (VXLAN)
roce	4791/tcp	0.000000	# IP Routable RocE
unified-bus	4792/tcp	0.000000	# IP Routable Unified Bus
unknown	4793/tcp	0.000076
unknown	4794/udp	0.000330
unknown	4797/udp	0.000330
unknown	4798/udp	0.000330
iims	4800/tcp	0.000076	# Icona Instant Messenging System
iims	4800/udp	0.000330	# Icona Instant Messenging System
iwec	4801/tcp	0.000000	# Icona Web Embedded Chat
iwec	4801/udp	0.000330	# Icona Web Embedded Chat
ilss	4802/tcp	0.000000	# Icona License System Server
ilss	4802/udp	0.000000	# Icona License System Server
notateit	4803/tcp	0.000000	# notateit-disc | Notateit Messaging | Notateit Messaging Discovery
notateit-disc	4803/udp	0.000000	# Notateit Messaging Discovery
aja-ntv4-disc	4804/tcp	0.000000	# AJA ntv4 Video System Discovery
aja-ntv4-disc	4804/udp	0.000000	# AJA ntv4 Video System Discovery
unknown	4807/udp	0.000330
unknown	4812/udp	0.000330
unknown	4819/tcp	0.000076
htcp	4827/tcp	0.000000
squid-htcp	4827/udp	0.000923	# Squid proxy HTCP port
unknown	4829/udp	0.000330
unknown	4833/udp	0.000330
unknown	4835/udp	0.000330
unknown	4836/udp	0.000661
varadero-0	4837/tcp	0.000000
varadero-0	4837/udp	0.000000
varadero-1	4838/tcp	0.000000
varadero-1	4838/udp	0.000330
varadero-2	4839/tcp	0.000000
varadero-2	4839/udp	0.000330
opcua-tcp	4840/tcp	0.000000	# opcua-udp | OPC UA TCP Protocol | OPC UA Connection Protocol | OPC UA Multicast Datagram Protocol
opcua-udp	4840/udp	0.000330	# OPC UA TCP Protocol
quosa	4841/tcp	0.000000	# QUOSA Virtual Library Service
quosa	4841/udp	0.000000	# QUOSA Virtual Library Service
gw-asv	4842/tcp	0.000000	# nCode ICE-flow Library AppServer
gw-asv	4842/udp	0.000000	# nCode ICE-flow Library AppServer
opcua-tls	4843/tcp	0.000000	# OPC UA TCP Protocol over TLS/SSL
opcua-tls	4843/udp	0.000000	# OPC UA TCP Protocol over TLS/SSL
gw-log	4844/tcp	0.000000	# nCode ICE-flow Library LogServer
gw-log	4844/udp	0.000330	# nCode ICE-flow Library LogServer
wcr-remlib	4845/tcp	0.000000	# WordCruncher Remote Library Service
wcr-remlib	4845/udp	0.000000	# WordCruncher Remote Library Service
contamac_icm	4846/tcp	0.000000	# contamac-icm | Contamac ICM Service
contamac_icm	4846/udp	0.000330	# Contamac ICM Service
wfc	4847/tcp	0.000000	# Web Fresh Communication
wfc	4847/udp	0.000000	# Web Fresh Communication
appserv-http	4848/tcp	0.000228	# App Server - Admin HTTP
appserv-http	4848/udp	0.000000	# App Server - Admin HTTP
appserv-https	4849/tcp	0.000000	# App Server - Admin HTTPS
appserv-https	4849/udp	0.000000	# App Server - Admin HTTPS
sun-as-nodeagt	4850/tcp	0.000000	# Sun App Server - NA
sun-as-nodeagt	4850/udp	0.000000	# Sun App Server - NA
derby-repli	4851/tcp	0.000000	# Apache Derby Replication
derby-repli	4851/udp	0.000330	# Apache Derby Replication
unknown	4854/udp	0.000330
unknown	4859/tcp	0.000076
unknown	4859/udp	0.000330
unknown	4860/tcp	0.000076
unify-debug	4867/tcp	0.000000	# Unify Debugger
unify-debug	4867/udp	0.000000	# Unify Debugger
phrelay	4868/tcp	0.000000	# Photon Relay
phrelay	4868/udp	0.000330	# Photon Relay
phrelaydbg	4869/tcp	0.000000	# Photon Relay Debug
phrelaydbg	4869/udp	0.000000	# Photon Relay Debug
cc-tracking	4870/tcp	0.000000	# Citcom Tracking Service
cc-tracking	4870/udp	0.000000	# Citcom Tracking Service
wired	4871/tcp	0.000000
wired	4871/udp	0.000000
unknown	4875/tcp	0.000152
unknown	4875/udp	0.000330
tritium-can	4876/tcp	0.000076	# Tritium CAN Bus Bridge Service
lmcs	4877/tcp	0.000076	# Lighting Management Control System
inst-discovery	4878/tcp	0.000000	# Agilent Instrument Discovery
wsdl-event	4879/tcp	0.000000	# WSDL Event Receiver
unknown	4879/udp	0.000330
hislip	4880/tcp	0.000000	# IVI High-Speed LAN Instrument Protocol
socp-t	4881/tcp	0.000076	# SOCP Time Synchronization Protocol
socp-t	4881/udp	0.000000	# SOCP Time Synchronization Protocol
socp-c	4882/tcp	0.000000	# SOCP Control Protocol
socp-c	4882/udp	0.000000	# SOCP Control Protocol
wmlserver	4883/tcp	0.000000	# Meier-Phelps License Server
hivestor	4884/tcp	0.000000	# HiveStor Distributed File System
hivestor	4884/udp	0.000330	# HiveStor Distributed File System
abbs	4885/tcp	0.000000
abbs	4885/udp	0.000000
xcap-portal	4888/tcp	0.000000	# xcap code analysis portal public user access
unknown	4888/udp	0.000330
xcap-control	4889/tcp	0.000000	# xcap code analysis portal cluster control and administration
unknown	4890/udp	0.000330
lyskom	4894/tcp	0.000000	# LysKOM Protocol A
lyskom	4894/udp	0.000000	# LysKOM Protocol A
unknown	4896/udp	0.000330
radmin	4899/tcp	0.003337	# radmin-port | Radmin (www.radmin.com) remote PC control software | RAdmin Port
radmin-port	4899/udp	0.000000	# RAdmin Port
hfcs	4900/tcp	0.000228	# HyperFileSQL Client/Server Database Engine | HFSQL Client/Server Database Engine
hfcs	4900/udp	0.000000	# HyperFileSQL Client/Server Database Engine
flr_agent	4901/tcp	0.000000	# flr-agent | FileLocator Remote Search Agent
magiccontrol	4902/tcp	0.000000	# magicCONROL RF and Data Interface
unknown	4903/tcp	0.000076
unknown	4907/udp	0.000330
unknown	4910/udp	0.000330
lutap	4912/tcp	0.000076	# Technicolor LUT Access Protocol
lutcp	4913/tcp	0.000000	# LUTher Control Protocol
bones	4914/tcp	0.000000	# Bones Remote Control
bones	4914/udp	0.000000	# Bones Remote Control
frcs	4915/tcp	0.000000	# Fibics Remote Control Service
unknown	4916/udp	0.000330
unknown	4918/udp	0.000330
unknown	4919/udp	0.000330
unknown	4923/udp	0.000330
unknown	4931/tcp	0.000076
unknown	4934/udp	0.000661
an-signaling	4936/tcp	0.000000	# Signal protocol port for autonomic networking
atsc-mh-ssc	4937/tcp	0.000000	# ATSC-M/H Service Signaling Channel
atsc-mh-ssc	4937/udp	0.000000	# ATSC-M/H Service Signaling Channel
unknown	4938/udp	0.000330
eq-office-4940	4940/tcp	0.000000	# Equitrac Office
eq-office-4940	4940/udp	0.000330	# Equitrac Office
eq-office-4941	4941/tcp	0.000000	# Equitrac Office
eq-office-4941	4941/udp	0.000330	# Equitrac Office
eq-office-4942	4942/tcp	0.000000	# Equitrac Office
eq-office-4942	4942/udp	0.000000	# Equitrac Office
unknown	4943/udp	0.000330
unknown	4948/udp	0.000330
munin	4949/tcp	0.000152	# Munin Graphing Framework
munin	4949/udp	0.000000	# Munin Graphing Framework
sybasesrvmon	4950/tcp	0.000000	# Sybase Server Monitor
sybasesrvmon	4950/udp	0.000000	# Sybase Server Monitor
pwgwims	4951/tcp	0.000000	# PWG WIMS
pwgwims	4951/udp	0.000000	# PWG WIMS
sagxtsds	4952/tcp	0.000000	# SAG Directory Server
sagxtsds	4952/udp	0.000000	# SAG Directory Server
dbsyncarbiter	4953/tcp	0.000000	# Synchronization Arbiter
unknown	4953/udp	0.000330
unknown	4955/udp	0.000330
unknown	4961/udp	0.000330
unknown	4962/udp	0.000330
unknown	4963/udp	0.000330
ccss-qmm	4969/tcp	0.000000	# CCSS QMessageMonitor
ccss-qmm	4969/udp	0.000000	# CCSS QMessageMonitor
ccss-qsm	4970/tcp	0.000000	# CCSS QSystemMonitor
ccss-qsm	4970/udp	0.000000	# CCSS QSystemMonitor
burp	4971/tcp	0.000000	# BackUp and Restore Program
unknown	4972/udp	0.000330
unknown	4973/udp	0.000330
ctxs-vpp	4980/tcp	0.000000	# Citrix Virtual Path
webyast	4984/tcp	0.000000
gerhcs	4985/tcp	0.000000	# GER HC Standard
mrip	4986/tcp	0.000000	# Model Railway Interface Program
mrip	4986/udp	0.000000	# Model Railway Interface Program
maybe-veritas	4987/tcp	0.000013	# smar-se-port1 | SMAR Ethernet Port 1
smar-se-port1	4987/udp	0.000000	# SMAR Ethernet Port 1
smar-se-port2	4988/tcp	0.000000	# SMAR Ethernet Port 2
smar-se-port2	4988/udp	0.000000	# SMAR Ethernet Port 2
parallel	4989/tcp	0.000000	# Parallel for GAUSS (tm)
parallel	4989/udp	0.000000	# Parallel for GAUSS (tm)
busycal	4990/tcp	0.000000	# BusySync Calendar Synch. Protocol
busycal	4990/udp	0.000000	# BusySync Calendar Synch. Protocol
vrt	4991/tcp	0.000000	# VITA Radio Transport
vrt	4991/udp	0.000330	# VITA Radio Transport
maybe-veritas	4998/tcp	0.000226
hfcs-manager	4999/tcp	0.000076	# HyperFileSQL Client/Server Database Engine Manager | HFSQL Client/Server Database Engine Manager
hfcs-manager	4999/udp	0.000000	# HyperFileSQL Client/Server Database Engine Manager
upnp	5000/tcp	0.006423	# commplex-main | Universal PnP, also Free Internet Chess Server
upnp	5000/udp	0.008913	# also complex-main
commplex-link	5001/tcp	0.003023
commplex-link	5001/udp	0.007018
rfe	5002/tcp	0.000765	# Radio Free Ethernet | radio free ethernet
rfe	5002/udp	0.002504	# Radio Free Ethernet
filemaker	5003/tcp	0.001756	# fmpro-internal | Filemaker Server - http://www.filemaker.com/ti/104289.html | FileMaker, Inc. - Proprietary transport | FileMaker, Inc. - Proprietary name binding
filemaker	5003/udp	0.002356	# Filemaker Server - http://www.filemaker.com/ti/104289.html
avt-profile-1	5004/tcp	0.000532	# RTP media data [RFC 3551][RFC 4571] | RTP media data
avt-profile-1	5004/udp	0.000330	# RTP media data [RFC 3551]
avt-profile-2	5005/tcp	0.000076	# RTP control protocol [RFC 3551][RFC 4571] | RTP control protocol
avt-profile-2	5005/udp	0.000330	# RTP control protocol [RFC 3551]
wsm-server	5006/tcp	0.000000	# wsm server
wsm-server	5006/udp	0.000000	# wsm server
wsm-server-ssl	5007/tcp	0.000000	# wsm server ssl
wsm-server-ssl	5007/udp	0.000000	# wsm server ssl
synapsis-edge	5008/tcp	0.000000	# Synapsis EDGE
synapsis-edge	5008/udp	0.000000	# Synapsis EDGE
airport-admin	5009/tcp	0.004416	# winfs | Apple AirPort WAP Administration | Microsoft Windows Filesystem
winfs	5009/udp	0.000000	# Microsoft Windows Filesystem
telelpathstart	5010/tcp	0.000138	# TelepathStart
telelpathstart	5010/udp	0.001582
telelpathattack	5011/tcp	0.000088	# TelepathAttack
telelpathattack	5011/udp	0.001120
nsp	5012/tcp	0.000076	# NetOnTap Service
nsp	5012/udp	0.000330	# NetOnTap Service
fmpro-v6	5013/tcp	0.000076	# FileMaker, Inc. - Proprietary transport
fmpro-v6	5013/udp	0.000330	# FileMaker, Inc. - Proprietary transport
onpsocket	5014/tcp	0.000076	# Overlay Network Protocol
onpsocket	5014/udp	0.000000	# Overlay Network Protocol
fmwp	5015/tcp	0.000076	# FileMaker, Inc. - Web publishing
unknown	5016/tcp	0.000076
unknown	5017/tcp	0.000076
unknown	5018/udp	0.000991
zenginkyo-1	5020/tcp	0.000076
zenginkyo-1	5020/udp	0.000000
zenginkyo-2	5021/tcp	0.000076
zenginkyo-2	5021/udp	0.000330
mice	5022/tcp	0.000000	# mice server
mice	5022/udp	0.000000	# mice server
htuilsrv	5023/tcp	0.000076	# Htuil Server for PLD2
htuilsrv	5023/udp	0.000000	# Htuil Server for PLD2
scpi-telnet	5024/tcp	0.000000
scpi-telnet	5024/udp	0.000000
scpi-raw	5025/tcp	0.000000
scpi-raw	5025/udp	0.000330
strexec-d	5026/tcp	0.000000	# Storix I/O daemon (data)
strexec-d	5026/udp	0.000000	# Storix I/O daemon (data)
strexec-s	5027/tcp	0.000000	# Storix I/O daemon (stat)
strexec-s	5027/udp	0.000000	# Storix I/O daemon (stat)
qvr	5028/tcp	0.000000	# Quiqum Virtual Relais
infobright	5029/tcp	0.000000	# Infobright Database Server
infobright	5029/udp	0.000000	# Infobright Database Server
surfpass	5030/tcp	0.000380
surfpass	5030/udp	0.000000
dmp	5031/tcp	0.000000	# Direct Message Protocol
dmp	5031/udp	0.000000	# Direct Message Protocol
signacert-agent	5032/tcp	0.000000	# SignaCert Enterprise Trust Server Agent
jtnetd-server	5033/tcp	0.000228	# Janstor Secure Data
jtnetd-status	5034/tcp	0.000000	# Janstor Status
unknown	5034/udp	0.000661
unknown	5040/tcp	0.000152
asnaacceler8db	5042/tcp	0.000000
asnaacceler8db	5042/udp	0.000330
swxadmin	5043/tcp	0.000000	# ShopWorX Administration
swxadmin	5043/udp	0.000330	# ShopWorX Administration
lxi-evntsvc	5044/tcp	0.000000	# LXI Event Service
lxi-evntsvc	5044/udp	0.000000	# LXI Event Service
osp	5045/tcp	0.000000	# Open Settlement Protocol
vpm-udp	5046/tcp	0.000000	# Vishay PM UDP Service
vpm-udp	5046/udp	0.000000	# Vishay PM UDP Service
iscape	5047/tcp	0.000000	# iSCAPE Data Broadcasting
iscape	5047/udp	0.000000	# iSCAPE Data Broadcasting
texai	5048/tcp	0.000000	# Texai Message Service
unknown	5048/udp	0.000661
ivocalize	5049/tcp	0.000000	# iVocalize Web Conference
ivocalize	5049/udp	0.000000	# iVocalize Web Conference
mmcc	5050/tcp	0.002584	# multimedia conference control tool
mmcc	5050/udp	0.002636	# multimedia conference control tool
ida-agent	5051/tcp	0.003649	# ita-agent | Symantec Intruder Alert | ITA Agent
ita-agent	5051/udp	0.000330	# ITA Agent
ita-manager	5052/tcp	0.000076	# ITA Manager
ita-manager	5052/udp	0.000000	# ITA Manager
rlm	5053/tcp	0.000076	# rlm-disc | RLM License Server | RLM Discovery Server
rlm-admin	5054/tcp	0.000304	# RLM administrative interface
unot	5055/tcp	0.000076
unot	5055/udp	0.000330
intecom-ps1	5056/tcp	0.000000	# Intecom Pointspan 1
intecom-ps1	5056/udp	0.000330	# Intecom Pointspan 1
intecom-ps2	5057/tcp	0.000000	# Intecom Pointspan 2
intecom-ps2	5057/udp	0.000000	# Intecom Pointspan 2
locus-disc	5058/tcp	0.000000	# Locus Discovery
locus-disc	5058/udp	0.000000	# Locus Discovery
sds	5059/tcp	0.000000	# SIP Directory Services
sds	5059/udp	0.000330	# SIP Directory Services
sip	5060/sctp	0.000000	# Session Initiation Protocol (SIP)
sip	5060/tcp	0.010613	# Session Initiation Protocol (SIP)
sip	5060/udp	0.044350	# Session Initiation Protocol (SIP)
sip-tls	5061/sctp	0.000000	# sips
sip-tls	5061/tcp	0.000228
sip-tls	5061/udp	0.000330
na-localise	5062/tcp	0.000000	# Localisation access
na-localise	5062/udp	0.000000	# Localisation access
csrpc	5063/tcp	0.000152	# centrify secure RPC
ca-1	5064/tcp	0.000000	# Channel Access 1
ca-1	5064/udp	0.000000	# Channel Access 1
ca-2	5065/tcp	0.000000	# Channel Access 2
ca-2	5065/udp	0.000000	# Channel Access 2
stanag-5066	5066/tcp	0.000076	# STANAG-5066-SUBNET-INTF
stanag-5066	5066/udp	0.000000	# STANAG-5066-SUBNET-INTF
authentx	5067/tcp	0.000000	# Authentx Service
authentx	5067/udp	0.000000	# Authentx Service
bitforestsrv	5068/tcp	0.000000	# Bitforest Data Service
unknown	5068/udp	0.000330
i-net-2000-npr	5069/tcp	0.000000	# I/Net 2000-NPR
i-net-2000-npr	5069/udp	0.000330	# I/Net 2000-NPR
vtsas	5070/tcp	0.000076	# VersaTrans Server Agent Service
vtsas	5070/udp	0.000000	# VersaTrans Server Agent Service
powerschool	5071/tcp	0.000000
powerschool	5071/udp	0.000330
ayiya	5072/tcp	0.000000	# Anything In Anything
ayiya	5072/udp	0.000000	# Anything In Anything
tag-pm	5073/tcp	0.000000	# Advantage Group Port Mgr
tag-pm	5073/udp	0.000000	# Advantage Group Port Mgr
alesquery	5074/tcp	0.000152	# ALES Query
alesquery	5074/udp	0.000000	# ALES Query
pvaccess	5075/tcp	0.000000	# Experimental Physics and Industrial Control System
unknown	5077/udp	0.000661
pixelpusher	5078/tcp	0.000000	# PixelPusher pixel data
cp-spxrpts	5079/tcp	0.000000	# Cambridge Pixel SPx Reports
cp-spxrpts	5079/udp	0.000000	# Cambridge Pixel SPx Reports
onscreen	5080/tcp	0.000228	# OnScreen Data Collection Service
onscreen	5080/udp	0.000000	# OnScreen Data Collection Service
sdl-ets	5081/tcp	0.000152	# SDL - Ent Trans Server
sdl-ets	5081/udp	0.000330	# SDL - Ent Trans Server
qcp	5082/tcp	0.000000	# Qpur Communication Protocol
qcp	5082/udp	0.000661	# Qpur Communication Protocol
qfp	5083/tcp	0.000000	# Qpur File Protocol
qfp	5083/udp	0.000000	# Qpur File Protocol
llrp	5084/tcp	0.000000	# EPCglobal Low-Level Reader Protocol
llrp	5084/udp	0.000000	# EPCglobal Low-Level Reader Protocol
encrypted-llrp	5085/tcp	0.000000	# EPCglobal Encrypted LLRP
encrypted-llrp	5085/udp	0.000000	# EPCglobal Encrypted LLRP
aprigo-cs	5086/tcp	0.000000	# Aprigo Collection Service
biotic	5087/tcp	0.000228	# BIOTIC - Binary Internet of Things Interoperable Communication
unknown	5088/tcp	0.000076
car	5090/sctp	0.000000	# Candidate AR
unknown	5090/tcp	0.000076
unknown	5090/udp	0.000330
cxtp	5091/sctp	0.000000	# Context Transfer Protocol
magpie	5092/tcp	0.000000	# Magpie Binary
magpie	5092/udp	0.000000	# Magpie Binary
sentinel-lm	5093/tcp	0.000000	# Sentinel LM
sentinel-lm	5093/udp	0.003304	# Sentinel LM
hart-ip	5094/tcp	0.000000
hart-ip	5094/udp	0.000330
unknown	5095/tcp	0.000076
unknown	5096/tcp	0.000076
unknown	5096/udp	0.000330
unknown	5098/tcp	0.000076
sentlm-srv2srv	5099/tcp	0.000000	# SentLM Srv2Srv
sentlm-srv2srv	5099/udp	0.000000	# SentLM Srv2Srv
admd	5100/tcp	0.000778	# socalia | (chili!soft asp admin port) or Yahoo pager | Socalia service mux
socalia	5100/udp	0.000330	# Socalia service mux
admdog	5101/tcp	0.005156	# talarian-udp | talarian-tcp | (chili!soft asp) | Talarian_TCP | Talarian_UDP
talarian-udp	5101/udp	0.000000	# Talarian_UDP
admeng	5102/tcp	0.000602	# oms-nonsecure | (chili!soft asp) | Oracle OMS non-secure
oms-nonsecure	5102/udp	0.000000	# Oracle OMS non-secure
actifio-c2c	5103/tcp	0.000000	# Actifio C2C
tinymessage	5104/tcp	0.000000
tinymessage	5104/udp	0.000000
hughes-ap	5105/tcp	0.000000	# Hughes Association Protocol
hughes-ap	5105/udp	0.000000	# Hughes Association Protocol
actifioudsagent	5106/tcp	0.000000	# Actifio UDS Agent
actifioreplic	5107/tcp	0.000000	# Disk to Disk replication between Actifio Clusters
unknown	5109/udp	0.000330
unknown	5110/udp	0.000661
taep-as-svc	5111/tcp	0.000076	# TAEP AS service
taep-as-svc	5111/udp	0.000000	# TAEP AS service
pm-cmdsvr	5112/tcp	0.000000	# PeerMe Msg Cmd Service
pm-cmdsvr	5112/udp	0.000000	# PeerMe Msg Cmd Service
unknown	5113/udp	0.000330
ev-services	5114/tcp	0.000076	# Enterprise Vault Services
autobuild	5115/tcp	0.000000	# Symantec Autobuild Service
emb-proj-cmd	5116/tcp	0.000000	# EPSON Projecter Image Transfer
emb-proj-cmd	5116/udp	0.000330	# EPSON Projecter Image Transfer
gradecam	5117/tcp	0.000000	# GradeCam Image Processing
unknown	5118/udp	0.000330
unknown	5119/udp	0.000661
barracuda-bbs	5120/tcp	0.002129	# Barracuda Backup Protocol
unknown	5120/udp	0.000330
unknown	5121/tcp	0.000076
unknown	5122/tcp	0.000076
unknown	5122/udp	0.000330
unknown	5125/tcp	0.000076
nbt-pc	5133/tcp	0.000076	# Policy Commander
nbt-pc	5133/udp	0.000000	# Policy Commander
ppactivation	5134/tcp	0.000000	# PP ActivationServer
erp-scale	5135/tcp	0.000000
minotaur-sa	5136/tcp	0.000000	# Minotaur SA
minotaur-sa	5136/udp	0.000000	# Minotaur SA
ctsd	5137/tcp	0.000076	# MyCTS server port
ctsd	5137/udp	0.000000	# MyCTS server port
unknown	5139/udp	0.000661
rmonitor_secure	5145/tcp	0.000050	# rmonitor-secure | RMONITOR SECURE
rmonitor_secure	5145/udp	0.000610
social-alarm	5146/tcp	0.000000	# Social Alarm Service
unknown	5147/tcp	0.000076
atmp	5150/tcp	0.000000	# Ascend Tunnel Management Protocol
atmp	5150/udp	0.000000	# Ascend Tunnel Management Protocol
esri_sde	5151/tcp	0.000152	# esri-sde | ESRI SDE Instance | ESRI SDE Remote Start
esri_sde	5151/udp	0.000000	# ESRI SDE Remote Start
sde-discovery	5152/tcp	0.000076	# ESRI SDE Instance Discovery
sde-discovery	5152/udp	0.000330	# ESRI SDE Instance Discovery
toruxserver	5153/tcp	0.000000	# ToruX Game Server
bzflag	5154/tcp	0.000000	# BZFlag game server
bzflag	5154/udp	0.000000	# BZFlag game server
asctrl-agent	5155/tcp	0.000000	# Oracle asControl Agent
asctrl-agent	5155/udp	0.000000	# Oracle asControl Agent
rugameonline	5156/tcp	0.000000	# Russian Online Game
mediat	5157/tcp	0.000000	# Mediat Remote Object Exchange
snmpssh	5161/tcp	0.000000	# SNMP over SSH Transport Model
unknown	5161/udp	0.000330
snmpssh-trap	5162/tcp	0.000000	# SNMP Notification over SSH Transport Model
unknown	5162/udp	0.000330
sbackup	5163/tcp	0.000000	# Shadow Backup
vpa	5164/tcp	0.000000	# vpa-disc | Virtual Protocol Adapter | Virtual Protocol Adapter Discovery
vpa-disc	5164/udp	0.000000	# Virtual Protocol Adapter Discovery
ife_icorp	5165/tcp	0.000000	# ife-icorp | ife_1corp
ife_icorp	5165/udp	0.000000	# ife_1corp
winpcs	5166/tcp	0.000000	# WinPCS Service Connection
winpcs	5166/udp	0.000330	# WinPCS Service Connection
scte104	5167/tcp	0.000000	# SCTE104 Connection
scte104	5167/udp	0.000000	# SCTE104 Connection
scte30	5168/tcp	0.000000	# SCTE30 Connection
scte30	5168/udp	0.000661	# SCTE30 Connection
pcoip-mgmt	5172/tcp	0.000000	# PC over IP Endpoint Management
unknown	5174/udp	0.000330
unknown	5185/udp	0.000330
unknown	5187/udp	0.000330
aol	5190/tcp	0.004190	# America-Online.  Also can be used by ICQ | America-Online
aol	5190/udp	0.000692	# America-Online.
aol-1	5191/tcp	0.000050	# AmericaOnline1
aol-1	5191/udp	0.000593	# AmericaOnline1
aol-2	5192/tcp	0.000000	# AmericaOnline2
aol-2	5192/udp	0.000494	# AmericaOnline2
aol-3	5193/tcp	0.000013	# AmericaOnline3
aol-3	5193/udp	0.000511	# AmericaOnline3
cpscomm	5194/tcp	0.000000	# CipherPoint Config Service
ampl-lic	5195/tcp	0.000000	# The protocol is used by a license server and client programs to control use of program licenses that float to networked machines
ampl-tableproxy	5196/tcp	0.000000	# The protocol is used by two programs that exchange "table" data used in the AMPL modeling language
unknown	5196/udp	0.000330
tunstall-lwp	5197/tcp	0.000000	# Tunstall Lone worker device interface
targus-getdata	5200/tcp	0.000304	# TARGUS GetData
targus-getdata	5200/udp	0.000000	# TARGUS GetData
targus-getdata1	5201/tcp	0.000076	# TARGUS GetData 1
targus-getdata1	5201/udp	0.000000	# TARGUS GetData 1
targus-getdata2	5202/tcp	0.000076	# TARGUS GetData 2
targus-getdata2	5202/udp	0.000000	# TARGUS GetData 2
targus-getdata3	5203/tcp	0.000000	# TARGUS GetData 3
targus-getdata3	5203/udp	0.000000	# TARGUS GetData 3
unknown	5204/udp	0.000330
unknown	5207/udp	0.000330
unknown	5208/udp	0.000330
nomad	5209/tcp	0.000000	# Nomad Device Video Transfer
unknown	5210/udp	0.000661
unknown	5212/tcp	0.000152
unknown	5214/tcp	0.000532
noteza	5215/tcp	0.000000	# NOTEZA Data Safety Service
unknown	5219/tcp	0.000076
3exmp	5221/tcp	0.000228	# 3eTI Extensible Management Protocol for OAMP
xmpp-client	5222/tcp	0.000380	# XMPP Client Connection
xmpp-client	5222/udp	0.000000	# XMPP Client Connection
hpvirtgrp	5223/tcp	0.000152	# HP Virtual Machine Group Management
hpvirtgrp	5223/udp	0.000000	# HP Virtual Machine Group Management
hpvirtctrl	5224/tcp	0.000000	# HP Virtual Machine Console Operations
hpvirtctrl	5224/udp	0.000000	# HP Virtual Machine Console Operations
hp-server	5225/tcp	0.000760	# HP Server
hp-server	5225/udp	0.000330	# HP Server
hp-status	5226/tcp	0.000760	# HP Status
hp-status	5226/udp	0.000000	# HP Status
perfd	5227/tcp	0.000000	# HP System Performance Metric Service
perfd	5227/udp	0.000330	# HP System Performance Metric Service
hpvroom	5228/tcp	0.000000	# HP Virtual Room Service
unknown	5228/udp	0.000330
jaxflow	5229/tcp	0.000000	# Netflow/IPFIX/sFlow Collector and Forwarder Management
unknown	5229/udp	0.000330
jaxflow-data	5230/tcp	0.000000	# JaxMP RealFlow application and protocol data
unknown	5230/udp	0.000330
crusecontrol	5231/tcp	0.000000	# Remote Control of Scan Software for Cruse Scanners
sgi-dgl	5232/tcp	0.000050	# csedaemon | SGI Distributed Graphics | Cruse Scanning System Service
enfs	5233/tcp	0.000076	# Etinnae Network File Service
eenet	5234/tcp	0.000076	# EEnet communications
eenet	5234/udp	0.000330	# EEnet communications
galaxy-network	5235/tcp	0.000076	# Galaxy Network Service
galaxy-network	5235/udp	0.000000	# Galaxy Network Service
padl2sim	5236/tcp	0.000000
padl2sim	5236/udp	0.000577
mnet-discovery	5237/tcp	0.000000	# m-net discovery
mnet-discovery	5237/udp	0.000000	# m-net discovery
attune	5242/tcp	0.000152	# ATTUne API
unknown	5242/udp	0.000330
xycstatus	5243/tcp	0.000000	# xyClient Status API and rendevous point
downtools	5245/tcp	0.000000	# downtools-disc | DownTools Control Protocol | DownTools Discovery Protocol
downtools-disc	5245/udp	0.000330	# DownTools Discovery Protocol
capwap-control	5246/tcp	0.000000	# CAPWAP Control Protocol
capwap-control	5246/udp	0.000330	# CAPWAP Control Protocol
capwap-data	5247/tcp	0.000000	# CAPWAP Data Protocol
capwap-data	5247/udp	0.000000	# CAPWAP Data Protocol
caacws	5248/tcp	0.000000	# CA Access Control Web Service
caacws	5248/udp	0.000000	# CA Access Control Web Service
caaclang2	5249/tcp	0.000000	# CA AC Lang Service
caaclang2	5249/udp	0.000000	# CA AC Lang Service
soagateway	5250/tcp	0.000076
soagateway	5250/udp	0.000000
caevms	5251/tcp	0.000000	# CA eTrust VM Service
caevms	5251/udp	0.000000	# CA eTrust VM Service
movaz-ssc	5252/tcp	0.000076	# Movaz SSC
movaz-ssc	5252/udp	0.000000	# Movaz SSC
kpdp	5253/tcp	0.000000	# Kohler Power Device Protocol
logcabin	5254/tcp	0.000000	# LogCabin storage service
unknown	5254/udp	0.000330
unknown	5259/tcp	0.000076
unknown	5260/udp	0.000330
unknown	5261/tcp	0.000076
3com-njack-1	5264/tcp	0.000000	# 3Com Network Jack Port 1
3com-njack-1	5264/udp	0.000330	# 3Com Network Jack Port 1
3com-njack-2	5265/tcp	0.000000	# 3Com Network Jack Port 2
3com-njack-2	5265/udp	0.000000	# 3Com Network Jack Port 2
unknown	5267/udp	0.000330
xmpp-server	5269/tcp	0.000380	# XMPP Server Connection
xmpp-server	5269/udp	0.000330	# XMPP Server Connection
xmp	5270/tcp	0.000000	# cartographerxmp | Cartographer XMP
xmp	5270/udp	0.000000	# Cartographer XMP
cuelink	5271/tcp	0.000000	# cuelink-disc | StageSoft CueLink messaging | StageSoft CueLink discovery
cuelink-disc	5271/udp	0.000330	# StageSoft CueLink discovery
pk	5272/tcp	0.000000
pk	5272/udp	0.000330
unknown	5277/udp	0.000330
unknown	5279/tcp	0.000152
unknown	5279/udp	0.000661
xmpp-bosh	5280/tcp	0.000304	# Bidirectional-streams Over Synchronous HTTP (BOSH)
undo-lm	5281/tcp	0.000000	# Undo License Manager
unknown	5281/udp	0.000330
transmit-port	5282/tcp	0.000000	# Marimba Transmitter Port
transmit-port	5282/udp	0.000000	# Marimba Transmitter Port
unknown	5285/udp	0.000330
unknown	5291/tcp	0.000076
unknown	5291/udp	0.000330
unknown	5293/udp	0.000330
unknown	5297/udp	0.000330
presence	5298/tcp	0.000304	# XMPP Link-Local Messaging
presence	5298/udp	0.000000	# XMPP Link-Local Messaging
nlg-data	5299/tcp	0.000000	# NLG Data Service
nlg-data	5299/udp	0.000000	# NLG Data Service
hacl-hb	5300/tcp	0.000050	# HA cluster heartbeat
hacl-hb	5300/udp	0.000412	# HA cluster heartbeat
hacl-gs	5301/tcp	0.000025	# HA cluster general services
hacl-gs	5301/udp	0.000511	# HA cluster general services
hacl-cfg	5302/tcp	0.000025	# HA cluster configuration
hacl-cfg	5302/udp	0.000511	# HA cluster configuration
hacl-probe	5303/tcp	0.000013	# HA cluster probing
hacl-probe	5303/udp	0.000395	# HA cluster probing
hacl-local	5304/tcp	0.000000	# HA Cluster Commands
hacl-local	5304/udp	0.000692
hacl-test	5305/tcp	0.000000	# HA Cluster Test
hacl-test	5305/udp	0.000412
sun-mc-grp	5306/tcp	0.000000	# Sun MC Group
sun-mc-grp	5306/udp	0.000000	# Sun MC Group
sco-aip	5307/tcp	0.000000	# SCO AIP
sco-aip	5307/udp	0.000000	# SCO AIP
cfengine	5308/tcp	0.000075
cfengine	5308/udp	0.001021
jprinter	5309/tcp	0.000000	# J Printer
jprinter	5309/udp	0.000330	# J Printer
outlaws	5310/tcp	0.000000
outlaws	5310/udp	0.000000
permabit-cs	5312/tcp	0.000000	# Permabit Client-Server
permabit-cs	5312/udp	0.000000	# Permabit Client-Server
rrdp	5313/tcp	0.000000	# Real-time & Reliable Data
rrdp	5313/udp	0.000000	# Real-time & Reliable Data
opalis-rbt-ipc	5314/tcp	0.000000
opalis-rbt-ipc	5314/udp	0.000000
hacl-poll	5315/tcp	0.000000	# HA Cluster UDP Polling
hacl-poll	5315/udp	0.000000	# HA Cluster UDP Polling
hpdevms	5316/tcp	0.000000	# hpbladems | HP Device Monitor Service | HPBladeSystem Monitor Service
hpdevms	5316/udp	0.000000	# HP Device Monitor Service
hpdevms	5317/tcp	0.000000	# HP Device Monitor Service
pkix-cmc	5318/tcp	0.000000	# PKIX Certificate Management using CMS (CMC)
unknown	5318/udp	0.000661
bsfserver-zn	5320/tcp	0.000000	# Webservices-based Zn interface of BSF
unknown	5320/udp	0.000661
bsfsvr-zn-ssl	5321/tcp	0.000000	# Webservices-based Zn interface of BSF over SSL
unknown	5323/udp	0.000330
unknown	5324/udp	0.000330
unknown	5333/udp	0.000330
unknown	5337/udp	0.000330
unknown	5339/tcp	0.000152
kfserver	5343/tcp	0.000000	# Sculptor Database Server
kfserver	5343/udp	0.000330	# Sculptor Database Server
xkotodrcp	5344/tcp	0.000000	# xkoto DRCP
xkotodrcp	5344/udp	0.000000	# xkoto DRCP
unknown	5345/udp	0.000330
unknown	5347/tcp	0.000076
unknown	5347/udp	0.000991
stuns	5349/tcp	0.000000	# stun-behaviors | turns | STUN over TLS | STUN over DTLS | TURN over TLS | TURN over DTLS | STUN Behavior Discovery over TLS | Reserved for a future enhancement of STUN-BEHAVIOR | Session Traversal Utilities for NAT (STUN) port
stuns	5349/udp	0.000000	# Reserved for a future enhancement of STUN
nat-pmp-status	5350/tcp	0.000000	# pcp-multicast | NAT-PMP Status Announcements | Port Control Protocol Multicast
nat-pmp-status	5350/udp	0.000000	# NAT-PMP Status Announcements
nat-pmp	5351/tcp	0.000000	# pcp | NAT Port Mapping Protocol | Port Control Protocol
nat-pmp	5351/udp	0.003304
dns-llq	5352/tcp	0.000000	# DNS Long-Lived Queries
dns-llq	5352/udp	0.000330	# DNS Long-Lived Queries
mdns	5353/tcp	0.000152	# Multicast DNS
zeroconf	5353/udp	0.100166	# Mac OS X Bonjour/Zeroconf port
mdnsresponder	5354/tcp	0.000000	# Multicast DNS Responder IPC
mdnsresponder	5354/udp	0.000661	# Multicast DNS Responder IPC
llmnr	5355/tcp	0.000000
llmnr	5355/udp	0.006938
ms-smlbiz	5356/tcp	0.000000	# Microsoft Small Business
ms-smlbiz	5356/udp	0.000000	# Microsoft Small Business
wsdapi	5357/tcp	0.005474	# Web Services for Devices
wsdapi	5357/udp	0.000661	# Web Services for Devices
wsdapi-s	5358/tcp	0.000000	# WS for Devices Secured
wsdapi-s	5358/udp	0.000000	# WS for Devices Secured
ms-alerter	5359/tcp	0.000000	# Microsoft Alerter
ms-alerter	5359/udp	0.000000	# Microsoft Alerter
ms-sideshow	5360/tcp	0.000000	# Protocol for Windows SideShow
ms-sideshow	5360/udp	0.000000	# Protocol for Windows SideShow
ms-s-sideshow	5361/tcp	0.000000	# Secure Protocol for Windows SideShow
ms-s-sideshow	5361/udp	0.000000	# Secure Protocol for Windows SideShow
serverwsd2	5362/tcp	0.000000	# Microsoft Windows Server WSD2 Service
serverwsd2	5362/udp	0.000000	# Microsoft Windows Server WSD2 Service
net-projection	5363/tcp	0.000000	# Windows Network Projection
net-projection	5363/udp	0.000000	# Windows Network Projection
kdnet	5364/tcp	0.000000	# Microsoft Kernel Debugger
unknown	5366/udp	0.000661
unknown	5370/tcp	0.000076
unknown	5374/udp	0.000330
unknown	5377/tcp	0.000076
unknown	5382/udp	0.000330
stresstester	5397/tcp	0.000000	# StressTester(tm) Injector
stresstester	5397/udp	0.000000	# StressTester(tm) Injector
elektron-admin	5398/tcp	0.000000	# Elektron Administration
elektron-admin	5398/udp	0.000330	# Elektron Administration
securitychase	5399/tcp	0.000000
securitychase	5399/udp	0.000000
pcduo-old	5400/tcp	0.000050	# excerpt | RemCon PC-Duo - old port | Excerpt Search
excerpt	5400/udp	0.000330	# Excerpt Search
excerpts	5401/tcp	0.000000	# Excerpt Search Secure
excerpts	5401/udp	0.000000	# Excerpt Search Secure
mftp	5402/tcp	0.000000	# OmniCast MFTP
mftp	5402/udp	0.000000	# OmniCast MFTP
hpoms-ci-lstn	5403/tcp	0.000000
hpoms-ci-lstn	5403/udp	0.000000
hpoms-dps-lstn	5404/tcp	0.000000
hpoms-dps-lstn	5404/udp	0.000000
pcduo	5405/tcp	0.000314	# netsupport | RemCon PC-Duo - new port | NetSupport
netsupport	5405/udp	0.000000
systemics-sox	5406/tcp	0.000000	# Systemics Sox
systemics-sox	5406/udp	0.000000	# Systemics Sox
foresyte-clear	5407/tcp	0.000000
foresyte-clear	5407/udp	0.000000
foresyte-sec	5408/tcp	0.000000
foresyte-sec	5408/udp	0.000330
salient-dtasrv	5409/tcp	0.000000	# Salient Data Server
salient-dtasrv	5409/udp	0.000000	# Salient Data Server
salient-usrmgr	5410/tcp	0.000000	# Salient User Manager
salient-usrmgr	5410/udp	0.000000	# Salient User Manager
actnet	5411/tcp	0.000000
actnet	5411/udp	0.000000
continuus	5412/tcp	0.000000
continuus	5412/udp	0.000000
wwiotalk	5413/tcp	0.000000
wwiotalk	5413/udp	0.000000
statusd	5414/tcp	0.000380
statusd	5414/udp	0.000000
ns-server	5415/tcp	0.000000	# NS Server
ns-server	5415/udp	0.000000	# NS Server
sns-gateway	5416/tcp	0.000000	# SNS Gateway
sns-gateway	5416/udp	0.000000	# SNS Gateway
sns-agent	5417/tcp	0.000000	# SNS Agent
sns-agent	5417/udp	0.000000	# SNS Agent
mcntp	5418/tcp	0.000000
mcntp	5418/udp	0.000000
dj-ice	5419/tcp	0.000000
dj-ice	5419/udp	0.000000
cylink-c	5420/tcp	0.000000
cylink-c	5420/udp	0.000000
netsupport2	5421/tcp	0.000000	# Net Support 2
netsupport2	5421/udp	0.000000	# Net Support 2
salient-mux	5422/tcp	0.000000	# Salient MUX
salient-mux	5422/udp	0.000000	# Salient MUX
virtualuser	5423/tcp	0.000076
virtualuser	5423/udp	0.000330
beyond-remote	5424/tcp	0.000000	# Beyond Remote
beyond-remote	5424/udp	0.000330	# Beyond Remote
br-channel	5425/tcp	0.000000	# Beyond Remote Command Channel
br-channel	5425/udp	0.000000	# Beyond Remote Command Channel
devbasic	5426/tcp	0.000000
devbasic	5426/udp	0.000000
sco-peer-tta	5427/tcp	0.000000
sco-peer-tta	5427/udp	0.000000
telaconsole	5428/tcp	0.000000
omid	5428/udp	0.000527	# OpenMosix Info Dissemination
base	5429/tcp	0.000000	# Billing and Accounting System Exchange
base	5429/udp	0.000000	# Billing and Accounting System Exchange
radec-corp	5430/tcp	0.000000	# RADEC CORP
radec-corp	5430/udp	0.000000	# RADEC CORP
park-agent	5431/tcp	0.000684	# PARK AGENT
park-agent	5431/udp	0.000000
postgresql	5432/tcp	0.004090	# PostgreSQL database server | PostgreSQL Database
postgresql	5432/udp	0.000000	# PostgreSQL Database
pyrrho	5433/tcp	0.000076	# Pyrrho DBMS
pyrrho	5433/udp	0.000000	# Pyrrho DBMS
sgi-arrayd	5434/tcp	0.000000	# SGI Array Services Daemon
sgi-arrayd	5434/udp	0.000000	# SGI Array Services Daemon
sceanics	5435/tcp	0.000000	# SCEANICS situation and action notification
sceanics	5435/udp	0.000661	# SCEANICS situation and action notification
pmip6-cntl	5436/tcp	0.000000
pmip6-cntl	5436/udp	0.000000
pmip6-data	5437/tcp	0.000000
pmip6-data	5437/udp	0.000000
unknown	5439/udp	0.000661
unknown	5440/tcp	0.000228
unknown	5440/udp	0.000330
unknown	5441/tcp	0.000076
unknown	5442/tcp	0.000076
spss	5443/tcp	0.000000	# Pearson HTTPS
spss	5443/udp	0.000330	# Pearson HTTPS
unknown	5444/tcp	0.000076
unknown	5444/udp	0.000661
smbdirect	5445/tcp	0.000000	# Server Message Block over Remote Direct Memory Access
unknown	5446/udp	0.000330
tiepie	5450/tcp	0.000000	# tiepie-disc | TiePie engineering data acquisition | TiePie engineering data acquisition (discovery)
unknown	5452/udp	0.000330
surebox	5453/tcp	0.000000
surebox	5453/udp	0.000000
apc-5454	5454/tcp	0.000000	# APC 5454
apc-5454	5454/udp	0.000000	# APC 5454
apc-5455	5455/tcp	0.000000	# APC 5455
apc-5455	5455/udp	0.000000	# APC 5455
apc-5456	5456/tcp	0.000000	# APC 5456
apc-5456	5456/udp	0.000000	# APC 5456
unknown	5457/tcp	0.000076
unknown	5458/tcp	0.000076
silkmeter	5461/tcp	0.000000
silkmeter	5461/udp	0.000000
ttl-publisher	5462/tcp	0.000000	# TTL Publisher
ttl-publisher	5462/udp	0.000000	# TTL Publisher
ttlpriceproxy	5463/tcp	0.000000	# TTL Price Proxy
ttlpriceproxy	5463/udp	0.000000	# TTL Price Proxy
quailnet	5464/tcp	0.000000	# Quail Networks Object Broker
quailnet	5464/udp	0.000000	# Quail Networks Object Broker
netops-broker	5465/tcp	0.000000
netops-broker	5465/udp	0.000000
apsolab-col	5470/tcp	0.000000	# The Apsolab company's data collection protocol (native api)
apsolab-cols	5471/tcp	0.000000	# The Apsolab company's secure data collection protocol (native api)
apsolab-tag	5472/tcp	0.000000	# The Apsolab company's dynamic tag protocol
unknown	5472/udp	0.000330
apsolab-tags	5473/tcp	0.000076	# The Apsolab company's secure dynamic tag protocol
apsolab-rpc	5474/tcp	0.000000	# The Apsolab company's status query protocol
apsolab-data	5475/tcp	0.000076	# The Apsolab company's data retrieval protocol
unknown	5476/udp	0.000330
unknown	5477/udp	0.000330
unknown	5478/udp	0.000330
unknown	5479/udp	0.000330
connect-proxy	5490/tcp	0.000013	# Many HTTP CONNECT proxies
unknown	5496/udp	0.000330
hotline	5500/tcp	0.000690	# Hotline file sharing client/server | fcp-addr-srvr1
securid	5500/udp	0.003295
fcp-addr-srvr2	5501/tcp	0.000152
fcp-addr-srvr2	5501/udp	0.000000
fcp-srvr-inst1	5502/tcp	0.000076
fcp-srvr-inst1	5502/udp	0.000000
fcp-srvr-inst2	5503/tcp	0.000000
fcp-srvr-inst2	5503/udp	0.000000
fcp-cics-gw1	5504/tcp	0.000000
fcp-cics-gw1	5504/udp	0.000000
checkoutdb	5505/tcp	0.000000	# Checkout Database
checkoutdb	5505/udp	0.000000	# Checkout Database
amc	5506/tcp	0.000000	# Amcom Mobile Connect
amc	5506/udp	0.000000	# Amcom Mobile Connect
psl-management	5507/tcp	0.000000	# PowerSysLab Electrical Management
unknown	5509/udp	0.000661
secureidprop	5510/tcp	0.000339	# ACE/Server services
unknown	5518/udp	0.000330
unknown	5519/udp	0.000330
sdlog	5520/tcp	0.000125	# ACE/Server services
sdserv	5530/tcp	0.000038	# ACE/Server services
unknown	5532/udp	0.000330
unknown	5533/udp	0.000330
unknown	5537/udp	0.000330
unknown	5538/udp	0.000330
sdreport	5540/tcp	0.000000	# matter | ACE/Server services | Matter Operational Discovery and Communi
sdxauthd	5540/udp	0.000445	# ACE/Server services
unknown	5541/udp	0.000330
qftest-licserve	5543/tcp	0.000000	# QF-Test License Server
unknown	5544/tcp	0.000228
unknown	5545/udp	0.000330
unknown	5547/udp	0.000330
sdadmind	5550/tcp	0.000853	# cbus | ACE/Server services | Model Railway control using the CBUS message protocol
unknown	5552/tcp	0.000076
unknown	5552/udp	0.000661
sgi-eventmond	5553/tcp	0.000076	# SGI Eventmond Port
sgi-eventmond	5553/udp	0.000000	# SGI Eventmond Port
sgi-esphttp	5554/tcp	0.000076	# SGI ESP HTTP
sgi-esphttp	5554/udp	0.000000	# SGI ESP HTTP
freeciv	5555/tcp	0.001305	# personal-agent | Personal Agent
rplay	5555/udp	0.001615
freeciv	5556/tcp	0.000000	# Freeciv gameplay
freeciv	5556/udp	0.000000	# Freeciv gameplay
farenet	5557/tcp	0.000076	# Sandlab FARENET
isqlplus	5560/tcp	0.000238	# Oracle web enabled SQL interface (version 10g+)
hpe-dp-bura	5565/tcp	0.000000	# dp-bura | HPE Advanced BURA | Data Protector BURA
westec-connect	5566/tcp	0.000608	# Westec Connect
m-oap	5567/tcp	0.000000	# dof-dps-mc-sec | Multicast Object Access Protocol | DOF Protocol Stack Multicast/Secure Transport
m-oap	5567/udp	0.000000	# Multicast Object Access Protocol
sdt	5568/tcp	0.000000	# Session Data Transport Multicast
sdt	5568/udp	0.000000	# Session Data Transport Multicast
rdmnet-ctrl	5569/tcp	0.000000	# rdmnet-device | PLASA E1.33, Remote Device Management (RDM) controller status notifications | PLASA E1.33, Remote Device Management (RDM) messages
sdmmp	5573/tcp	0.000000	# SAS Domain Management Messaging Protocol
sdmmp	5573/udp	0.000000	# SAS Domain Management Messaging Protocol
lsi-bobcat	5574/tcp	0.000000	# SAS IO Forwarding
ora-oap	5575/tcp	0.000000	# Oracle Access Protocol
unknown	5577/udp	0.000330
fdtracks	5579/tcp	0.000000	# FleetDisplay Tracking Service
tmosms0	5580/tcp	0.000076	# T-Mobile SMS Protocol Message 0
tmosms0	5580/udp	0.000330	# T-Mobile SMS Protocol Message 0
tmosms1	5581/tcp	0.000076	# T-Mobile SMS Protocol Message 1
tmosms1	5581/udp	0.000000	# T-Mobile SMS Protocol Message 1
fac-restore	5582/tcp	0.000000	# T-Mobile SMS Protocol Message 3
fac-restore	5582/udp	0.000000	# T-Mobile SMS Protocol Message 3
tmo-icon-sync	5583/tcp	0.000000	# T-Mobile SMS Protocol Message 2
tmo-icon-sync	5583/udp	0.000330	# T-Mobile SMS Protocol Message 2
bis-web	5584/tcp	0.000000	# BeInSync-Web
bis-web	5584/udp	0.000000	# BeInSync-Web
bis-sync	5585/tcp	0.000000	# BeInSync-sync
bis-sync	5585/udp	0.000000	# BeInSync-sync
att-mt-sms	5586/tcp	0.000000	# Planning to send mobile terminated SMS to the specific port so that the SMS is not visible to the client
unknown	5587/udp	0.000330
unknown	5589/udp	0.000661
ininmessaging	5597/tcp	0.000000	# inin secure messaging
ininmessaging	5597/udp	0.000000	# inin secure messaging
mctfeed	5598/tcp	0.000000	# MCT Market Data Feed
mctfeed	5598/udp	0.000000	# MCT Market Data Feed
esinstall	5599/tcp	0.000000	# Enterprise Security Remote Install
esinstall	5599/udp	0.000000	# Enterprise Security Remote Install
esmmanager	5600/tcp	0.000000	# Enterprise Security Manager
esmmanager	5600/udp	0.000000	# Enterprise Security Manager
esmagent	5601/tcp	0.000000	# Enterprise Security Agent
esmagent	5601/udp	0.000000	# Enterprise Security Agent
a1-msc	5602/tcp	0.000000
a1-msc	5602/udp	0.000000
a1-bs	5603/tcp	0.000000
a1-bs	5603/udp	0.000000
a3-sdunode	5604/tcp	0.000000
a3-sdunode	5604/udp	0.000000
a4-sdunode	5605/tcp	0.000000
a4-sdunode	5605/udp	0.000000
unknown	5611/tcp	0.000076
unknown	5612/tcp	0.000076
unknown	5613/udp	0.000330
unknown	5614/udp	0.000330
unknown	5616/udp	0.000330
efr	5618/tcp	0.000000	# Fiscal Registering Protocol
unknown	5620/tcp	0.000076
unknown	5621/tcp	0.000076
unknown	5622/tcp	0.000076
ninaf	5627/tcp	0.000000	# Node Initiated Network Association Forma
ninaf	5627/udp	0.000000	# Node Initiated Network Association Forma
htrust	5628/tcp	0.000000	# HTrust API
htrust	5628/udp	0.000000	# HTrust API
symantec-sfdb	5629/tcp	0.000000	# Symantec Storage Foundation for Database
symantec-sfdb	5629/udp	0.000661	# Symantec Storage Foundation for Database
precise-comm	5630/tcp	0.000000	# PreciseCommunication
precise-comm	5630/udp	0.000330	# PreciseCommunication
pcanywheredata	5631/tcp	0.006248
pcanywheredata	5631/udp	0.000000
pcanywherestat	5632/tcp	0.000075
pcanywherestat	5632/udp	0.007694
beorl	5633/tcp	0.000380	# BE Operations Request Listener
beorl	5633/udp	0.000330	# BE Operations Request Listener
xprtld	5634/tcp	0.000000	# SF Message Service
xprtld	5634/udp	0.000330	# SF Message Service
sfmsso	5635/tcp	0.000000	# SFM Authentication Subsystem
sfm-db-server	5636/tcp	0.000000	# SFMdb - SFM DB server
cssc	5637/tcp	0.000000	# Symantec CSSC
flcrs	5638/tcp	0.000000	# Symantec Fingerprint Lookup and Container Reference Service
ics	5639/tcp	0.000000	# Symantec Integrity Checking Service
vfmobile	5646/tcp	0.000000	# Ventureforth Mobile
unknown	5648/udp	0.000661
unknown	5652/udp	0.000330
unknown	5660/udp	0.000330
unknown	5663/udp	0.000330
unknown	5665/tcp	0.000076
nrpe	5666/tcp	0.006614	# Nagios NRPE | Nagios Remote Plugin Executor
unknown	5667/tcp	0.000076
unknown	5667/udp	0.000330
filemq	5670/tcp	0.000000	# zre-disc | ZeroMQ file publish-subscribe protocol | Local area discovery and messaging over ZeroMQ
amqps	5671/tcp	0.000000	# amqp protocol over TLS/SSL
amqps	5671/udp	0.000000	# amqp protocol over TLS/SSL
amqp	5672/sctp	0.000000
amqp	5672/tcp	0.000076
amqp	5672/udp	0.000000
jms	5673/tcp	0.000000	# JACL Message Server
jms	5673/udp	0.000000	# JACL Message Server
hyperscsi-port	5674/tcp	0.000000	# HyperSCSI Port
hyperscsi-port	5674/udp	0.000000	# HyperSCSI Port
v5ua	5675/sctp	0.000000	# V5UA application port
v5ua	5675/tcp	0.000000	# V5UA application port
v5ua	5675/udp	0.000000	# V5UA application port
raadmin	5676/tcp	0.000000	# RA Administration
raadmin	5676/udp	0.000000	# RA Administration
questdb2-lnchr	5677/tcp	0.000000	# Quest Central DB2 Launchr
questdb2-lnchr	5677/udp	0.000000	# Quest Central DB2 Launchr
rrac	5678/tcp	0.000228	# Remote Replication Agent Connection
rrac	5678/udp	0.000000	# Remote Replication Agent Connection
activesync	5679/tcp	0.000590	# dccm | Microsoft ActiveSync PDY synchronization | Direct Cable Connect Manager
dccm	5679/udp	0.000000	# Direct Cable Connect Manager
canna	5680/tcp	0.000151	# auriga-router | Canna (Japanese Input) | Auriga Router Service
auriga-router	5680/udp	0.000000	# Auriga Router Service
ncxcp	5681/tcp	0.000000	# Net-coneX Control Protocol
ncxcp	5681/udp	0.000000	# Net-coneX Control Protocol
brightcore	5682/tcp	0.000000	# BrightCore control & data transfer exchange
brightcore	5682/udp	0.000330	# BrightCore control & data transfer exchange
coap	5683/tcp	0.000000	# Constrained Application Protocol | Constrained Application Protocol (CoAP)
coap	5683/udp	0.000330	# Constrained Application Protocol
coaps	5684/tcp	0.000000	# DTLS-secured CoAP | Constrained Application Protocol (CoAP)
coaps	5684/udp	0.000330	# DTLS-secured Constrained Application Protocol
gog-multiplayer	5687/tcp	0.000000	# GOG multiplayer game protocol
ggz	5688/tcp	0.000000	# GGZ Gaming Zone
ggz	5688/udp	0.000000	# GGZ Gaming Zone
qmvideo	5689/tcp	0.000000	# QM video network management protocol
qmvideo	5689/udp	0.000330	# QM video network management protocol
rbsystem	5693/tcp	0.000000	# Robert Bosch Data Transfer
unknown	5693/udp	0.000330
kmip	5696/tcp	0.000000	# Key Management Interoperability Protocol
unknown	5699/udp	0.000330
supportassist	5700/tcp	0.000000	# Dell SupportAssist data center management
unknown	5704/udp	0.000661
storageos	5705/tcp	0.000000	# StorageOS REST API
unknown	5709/udp	0.000330
unknown	5711/tcp	0.000076
proshareaudio	5713/tcp	0.000013	# proshare conf audio
proshareaudio	5713/udp	0.000511	# proshare conf audio
prosharevideo	5714/tcp	0.000013	# proshare conf video
prosharevideo	5714/udp	0.000297	# proshare conf video
prosharedata	5715/tcp	0.000000	# proshare conf data
prosharedata	5715/udp	0.000395	# proshare conf data
prosharerequest	5716/tcp	0.000000	# proshare conf request
prosharerequest	5716/udp	0.000445	# proshare conf request
prosharenotify	5717/tcp	0.000013	# proshare conf notify
prosharenotify	5717/udp	0.000593	# proshare conf notify
dpm	5718/tcp	0.000380	# DPM Communication Server
dpm	5718/udp	0.000330	# DPM Communication Server
dpm-agent	5719/tcp	0.000000	# DPM Agent Coordinator
dpm-agent	5719/udp	0.000000	# DPM Agent Coordinator
ms-licensing	5720/tcp	0.000000
ms-licensing	5720/udp	0.000000
dtpt	5721/tcp	0.000076	# Desktop Passthru Service
dtpt	5721/udp	0.000000	# Desktop Passthru Service
msdfsr	5722/tcp	0.000076	# Microsoft DFS Replication Service
msdfsr	5722/udp	0.000000	# Microsoft DFS Replication Service
omhs	5723/tcp	0.000076	# Operations Manager - Health Service
omhs	5723/udp	0.000000	# Operations Manager - Health Service
omsdk	5724/tcp	0.000000	# Operations Manager - SDK Service
omsdk	5724/udp	0.000000	# Operations Manager - SDK Service
ms-ilm	5725/tcp	0.000000	# Microsoft Identity Lifecycle Manager
ms-ilm-sts	5726/tcp	0.000000	# Microsoft Lifecycle Manager Secure Token Service
asgenf	5727/tcp	0.000000	# ASG Event Notification Framework
io-dist-data	5728/tcp	0.000000	# io-dist-group | Dist. I/O Comm. Service Data and Control | Dist. I/O Comm. Service Group Membership
io-dist-group	5728/udp	0.000000	# Dist. I/O Comm. Service Group Membership
openmail	5729/tcp	0.000000	# Openmail User Agent Layer
openmail	5729/udp	0.000000	# Openmail User Agent Layer
unieng	5730/tcp	0.000228	# Steltor's calendar access
unieng	5730/udp	0.000000	# Steltor's calendar access
unknown	5732/tcp	0.000076
unknown	5734/tcp	0.000076
unknown	5737/tcp	0.000076
ida-discover1	5741/tcp	0.000000	# IDA Discover Port 1
ida-discover1	5741/udp	0.000000	# IDA Discover Port 1
ida-discover2	5742/tcp	0.000000	# IDA Discover Port 2
ida-discover2	5742/udp	0.000000	# IDA Discover Port 2
watchdoc-pod	5743/tcp	0.000000	# Watchdoc NetPOD Protocol
watchdoc-pod	5743/udp	0.000000	# Watchdoc NetPOD Protocol
watchdoc	5744/tcp	0.000000	# Watchdoc Server
watchdoc	5744/udp	0.000000	# Watchdoc Server
fcopy-server	5745/tcp	0.000000
fcopy-server	5745/udp	0.000000
fcopys-server	5746/tcp	0.000000
fcopys-server	5746/udp	0.000000
tunatic	5747/tcp	0.000000	# Wildbits Tunatic
tunatic	5747/udp	0.000000	# Wildbits Tunatic
tunalyzer	5748/tcp	0.000000	# Wildbits Tunalyzer
tunalyzer	5748/udp	0.000000	# Wildbits Tunalyzer
unknown	5749/udp	0.000661
rscd	5750/tcp	0.000000	# Bladelogic Agent Service
rscd	5750/udp	0.000000	# Bladelogic Agent Service
unknown	5753/udp	0.000330
openmailg	5755/tcp	0.000000	# OpenMail Desk Gateway server
openmailg	5755/udp	0.000000	# OpenMail Desk Gateway server
unknown	5756/udp	0.000330
x500ms	5757/tcp	0.000000	# OpenMail X.500 Directory Server
x500ms	5757/udp	0.000000	# OpenMail X.500 Directory Server
unknown	5758/udp	0.000330
unknown	5764/udp	0.000330
openmailns	5766/tcp	0.000000	# OpenMail NewMail Server
openmailns	5766/udp	0.000000	# OpenMail NewMail Server
s-openmail	5767/tcp	0.000000	# OpenMail Suer Agent Layer (Secure)
s-openmail	5767/udp	0.000000	# OpenMail Suer Agent Layer (Secure)
openmailpxy	5768/tcp	0.000000	# OpenMail CMTS Server
openmailpxy	5768/udp	0.000000	# OpenMail CMTS Server
spramsca	5769/tcp	0.000000	# x509solutions Internal CA
spramsca	5769/udp	0.000000	# x509solutions Internal CA
spramsd	5770/tcp	0.000000	# x509solutions Secure Data
spramsd	5770/udp	0.000330	# x509solutions Secure Data
netagent	5771/tcp	0.000000
netagent	5771/udp	0.000000
dali-port	5777/tcp	0.000000	# starfield-io | DALI Port | Control commands and responses
dali-port	5777/udp	0.000000	# DALI Port
vts-rpc	5780/tcp	0.000000	# Visual Tag System RPC
3par-evts	5781/tcp	0.000000	# 3PAR Event Reporting Service
3par-evts	5781/udp	0.000000	# 3PAR Event Reporting Service
3par-mgmt	5782/tcp	0.000000	# 3PAR Management Service
3par-mgmt	5782/udp	0.000000	# 3PAR Management Service
3par-mgmt-ssl	5783/tcp	0.000000	# 3PAR Management Service with SSL
3par-mgmt-ssl	5783/udp	0.000000	# 3PAR Management Service with SSL
ibar	5784/tcp	0.000000	# Cisco Interbox Application Redundancy
ibar	5784/udp	0.000000	# Cisco Interbox Application Redundancy
3par-rcopy	5785/tcp	0.000000	# 3PAR Inform Remote Copy
3par-rcopy	5785/udp	0.000000	# 3PAR Inform Remote Copy
cisco-redu	5786/tcp	0.000000	# redundancy notification
cisco-redu	5786/udp	0.000000	# redundancy notification
waascluster	5787/tcp	0.000000	# Cisco WAAS Cluster Protocol
xtreamx	5793/tcp	0.000000	# XtreamX Supervised Peer message
xtreamx	5793/udp	0.000330	# XtreamX Supervised Peer message
spdp	5794/tcp	0.000000	# Simple Peered Discovery Protocol
spdp	5794/udp	0.000330	# Simple Peered Discovery Protocol
enlabel-dpl	5798/tcp	0.000000	# Proprietary Website deployment service
vnc-http	5800/tcp	0.005947	# Virtual Network Computer HTTP Access, display 0
unknown	5800/udp	0.000330
vnc-http-1	5801/tcp	0.000841	# Virtual Network Computer HTTP Access, display 1
vnc-http-2	5802/tcp	0.000276	# Virtual Network Computer HTTP Access, display 2
vnc-http-3	5803/tcp	0.000125	# Virtual Network Computer HTTP Access, display 3
unknown	5804/tcp	0.000076
unknown	5804/udp	0.000330
unknown	5806/tcp	0.000076
unknown	5806/udp	0.000330
unknown	5807/tcp	0.000152
unknown	5808/tcp	0.000076
unknown	5810/tcp	0.000380
unknown	5810/udp	0.000330
unknown	5811/tcp	0.000228
unknown	5811/udp	0.000330
unknown	5812/tcp	0.000152
unknown	5812/udp	0.000330
icmpd	5813/tcp	0.000000
icmpd	5813/udp	0.000000
spt-automation	5814/tcp	0.000076	# Support Automation
spt-automation	5814/udp	0.000000	# Support Automation
unknown	5815/tcp	0.000228
unknown	5815/udp	0.000330
unknown	5817/tcp	0.000076
unknown	5817/udp	0.000661
unknown	5818/tcp	0.000152
unknown	5819/udp	0.000330
autopassdaemon	5820/tcp	0.000076	# AutoPass licensing
unknown	5821/tcp	0.000076
unknown	5822/tcp	0.000304
unknown	5823/tcp	0.000152
unknown	5824/tcp	0.000076
unknown	5825/tcp	0.000380
unknown	5826/tcp	0.000076
unknown	5827/tcp	0.000076
unknown	5831/tcp	0.000076
unknown	5834/tcp	0.000076
unknown	5836/tcp	0.000076
unknown	5838/tcp	0.000076
unknown	5839/tcp	0.000076
unknown	5840/tcp	0.000076
shiprush-d-ch	5841/tcp	0.000000	# Z-firm ShipRush interface for web access and bidirectional data
unknown	5841/udp	0.000330
reversion	5842/tcp	0.000000	# Reversion Backup/Restore
unknown	5845/tcp	0.000076
unknown	5848/tcp	0.000076
unknown	5849/tcp	0.000076
unknown	5850/tcp	0.000228
unknown	5851/udp	0.000330
unknown	5852/tcp	0.000076
unknown	5853/tcp	0.000076
unknown	5854/tcp	0.000076
unknown	5858/tcp	0.000076
wherehoo	5859/tcp	0.000304
wherehoo	5859/udp	0.000000
unknown	5860/tcp	0.000076
unknown	5862/tcp	0.000228
ppsuitemsg	5863/tcp	0.000000	# PlanetPress Suite Messeng
ppsuitemsg	5863/udp	0.000000	# PlanetPress Suite Messeng
unknown	5864/udp	0.000330
unknown	5865/udp	0.000330
diameters	5868/tcp	0.000152	# Diameter over TLS/TCP | Diameter over DTLS/SCTP
unknown	5869/tcp	0.000152
unknown	5869/udp	0.000330
unknown	5871/tcp	0.000076
unknown	5873/udp	0.000661
unknown	5874/tcp	0.000076
unknown	5875/tcp	0.000076
unknown	5877/tcp	0.000380
unknown	5878/tcp	0.000076
unknown	5881/tcp	0.000076
unknown	5882/udp	0.000330
jute	5883/tcp	0.000000	# Javascript Unit Test Environment
unknown	5883/udp	0.000330
unknown	5887/tcp	0.000076
unknown	5888/tcp	0.000076
unknown	5899/tcp	0.000152
vnc	5900/tcp	0.023560	# rfb | Virtual Network Computer display 0 | Remote Framebuffer
rfb	5900/udp	0.000661	# Remote Framebuffer
vnc-1	5901/tcp	0.002145	# Virtual Network Computer display 1
vnc-2	5902/tcp	0.000715	# Virtual Network Computer display 2
unknown	5902/udp	0.000330
vnc-3	5903/tcp	0.000326	# ff-ice | Virtual Network Computer display 3 | Flight & Flow Info for Collaborative Env
ag-swim	5904/tcp	0.000304	# Air-Ground SWIM
asmgcs	5905/tcp	0.000152	# Adv Surface Mvmnt and Guidance Cont Sys
unknown	5905/udp	0.000330
rpas-c2	5906/tcp	0.000228	# Remotely Piloted Vehicle C&C
unknown	5906/udp	0.000330
dsd	5907/tcp	0.000228	# Distress and Safety Data App
ipsma	5908/tcp	0.000076	# IPS Management Application
unknown	5908/udp	0.000330
agma	5909/tcp	0.000152	# Air-ground media advisory
cm	5910/tcp	0.000380	# ats-atn | Context Management | Air Traffic Services applications using ATN
cm	5910/udp	0.000000	# Context Management
cpdlc	5911/tcp	0.000380	# ats-acars | Controller Pilot Data Link Communication | Air Traffic Services applications using ACARS
cpdlc	5911/udp	0.000000	# Controller Pilot Data Link Communication
fis	5912/tcp	0.000076	# ais-met | Flight Information Services | Aeronautical Information Service/Meteorological applications using ACARS
fis	5912/udp	0.000000	# Flight Information Services
ads-c	5913/tcp	0.000000	# aoc-acars | Automatic Dependent Surveillance | Airline operational communications applications using ACARS
ads-c	5913/udp	0.000000	# Automatic Dependent Surveillance
unknown	5914/tcp	0.000152
unknown	5915/tcp	0.000304
unknown	5915/udp	0.000330
unknown	5917/tcp	0.000076
unknown	5918/tcp	0.000152
unknown	5920/tcp	0.000076
unknown	5921/tcp	0.000076
unknown	5921/udp	0.000330
unknown	5922/tcp	0.000304
unknown	5923/tcp	0.000076
unknown	5924/tcp	0.000076
unknown	5925/tcp	0.000380
unknown	5926/tcp	0.000076
unknown	5927/tcp	0.000076
unknown	5930/udp	0.000330
unknown	5931/tcp	0.000076
unknown	5934/tcp	0.000076
unknown	5936/tcp	0.000076
teamviewer	5938/tcp	0.000152	# teamviewer - http://www.teamviewer.com/en/help/334-Which-ports-are-used-by-TeamViewer.aspx
unknown	5939/tcp	0.000076
unknown	5940/tcp	0.000152
unknown	5945/tcp	0.000076
unknown	5946/udp	0.000330
unknown	5948/tcp	0.000076
unknown	5949/tcp	0.000076
unknown	5950/tcp	0.000228
unknown	5952/tcp	0.000228
unknown	5953/tcp	0.000076
unknown	5953/udp	0.000330
unknown	5954/tcp	0.000076
unknown	5958/tcp	0.000076
unknown	5959/tcp	0.000380
unknown	5960/tcp	0.000380
unknown	5961/tcp	0.000380
unknown	5962/tcp	0.000380
indy	5963/tcp	0.000304	# Indy Application Server
indy	5963/udp	0.000000	# Indy Application Server
unknown	5964/udp	0.000330
unknown	5966/tcp	0.000076
mppolicy-v5	5968/tcp	0.000152
mppolicy-v5	5968/udp	0.000000
mppolicy-mgr	5969/tcp	0.000076
mppolicy-mgr	5969/udp	0.000000
unknown	5971/tcp	0.000076
unknown	5974/tcp	0.000076
unknown	5975/tcp	0.000076
unknown	5976/udp	0.000330
ncd-pref-tcp	5977/tcp	0.000075	# NCD preferences tcp port
ncd-diag-tcp	5978/tcp	0.000050	# NCD diagnostic tcp port
ncd-conf-tcp	5979/tcp	0.000000	# NCD configuration tcp port
unknown	5981/tcp	0.000152
unknown	5981/udp	0.000330
couchdb	5984/tcp	0.000000
couchdb	5984/udp	0.000000
wsman	5985/tcp	0.000380	# WBEM WS-Management HTTP
wsman	5985/udp	0.000000	# WBEM WS-Management HTTP
wsmans	5986/tcp	0.000380	# WBEM WS-Management HTTP over TLS/SSL
wsmans	5986/udp	0.000000	# WBEM WS-Management HTTP over TLS/SSL
wbem-rmi	5987/tcp	0.000380	# WBEM RMI
wbem-rmi	5987/udp	0.000000	# WBEM RMI
wbem-http	5988/tcp	0.000380	# WBEM CIM-XML (HTTP)
wbem-http	5988/udp	0.000000	# WBEM CIM-XML (HTTP)
wbem-https	5989/tcp	0.000380	# WBEM CIM-XML (HTTPS)
wbem-https	5989/udp	0.000000	# WBEM CIM-XML (HTTPS)
wbem-exp-https	5990/tcp	0.000000	# WBEM Export HTTPS
wbem-exp-https	5990/udp	0.000000	# WBEM Export HTTPS
nuxsl	5991/tcp	0.000000
nuxsl	5991/udp	0.000000
consul-insight	5992/tcp	0.000000	# Consul InSight Security
consul-insight	5992/udp	0.000000	# Consul InSight Security
cim-rs	5993/tcp	0.000000	# DMTF WBEM CIM REST
rms-agent	5994/tcp	0.000000	# RMS Agent Listening Service
unknown	5994/udp	0.000330
ncd-pref	5997/tcp	0.000025	# NCD preferences telnet port
ncd-diag	5998/tcp	0.000163	# NCD diagnostic telnet port
ncd-conf	5999/tcp	0.000213	# cvsup | NCD configuration telnet port | CVSup
cvsup	5999/udp	0.000000
X11	6000/tcp	0.005683	# X Window server
X11	6000/udp	0.003304
X11:1	6001/tcp	0.011730	# X Window server
X11:1	6001/udp	0.004625
X11:2	6002/tcp	0.001518	# X Window server
X11:2	6002/udp	0.001652
X11:3	6003/tcp	0.000351	# X Window server
X11:3	6003/udp	0.000000
X11:4	6004/tcp	0.002597	# X Window server
X11:4	6004/udp	0.002973
X11:5	6005/tcp	0.000602	# X Window server
X11:5	6005/udp	0.000000
X11:6	6006/tcp	0.000188	# X Window server
X11:6	6006/udp	0.000000
X11:7	6007/tcp	0.000238	# X Window server
X11:7	6007/udp	0.000000
X11:8	6008/tcp	0.000125	# X Window server
X11:8	6008/udp	0.000000
X11:9	6009/tcp	0.000201	# X Window server
X11:9	6009/udp	0.000000
x11	6010/tcp	0.000076	# X Window System
x11	6010/udp	0.000000	# X Window System
x11	6011/tcp	0.000000	# X Window System
x11	6011/udp	0.000000	# X Window System
x11	6012/tcp	0.000000	# X Window System
x11	6012/udp	0.000000	# X Window System
x11	6013/tcp	0.000000	# X Window System
x11	6013/udp	0.000000	# X Window System
x11	6014/tcp	0.000000	# X Window System
x11	6014/udp	0.000000	# X Window System
x11	6015/tcp	0.000076	# X Window System
x11	6015/udp	0.000000	# X Window System
x11	6016/tcp	0.000000	# X Window System
x11	6016/udp	0.000000	# X Window System
xmail-ctrl	6017/tcp	0.000088	# XMail CTRL server
x11	6017/udp	0.000330	# X Window System
x11	6018/tcp	0.000000	# X Window System
x11	6018/udp	0.000000	# X Window System
x11	6019/tcp	0.000000	# X Window System
x11	6019/udp	0.000000	# X Window System
x11	6020/tcp	0.000000	# X Window System
x11	6020/udp	0.000330	# X Window System
x11	6021/tcp	0.000076	# X Window System
x11	6021/udp	0.000000	# X Window System
x11	6022/tcp	0.000000	# X Window System
x11	6022/udp	0.000330	# X Window System
x11	6023/tcp	0.000000	# X Window System
x11	6023/udp	0.000000	# X Window System
x11	6024/tcp	0.000000	# X Window System
x11	6024/udp	0.000000	# X Window System
x11	6025/tcp	0.000228	# X Window System
x11	6025/udp	0.000000	# X Window System
x11	6026/tcp	0.000000	# X Window System
x11	6026/udp	0.000330	# X Window System
x11	6027/tcp	0.000000	# X Window System
x11	6027/udp	0.000000	# X Window System
x11	6028/tcp	0.000000	# X Window System
x11	6028/udp	0.000000	# X Window System
x11	6029/tcp	0.000000	# X Window System
x11	6029/udp	0.000000	# X Window System
x11	6030/tcp	0.000076	# X Window System
x11	6030/udp	0.000330	# X Window System
x11	6031/tcp	0.000000	# X Window System
x11	6031/udp	0.000000	# X Window System
x11	6032/tcp	0.000000	# X Window System
x11	6032/udp	0.000000	# X Window System
x11	6033/tcp	0.000000	# X Window System
x11	6033/udp	0.000661	# X Window System
x11	6034/tcp	0.000000	# X Window System
x11	6034/udp	0.000000	# X Window System
x11	6035/tcp	0.000000	# X Window System
x11	6035/udp	0.000000	# X Window System
x11	6036/tcp	0.000000	# X Window System
x11	6036/udp	0.000000	# X Window System
x11	6037/tcp	0.000000	# X Window System
x11	6037/udp	0.000000	# X Window System
x11	6038/tcp	0.000000	# X Window System
x11	6038/udp	0.000330	# X Window System
x11	6039/tcp	0.000000	# X Window System
x11	6039/udp	0.000000	# X Window System
x11	6040/tcp	0.000000	# X Window System
x11	6040/udp	0.000000	# X Window System
x11	6041/tcp	0.000000	# X Window System
x11	6041/udp	0.000000	# X Window System
x11	6042/tcp	0.000000	# X Window System
x11	6042/udp	0.000330	# X Window System
x11	6043/tcp	0.000000	# X Window System
x11	6043/udp	0.000000	# X Window System
x11	6044/tcp	0.000000	# X Window System
x11	6044/udp	0.000000	# X Window System
x11	6045/tcp	0.000000	# X Window System
x11	6045/udp	0.000000	# X Window System
x11	6046/tcp	0.000000	# X Window System
x11	6046/udp	0.000000	# X Window System
x11	6047/tcp	0.000000	# X Window System
x11	6047/udp	0.000000	# X Window System
x11	6048/tcp	0.000000	# X Window System
x11	6048/udp	0.000330	# X Window System
x11	6049/tcp	0.000000	# X Window System
x11	6049/udp	0.000000	# X Window System
arcserve	6050/tcp	0.000100	# ARCserve agent
x11	6050/udp	0.001652	# X Window System
x11	6051/tcp	0.000152	# X Window System
x11	6051/udp	0.000000	# X Window System
x11	6052/tcp	0.000076	# X Window System
x11	6052/udp	0.000000	# X Window System
x11	6053/tcp	0.000000	# X Window System
x11	6053/udp	0.000000	# X Window System
x11	6054/tcp	0.000000	# X Window System
x11	6054/udp	0.000000	# X Window System
x11	6055/tcp	0.000076	# X Window System
x11	6055/udp	0.000000	# X Window System
x11	6056/tcp	0.000000	# X Window System
x11	6056/udp	0.000000	# X Window System
x11	6057/tcp	0.000000	# X Window System
x11	6057/udp	0.000330	# X Window System
x11	6058/tcp	0.000000	# X Window System
x11	6058/udp	0.000000	# X Window System
X11:59	6059/tcp	0.000760	# X Window server
X11:59	6059/udp	0.000000
x11	6060/tcp	0.000152	# X Window System
x11	6060/udp	0.000000	# X Window System
x11	6061/tcp	0.000000	# X Window System
x11	6061/udp	0.000330	# X Window System
x11	6062/tcp	0.000076	# X Window System
x11	6062/udp	0.000330	# X Window System
x11	6063/tcp	0.000076	# X Window System
x11	6063/udp	0.000000	# X Window System
ndl-ahp-svc	6064/tcp	0.000000
ndl-ahp-svc	6064/udp	0.000000
winpharaoh	6065/tcp	0.000076
winpharaoh	6065/udp	0.000000
ewctsp	6066/tcp	0.000000
ewctsp	6066/udp	0.000000
unknown	6067/tcp	0.000076
gsmp	6068/tcp	0.000152	# gsmp-ancp | GSMP/ANCP
gsmp	6068/udp	0.000000
trip	6069/tcp	0.000000
trip	6069/udp	0.000000
messageasap	6070/tcp	0.000000
messageasap	6070/udp	0.000000
ssdtp	6071/tcp	0.000000
ssdtp	6071/udp	0.000000
diagnose-proc	6072/tcp	0.000000
diagnose-proc	6072/udp	0.000330
directplay8	6073/tcp	0.000000
directplay8	6073/udp	0.000000
max	6074/tcp	0.000000	# Microsoft Max
max	6074/udp	0.000000	# Microsoft Max
dpm-acm	6075/tcp	0.000000	# Microsoft DPM Access Control Manager
msft-dpm-cert	6076/tcp	0.000000	# Microsoft DPM WCF Certificates
iconstructsrv	6077/tcp	0.000076	# iConstruct Server
unknown	6077/udp	0.000330
unknown	6078/udp	0.000330
gue	6080/tcp	0.000000	# Generic UDP Encapsulation
geneve	6081/tcp	0.000000	# Generic Network Virtualization Encapsulation (Geneve)
p25cai	6082/tcp	0.000000	# APCO Project 25 Common Air Interface - UDP encapsulation
miami-bcast	6083/tcp	0.000000	# telecomsoftware miami broadcast
p2p-sip	6084/tcp	0.000000	# reload-config | Peer to Peer Infrastructure Protocol | Peer to Peer Infrastructure Configuration
konspire2b	6085/tcp	0.000076	# konspire2b p2p network
konspire2b	6085/udp	0.000000	# konspire2b p2p network
pdtp	6086/tcp	0.000000	# PDTP P2P
pdtp	6086/udp	0.000330	# PDTP P2P
ldss	6087/tcp	0.000000	# Local Download Sharing Service
ldss	6087/udp	0.000000	# Local Download Sharing Service
doglms	6088/tcp	0.000000	# doglms-notify | SuperDog License Manager | SuperDog License Manager Notifier
unknown	6090/tcp	0.000076
unknown	6090/udp	0.000330
unknown	6091/tcp	0.000076
unknown	6095/udp	0.000330
raxa-mgmt	6099/tcp	0.000000	# RAXA Management
synchronet-db	6100/tcp	0.000228
synchronet-db	6100/udp	0.000330
backupexec	6101/tcp	0.000452	# synchronet-rtc | Backup Exec UNIX and 95/98/ME Aent | SynchroNet-rtc
synchronet-rtc	6101/udp	0.000000
synchronet-upd	6102/tcp	0.000000
synchronet-upd	6102/udp	0.000000
RETS-or-BackupExec	6103/tcp	0.000125	# rets | Backup Exec Agent Accelerator and Remote Agent also sql server and cisco works blue | RETS
rets	6103/udp	0.000000
dbdb	6104/tcp	0.000000
dbdb	6104/udp	0.000330
isdninfo	6105/tcp	0.000075	# primaserver | Prima Server
primaserver	6105/udp	0.000661	# Prima Server
isdninfo	6106/tcp	0.000314	# mpsserver | i4lmond | MPS Server
mpsserver	6106/udp	0.000000	# MPS Server
etc-control	6107/tcp	0.000000	# ETC Control
etc-control	6107/udp	0.000000	# ETC Control
sercomm-scadmin	6108/tcp	0.000000
sercomm-scadmin	6108/udp	0.000000
globecast-id	6109/tcp	0.000000
globecast-id	6109/udp	0.000000
softcm	6110/tcp	0.000063	# HP SoftBench CM
softcm	6110/udp	0.000824	# HP SoftBench CM
spc	6111/tcp	0.000025	# HP SoftBench Sub-Process Control
spc	6111/udp	0.001203	# HP SoftBench Sub-Process Control
dtspc	6112/tcp	0.001656	# dtspcd | CDE subprocess control | Desk-Top Sub-Process Control Daemon
dtspcd	6112/udp	0.000000	# Desk-Top Sub-Process Control Daemon
dayliteserver	6113/tcp	0.000076	# Daylite Server
unknown	6113/udp	0.000330
wrspice	6114/tcp	0.000000	# WRspice IPC Service
xic	6115/tcp	0.000076	# Xic IPC Service
xtlserv	6116/tcp	0.000000	# XicTools License Manager Service
daylitetouch	6117/tcp	0.000000	# Daylite Touch Sync
unknown	6117/udp	0.000330
tipc	6118/tcp	0.000000	# Transparent Inter Process Communication
unknown	6119/udp	0.000661
unknown	6120/tcp	0.000076
spdy	6121/tcp	0.000000	# SPDY for a faster web
bex-webadmin	6122/tcp	0.000000	# Backup Express Web Server
bex-webadmin	6122/udp	0.000330	# Backup Express Web Server
backup-express	6123/tcp	0.000380	# Backup Express
backup-express	6123/udp	0.000330	# Backup Express
pnbs	6124/tcp	0.000000	# Phlexible Network Backup Service
pnbs	6124/udp	0.000000	# Phlexible Network Backup Service
unknown	6125/udp	0.000330
unknown	6126/tcp	0.000076
unknown	6128/udp	0.000330
unknown	6129/tcp	0.000380
damewaremobgtwy	6130/tcp	0.000000	# The DameWare Mobile Gateway Service
nbt-wol	6133/tcp	0.000000	# New Boundary Tech WOL
nbt-wol	6133/udp	0.000000	# New Boundary Tech WOL
pulsonixnls	6140/tcp	0.000000	# Pulsonix Network License Service
pulsonixnls	6140/udp	0.000000	# Pulsonix Network License Service
meta-corp	6141/tcp	0.000013	# Meta Corporation License Manager
meta-corp	6141/udp	0.000577	# Meta Corporation License Manager
aspentec-lm	6142/tcp	0.000025	# Aspen Technology License Manager
aspentec-lm	6142/udp	0.000527	# Aspen Technology License Manager
watershed-lm	6143/tcp	0.000038	# Watershed License Manager
watershed-lm	6143/udp	0.000643	# Watershed License Manager
statsci1-lm	6144/tcp	0.000000	# StatSci License Manager - 1
statsci1-lm	6144/udp	0.000923	# StatSci License Manager - 1
statsci2-lm	6145/tcp	0.000025	# StatSci License Manager - 2
statsci2-lm	6145/udp	0.000807	# StatSci License Manager - 2
lonewolf-lm	6146/tcp	0.000025	# Lone Wolf Systems License Manager
lonewolf-lm	6146/udp	0.001071	# Lone Wolf Systems License Manager
montage-lm	6147/tcp	0.000025	# Montage License Manager
montage-lm	6147/udp	0.000774	# Montage License Manager
ricardo-lm	6148/tcp	0.000000	# Ricardo North America License Manager
ricardo-lm	6148/udp	0.000643	# Ricardo North America License Manager
tal-pod	6149/tcp	0.000000
tal-pod	6149/udp	0.000000
unknown	6156/tcp	0.000380
unknown	6158/udp	0.000330
efb-aci	6159/tcp	0.000000	# EFB Application Control Interface
ecmp	6160/tcp	0.000000	# ecmp-data | Emerson Extensible Control and Management Protocol | Emerson Extensible Control and Management Protocol Data
patrol-ism	6161/tcp	0.000076	# PATROL Internet Srv Mgr
patrol-ism	6161/udp	0.000000	# PATROL Internet Srv Mgr
patrol-coll	6162/tcp	0.000000	# PATROL Collector
patrol-coll	6162/udp	0.000000	# PATROL Collector
pscribe	6163/tcp	0.000000	# Precision Scribe Cnx Port
pscribe	6163/udp	0.000000	# Precision Scribe Cnx Port
unknown	6169/udp	0.000330
unknown	6170/udp	0.000330
unknown	6171/udp	0.000330
unknown	6189/udp	0.000330
unknown	6197/udp	0.000330
lm-x	6200/tcp	0.000000	# LM-X License Manager by X-Formation
lm-x	6200/udp	0.000000	# LM-X License Manager by X-Formation
thermo-calc	6201/tcp	0.000000	# Management of service nodes in a processing grid for thermodynamic calculations
unknown	6201/udp	0.000330
unknown	6203/tcp	0.000152
unknown	6203/udp	0.000330
unknown	6204/udp	0.000330
qmtps	6209/tcp	0.000000	# QMTP over TLS
unknown	6211/udp	0.000330
unknown	6212/udp	0.000661
radmind	6222/tcp	0.000151	# Radmind protocol | Radmind Access Protocol
radmind	6222/udp	0.000000	# Radmind Access Protocol
unknown	6226/udp	0.000330
unknown	6237/udp	0.000661
unknown	6238/udp	0.000330
jeol-nsdtp-1	6241/tcp	0.000000	# jeol-nsddp-1 | JEOL Network Services Data Transport Protocol 1 | JEOL Network Services Dynamic Discovery Protocol 1
jeol-nsddp-1	6241/udp	0.000000	# JEOL Network Services Dynamic Discovery Protocol 1
jeol-nsdtp-2	6242/tcp	0.000000	# jeol-nsddp-2 | JEOL Network Services Data Transport Protocol 2 | JEOL Network Services Dynamic Discovery Protocol 2
jeol-nsddp-2	6242/udp	0.000000	# JEOL Network Services Dynamic Discovery Protocol 2
jeol-nsdtp-3	6243/tcp	0.000000	# jeol-nsddp-3 | JEOL Network Services Data Transport Protocol 3 | JEOL Network Services Dynamic Discovery Protocol 3
jeol-nsddp-3	6243/udp	0.000330	# JEOL Network Services Dynamic Discovery Protocol 3
jeol-nsdtp-4	6244/tcp	0.000000	# jeol-nsddp-4 | JEOL Network Services Data Transport Protocol 4 | JEOL Network Services Dynamic Discovery Protocol 4
jeol-nsddp-4	6244/udp	0.000330	# JEOL Network Services Dynamic Discovery Protocol 4
unknown	6247/tcp	0.000152
unknown	6247/udp	0.000330
unknown	6250/tcp	0.000076
unknown	6250/udp	0.000661
tl1-raw-ssl	6251/tcp	0.000076	# TL1 Raw Over SSL/TLS
tl1-raw-ssl	6251/udp	0.000000	# TL1 Raw Over SSL/TLS
tl1-ssh	6252/tcp	0.000000	# TL1 over SSH
tl1-ssh	6252/udp	0.000000	# TL1 over SSH
crip	6253/tcp	0.000000
crip	6253/udp	0.000000
unknown	6256/udp	0.000330
unknown	6259/tcp	0.000076
gld	6267/tcp	0.000000	# GridLAB-D User Interface
grid	6268/tcp	0.000000	# Grid Authentication
grid	6268/udp	0.000000	# Grid Authentication
grid-alt	6269/tcp	0.000000	# Grid Authentication Alt
grid-alt	6269/udp	0.000000	# Grid Authentication Alt
unknown	6273/tcp	0.000076
unknown	6274/tcp	0.000076
unknown	6275/udp	0.000330
unknown	6277/udp	0.000330
unknown	6284/udp	0.000330
unknown	6297/udp	0.000330
unknown	6299/udp	0.000330
bmc-grx	6300/tcp	0.000000	# BMC GRX
bmc-grx	6300/udp	0.000000	# BMC GRX
bmc_ctd_ldap	6301/tcp	0.000000	# bmc-ctd-ldap | BMC CONTROL-D LDAP SERVER
bmc_ctd_ldap	6301/udp	0.000000	# BMC CONTROL-D LDAP SERVER
ufmp	6306/tcp	0.000000	# Unified Fabric Management Protocol
ufmp	6306/udp	0.000330	# Unified Fabric Management Protocol
unknown	6309/tcp	0.000076
unknown	6310/tcp	0.000076
scup	6315/tcp	0.000000	# scup-disc | Sensor Control Unit Protocol | Sensor Control Unit Protocol Discovery Protocol
scup-disc	6315/udp	0.000000	# Sensor Control Unit Protocol Discovery Protocol
abb-escp	6316/tcp	0.000000	# Ethernet Sensor Communications Protocol
abb-escp	6316/udp	0.000000	# Ethernet Sensor Communications Protocol
nav-data-cmd	6317/tcp	0.000000	# nav-data | Navtech Radar Sensor Data Command | Navtech Radar Sensor Data
unknown	6319/udp	0.000330
repsvc	6320/tcp	0.000000	# Double-Take Replication Service
repsvc	6320/udp	0.000330	# Double-Take Replication Service
emp-server1	6321/tcp	0.000000	# Empress Software Connectivity Server 1
emp-server1	6321/udp	0.000000	# Empress Software Connectivity Server 1
emp-server2	6322/tcp	0.000000	# Empress Software Connectivity Server 2
emp-server2	6322/udp	0.000000	# Empress Software Connectivity Server 2
unknown	6323/tcp	0.000076
hrd-ncs	6324/tcp	0.000076	# hrd-ns-disc | HR Device Network Configuration Service | HR Device Network service
dt-mgmtsvc	6325/tcp	0.000000	# Double-Take Management Service
unknown	6325/udp	0.000330
dt-vra	6326/tcp	0.000000	# Double-Take Virtual Recovery Assistant
unknown	6330/udp	0.000330
unknown	6331/udp	0.000330
sflow	6343/tcp	0.000000	# sFlow traffic monitoring
sflow	6343/udp	0.000000	# sFlow traffic monitoring
streletz	6344/tcp	0.000000	# Argus-Spectr security and fire-prevention systems service
unknown	6344/udp	0.000330
gnutella	6346/tcp	0.000226	# Gnutella file sharing protocol | gnutella-svc
gnutella	6346/udp	0.004893	# Gnutella file sharing protocol
gnutella2	6347/tcp	0.000050	# Gnutella2 file sharing protocol | gnutella-rtr
gnutella2	6347/udp	0.002142	# Gnutella2 file sharing protocol
unknown	6349/tcp	0.000076
unknown	6349/udp	0.000330
adap	6350/tcp	0.000076	# App Discovery and Access Protocol
adap	6350/udp	0.000000	# App Discovery and Access Protocol
unknown	6353/udp	0.000661
pmcs	6355/tcp	0.000000	# PMCS applications
pmcs	6355/udp	0.000000	# PMCS applications
metaedit-mu	6360/tcp	0.000000	# MetaEdit+ Multi-User
metaedit-mu	6360/udp	0.000000	# MetaEdit+ Multi-User
ndn	6363/tcp	0.000000	# Named Data Networking
metaedit-se	6370/tcp	0.000000	# MetaEdit+ Server Administration
metaedit-se	6370/udp	0.000000	# MetaEdit+ Server Administration
unknown	6372/udp	0.000661
redis	6379/tcp	0.000076	# An advanced key-value cache and store
metatude-mds	6382/tcp	0.000000	# Metatude Dialogue Server
metatude-mds	6382/udp	0.000000	# Metatude Dialogue Server
unknown	6386/udp	0.000330
clariion-evr01	6389/tcp	0.000380
clariion-evr01	6389/udp	0.000000
metaedit-ws	6390/tcp	0.000000	# MetaEdit+ WebService API
metaedit-ws	6390/udp	0.000000	# MetaEdit+ WebService API
unknown	6395/udp	0.000661
crystalreports	6400/tcp	0.000025	# boe-cms | Seagate Crystal Reports | Business Objects CMS contact port
boe-cms	6400/udp	0.000000	# Business Objects CMS contact port
crystalenterprise	6401/tcp	0.000050	# Seagate Crystal Enterprise | boe-was
boe-was	6401/udp	0.000000
boe-eventsrv	6402/tcp	0.000000
boe-eventsrv	6402/udp	0.000000
boe-cachesvr	6403/tcp	0.000000
boe-cachesvr	6403/udp	0.000000
boe-filesvr	6404/tcp	0.000000	# Business Objects Enterprise internal server
boe-filesvr	6404/udp	0.000000	# Business Objects Enterprise internal server
boe-pagesvr	6405/tcp	0.000000	# Business Objects Enterprise internal server
boe-pagesvr	6405/udp	0.000330	# Business Objects Enterprise internal server
boe-processsvr	6406/tcp	0.000000	# Business Objects Enterprise internal server
boe-processsvr	6406/udp	0.000330	# Business Objects Enterprise internal server
boe-resssvr1	6407/tcp	0.000000	# Business Objects Enterprise internal server
boe-resssvr1	6407/udp	0.000000	# Business Objects Enterprise internal server
boe-resssvr2	6408/tcp	0.000000	# Business Objects Enterprise internal server
boe-resssvr2	6408/udp	0.000000	# Business Objects Enterprise internal server
boe-resssvr3	6409/tcp	0.000000	# Business Objects Enterprise internal server
boe-resssvr3	6409/udp	0.000000	# Business Objects Enterprise internal server
boe-resssvr4	6410/tcp	0.000000	# Business Objects Enterprise internal server
boe-resssvr4	6410/udp	0.000000	# Business Objects Enterprise internal server
unknown	6411/udp	0.000330
unknown	6412/tcp	0.000076
unknown	6416/udp	0.000330
faxcomservice	6417/tcp	0.000000	# Faxcom Message Service
faxcomservice	6417/udp	0.000000	# Faxcom Message Service
syserverremote	6418/tcp	0.000000	# SYserver remote commands
svdrp	6419/tcp	0.000000	# svdrp-disc | Simple VDR Protocol | Simple VDR Protocol Discovery
nim-vdrshell	6420/tcp	0.000000	# NIM_VDRShell
nim-vdrshell	6420/udp	0.000000	# NIM_VDRShell
nim-wan	6421/tcp	0.000000	# NIM_WAN
nim-wan	6421/udp	0.000000	# NIM_WAN
unknown	6427/udp	0.000330
unknown	6430/udp	0.000991
pgbouncer	6432/tcp	0.000000
unknown	6435/udp	0.000330
heliosd	6440/tcp	0.000000	# heliosd daemon
unknown	6441/udp	0.000330
tarp	6442/tcp	0.000000	# Transitory Application Request Protocol
sun-sr-https	6443/tcp	0.000000	# Service Registry Default HTTPS Domain
sun-sr-https	6443/udp	0.000000	# Service Registry Default HTTPS Domain
sge_qmaster	6444/tcp	0.000000	# sge-qmaster | Grid Engine Qmaster Service
sge_qmaster	6444/udp	0.000330	# Grid Engine Qmaster Service
sge_execd	6445/tcp	0.000000	# sge-execd | Grid Engine Execution Service
sge_execd	6445/udp	0.000000	# Grid Engine Execution Service
mysql-proxy	6446/tcp	0.000000	# MySQL Proxy
mysql-proxy	6446/udp	0.000330	# MySQL Proxy
unknown	6451/udp	0.000661
skip-cert-recv	6455/tcp	0.000000	# SKIP Certificate Receive
skip-cert-send	6456/tcp	0.000000	# SKIP Certificate Send
skip-cert-send	6456/udp	0.000000	# SKIP Certificate Send
unknown	6457/udp	0.000330
unknown	6461/udp	0.000330
unknown	6463/udp	0.000661
ieee11073-20701	6464/tcp	0.000000	# Port assignment for medical device communication in accordance to IEEE 11073-20701
unknown	6467/udp	0.000330
unknown	6468/udp	0.000661
lvision-lm	6471/tcp	0.000000	# LVision License Manager
lvision-lm	6471/udp	0.000000	# LVision License Manager
unknown	6475/udp	0.000330
sun-sr-http	6480/tcp	0.000000	# Service Registry Default HTTP Domain
sun-sr-http	6480/udp	0.000000	# Service Registry Default HTTP Domain
servicetags	6481/tcp	0.000152	# Service Tags
servicetags	6481/udp	0.000000	# Service Tags
ldoms-mgmt	6482/tcp	0.000000	# Logical Domains Management Interface
ldoms-mgmt	6482/udp	0.000000	# Logical Domains Management Interface
SunVTS-RMI	6483/tcp	0.000000	# SunVTS RMI
SunVTS-RMI	6483/udp	0.000000	# SunVTS RMI
sun-sr-jms	6484/tcp	0.000000	# Service Registry Default JMS Domain
sun-sr-jms	6484/udp	0.000000	# Service Registry Default JMS Domain
sun-sr-iiop	6485/tcp	0.000000	# Service Registry Default IIOP Domain
sun-sr-iiop	6485/udp	0.000000	# Service Registry Default IIOP Domain
sun-sr-iiops	6486/tcp	0.000000	# Service Registry Default IIOPS Domain
sun-sr-iiops	6486/udp	0.000000	# Service Registry Default IIOPS Domain
sun-sr-iiop-aut	6487/tcp	0.000000	# Service Registry Default IIOPAuth Domain
sun-sr-iiop-aut	6487/udp	0.000000	# Service Registry Default IIOPAuth Domain
sun-sr-jmx	6488/tcp	0.000000	# Service Registry Default JMX Domain
sun-sr-jmx	6488/udp	0.000330	# Service Registry Default JMX Domain
sun-sr-admin	6489/tcp	0.000000	# Service Registry Default Admin Domain
sun-sr-admin	6489/udp	0.000000	# Service Registry Default Admin Domain
unknown	6491/udp	0.000330
boks	6500/tcp	0.000152	# BoKS Master
boks	6500/udp	0.000330	# BoKS Master
boks_servc	6501/tcp	0.000000	# boks-servc | BoKS Servc
boks_servc	6501/udp	0.000000	# BoKS Servc
netop-rc	6502/tcp	0.000314	# boks_servm | boks-servm | NetOp Remote Control (by Danware Data A/S) | BoKS Servm
netop-rc	6502/udp	0.000741	# NetOp Remote Control (by Danware Data A/S)
boks_clntd	6503/tcp	0.000076	# boks-clntd | BoKS Clntd
boks_clntd	6503/udp	0.000991	# BoKS Clntd
unknown	6504/tcp	0.000152
badm_priv	6505/tcp	0.000000	# badm-priv | BoKS Admin Private Port
badm_priv	6505/udp	0.000000	# BoKS Admin Private Port
badm_pub	6506/tcp	0.000000	# badm-pub | BoKS Admin Public Port
badm_pub	6506/udp	0.000000	# BoKS Admin Public Port
bdir_priv	6507/tcp	0.000000	# bdir-priv | BoKS Dir Server, Private Port
bdir_priv	6507/udp	0.000000	# BoKS Dir Server, Private Port
bdir_pub	6508/tcp	0.000000	# bdir-pub | BoKS Dir Server, Public Port
bdir_pub	6508/udp	0.000000	# BoKS Dir Server, Public Port
mgcs-mfp-port	6509/tcp	0.000000	# MGCS-MFP Port
mgcs-mfp-port	6509/udp	0.000000	# MGCS-MFP Port
mcer-port	6510/tcp	0.000228	# MCER Port
mcer-port	6510/udp	0.000000	# MCER Port
dccp-udp	6511/tcp	0.000000	# Datagram Congestion Control Protocol Encapsulation for NAT Traversal
netconf-tls	6513/tcp	0.000000	# NETCONF over TLS
syslog-tls	6514/tcp	0.000000	# Syslog over TLS | syslog over DTLS
syslog-tls	6514/udp	0.000000	# syslog over DTLS
elipse-rec	6515/tcp	0.000000	# Elipse RPC Protocol
elipse-rec	6515/udp	0.000000	# Elipse RPC Protocol
unknown	6520/tcp	0.000152
unknown	6520/udp	0.000661
unknown	6529/udp	0.000330
unknown	6533/udp	0.000330
unknown	6535/tcp	0.000076
unknown	6535/udp	0.000330
unknown	6538/udp	0.000330
unknown	6540/udp	0.000330
unknown	6542/udp	0.000330
mythtv	6543/tcp	0.001167	# lds-distrib | lds_distrib
lds-distrib	6543/udp	0.000000	# lds_distrib
mythtv	6544/tcp	0.000025	# lds-dump | LDS Dump Service
lds-dump	6544/udp	0.000000	# LDS Dump Service
powerchuteplus	6547/tcp	0.000251	# apc-6547 | APC 6547
apc-6547	6547/udp	0.000000	# APC 6547
powerchuteplus	6548/tcp	0.000013	# apc-6548 | APC 6548
apc-6548	6548/udp	0.000000	# APC 6548
apc-6549	6549/tcp	0.000000	# APC 6549
powerchuteplus	6549/udp	0.000511
fg-sysupdate	6550/tcp	0.000152
fg-sysupdate	6550/udp	0.000330
sum	6551/tcp	0.000000	# Software Update Manager
sum	6551/udp	0.000000	# Software Update Manager
checkmk-agent	6556/tcp	0.000000	# Checkmk Monitoring Agent
xdsxdm	6558/tcp	0.000000
xdsxdm	6558/udp	0.000478
unknown	6565/tcp	0.000228
sane-port	6566/tcp	0.000228	# SANE Control Port
sane-port	6566/udp	0.000000	# SANE Control Port
esp	6567/tcp	0.000228	# eSilo Storage Protocol
esp	6567/udp	0.000000	# eSilo Storage Protocol
canit_store	6568/tcp	0.000000	# rp-reputation | canit-store | CanIt Storage Manager | Roaring Penguin IP Address Reputation Collection
rp-reputation	6568/udp	0.000000	# Roaring Penguin IP Address Reputation Collection
unknown	6572/udp	0.000330
affiliate	6579/tcp	0.000076
affiliate	6579/udp	0.000000
parsec-master	6580/tcp	0.000380	# Parsec Masterserver
parsec-master	6580/udp	0.000000	# Parsec Masterserver
parsec-peer	6581/tcp	0.000000	# Parsec Peer-to-Peer
parsec-peer	6581/udp	0.000000	# Parsec Peer-to-Peer
parsec-game	6582/tcp	0.000000	# Parsec Gameserver
parsec-game	6582/udp	0.000000	# Parsec Gameserver
joaJewelSuite	6583/tcp	0.000000	# JOA Jewel Suite
joaJewelSuite	6583/udp	0.000330	# JOA Jewel Suite
unknown	6584/udp	0.000330
analogx	6588/tcp	0.000038	# AnalogX HTTP proxy port
unknown	6592/udp	0.000330
unknown	6598/udp	0.000330
mshvlm	6600/tcp	0.000152	# Microsoft Hyper-V Live Migration
mstmg-sstp	6601/tcp	0.000000	# Microsoft Threat Management Gateway SSTP
wsscomfrmwk	6602/tcp	0.000000	# Windows WSS Communication Framework
unknown	6606/tcp	0.000076
unknown	6607/udp	0.000330
unknown	6610/udp	0.000330
unknown	6616/udp	0.000330
odette-ftps	6619/tcp	0.000076	# ODETTE-FTP over TLS/SSL
odette-ftps	6619/udp	0.000000	# ODETTE-FTP over TLS/SSL
kftp-data	6620/tcp	0.000000	# Kerberos V5 FTP Data
kftp-data	6620/udp	0.000000	# Kerberos V5 FTP Data
kftp	6621/tcp	0.000000	# Kerberos V5 FTP Control
kftp	6621/udp	0.000000	# Kerberos V5 FTP Control
mcftp	6622/tcp	0.000000	# Multicast FTP
mcftp	6622/udp	0.000000	# Multicast FTP
ktelnet	6623/tcp	0.000000	# Kerberos V5 Telnet
ktelnet	6623/udp	0.000000	# Kerberos V5 Telnet
datascaler-db	6624/tcp	0.000000	# DataScaler database
datascaler-ctl	6625/tcp	0.000000	# DataScaler control
unknown	6625/udp	0.000661
wago-service	6626/tcp	0.000000	# WAGO Service and Update
wago-service	6626/udp	0.000000	# WAGO Service and Update
nexgen	6627/tcp	0.000000	# Allied Electronics NeXGen
nexgen	6627/udp	0.000661	# Allied Electronics NeXGen
afesc-mc	6628/tcp	0.000076	# AFE Stock Channel M/C
afesc-mc	6628/udp	0.000000	# AFE Stock Channel M/C
nexgen-aux	6629/tcp	0.000000	# Secondary, (non ANDI) multi-protocol multi-function interface to the Allied ANDI-based family of forecourt controllers
mxodbc-connect	6632/tcp	0.000000	# eGenix mxODBC Connect
cisco-vpath-tun	6633/tcp	0.000000	# Cisco vPath Services Overlay
unknown	6633/udp	0.000330
mpls-pm	6634/tcp	0.000000	# MPLS Performance Measurement out-of-band response
mpls-udp	6635/tcp	0.000000	# Encapsulate MPLS packets in UDP tunnels.
mpls-udp-dtls	6636/tcp	0.000000	# Encapsulate MPLS packets in UDP tunnels with DTLS.
unknown	6639/udp	0.000330
ovsdb	6640/tcp	0.000000	# Open vSwitch Database protocol
unknown	6644/tcp	0.000076
unknown	6646/tcp	0.003649
unknown	6647/tcp	0.000076
unknown	6650/tcp	0.000076
unknown	6652/udp	0.000330
openflow	6653/tcp	0.000000
pcs-sf-ui-man	6655/tcp	0.000000	# PC SOFT - Software factory UI/manager
emgmsg	6656/tcp	0.000000	# Emergency Message Control Service
palcom-disc	6657/tcp	0.000000	# PalCom Discovery
palcom-disc	6657/udp	0.000000	# PalCom Discovery
unknown	6660/udp	0.000330
radmind	6662/tcp	0.000100	# Radmind protocol (deprecated)
unknown	6664/udp	0.000330
irc	6665/tcp	0.000050	# Internet Relay Chat
ircu	6665/udp	0.000000
irc	6666/tcp	0.001179	# internet relay chat server
ircu	6666/udp	0.000330
irc	6667/tcp	0.000652	# Internet Relay Chat
ircu	6667/udp	0.000000
irc	6668/tcp	0.000176	# Internet Relay Chat
ircu	6668/udp	0.000000
irc	6669/tcp	0.000176	# Internet Relay Chat
ircu	6669/udp	0.000000
irc	6670/tcp	0.000088	# vocaltec-gold | Internet Relay Chat | Vocaltec Global Online Directory
vocaltec-gold	6670/udp	0.000000	# Vocaltec Global Online Directory
p4p-portal	6671/tcp	0.000000	# P4P Portal Service
p4p-portal	6671/udp	0.000000	# P4P Portal Service
vision_server	6672/tcp	0.000000	# vision-server
vision_server	6672/udp	0.000000
vision_elmd	6673/tcp	0.000000	# vision-elmd
vision_elmd	6673/udp	0.000000
vfbp	6678/tcp	0.000000	# vfbp-disc | Viscount Freedom Bridge Protocol | Viscount Freedom Bridge Discovery
osaut	6679/tcp	0.000000	# Osorno Automation
unknown	6686/udp	0.000330
clever-ctrace	6687/tcp	0.000000	# CleverView for cTrace Message Service
clever-tcpip	6688/tcp	0.000000	# CleverView for TCP/IP Message Service
tsa	6689/tcp	0.000228	# Tofino Security Appliance
tsa	6689/udp	0.000000	# Tofino Security Appliance
cleverdetect	6690/tcp	0.000000	# CLEVERDetect Message Service
unknown	6692/tcp	0.000228
babel	6696/tcp	0.000000	# Babel Routing Protocol
ircs-u	6697/tcp	0.000000	# Internet Relay Chat via TLS/SSL
babel	6697/udp	0.000330	# Babel Routing Protocol
napster	6699/tcp	0.000251	# babel-dtls | Napster File (MP3) sharing  software | Babel Routing Protocol over DTLS
unknown	6699/udp	0.000330
carracho	6700/tcp	0.000025	# Carracho file sharing
carracho	6701/tcp	0.000038	# kti-icad-srvr | Carracho file sharing | KTI/ICAD Nameserver
kti-icad-srvr	6701/udp	0.000000	# KTI/ICAD Nameserver
e-design-net	6702/tcp	0.000000	# e-Design network
e-design-net	6702/udp	0.000000	# e-Design network
e-design-web	6703/tcp	0.000000	# e-Design web
e-design-web	6703/udp	0.000330	# e-Design web
frc-hp	6704/sctp	0.000000	# ForCES HP (High Priority) channel
frc-mp	6705/sctp	0.000000	# ForCES MP (Medium Priority) channel
frc-lp	6706/sctp	0.000000	# ForCES LP (Low priority) channel
unknown	6709/tcp	0.000076
unknown	6710/tcp	0.000076
unknown	6711/tcp	0.000152
ibprotocol	6714/tcp	0.000000	# Internet Backplane Protocol
ibprotocol	6714/udp	0.000000	# Internet Backplane Protocol
fibotrader-com	6715/tcp	0.000000	# Fibotrader Communications
fibotrader-com	6715/udp	0.000000	# Fibotrader Communications
princity-agent	6716/tcp	0.000000	# Princity Agent
unknown	6725/tcp	0.000076
unknown	6727/udp	0.000330
unknown	6732/tcp	0.000152
unknown	6734/tcp	0.000076
unknown	6741/udp	0.000330
unknown	6746/udp	0.000330
unknown	6750/udp	0.000330
unknown	6752/udp	0.000330
unknown	6753/udp	0.000330
bmc-perf-agent	6767/tcp	0.000000	# BMC PERFORM AGENT
bmc-perf-agent	6767/udp	0.000330	# BMC PERFORM AGENT
bmc-perf-mgrd	6768/tcp	0.000000	# BMC PERFORM MGRD
bmc-perf-mgrd	6768/udp	0.000000	# BMC PERFORM MGRD
adi-gxp-srvprt	6769/tcp	0.000000	# ADInstruments GxP Server
adi-gxp-srvprt	6769/udp	0.000000	# ADInstruments GxP Server
plysrv-http	6770/tcp	0.000000	# PolyServe http
plysrv-http	6770/udp	0.000000	# PolyServe http
plysrv-https	6771/tcp	0.000000	# PolyServe https
plysrv-https	6771/udp	0.000000	# PolyServe https
unknown	6776/udp	0.000330
ntz-tracker	6777/tcp	0.000000	# netTsunami Tracker
ntz-p2p-storage	6778/tcp	0.000000	# netTsunami p2p storage system
unknown	6779/tcp	0.000228
unknown	6780/tcp	0.000076
bfd-lag	6784/tcp	0.000000	# Bidirectional Forwarding Detection (BFD) on Link Aggregation Group (LAG) Interfaces
unknown	6784/udp	0.000991
dgpf-exchg	6785/tcp	0.000000	# DGPF Individual Exchange
dgpf-exchg	6785/udp	0.000000	# DGPF Individual Exchange
smc-jmx	6786/tcp	0.000000	# Sun Java Web Console JMX
smc-jmx	6786/udp	0.000000	# Sun Java Web Console JMX
smc-admin	6787/tcp	0.000000	# Sun Web Console Admin
smc-admin	6787/udp	0.000000	# Sun Web Console Admin
smc-http	6788/tcp	0.000380
smc-http	6788/udp	0.000000
ibm-db2-admin	6789/tcp	0.000760	# radg | smc-https | IBM DB2 | SMC-HTTPS | GSS-API for the Oracle Remote Administration Daemon
smc-https	6789/udp	0.000330
hnmp	6790/tcp	0.000000
hnmp	6790/udp	0.000000
hnm	6791/tcp	0.000000	# Halcyon Network Manager
hnm	6791/udp	0.000000	# Halcyon Network Manager
unknown	6792/tcp	0.000228
unknown	6800/udp	0.000330
acnet	6801/tcp	0.000000	# ACNET Control System Protocol
acnet	6801/udp	0.000000	# ACNET Control System Protocol
unknown	6811/udp	0.000661
unknown	6816/udp	0.000330
pentbox-sim	6817/tcp	0.000000	# PenTBox Secure IM Protocol
unknown	6820/udp	0.000330
unknown	6824/udp	0.000330
unknown	6829/udp	0.000330
ambit-lm	6831/tcp	0.000000
ambit-lm	6831/udp	0.000000
unknown	6833/udp	0.000330
unknown	6837/udp	0.000330
unknown	6839/tcp	0.000228
unknown	6839/udp	0.000330
netmo-default	6841/tcp	0.000000	# Netmo Default
netmo-default	6841/udp	0.000000	# Netmo Default
netmo-http	6842/tcp	0.000000	# Netmo HTTP
netmo-http	6842/udp	0.000330	# Netmo HTTP
unknown	6843/udp	0.000330
unknown	6847/udp	0.000330
iccrushmore	6850/tcp	0.000000
iccrushmore	6850/udp	0.000330
unknown	6855/udp	0.000330
unknown	6857/udp	0.000330
unknown	6860/udp	0.000330
unknown	6864/udp	0.000330
acctopus-cc	6868/tcp	0.000000	# acctopus-st | Acctopus Command Channel | Acctopus Status
acctopus-st	6868/udp	0.000000	# Acctopus Status
unknown	6877/tcp	0.000076
unknown	6877/udp	0.000330
bittorrent-tracker	6881/tcp	0.000640	# BitTorrent tracker
muse	6888/tcp	0.000076
muse	6888/udp	0.000000
unknown	6895/udp	0.000330
unknown	6896/tcp	0.000152
unknown	6897/tcp	0.000076
rtimeviewer	6900/tcp	0.000000	# R*TIME Viewer Data Interface
jetstream	6901/tcp	0.000380	# Novell Jetstream messaging protocol
unknown	6905/udp	0.000991
unknown	6909/udp	0.000330
unknown	6912/udp	0.000330
unknown	6918/udp	0.000330
unknown	6920/tcp	0.000076
unknown	6922/tcp	0.000076
split-ping	6924/tcp	0.000000	# Ping with RX/TX latency/loss split
unknown	6925/udp	0.000661
unknown	6927/udp	0.000330
unknown	6932/udp	0.000330
ethoscan	6935/tcp	0.000000	# EthoScan Service
xsmsvc	6936/tcp	0.000000	# XenSource Management Service
xsmsvc	6936/udp	0.000000	# XenSource Management Service
unknown	6942/tcp	0.000076
unknown	6942/udp	0.000330
unknown	6943/udp	0.000330
unknown	6944/udp	0.000330
unknown	6945/udp	0.000330
bioserver	6946/tcp	0.000000	# Biometrics Server
bioserver	6946/udp	0.000000	# Biometrics Server
otlp	6951/tcp	0.000000
otlp	6951/udp	0.000000
unknown	6956/tcp	0.000076
unknown	6956/udp	0.000330
unknown	6957/udp	0.000330
unknown	6959/udp	0.000330
jmact3	6961/tcp	0.000000
jmact3	6961/udp	0.000661
jmevt2	6962/tcp	0.000000
jmevt2	6962/udp	0.000000
swismgr1	6963/tcp	0.000000
swismgr1	6963/udp	0.000000
swismgr2	6964/tcp	0.000000
swismgr2	6964/udp	0.000000
swistrap	6965/tcp	0.000000
swistrap	6965/udp	0.000000
swispol	6966/tcp	0.000000
swispol	6966/udp	0.000000
acmsoda	6969/tcp	0.000389
acmsoda	6969/udp	0.001104
conductor	6970/tcp	0.000000	# conductor-mpx | Conductor test coordination protocol | conductor for multiplex
unknown	6970/udp	0.002643
unknown	6971/udp	0.002643
unknown	6972/tcp	0.000076
unknown	6972/udp	0.000661
unknown	6973/tcp	0.000076
unknown	6973/udp	0.000330
unknown	6976/udp	0.000661
unknown	6978/udp	0.000330
qolyester	6980/tcp	0.000000	# QoS-extended OLSR protocol
unknown	6984/udp	0.000661
unknown	6991/udp	0.000330
unknown	6996/udp	0.000330
MobilitySrv	6997/tcp	0.000000	# Mobility XE Protocol
MobilitySrv	6997/udp	0.000000	# Mobility XE Protocol
iatp-highpri	6998/tcp	0.000000
iatp-highpri	6998/udp	0.000330
iatp-normalpri	6999/tcp	0.000000
iatp-normalpri	6999/udp	0.000000
afs3-fileserver	7000/tcp	0.001995	# file server itself, msdos | file server itself
afs3-fileserver	7000/udp	0.002339	# file server itself
afs3-callback	7001/tcp	0.000891	# callbacks to cache managers
afs3-callback	7001/udp	0.001005	# callbacks to cache managers
afs3-prserver	7002/tcp	0.000351	# users & groups database
afs3-prserver	7002/udp	0.000560	# users & groups database
afs3-vlserver	7003/tcp	0.000125	# volume location database
afs3-vlserver	7003/udp	0.000610	# volume location database
afs3-kaserver	7004/tcp	0.000201	# AFS/Kerberos authentication service
afs3-kaserver	7004/udp	0.000445	# AFS/Kerberos authentication service
afs3-volser	7005/tcp	0.000075	# volume managment server
afs3-volser	7005/udp	0.000972	# volume managment server
afs3-errors	7006/tcp	0.000025	# error interpretation service
afs3-errors	7006/udp	0.000494	# error interpretation service
afs3-bos	7007/tcp	0.000314	# basic overseer process
afs3-bos	7007/udp	0.000610	# basic overseer process
afs3-update	7008/tcp	0.000025	# server-to-server updater
afs3-update	7008/udp	0.000708	# server-to-server updater
afs3-rmtsys	7009/tcp	0.000038	# remote cache manager service
afs3-rmtsys	7009/udp	0.001021	# remote cache manager service
ups-onlinet	7010/tcp	0.000113	# onlinet uninterruptable power supplies
ups-onlinet	7010/udp	0.000643	# onlinet uninterruptable power supplies
talon-disc	7011/tcp	0.000000	# Talon Discovery Port
talon-disc	7011/udp	0.000000	# Talon Discovery Port
talon-engine	7012/tcp	0.000000	# Talon Engine
talon-engine	7012/udp	0.000661	# Talon Engine
microtalon-dis	7013/tcp	0.000000	# Microtalon Discovery
microtalon-dis	7013/udp	0.000000	# Microtalon Discovery
microtalon-com	7014/tcp	0.000000	# Microtalon Communications
microtalon-com	7014/udp	0.000000	# Microtalon Communications
talon-webserver	7015/tcp	0.000000	# Talon Webserver
talon-webserver	7015/udp	0.000000	# Talon Webserver
spg	7016/tcp	0.000000	# SPG Controls Carrier
grasp	7017/tcp	0.000000	# GeneRic Autonomic Signaling Protocol (TEMPORARY - registered 2017-04-28, expires 2018-04-28) | GeneRic Autonomic Signaling Protocol
fisa-svc	7018/tcp	0.000000	# FISA Service
doceri-ctl	7019/tcp	0.000836	# doceri-view | doceri drawing service control | doceri drawing service screen view
dpserve	7020/tcp	0.000000	# DP Serve
dpserve	7020/udp	0.000000	# DP Serve
dpserveadmin	7021/tcp	0.000000	# DP Serve Admin
dpserveadmin	7021/udp	0.000000	# DP Serve Admin
ctdp	7022/tcp	0.000000	# CT Discovery Protocol
ctdp	7022/udp	0.000000	# CT Discovery Protocol
ct2nmcs	7023/tcp	0.000000	# Comtech T2 NMCS
ct2nmcs	7023/udp	0.000000	# Comtech T2 NMCS
vmsvc	7024/tcp	0.000152	# Vormetric service
vmsvc	7024/udp	0.000000	# Vormetric service
vmsvc-2	7025/tcp	0.000228	# Vormetric Service II
vmsvc-2	7025/udp	0.000000	# Vormetric Service II
loreji-panel	7026/tcp	0.000000	# Loreji Webhosting Panel
unknown	7026/udp	0.000330
unknown	7027/udp	0.000330
unknown	7028/udp	0.000330
unknown	7029/udp	0.000330
op-probe	7030/tcp	0.000000	# ObjectPlanet probe
op-probe	7030/udp	0.000000	# ObjectPlanet probe
iposplanet	7031/tcp	0.000000	# IPOSPLANET retailing multi devices protocol
unknown	7033/tcp	0.000076
unknown	7033/udp	0.000330
unknown	7039/udp	0.000330
quest-disc	7040/tcp	0.000000	# Quest application level network service discovery
unknown	7043/tcp	0.000076
unknown	7050/tcp	0.000152
unknown	7051/tcp	0.000152
unknown	7051/udp	0.000661
unknown	7055/udp	0.000330
unknown	7060/udp	0.000330
unknown	7065/udp	0.000330
unknown	7067/tcp	0.000076
unknown	7068/tcp	0.000076
unknown	7069/udp	0.000330
realserver	7070/tcp	0.004328	# arcp | ARCP
arcp	7070/udp	0.000000
iwg1	7071/tcp	0.000076	# IWGADTS Aircraft Housekeeping Message
iwg1	7071/udp	0.000000	# IWGADTS Aircraft Housekeeping Message
iba-cfg	7072/tcp	0.000076	# iba-cfg-disc | iba Device Configuration Protocol
martalk	7073/tcp	0.000000	# MarTalk protocol
unknown	7074/udp	0.000661
unknown	7079/udp	0.000330
empowerid	7080/tcp	0.000152	# EmpowerID Communication
empowerid	7080/udp	0.000330	# EmpowerID Communication
unknown	7081/udp	0.000330
unknown	7085/udp	0.000330
zixi-transport	7088/tcp	0.000000	# Zixi live video transport protocol
unknown	7089/udp	0.000330
unknown	7092/tcp	0.000076
jdp-disc	7095/tcp	0.000000	# Java Discovery Protocol
lazy-ptop	7099/tcp	0.000076
lazy-ptop	7099/udp	0.000000
font-service	7100/tcp	0.000928	# X Font Service
font-service	7100/udp	0.001170	# X Font Service
elcn	7101/tcp	0.000076	# Embedded Light Control Network
elcn	7101/udp	0.000000	# Embedded Light Control Network
unknown	7102/tcp	0.000076
unknown	7103/tcp	0.000304
unknown	7104/tcp	0.000076
unknown	7106/tcp	0.000380
aes-x170	7107/tcp	0.000000
unknown	7108/udp	0.000330
unknown	7109/udp	0.000330
unknown	7113/udp	0.000330
unknown	7114/udp	0.000330
rothaga	7117/tcp	0.000000	# Encrypted chat and file transfer service
unknown	7119/tcp	0.000076
unknown	7120/udp	0.000330
virprot-lm	7121/tcp	0.000076	# Virtual Prototypes License Manager
virprot-lm	7121/udp	0.000000	# Virtual Prototypes License Manager
snif	7123/tcp	0.000152	# End-to-end TLS Relay Control Connection
scenidm	7128/tcp	0.000000	# intelligent data manager
scenidm	7128/udp	0.000000	# intelligent data manager
scenccs	7129/tcp	0.000000	# Catalog Content Search
scenccs	7129/udp	0.000000	# Catalog Content Search
unknown	7132/udp	0.000330
unknown	7133/udp	0.000330
unknown	7139/udp	0.000330
unknown	7140/udp	0.000330
unknown	7148/udp	0.000330
unknown	7156/udp	0.000330
unknown	7159/udp	0.000330
unknown	7160/udp	0.000330
cabsm-comm	7161/tcp	0.000000	# CA BSM Comm
cabsm-comm	7161/udp	0.000000	# CA BSM Comm
caistoragemgr	7162/tcp	0.000000	# CA Storage Manager
caistoragemgr	7162/udp	0.000000	# CA Storage Manager
cacsambroker	7163/tcp	0.000000	# CA Connection Broker
cacsambroker	7163/udp	0.000000	# CA Connection Broker
fsr	7164/tcp	0.000000	# File System Repository Agent
fsr	7164/udp	0.000000	# File System Repository Agent
doc-server	7165/tcp	0.000000	# Document WCF Server
doc-server	7165/udp	0.000000	# Document WCF Server
aruba-server	7166/tcp	0.000000	# Aruba eDiscovery Server
aruba-server	7166/udp	0.000000	# Aruba eDiscovery Server
casrmagent	7167/tcp	0.000000	# CA SRM Agent
unknown	7167/udp	0.000330
cnckadserver	7168/tcp	0.000000	# cncKadServer DB & Inventory Services
ccag-pib	7169/tcp	0.000000	# Consequor Consulting Process Integration Bridge
ccag-pib	7169/udp	0.000000	# Consequor Consulting Process Integration Bridge
nsrp	7170/tcp	0.000000	# Adaptive Name/Service Resolution
nsrp	7170/udp	0.000000	# Adaptive Name/Service Resolution
drm-production	7171/tcp	0.000000	# Discovery and Retention Mgt Production
drm-production	7171/udp	0.000000	# Discovery and Retention Mgt Production
metalbend	7172/tcp	0.000000	# Port used for MetalBend programmable interface
zsecure	7173/tcp	0.000000	# zSecure Server
unknown	7173/udp	0.000330
clutild	7174/tcp	0.000000
clutild	7174/udp	0.000000
unknown	7178/udp	0.000330
unknown	7180/udp	0.000330
janus-disc	7181/tcp	0.000000	# Janus Guidewire Enterprise Discovery Service Bus
unknown	7182/udp	0.000330
unknown	7184/tcp	0.000076
unknown	7187/udp	0.000330
fodms	7200/tcp	0.000439	# FODMS FLIP
fodms	7200/udp	0.000346	# FODMS FLIP
dlip	7201/tcp	0.000188
dlip	7201/udp	0.000527
pon-ictp	7202/tcp	0.000000	# Inter-Channel Termination Protocol (ICTP) for multi-wavelength PON (Passive Optical Network) systems
unknown	7205/udp	0.000330
PS-Server	7215/tcp	0.000000	# Communication ports for PaperStream Server services
PS-Capture-Pro	7216/tcp	0.000000	# PaperStream Capture Professional
unknown	7218/tcp	0.000076
unknown	7224/udp	0.000330
unknown	7225/udp	0.000330
ramp	7227/tcp	0.000000	# Registry A & M Protocol | Registry A $ M Protocol
ramp	7227/udp	0.000000	# Registry A $ M Protocol
citrixupp	7228/tcp	0.000000	# Citrix Universal Printing Port
citrixuppg	7229/tcp	0.000000	# Citrix UPP Gateway
unknown	7230/udp	0.000330
unknown	7231/tcp	0.000076
unknown	7231/udp	0.000330
asa-gateways	7234/tcp	0.000000	# Traffic forwarding for Okta cloud infra
aspcoordination	7235/tcp	0.000000	# ASP Coordination Protocol
display	7236/tcp	0.000000	# Wi-Fi Alliance Wi-Fi Display Protocol
pads	7237/tcp	0.000000	# PADS (Public Area Display System) Server
unknown	7237/udp	0.000330
unknown	7238/udp	0.000330
unknown	7241/tcp	0.000152
unknown	7242/udp	0.000330
unknown	7243/udp	0.000330
frc-hicp	7244/tcp	0.000000	# frc-hicp-disc | FrontRow Calypso Human Interface Control Protocol
unknown	7247/udp	0.000330
unknown	7250/udp	0.000330
unknown	7257/udp	0.000330
unknown	7259/udp	0.000330
unknown	7260/udp	0.000330
cnap	7262/tcp	0.000000	# Calypso Network Access Protocol
cnap	7262/udp	0.000000	# Calypso Network Access Protocol
unknown	7263/udp	0.000330
unknown	7267/udp	0.000661
watchme-7272	7272/tcp	0.000152	# WatchMe Monitoring 7272
watchme-7272	7272/udp	0.000000	# WatchMe Monitoring 7272
openmanage	7273/tcp	0.000050	# oma-rlp | Dell OpenManage | OMA Roaming Location
oma-rlp	7273/udp	0.000000	# OMA Roaming Location
oma-rlp-s	7274/tcp	0.000000	# OMA Roaming Location SEC
oma-rlp-s	7274/udp	0.000661	# OMA Roaming Location SEC
oma-ulp	7275/tcp	0.000000	# OMA UserPlane Location
oma-ulp	7275/udp	0.000330	# OMA UserPlane Location
oma-ilp	7276/tcp	0.000000	# OMA Internal Location Protocol
oma-ilp	7276/udp	0.000000	# OMA Internal Location Protocol
oma-ilp-s	7277/tcp	0.000000	# OMA Internal Location Secure Protocol
oma-ilp-s	7277/udp	0.000000	# OMA Internal Location Secure Protocol
oma-dcdocbs	7278/tcp	0.000152	# OMA Dynamic Content Delivery over CBS
oma-dcdocbs	7278/udp	0.000330	# OMA Dynamic Content Delivery over CBS
ctxlic	7279/tcp	0.000000	# Citrix Licensing
ctxlic	7279/udp	0.000000	# Citrix Licensing
itactionserver1	7280/tcp	0.000000	# ITACTIONSERVER 1
itactionserver1	7280/udp	0.000000	# ITACTIONSERVER 1
itactionserver2	7281/tcp	0.000152	# ITACTIONSERVER 2
itactionserver2	7281/udp	0.000000	# ITACTIONSERVER 2
mzca-action	7282/tcp	0.000000	# mzca-alert | eventACTION/ussACTION (MZCA) server | eventACTION/ussACTION (MZCA) alert
mzca-alert	7282/udp	0.000000	# eventACTION/ussACTION (MZCA) alert
genstat	7283/tcp	0.000000	# General Statistics Rendezvous Protocol
unknown	7285/udp	0.000330
unknown	7287/udp	0.000330
unknown	7294/udp	0.000330
unknown	7298/udp	0.000661
swx	7300/tcp	0.000076	# The Swiss Exchange
swx	7300/udp	0.000000	# The Swiss Exchange
swx	7301/tcp	0.000000	# The Swiss Exchange
swx	7301/udp	0.000330	# The Swiss Exchange
swx	7302/tcp	0.000000	# The Swiss Exchange
swx	7302/udp	0.000000	# The Swiss Exchange
swx	7303/tcp	0.000000	# The Swiss Exchange
swx	7303/udp	0.000661	# The Swiss Exchange
swx	7304/tcp	0.000000	# The Swiss Exchange
swx	7304/udp	0.000000	# The Swiss Exchange
swx	7305/tcp	0.000000	# The Swiss Exchange
swx	7305/udp	0.000330	# The Swiss Exchange
swx	7306/tcp	0.000000	# The Swiss Exchange
swx	7306/udp	0.000000	# The Swiss Exchange
swx	7307/tcp	0.000000	# The Swiss Exchange
swx	7307/udp	0.000330	# The Swiss Exchange
swx	7308/tcp	0.000000	# The Swiss Exchange
swx	7308/udp	0.000000	# The Swiss Exchange
swx	7309/tcp	0.000000	# The Swiss Exchange
swx	7309/udp	0.000330	# The Swiss Exchange
swx	7310/tcp	0.000000	# The Swiss Exchange
swx	7310/udp	0.000330	# The Swiss Exchange
swx	7311/tcp	0.000000	# The Swiss Exchange
swx	7311/udp	0.000000	# The Swiss Exchange
swx	7312/tcp	0.000000	# The Swiss Exchange
swx	7312/udp	0.000000	# The Swiss Exchange
swx	7313/tcp	0.000000	# The Swiss Exchange
swx	7313/udp	0.000000	# The Swiss Exchange
swx	7314/tcp	0.000000	# The Swiss Exchange
swx	7314/udp	0.000330	# The Swiss Exchange
swx	7315/tcp	0.000000	# The Swiss Exchange
swx	7315/udp	0.000000	# The Swiss Exchange
swx	7316/tcp	0.000000	# The Swiss Exchange
swx	7316/udp	0.000330	# The Swiss Exchange
swx	7317/tcp	0.000000	# The Swiss Exchange
swx	7317/udp	0.000000	# The Swiss Exchange
swx	7318/tcp	0.000000	# The Swiss Exchange
swx	7318/udp	0.000330	# The Swiss Exchange
swx	7319/tcp	0.000000	# The Swiss Exchange
swx	7319/udp	0.000000	# The Swiss Exchange
swx	7320/tcp	0.000076	# The Swiss Exchange
swx	7320/udp	0.000000	# The Swiss Exchange
swx	7321/tcp	0.000000	# The Swiss Exchange
swx	7321/udp	0.000000	# The Swiss Exchange
swx	7322/tcp	0.000000	# The Swiss Exchange
swx	7322/udp	0.000000	# The Swiss Exchange
swx	7323/tcp	0.000000	# The Swiss Exchange
swx	7323/udp	0.000000	# The Swiss Exchange
swx	7324/tcp	0.000000	# The Swiss Exchange
swx	7324/udp	0.000000	# The Swiss Exchange
swx	7325/tcp	0.000076	# The Swiss Exchange
swx	7325/udp	0.000000	# The Swiss Exchange
icb	7326/tcp	0.000013	# Internet Citizen's Band
swx	7326/udp	0.000000	# The Swiss Exchange
swx	7327/tcp	0.000000	# The Swiss Exchange
swx	7327/udp	0.000000	# The Swiss Exchange
swx	7328/tcp	0.000000	# The Swiss Exchange
swx	7328/udp	0.000000	# The Swiss Exchange
swx	7329/tcp	0.000000	# The Swiss Exchange
swx	7329/udp	0.000330	# The Swiss Exchange
swx	7330/tcp	0.000000	# The Swiss Exchange
swx	7330/udp	0.000000	# The Swiss Exchange
swx	7331/tcp	0.000000	# The Swiss Exchange
swx	7331/udp	0.000000	# The Swiss Exchange
swx	7332/tcp	0.000000	# The Swiss Exchange
swx	7332/udp	0.000000	# The Swiss Exchange
swx	7333/tcp	0.000000	# The Swiss Exchange
swx	7333/udp	0.000000	# The Swiss Exchange
swx	7334/tcp	0.000000	# The Swiss Exchange
swx	7334/udp	0.000000	# The Swiss Exchange
swx	7335/tcp	0.000000	# The Swiss Exchange
swx	7335/udp	0.000000	# The Swiss Exchange
swx	7336/tcp	0.000000	# The Swiss Exchange
swx	7336/udp	0.000330	# The Swiss Exchange
swx	7337/tcp	0.000000	# The Swiss Exchange
swx	7337/udp	0.000000	# The Swiss Exchange
swx	7338/tcp	0.000000	# The Swiss Exchange
swx	7338/udp	0.000330	# The Swiss Exchange
swx	7339/tcp	0.000000	# The Swiss Exchange
swx	7339/udp	0.000000	# The Swiss Exchange
swx	7340/tcp	0.000000	# The Swiss Exchange
swx	7340/udp	0.000000	# The Swiss Exchange
swx	7341/tcp	0.000000	# The Swiss Exchange
swx	7341/udp	0.000000	# The Swiss Exchange
swx	7342/tcp	0.000000	# The Swiss Exchange
swx	7342/udp	0.000000	# The Swiss Exchange
swx	7343/tcp	0.000000	# The Swiss Exchange
swx	7343/udp	0.000000	# The Swiss Exchange
swx	7344/tcp	0.000000	# The Swiss Exchange
swx	7344/udp	0.000000	# The Swiss Exchange
swx	7345/tcp	0.000076	# The Swiss Exchange
swx	7345/udp	0.000330	# The Swiss Exchange
swx	7346/tcp	0.000000	# The Swiss Exchange
swx	7346/udp	0.000330	# The Swiss Exchange
swx	7347/tcp	0.000000	# The Swiss Exchange
swx	7347/udp	0.000000	# The Swiss Exchange
swx	7348/tcp	0.000000	# The Swiss Exchange
swx	7348/udp	0.000000	# The Swiss Exchange
swx	7349/tcp	0.000000	# The Swiss Exchange
swx	7349/udp	0.000000	# The Swiss Exchange
swx	7350/tcp	0.000000	# The Swiss Exchange
swx	7350/udp	0.000000	# The Swiss Exchange
swx	7351/tcp	0.000000	# The Swiss Exchange
swx	7351/udp	0.000000	# The Swiss Exchange
swx	7352/tcp	0.000000	# The Swiss Exchange
swx	7352/udp	0.000000	# The Swiss Exchange
swx	7353/tcp	0.000000	# The Swiss Exchange
swx	7353/udp	0.000000	# The Swiss Exchange
swx	7354/tcp	0.000000	# The Swiss Exchange
swx	7354/udp	0.000661	# The Swiss Exchange
swx	7355/tcp	0.000000	# The Swiss Exchange
swx	7355/udp	0.000000	# The Swiss Exchange
swx	7356/tcp	0.000000	# The Swiss Exchange
swx	7356/udp	0.000000	# The Swiss Exchange
swx	7357/tcp	0.000000	# The Swiss Exchange
swx	7357/udp	0.000000	# The Swiss Exchange
swx	7358/tcp	0.000000	# The Swiss Exchange
swx	7358/udp	0.000000	# The Swiss Exchange
swx	7359/tcp	0.000000	# The Swiss Exchange
swx	7359/udp	0.000000	# The Swiss Exchange
lcm-server	7365/tcp	0.000000	# LifeKeeper Communications
lcm-server	7365/udp	0.000000	# LifeKeeper Communications
unknown	7373/udp	0.000330
unknown	7376/udp	0.000330
unknown	7380/udp	0.000330
unknown	7382/udp	0.000330
unknown	7387/udp	0.000330
mindfilesys	7391/tcp	0.000000	# mind-file system server
mindfilesys	7391/udp	0.000000	# mind-file system server
mrssrendezvous	7392/tcp	0.000000	# mrss-rendezvous server
mrssrendezvous	7392/udp	0.000000	# mrss-rendezvous server
nfoldman	7393/tcp	0.000000	# nFoldMan Remote Publish
nfoldman	7393/udp	0.000000	# nFoldMan Remote Publish
fse	7394/tcp	0.000000	# File system export of backup images
fse	7394/udp	0.000000	# File system export of backup images
winqedit	7395/tcp	0.000000
winqedit	7395/udp	0.000000
hexarc	7397/tcp	0.000000	# Hexarc Command Language
hexarc	7397/udp	0.000000	# Hexarc Command Language
rtps-discovery	7400/tcp	0.000076	# RTPS Discovery
rtps-discovery	7400/udp	0.000000	# RTPS Discovery
rtps-dd-ut	7401/tcp	0.000000	# RTPS Data-Distribution User-Traffic
rtps-dd-ut	7401/udp	0.000000	# RTPS Data-Distribution User-Traffic
rtps-dd-mt	7402/tcp	0.000304	# RTPS Data-Distribution Meta-Traffic
rtps-dd-mt	7402/udp	0.000000	# RTPS Data-Distribution Meta-Traffic
unknown	7405/udp	0.000330
unknown	7407/udp	0.000330
ionixnetmon	7410/tcp	0.000000	# Ionix Network Monitor
ionixnetmon	7410/udp	0.000330	# Ionix Network Monitor
daqstream	7411/tcp	0.000000	# Streaming of measurement data
ipluminary	7420/tcp	0.000000	# Multichannel real-time lighting control
mtportmon	7421/tcp	0.000000	# Matisse Port Monitor
mtportmon	7421/udp	0.000000	# Matisse Port Monitor
unknown	7423/udp	0.000330
unknown	7425/udp	0.000330
pmdmgr	7426/tcp	0.000000	# OpenView DM Postmaster Manager
pmdmgr	7426/udp	0.000000	# OpenView DM Postmaster Manager
oveadmgr	7427/tcp	0.000000	# OpenView DM Event Agent Manager
oveadmgr	7427/udp	0.000330	# OpenView DM Event Agent Manager
ovladmgr	7428/tcp	0.000000	# OpenView DM Log Agent Manager
ovladmgr	7428/udp	0.000000	# OpenView DM Log Agent Manager
opi-sock	7429/tcp	0.000000	# OpenView DM rqt communication
opi-sock	7429/udp	0.000000	# OpenView DM rqt communication
xmpv7	7430/tcp	0.000000	# OpenView DM xmpv7 api pipe
xmpv7	7430/udp	0.000000	# OpenView DM xmpv7 api pipe
pmd	7431/tcp	0.000000	# OpenView DM ovc/xmpv3 api pipe
pmd	7431/udp	0.000000	# OpenView DM ovc/xmpv3 api pipe
unknown	7432/udp	0.000330
unknown	7435/tcp	0.000304
faximum	7437/tcp	0.000000
faximum	7437/udp	0.000000
unknown	7438/tcp	0.000152
unknown	7438/udp	0.000330
oracleas-https	7443/tcp	0.000304	# Oracle Application Server HTTPS
oracleas-https	7443/udp	0.000000	# Oracle Application Server HTTPS
unknown	7445/udp	0.000330
unknown	7446/udp	0.000330
unknown	7451/tcp	0.000076
unknown	7456/tcp	0.000076
unknown	7458/udp	0.000330
pythonds	7464/tcp	0.000013	# Python Documentation Server
unknown	7465/udp	0.000330
unknown	7466/udp	0.000330
unknown	7467/udp	0.000330
sttunnel	7471/tcp	0.000000	# Stateless Transport Tunneling Protocol
unknown	7471/udp	0.000330
rise	7473/tcp	0.000000	# Rise: The Vieneo Province
rise	7473/udp	0.000000	# Rise: The Vieneo Province
neo4j	7474/tcp	0.000000	# Neo4j Graph Database
openit	7478/tcp	0.000000	# IT Asset Management
unknown	7486/udp	0.000330
telops-lmd	7491/tcp	0.000000
telops-lmd	7491/udp	0.000000
unknown	7496/tcp	0.000228
silhouette	7500/tcp	0.000076	# Silhouette User
silhouette	7500/udp	0.000330	# Silhouette User
ovbus	7501/tcp	0.000076	# HP OpenView Bus Daemon
ovbus	7501/udp	0.000000	# HP OpenView Bus Daemon
adcp	7508/tcp	0.000000	# Automation Device Configuration Protocol
acplt	7509/tcp	0.000000	# ACPLT - process automation service
unknown	7509/udp	0.000330
ovhpas	7510/tcp	0.000000	# HP OpenView Application Server
ovhpas	7510/udp	0.000000	# HP OpenView Application Server
pafec-lm	7511/tcp	0.000000
pafec-lm	7511/udp	0.000000
unknown	7512/tcp	0.000304
unknown	7516/udp	0.000991
unknown	7517/udp	0.000330
unknown	7521/udp	0.000330
unknown	7524/udp	0.000661
unknown	7526/udp	0.000330
unknown	7533/udp	0.000330
unknown	7536/udp	0.000661
saratoga	7542/tcp	0.000000	# Saratoga Transfer Protocol
saratoga	7542/udp	0.000000	# Saratoga Transfer Protocol
atul	7543/tcp	0.000000	# atul server
atul	7543/udp	0.000000	# atul server
nta-ds	7544/tcp	0.000000	# FlowAnalyzer DisplayServer
nta-ds	7544/udp	0.000000	# FlowAnalyzer DisplayServer
nta-us	7545/tcp	0.000000	# FlowAnalyzer UtilityServer
nta-us	7545/udp	0.000000	# FlowAnalyzer UtilityServer
cfs	7546/tcp	0.000000	# Cisco Fabric service
cfs	7546/udp	0.000000	# Cisco Fabric service
cwmp	7547/tcp	0.000000	# DSL Forum CWMP | Broadband Forum CWMP
cwmp	7547/udp	0.000000	# DSL Forum CWMP
tidp	7548/tcp	0.000000	# Threat Information Distribution Protocol
tidp	7548/udp	0.000000	# Threat Information Distribution Protocol
nls-tl	7549/tcp	0.000000	# Network Layer Signaling Transport Layer
nls-tl	7549/udp	0.000000	# Network Layer Signaling Transport Layer
cloudsignaling	7550/tcp	0.000000	# Cloud Signaling Service
controlone-con	7551/tcp	0.000000	# ControlONE Console signaling
unknown	7553/tcp	0.000076
unknown	7554/udp	0.000330
unknown	7555/tcp	0.000076
sncp	7560/tcp	0.000000	# Sniffer Command Protocol
sncp	7560/udp	0.000000	# Sniffer Command Protocol
cfw	7563/tcp	0.000000	# Control Framework
unknown	7563/udp	0.000330
vsi-omega	7566/tcp	0.000000	# VSI Omega
vsi-omega	7566/udp	0.000000	# VSI Omega
dell-eql-asm	7569/tcp	0.000000	# Dell EqualLogic Host Group Management
aries-kfinder	7570/tcp	0.000000	# Aries Kfinder
aries-kfinder	7570/udp	0.000000	# Aries Kfinder
coherence	7574/tcp	0.000000	# coherence-disc | Oracle Coherence Cluster Service | Oracle Coherence Cluster discovery service
unknown	7578/udp	0.000330
unknown	7584/udp	0.000330
unknown	7587/udp	0.000330
sun-lm	7588/tcp	0.000000	# Sun License Manager
sun-lm	7588/udp	0.000000	# Sun License Manager
unknown	7591/udp	0.000330
unknown	7596/udp	0.000330
qaz	7597/tcp	0.000050	# Quaz trojan worm
unknown	7600/tcp	0.000076
unknown	7604/udp	0.000330
mipi-debug	7606/tcp	0.000000	# MIPI Alliance Debug
unknown	7609/udp	0.000330
unknown	7613/udp	0.000661
unknown	7617/udp	0.000330
indi	7624/tcp	0.000000	# Instrument Neutral Distributed Interface
indi	7624/udp	0.000000	# Instrument Neutral Distributed Interface
unknown	7625/tcp	0.000380
simco	7626/sctp	0.000000	# SImple Middlebox COnfiguration (SIMCO) | SImple Middlebox COnfiguration (SIMCO) Server
simco	7626/tcp	0.000000	# SImple Middlebox COnfiguration (SIMCO) Server
soap-http	7627/tcp	0.000380	# SOAP Service Port
soap-http	7627/udp	0.000000	# SOAP Service Port
zen-pawn	7628/tcp	0.000076	# Primary Agent Work Notification
zen-pawn	7628/udp	0.000000	# Primary Agent Work Notification
xdas	7629/tcp	0.000000	# OpenXDAS Wire Protocol
xdas	7629/udp	0.000000	# OpenXDAS Wire Protocol
hawk	7630/tcp	0.000000	# HA Web Konsole
unknown	7630/udp	0.000330
tesla-sys-msg	7631/tcp	0.000000	# TESLA System Messaging
pmdfmgt	7633/tcp	0.000000	# PMDF Management
pmdfmgt	7633/udp	0.000330	# PMDF Management
hddtemp	7634/tcp	0.000025	# A cross-platform hard disk temperature monitoring daemon
unknown	7637/tcp	0.000076
unknown	7638/udp	0.000330
unknown	7639/udp	0.000330
cuseeme	7648/tcp	0.000000	# bonjour-cuseeme
cucme-1	7648/udp	0.000923	# cucme live video/audio server
cucme-2	7649/udp	0.000379	# cucme live video/audio server
cucme-3	7650/udp	0.000395	# cucme live video/audio server
cucme-4	7651/udp	0.000988	# cucme live video/audio server
unknown	7654/tcp	0.000076
unknown	7660/udp	0.000330
rome	7663/tcp	0.000000	# Proprietary immutable distributed data storage
unknown	7667/udp	0.000330
imqstomp	7672/tcp	0.000000	# iMQ STOMP Server
imqstomps	7673/tcp	0.000000	# iMQ STOMP Server over SSL
imqtunnels	7674/tcp	0.000000	# iMQ SSL tunnel
imqtunnels	7674/udp	0.000000	# iMQ SSL tunnel
imqtunnel	7675/tcp	0.000000	# iMQ Tunnel
imqtunnel	7675/udp	0.000000	# iMQ Tunnel
imqbrokerd	7676/tcp	0.000228	# iMQ Broker Rendezvous
imqbrokerd	7676/udp	0.000000	# iMQ Broker Rendezvous
sun-user-https	7677/tcp	0.000000	# Sun App Server - HTTPS
sun-user-https	7677/udp	0.000991	# Sun App Server - HTTPS
unknown	7679/udp	0.000330
pando-pub	7680/tcp	0.000000	# ms-do | Pando Media Public Distribution | Microsoft Delivery Optimization Peer-to-Peer
pando-pub	7680/udp	0.000330	# Pando Media Public Distribution
dmt	7683/tcp	0.000000	# Cleondris DMT
unknown	7684/udp	0.000330
unknown	7685/tcp	0.000076
bolt	7687/tcp	0.000000	# Bolt database connection
unknown	7688/tcp	0.000076
unknown	7688/udp	0.000330
collaber	7689/tcp	0.000000	# Collaber Network Service
collaber	7689/udp	0.000000	# Collaber Network Service
sovd	7690/tcp	0.000000	# Service-Oriented Vehicle Diagnostics
unknown	7696/udp	0.000330
klio	7697/tcp	0.000000	# KLIO communications
klio	7697/udp	0.000330	# KLIO communications
em7-secom	7700/tcp	0.000000	# EM7 Secure Communications
nfapi	7701/tcp	0.000000	# SCF nFAPI defining MAC/PHY split
unknown	7704/udp	0.000330
sync-em7	7707/tcp	0.000000	# EM7 Dynamic Updates
sync-em7	7707/udp	0.000000	# EM7 Dynamic Updates
scinet	7708/tcp	0.000000	# scientia.net
scinet	7708/udp	0.000000	# scientia.net
unknown	7710/udp	0.000330
unknown	7714/udp	0.000330
unknown	7716/udp	0.000330
medimageportal	7720/tcp	0.000000	# MedImage Portal
medimageportal	7720/udp	0.000330	# MedImage Portal
unknown	7723/udp	0.000330
nsdeepfreezectl	7724/tcp	0.000000	# Novell Snap-in Deep Freeze Control
nsdeepfreezectl	7724/udp	0.000000	# Novell Snap-in Deep Freeze Control
nitrogen	7725/tcp	0.000152	# Nitrogen Service
nitrogen	7725/udp	0.000330	# Nitrogen Service
freezexservice	7726/tcp	0.000000	# FreezeX Console Service
freezexservice	7726/udp	0.000000	# FreezeX Console Service
trident-data	7727/tcp	0.000000	# Trident Systems Data
trident-data	7727/udp	0.000330	# Trident Systems Data
osvr	7728/tcp	0.000000	# Open-Source Virtual Reality
unknown	7728/udp	0.000330
smip	7734/tcp	0.000000	# Smith Protocol over IP
smip	7734/udp	0.000000	# Smith Protocol over IP
unknown	7737/udp	0.000330
aiagent	7738/tcp	0.000000	# HP Enterprise Discovery Agent
aiagent	7738/udp	0.000330	# HP Enterprise Discovery Agent
unknown	7739/udp	0.000330
scriptview	7741/tcp	0.000380	# ScriptView Network
scriptview	7741/udp	0.000330	# ScriptView Network
msss	7742/tcp	0.000000	# Mugginsoft Script Server Service
sstp-1	7743/tcp	0.000000	# Sakura Script Transfer Protocol
sstp-1	7743/udp	0.000000	# Sakura Script Transfer Protocol
raqmon-pdu	7744/tcp	0.000152	# RAQMON PDU
raqmon-pdu	7744/udp	0.000000	# RAQMON PDU
unknown	7746/udp	0.000330
prgp	7747/tcp	0.000000	# Put/Run/Get Protocol
prgp	7747/udp	0.000330	# Put/Run/Get Protocol
unknown	7749/tcp	0.000152
unknown	7751/udp	0.000330
unknown	7753/udp	0.000330
unknown	7759/udp	0.000330
unknown	7763/udp	0.000330
unknown	7770/tcp	0.000152
unknown	7771/tcp	0.000076
unknown	7772/tcp	0.000076
unknown	7773/udp	0.000330
inetfs	7775/tcp	0.000000	# A File System using TLS over a wide area network
unknown	7775/udp	0.000330
cbt	7777/tcp	0.000380
cbt	7777/udp	0.000000
interwise	7778/tcp	0.000380
interwise	7778/udp	0.000330
vstat	7779/tcp	0.000000
vstat	7779/udp	0.000330
unknown	7780/tcp	0.000076
accu-lmgr	7781/tcp	0.000000
accu-lmgr	7781/udp	0.000000
s-bfd	7784/tcp	0.000000	# Seamless Bidirectional Forwarding Detection (S-BFD)
minivend	7786/tcp	0.000000
minivend	7786/udp	0.000000
popup-reminders	7787/tcp	0.000000	# Popup Reminders Receive
popup-reminders	7787/udp	0.000330	# Popup Reminders Receive
unknown	7788/tcp	0.000076
unknown	7788/udp	0.000330
office-tools	7789/tcp	0.000076	# Office Tools Pro Receive
office-tools	7789/udp	0.000000	# Office Tools Pro Receive
unknown	7792/udp	0.000330
unknown	7793/udp	0.000330
q3ade	7794/tcp	0.000000	# Q3ADE Cluster Service
q3ade	7794/udp	0.000000	# Q3ADE Cluster Service
unknown	7795/udp	0.000330
pnet-conn	7797/tcp	0.000000	# Propel Connector port
pnet-conn	7797/udp	0.000000	# Propel Connector port
pnet-enc	7798/tcp	0.000000	# Propel Encoder port
pnet-enc	7798/udp	0.000000	# Propel Encoder port
altbsdp	7799/tcp	0.000000	# Alternate BSDP Service
altbsdp	7799/udp	0.000330	# Alternate BSDP Service
asr	7800/tcp	0.000228	# Apple Software Restore
asr	7800/udp	0.000000	# Apple Software Restore
ssp-client	7801/tcp	0.000000	# Secure Server Protocol - client
ssp-client	7801/udp	0.000330	# Secure Server Protocol - client
vns-tp	7802/tcp	0.000000	# Virtualized Network Services Tunnel Protocol
unknown	7804/udp	0.000661
rbt-wanopt	7810/tcp	0.000000	# Riverbed WAN Optimization Protocol
rbt-wanopt	7810/udp	0.000000	# Riverbed WAN Optimization Protocol
unknown	7813/tcp	0.000076
unknown	7830/tcp	0.000076
unknown	7832/udp	0.000330
unknown	7836/udp	0.000330
unknown	7842/udp	0.000330
apc-7845	7845/tcp	0.000000	# APC 7845
apc-7845	7845/udp	0.000000	# APC 7845
apc-7846	7846/tcp	0.000000	# APC 7846
apc-7846	7846/udp	0.000991	# APC 7846
csoauth	7847/tcp	0.000000	# A product key authentication protocol made by CSO
unknown	7852/tcp	0.000076
unknown	7853/tcp	0.000076
unknown	7854/tcp	0.000076
unknown	7854/udp	0.000330
unknown	7855/udp	0.000330
unknown	7857/udp	0.000330
unknown	7867/udp	0.000661
mobileanalyzer	7869/tcp	0.000000	# MobileAnalyzer& MobileMonitor
unknown	7869/udp	0.000330
rbt-smc	7870/tcp	0.000000	# Riverbed Steelhead Mobile Service
mdm	7871/tcp	0.000000	# Mobile Device Management
mipv6tls	7872/tcp	0.000000	# TLS-based Mobile IPv6 Security
unknown	7873/udp	0.000330
unknown	7874/udp	0.000330
owms	7878/tcp	0.000152	# Opswise Message Service
pss	7880/tcp	0.000000	# Pearson
pss	7880/udp	0.000000	# Pearson
unknown	7884/udp	0.000330
ubroker	7887/tcp	0.000000	# Universal Broker
ubroker	7887/udp	0.000330	# Universal Broker
unknown	7894/udp	0.000330
unknown	7895/tcp	0.000076
unknown	7895/udp	0.000330
unknown	7898/udp	0.000330
mevent	7900/tcp	0.000152	# Multicast Event
mevent	7900/udp	0.000000	# Multicast Event
tnos-sp	7901/tcp	0.000000	# TNOS Service Protocol
tnos-sp	7901/udp	0.000000	# TNOS Service Protocol
tnos-dp	7902/tcp	0.000000	# TNOS shell Protocol
tnos-dp	7902/udp	0.000000	# TNOS shell Protocol
tnos-dps	7903/tcp	0.000000	# TNOS Secure DiaguardProtocol
tnos-dps	7903/udp	0.000000	# TNOS Secure DiaguardProtocol
unknown	7907/udp	0.000330
unknown	7908/udp	0.000330
unknown	7911/tcp	0.000380
qo-secure	7913/tcp	0.000152	# QuickObjects secure port
qo-secure	7913/udp	0.000000	# QuickObjects secure port
unknown	7918/udp	0.000330
unknown	7919/udp	0.000330
unknown	7920/tcp	0.000228
unknown	7920/udp	0.000330
unknown	7921/tcp	0.000228
unknown	7923/udp	0.000330
unknown	7929/tcp	0.000152
unknown	7931/udp	0.000330
t2-drm	7932/tcp	0.000000	# Tier 2 Data Resource Manager
t2-drm	7932/udp	0.000000	# Tier 2 Data Resource Manager
t2-brm	7933/tcp	0.000000	# Tier 2 Business Rules Manager
t2-brm	7933/udp	0.000330	# Tier 2 Business Rules Manager
nsrexecd	7937/tcp	0.001455	# Legato NetWorker
lgtomapper	7938/tcp	0.001229	# Legato portmapper
unknown	7938/udp	0.003304
unknown	7946/udp	0.000661
unknown	7948/udp	0.000330
unknown	7949/udp	0.000330
unknown	7953/udp	0.000330
generalsync	7962/tcp	0.000000	# Encrypted, extendable, general-purpose synchronization protocol
unknown	7963/udp	0.000661
unknown	7965/udp	0.000330
supercell	7967/tcp	0.000000
supercell	7967/udp	0.000000
unknown	7969/udp	0.000330
unknown	7975/tcp	0.000076
unknown	7976/udp	0.000330
unknown	7977/udp	0.000330
micromuse-ncps	7979/tcp	0.000000
micromuse-ncps	7979/udp	0.000000
quest-vista	7980/tcp	0.000000	# Quest Vista
quest-vista	7980/udp	0.000330	# Quest Vista
sossd-collect	7981/tcp	0.000000	# Spotlight on SQL Server Desktop Collect
sossd-agent	7982/tcp	0.000000	# sossd-disc | Spotlight on SQL Server Desktop Agent | Spotlight on SQL Server Desktop Agent Discovery
sossd-disc	7982/udp	0.000000	# Spotlight on SQL Server Desktop Agent Discovery
unknown	7985/udp	0.000330
unknown	7988/udp	0.000330
unknown	7991/udp	0.000330
unknown	7993/udp	0.000330
unknown	7994/udp	0.000330
pushns	7997/tcp	0.000000	# PUSH Notification Service
usicontentpush	7998/tcp	0.000076	# USI Content Push Service
usicontentpush	7998/udp	0.000000	# USI Content Push Service
irdmi2	7999/tcp	0.000228
irdmi2	7999/udp	0.000000
http-alt	8000/tcp	0.009710	# irdmi | A common alternative http port | iRDMI
irdmi	8000/udp	0.001652
vcom-tunnel	8001/tcp	0.000532	# VCOM Tunnel
vcom-tunnel	8001/udp	0.001982	# VCOM Tunnel
teradataordbms	8002/tcp	0.001216	# Teradata ORDBMS
teradataordbms	8002/udp	0.000000	# Teradata ORDBMS
mcreport	8003/tcp	0.000076	# Mulberry Connect Reporting Service
mcreport	8003/udp	0.000000	# Mulberry Connect Reporting Service
p2pevolvenet	8004/tcp	0.000000	# Opensource Evolv Enterprise Platform P2P Network Node Connection Protocol
mxi	8005/tcp	0.000076	# MXI Generation II for z/OS
mxi	8005/udp	0.000000	# MXI Generation II for z/OS
wpl-analytics	8006/tcp	0.000076	# wpl-disc | World Programming analytics | World Programming analytics discovery
ajp12	8007/tcp	0.000477	# warppipe | Apache JServ Protocol 1.x | I/O oriented cluster computing software
http	8008/tcp	0.006843	# http-alt | IBM HTTP server | HTTP Alternate
http-alt	8008/udp	0.000330	# HTTP Alternate
ajp13	8009/tcp	0.004642	# nvme-disc | Apache JServ Protocol 1.3 | NVMe over Fabrics Discovery Service
xmpp	8010/tcp	0.002129	# XMPP File Transfer
unknown	8010/udp	0.001652
unknown	8011/tcp	0.000304
unknown	8014/tcp	0.000076
cfg-cloud	8015/tcp	0.000152	# Configuration Cloud Service
ads-s	8016/tcp	0.000152	# Beckhoff Automation Device Specification
cisco-cloudsec	8017/tcp	0.000000	# Cisco Cloudsec Dataplane Port Number
unknown	8018/tcp	0.000076
qbdb	8019/tcp	0.000152	# QB DB Dynamic Port
qbdb	8019/udp	0.000000	# QB DB Dynamic Port
intu-ec-svcdisc	8020/tcp	0.000000	# Intuit Entitlement Service and Discovery
intu-ec-svcdisc	8020/udp	0.000000	# Intuit Entitlement Service and Discovery
ftp-proxy	8021/tcp	0.000627	# intu-ec-client | Common FTP proxy port | Intuit Entitlement Client
intu-ec-client	8021/udp	0.000000	# Intuit Entitlement Client
oa-system	8022/tcp	0.000228
oa-system	8022/udp	0.000000
arca-api	8023/tcp	0.000076	# ARCATrust vault API
unknown	8023/udp	0.000330
ca-audit-da	8025/tcp	0.000076	# CA Audit Distribution Agent
ca-audit-da	8025/udp	0.000000	# CA Audit Distribution Agent
ca-audit-ds	8026/tcp	0.000000	# CA Audit Distribution Server
ca-audit-ds	8026/udp	0.000330	# CA Audit Distribution Server
papachi-p2p-srv	8027/tcp	0.000000	# peer tracker and data relay service
unknown	8029/tcp	0.000076
unknown	8031/tcp	0.002509
pro-ed	8032/tcp	0.000000	# ProEd
pro-ed	8032/udp	0.000000	# ProEd
mindprint	8033/tcp	0.000000
mindprint	8033/udp	0.000000
vantronix-mgmt	8034/tcp	0.000000	# .vantronix Management
vantronix-mgmt	8034/udp	0.000000	# .vantronix Management
unknown	8035/udp	0.000330
unknown	8037/tcp	0.000076
unknown	8037/udp	0.000330
ampify	8040/tcp	0.000000	# Ampify Messaging Protocol
ampify	8040/udp	0.000661	# Ampify Messaging Protocol
enguity-xccetp	8041/tcp	0.000000	# Xcorpeon ASIC Carrier Ethernet Transport
fs-agent	8042/tcp	0.000228	# FireScope Agent
fs-server	8043/tcp	0.000000	# FireScope Server
fs-mgmt	8044/tcp	0.000000	# FireScope Management Interface
unknown	8045/tcp	0.000228
unknown	8048/udp	0.000330
unknown	8050/tcp	0.000152
rocrail	8051/tcp	0.000000	# Rocrail Client Service
senomix01	8052/tcp	0.000076	# Senomix Timesheets Server
senomix01	8052/udp	0.000000	# Senomix Timesheets Server
senomix02	8053/tcp	0.000000	# Senomix Timesheets Client [1 year assignment]
senomix02	8053/udp	0.000000	# Senomix Timesheets Client [1 year assignment]
senomix03	8054/tcp	0.000000	# Senomix Timesheets Server [1 year assignment]
senomix03	8054/udp	0.000000	# Senomix Timesheets Server [1 year assignment]
senomix04	8055/tcp	0.000000	# Senomix Timesheets Server [1 year assignment]
senomix04	8055/udp	0.000000	# Senomix Timesheets Server [1 year assignment]
senomix05	8056/tcp	0.000000	# Senomix Timesheets Server [1 year assignment]
senomix05	8056/udp	0.000000	# Senomix Timesheets Server [1 year assignment]
senomix06	8057/tcp	0.000000	# Senomix Timesheets Client [1 year assignment]
senomix06	8057/udp	0.000000	# Senomix Timesheets Client [1 year assignment]
senomix07	8058/tcp	0.000000	# Senomix Timesheets Client [1 year assignment]
senomix07	8058/udp	0.000000	# Senomix Timesheets Client [1 year assignment]
senomix08	8059/tcp	0.000000	# Senomix Timesheets Client [1 year assignment]
senomix08	8059/udp	0.000000	# Senomix Timesheets Client [1 year assignment]
aero	8060/tcp	0.000076	# Asymmetric Extended Route Optimization (AERO)
nikatron-dev	8061/tcp	0.000000	# Nikatron Device Protocol
unknown	8064/tcp	0.000076
unknown	8064/udp	0.000330
toad-bi-appsrvr	8066/tcp	0.000000	# Toad BI Application Server
unknown	8066/udp	0.000330
infi-async	8067/tcp	0.000000	# Infinidat async replication
ucs-isc	8070/tcp	0.000000	# Oracle Unified Communication Suite's Indexed Search Converter
gadugadu	8074/tcp	0.000000	# Gadu-Gadu
gadugadu	8074/udp	0.000000	# Gadu-Gadu
slnp	8076/tcp	0.000050	# SLNP (Simple Library Network Protocol) by Sisis Informationssysteme GmbH
mles	8077/tcp	0.000000	# Mles is a client-server data distribution protocol targeted to serve as a lightweight and reliable distributed publish/subscribe database service.
unknown	8079/udp	0.000330
http-proxy	8080/tcp	0.042052	# http-alt | Common HTTP proxy/second web server port | HTTP Alternate (see port 80)
http-alt	8080/udp	0.000000	# HTTP Alternate (see port 80)
blackice-icecap	8081/tcp	0.006147	# sunproxyadmin | ICECap user console | Sun Proxy Admin Service
sunproxyadmin	8081/udp	0.000000	# Sun Proxy Admin Service
blackice-alerts	8082/tcp	0.000878	# us-cli | BlackIce Alerts sent to this port | Utilistor (Client)
us-cli	8082/udp	0.000000	# Utilistor (Client)
us-srv	8083/tcp	0.000532	# Utilistor (Server)
us-srv	8083/udp	0.000000	# Utilistor (Server)
websnp	8084/tcp	0.000532	# Snarl Network Protocol over HTTP
unknown	8085/tcp	0.000684
d-s-n	8086/tcp	0.000380	# Distributed SCADA Networking Rendezvous Port
d-s-n	8086/udp	0.000000	# Distributed SCADA Networking Rendezvous Port
simplifymedia	8087/tcp	0.000380	# Simplify Media SPP Protocol
simplifymedia	8087/udp	0.000000	# Simplify Media SPP Protocol
radan-http	8088/tcp	0.000608	# Radan HTTP
radan-http	8088/udp	0.000000	# Radan HTTP
unknown	8089/tcp	0.000760
opsmessaging	8090/tcp	0.000304	# Vehicle to station messaging
jamlink	8091/tcp	0.000000	# Jam Link Framework
unknown	8092/tcp	0.000076
unknown	8093/tcp	0.000228
unknown	8095/tcp	0.000152
sac	8097/tcp	0.000152	# SAC Port Id
sac	8097/udp	0.000000	# SAC Port Id
unknown	8098/tcp	0.000152
unknown	8099/tcp	0.000228
xprint-server	8100/tcp	0.000304	# Xprint Server
xprint-server	8100/udp	0.000000	# Xprint Server
ldoms-migr	8101/tcp	0.000000	# Logical Domains Migration
kz-migr	8102/tcp	0.000000	# Oracle Kernel zones migration server
unknown	8110/tcp	0.000076
skynetflow	8111/tcp	0.000000	# Skynetflow network services
unknown	8112/udp	0.000330
mtl8000-matrix	8115/tcp	0.000000	# MTL8000 Matrix
mtl8000-matrix	8115/udp	0.000330	# MTL8000 Matrix
cp-cluster	8116/tcp	0.000076	# Check Point Clustering
cp-cluster	8116/udp	0.000000	# Check Point Clustering
purityrpc	8117/tcp	0.000000	# Purity replication clustering and remote management
privoxy	8118/tcp	0.000138	# Privoxy, www.privoxy.org | Privoxy HTTP proxy
privoxy	8118/udp	0.000000	# Privoxy HTTP proxy
apollo-data	8121/tcp	0.000000	# Apollo Data Port
apollo-data	8121/udp	0.000000	# Apollo Data Port
apollo-admin	8122/tcp	0.000000	# Apollo Admin Port
apollo-admin	8122/udp	0.000000	# Apollo Admin Port
polipo	8123/tcp	0.000038	# Polipo open source web proxy cache
paycash-online	8128/tcp	0.000000	# PayCash Online Protocol
paycash-online	8128/udp	0.000000	# PayCash Online Protocol
paycash-wbp	8129/tcp	0.000000	# PayCash Wallet-Browser
paycash-wbp	8129/udp	0.000000	# PayCash Wallet-Browser
indigo-vrmi	8130/tcp	0.000000
indigo-vrmi	8130/udp	0.000000
indigo-vbcp	8131/tcp	0.000000
indigo-vbcp	8131/udp	0.000000
dbabble	8132/tcp	0.000000
dbabble	8132/udp	0.000000
unknown	8133/tcp	0.000076
unknown	8136/udp	0.000330
puppet	8140/tcp	0.000000	# The Puppet server service | The Puppet master service
unknown	8143/udp	0.000330
unknown	8144/tcp	0.000076
unknown	8144/udp	0.000330
unknown	8145/udp	0.000330
unknown	8146/udp	0.000330
isdd	8148/tcp	0.000000	# i-SDD file transfer
isdd	8148/udp	0.000000	# i-SDD file transfer
eor-game	8149/tcp	0.000000	# Edge of Reality game data
quantastor	8153/tcp	0.000000	# QuantaStor Management Interface
patrol	8160/tcp	0.000000
patrol	8160/udp	0.000000
patrol-snmp	8161/tcp	0.000000	# Patrol SNMP
patrol-snmp	8161/udp	0.000000	# Patrol SNMP
lpar2rrd	8162/tcp	0.000000	# LPAR2RRD client server communication
unknown	8162/udp	0.000330
unknown	8168/udp	0.000330
unknown	8171/udp	0.000330
unknown	8180/tcp	0.000304
intermapper	8181/tcp	0.000380	# Intermapper network management system
unknown	8181/udp	0.001982
vmware-fdm	8182/tcp	0.000000	# VMware Fault Domain Manager
vmware-fdm	8182/udp	0.000330	# VMware Fault Domain Manager
proremote	8183/tcp	0.000000
itach	8184/tcp	0.000000	# Remote iTach Connection
itach	8184/udp	0.000000	# Remote iTach Connection
unknown	8185/udp	0.000330
unknown	8189/tcp	0.000152
gcp-rphy	8190/tcp	0.000000	# Generic control plane for RPHY
limnerpressure	8191/tcp	0.000000	# Limner Pressure
sophos	8192/tcp	0.000760	# spytechphone | Sophos Remote Management System | SpyTech Phone Service
sophos	8192/udp	0.000000	# Sophos Remote Management System
sophos	8193/tcp	0.000760	# Sophos Remote Management System
sophos	8193/udp	0.002973	# Sophos Remote Management System
sophos	8194/tcp	0.000760	# blp1 | Sophos Remote Management System | Bloomberg data API
sophos	8194/udp	0.000000	# Sophos Remote Management System
blp2	8195/tcp	0.000000	# Bloomberg feed
blp2	8195/udp	0.000000	# Bloomberg feed
vvr-data	8199/tcp	0.000000	# VVR DATA
vvr-data	8199/udp	0.000330	# VVR DATA
trivnet1	8200/tcp	0.000228	# TRIVNET
trivnet1	8200/udp	0.000000	# TRIVNET
trivnet2	8201/tcp	0.000076	# TRIVNET
trivnet2	8201/udp	0.000661	# TRIVNET
aesop	8202/tcp	0.000076	# Audio+Ethernet Standard Open Protocol
lm-perfworks	8204/tcp	0.000000	# LM Perfworks
lm-perfworks	8204/udp	0.000000	# LM Perfworks
lm-instmgr	8205/tcp	0.000000	# LM Instmgr
lm-instmgr	8205/udp	0.000000	# LM Instmgr
lm-dta	8206/tcp	0.000000	# LM Dta
lm-dta	8206/udp	0.000000	# LM Dta
lm-sserver	8207/tcp	0.000000	# LM SServer
lm-sserver	8207/udp	0.000991	# LM SServer
lm-webwatcher	8208/tcp	0.000000	# LM Webwatcher
lm-webwatcher	8208/udp	0.000000	# LM Webwatcher
aruba-papi	8211/tcp	0.000000	# Aruba Networks AP management
unknown	8215/udp	0.000330
unknown	8216/udp	0.000330
unknown	8221/udp	0.000330
unknown	8222/tcp	0.000380
unknown	8228/udp	0.000330
rexecj	8230/tcp	0.000000	# RexecJ Server
rexecj	8230/udp	0.000000	# RexecJ Server
hncp-udp-port	8231/tcp	0.000000	# HNCP
hncp-dtls-port	8232/tcp	0.000076	# HNCP over DTLS
unknown	8235/udp	0.000330
synapse-nhttps	8243/tcp	0.000000	# Synapse Non Blocking HTTPS
synapse-nhttps	8243/udp	0.000000	# Synapse Non Blocking HTTPS
unknown	8245/tcp	0.000076
unknown	8248/tcp	0.000076
unknown	8254/tcp	0.000304
unknown	8255/tcp	0.000076
unknown	8255/udp	0.000330
unknown	8262/udp	0.000330
unknown	8265/udp	0.000330
espeasy-p2p	8266/tcp	0.000000	# ESPeasy peer-2-peer communication
unknown	8268/tcp	0.000076
robot-remote	8270/tcp	0.000000	# Robot Framework Remote Library Interface
unknown	8271/udp	0.000330
unknown	8273/tcp	0.000076
pando-sec	8276/tcp	0.000000	# ms-mcc | Pando Media Controlled Distribution | Microsoft Connected Cache
pando-sec	8276/udp	0.000000	# Pando Media Controlled Distribution
synapse-nhttp	8280/tcp	0.000000	# Synapse Non Blocking HTTP
synapse-nhttp	8280/udp	0.000000	# Synapse Non Blocking HTTP
libelle	8282/tcp	0.000076	# libelle-disc | Libelle EnterpriseBus | Libelle EnterpriseBus discovery
unknown	8282/udp	0.000330
unknown	8284/udp	0.000661
unknown	8289/udp	0.000330
unknown	8290/tcp	0.000228
unknown	8291/tcp	0.000456
blp3	8292/tcp	0.000228	# Bloomberg professional
blp3	8292/udp	0.000330	# Bloomberg professional
hiperscan-id	8293/tcp	0.000152	# Hiperscan Identification Service
blp4	8294/tcp	0.000152	# Bloomberg intelligent client
blp4	8294/udp	0.000000	# Bloomberg intelligent client
unknown	8295/tcp	0.000076
tmi	8300/tcp	0.000228	# Transport Management Interface
tmi	8300/udp	0.000000	# Transport Management Interface
amberon	8301/tcp	0.000000	# Amberon PPC/PPS
amberon	8301/udp	0.000000	# Amberon PPC/PPS
unknown	8308/tcp	0.000076
unknown	8310/udp	0.000330
unknown	8312/udp	0.000330
hub-open-net	8313/tcp	0.000000	# Hub Open Network
unknown	8316/udp	0.000330
unknown	8319/udp	0.000330
tnp-discover	8320/tcp	0.000000	# Thin(ium) Network Protocol
tnp-discover	8320/udp	0.000000	# Thin(ium) Network Protocol
tnp	8321/tcp	0.000000	# Thin(ium) Network Protocol
tnp	8321/udp	0.000330	# Thin(ium) Network Protocol
garmin-marine	8322/tcp	0.000000	# Garmin Marine
unknown	8329/udp	0.000330
bitcoin	8333/tcp	0.000380	# Bitcoin crypto currency - https://en.bitcoin.it/wiki/Running_Bitcoin
unknown	8336/udp	0.000661
unknown	8338/udp	0.000330
unknown	8339/tcp	0.000076
unknown	8343/udp	0.000661
unknown	8347/udp	0.000330
server-find	8351/tcp	0.000000	# Server Find
server-find	8351/udp	0.000000	# Server Find
unknown	8359/udp	0.000330
unknown	8361/udp	0.000330
unknown	8363/udp	0.000330
unknown	8371/udp	0.000330
unknown	8374/udp	0.000330
cruise-enum	8376/tcp	0.000000	# Cruise ENUM
cruise-enum	8376/udp	0.000000	# Cruise ENUM
cruise-swroute	8377/tcp	0.000000	# Cruise SWROUTE
cruise-swroute	8377/udp	0.000000	# Cruise SWROUTE
cruise-config	8378/tcp	0.000000	# Cruise CONFIG
cruise-config	8378/udp	0.000000	# Cruise CONFIG
cruise-diags	8379/tcp	0.000000	# Cruise DIAGS
cruise-diags	8379/udp	0.000000	# Cruise DIAGS
cruise-update	8380/tcp	0.000000	# Cruise UPDATE
cruise-update	8380/udp	0.000000	# Cruise UPDATE
unknown	8382/udp	0.000330
m2mservices	8383/tcp	0.000228	# M2m Services
m2mservices	8383/udp	0.000000	# M2m Services
marathontp	8384/tcp	0.000000	# Marathon Transport Protocol
unknown	8385/tcp	0.000152
unknown	8386/udp	0.000330
unknown	8388/udp	0.000330
unknown	8393/udp	0.000330
cvd	8400/tcp	0.000380
cvd	8400/udp	0.000000
sabarsd	8401/tcp	0.000076
sabarsd	8401/udp	0.000000
abarsd	8402/tcp	0.000380
abarsd	8402/udp	0.000661
admind	8403/tcp	0.000076
admind	8403/udp	0.000330
svcloud	8404/tcp	0.000000	# SuperVault Cloud
svbackup	8405/tcp	0.000000	# SuperVault Backup
unknown	8409/tcp	0.000076
unknown	8409/udp	0.000330
unknown	8411/udp	0.000330
dlpx-sp	8415/tcp	0.000000	# Delphix Session Protocol
espeech	8416/tcp	0.000000	# eSpeech Session Protocol
espeech	8416/udp	0.000000	# eSpeech Session Protocol
espeech-rtp	8417/tcp	0.000000	# eSpeech RTP Protocol
espeech-rtp	8417/udp	0.000000	# eSpeech RTP Protocol
aritts	8423/tcp	0.000000	# Aristech text-to-speech server
unknown	8424/udp	0.000330
unknown	8429/udp	0.000330
unknown	8431/udp	0.000330
pgbackrest	8432/tcp	0.000000	# PostgreSQL Backup
aws-as2	8433/tcp	0.000000	# Non Persistent Desktop and Application Streaming
unknown	8435/udp	0.000991
cybro-a-bus	8442/tcp	0.000000	# CyBro A-bus Protocol
cybro-a-bus	8442/udp	0.000330	# CyBro A-bus Protocol
https-alt	8443/tcp	0.009986	# pcsync-https | Common alternative https port | PCsync HTTPS
pcsync-https	8443/udp	0.000000	# PCsync HTTPS
pcsync-http	8444/tcp	0.000000	# PCsync HTTP
pcsync-http	8444/udp	0.000000	# PCsync HTTP
copy	8445/tcp	0.000076	# copy-disc | Port for copy peer sync feature | Port for copy discovery
unknown	8447/udp	0.000330
matrix-fed	8448/tcp	0.000000	# Matrix Federation Protocol
npmp	8450/tcp	0.000000
npmp	8450/udp	0.000000
unknown	8451/tcp	0.000076
unknown	8452/tcp	0.000076
unknown	8453/tcp	0.000076
unknown	8454/tcp	0.000076
unknown	8455/tcp	0.000076
unknown	8455/udp	0.000330
nexentamv	8457/tcp	0.000000	# Nexenta Management GUI
unknown	8458/udp	0.000330
unknown	8468/udp	0.000330
cisco-avp	8470/tcp	0.000076	# Cisco Address Validation Protocol
pim-port	8471/sctp	0.000000	# PIM over Reliable Transport
pim-port	8471/tcp	0.000076	# PIM over Reliable Transport
pim-port	8471/udp	0.000330	# PIM over Reliable Transport
otv	8472/tcp	0.000076	# Overlay Transport Virtualization (OTV)
otv	8472/udp	0.000000	# Overlay Transport Virtualization (OTV)
vp2p	8473/tcp	0.000000	# Virtual Point to Point
vp2p	8473/udp	0.000330	# Virtual Point to Point
noteshare	8474/tcp	0.000076	# AquaMinds NoteShare
noteshare	8474/udp	0.000000	# AquaMinds NoteShare
unknown	8475/udp	0.000330
unknown	8477/tcp	0.000076
unknown	8479/tcp	0.000076
unknown	8481/tcp	0.000152
unknown	8482/udp	0.000330
unknown	8484/tcp	0.000076
fmtp	8500/tcp	0.000304	# Flight Message Transfer Protocol
fmtp	8500/udp	0.000000	# Flight Message Transfer Protocol
cmtp-mgt	8501/tcp	0.000000	# cmtp-av | CYTEL Message Transfer Management | CYTEL Message Transfer Audio and Video
ftnmtp	8502/tcp	0.000000	# FTN Message Transfer Protocol
lsp-self-ping	8503/tcp	0.000000	# MPLS LSP Self-Ping
unknown	8508/udp	0.000330
unknown	8515/tcp	0.000076
unknown	8520/udp	0.000330
unknown	8530/tcp	0.000076
unknown	8531/tcp	0.000076
unknown	8531/udp	0.000330
unknown	8538/udp	0.000330
unknown	8539/tcp	0.000076
unknown	8540/tcp	0.000152
unknown	8548/udp	0.000330
rtsp-alt	8554/tcp	0.000000	# RTSP Alternate (see port 554)
rtsp-alt	8554/udp	0.000000	# RTSP Alternate (see port 554)
d-fence	8555/tcp	0.000000	# SYMAX D-FENCE
d-fence	8555/udp	0.000000	# SYMAX D-FENCE
unknown	8556/udp	0.000661
unknown	8562/tcp	0.000076
oap-admin	8567/tcp	0.000000	# dof-tunnel | Object Access Protocol Administration | DOF Tunneling Protocol
oap-admin	8567/udp	0.000000	# Object Access Protocol Administration
unknown	8569/udp	0.000330
unknown	8573/udp	0.000330
unknown	8576/udp	0.000330
unknown	8577/udp	0.000330
unknown	8578/udp	0.000330
unknown	8585/udp	0.000330
unknown	8591/udp	0.000661
unknown	8597/udp	0.000330
asterix	8600/tcp	0.000380	# Surveillance Data
asterix	8600/udp	0.000000	# Surveillance Data
unknown	8601/tcp	0.000076
canon-cpp-disc	8609/tcp	0.000000	# Canon Compact Printer Protocol Discovery
canon-mfnp	8610/tcp	0.000000	# Canon MFNP Service
canon-mfnp	8610/udp	0.000000	# Canon MFNP Service
canon-bjnp1	8611/tcp	0.000000	# Canon BJNP Port 1
canon-bjnp1	8611/udp	0.000330	# Canon BJNP Port 1
canon-bjnp2	8612/tcp	0.000000	# Canon BJNP Port 2
canon-bjnp2	8612/udp	0.000330	# Canon BJNP Port 2
canon-bjnp3	8613/tcp	0.000000	# Canon BJNP Port 3
canon-bjnp3	8613/udp	0.000330	# Canon BJNP Port 3
canon-bjnp4	8614/tcp	0.000000	# Canon BJNP Port 4
canon-bjnp4	8614/udp	0.000330	# Canon BJNP Port 4
imink	8615/tcp	0.000000	# Imink Service Control
unknown	8621/tcp	0.000076
unknown	8632/udp	0.000330
unknown	8635/udp	0.000330
unknown	8640/tcp	0.000076
unknown	8644/tcp	0.000076
unknown	8648/tcp	0.000152
unknown	8649/tcp	0.000380
unknown	8651/tcp	0.000760
unknown	8652/tcp	0.000760
unknown	8652/udp	0.000330
unknown	8654/tcp	0.000304
unknown	8655/tcp	0.000076
unknown	8655/udp	0.000330
unknown	8658/tcp	0.000076
unknown	8661/udp	0.000661
monetra	8665/tcp	0.000000
monetra-admin	8666/tcp	0.000000	# Monetra Administrative Access
unknown	8666/udp	0.000330
unknown	8667/udp	0.000330
spartan	8668/tcp	0.000000	# Spartan management
unknown	8673/tcp	0.000076
unknown	8674/udp	0.000330
msi-cps-rm	8675/tcp	0.000152	# msi-cps-rm-disc | Motorola Solutions Customer Programming Software for Radio Management | Motorola Solutions Customer Programming Software for Radio Management Discovery
unknown	8676/tcp	0.000152
unknown	8679/udp	0.000330
unknown	8680/tcp	0.000076
unknown	8684/udp	0.000661
sun-as-jmxrmi	8686/tcp	0.000152	# Sun App Server - JMX/RMI
sun-as-jmxrmi	8686/udp	0.000000	# Sun App Server - JMX/RMI
openremote-ctrl	8688/tcp	0.000000	# OpenRemote Controller HTTP/REST
unknown	8692/udp	0.000330
unknown	8694/udp	0.000330
vnyx	8699/tcp	0.000000	# VNYX Primary Port
vnyx	8699/udp	0.000000	# VNYX Primary Port
unknown	8701/tcp	0.000760
unknown	8701/udp	0.000330
semi-grpc	8710/tcp	0.000000	# gRPC for SEMI Standards implementations
nvc	8711/tcp	0.000000	# Nuance Voice Control
unknown	8715/udp	0.000330
unknown	8719/udp	0.000661
unknown	8720/udp	0.000330
unknown	8724/udp	0.000330
unknown	8726/udp	0.000330
dtp-net	8732/tcp	0.000000	# DASGIP Net Services
dtp-net	8732/udp	0.000000	# DASGIP Net Services
ibus	8733/tcp	0.000000
ibus	8733/udp	0.000000
unknown	8736/tcp	0.000076
unknown	8742/udp	0.000661
unknown	8748/udp	0.000330
dey-keyneg	8750/tcp	0.000000	# DEY Storage Key Negotiation
unknown	8752/tcp	0.000076
unknown	8752/udp	0.000330
unknown	8756/tcp	0.000076
unknown	8760/udp	0.000330
mc-appserver	8763/tcp	0.000000
mc-appserver	8763/udp	0.000000
openqueue	8764/tcp	0.000000
openqueue	8764/udp	0.000000
ultraseek-http	8765/tcp	0.000152	# Ultraseek HTTP
ultraseek-http	8765/udp	0.000000	# Ultraseek HTTP
amcs	8766/tcp	0.000152	# Agilent Connectivity Service
core-of-source	8767/tcp	0.000000	# Online mobile multiplayer game
sandpolis	8768/tcp	0.000000	# Sandpolis Server
oktaauthenticat	8769/tcp	0.000000	# Okta MultiPlatform Access Mgmt for Cloud Svcs
apple-iphoto	8770/tcp	0.000025	# dpap | Apple iPhoto sharing | Digital Photo Access Protocol (iPhoto)
dpap	8770/udp	0.000000	# Digital Photo Access Protocol
unknown	8772/tcp	0.000076
unknown	8777/udp	0.000330
uec	8778/tcp	0.000000	# Stonebranch Universal Enterprise Controller
unknown	8780/udp	0.000330
msgclnt	8786/tcp	0.000000	# Message Client
msgclnt	8786/udp	0.000000	# Message Client
msgsrvr	8787/tcp	0.000000	# Message Server
msgsrvr	8787/udp	0.000000	# Message Server
unknown	8790/tcp	0.000076
acd-pm	8793/tcp	0.000000	# Accedian Performance Measurement
unknown	8793/udp	0.000661
unknown	8798/tcp	0.000076
unknown	8798/udp	0.000330
sunwebadmin	8800/tcp	0.000228	# Sun Web Server Admin Service
sunwebadmin	8800/udp	0.000000	# Sun Web Server Admin Service
unknown	8801/tcp	0.000076
truecm	8804/tcp	0.000000
truecm	8804/udp	0.000000
pfcp	8805/tcp	0.000000	# Destination Port number for PFCP
unknown	8805/udp	0.000330
unknown	8806/udp	0.000330
hes-clip	8807/tcp	0.000000	# HES-CLIP Interoperability protocol
unknown	8807/udp	0.000330
ssports-bcast	8808/tcp	0.000000	# STATSports Broadcast Service
3gpp-monp	8809/tcp	0.000000	# MCPTT Off-Network Protocol (MONP)
unknown	8814/udp	0.000330
unknown	8818/udp	0.000330
unknown	8819/udp	0.000330
unknown	8820/udp	0.000661
unknown	8828/udp	0.000330
unknown	8831/udp	0.000330
unknown	8832/udp	0.000330
nessus-xmlrpc	8834/tcp	0.000000
unknown	8837/udp	0.000330
unknown	8841/udp	0.000330
unknown	8843/tcp	0.000076
unknown	8848/udp	0.000330
unknown	8853/udp	0.000330
unknown	8865/tcp	0.000076
unknown	8865/udp	0.000330
unknown	8867/udp	0.000330
dxspider	8873/tcp	0.000380	# dxspider linking protocol
dxspider	8873/udp	0.000000	# dxspider linking protocol
unknown	8877/tcp	0.000152
unknown	8878/tcp	0.000076
unknown	8879/tcp	0.000076
cddbp-alt	8880/tcp	0.000076	# CDDBP
cddbp-alt	8880/udp	0.000000	# CDDBP
galaxy4d	8881/tcp	0.000000	# Galaxy4D Online Game Engine
unknown	8882/tcp	0.000076
secure-mqtt	8883/tcp	0.000076	# Secure MQTT
secure-mqtt	8883/udp	0.000000	# Secure MQTT
unknown	8885/udp	0.000330
unknown	8886/udp	0.000330
unknown	8887/tcp	0.000076
sun-answerbook	8888/tcp	0.016522	# ddi-udp-1 | ddi-tcp-1 | Sun Answerbook HTTP server.  Or gnump3d streaming music server | NewsEDGE server TCP (TCP 1) | NewsEDGE server UDP (UDP 1)
ddi-udp-1	8888/udp	0.000000	# NewsEDGE server UDP (UDP 1)
ddi-tcp-2	8889/tcp	0.000152	# ddi-udp-2 | Desktop Data TCP 1 | NewsEDGE server broadcast
ddi-udp-2	8889/udp	0.000000	# NewsEDGE server broadcast
ddi-tcp-3	8890/tcp	0.000000	# ddi-udp-3 | Desktop Data TCP 2 | NewsEDGE client broadcast
ddi-udp-3	8890/udp	0.000000	# NewsEDGE client broadcast
ddi-tcp-4	8891/tcp	0.000000	# ddi-udp-4 | Desktop Data TCP 3: NESS application | Desktop Data UDP 3: NESS application
ddi-udp-4	8891/udp	0.000000	# Desktop Data UDP 3: NESS application
seosload	8892/tcp	0.000038	# ddi-udp-5 | ddi-tcp-5 | From the new Computer Associates eTrust ACX | Desktop Data TCP 4: FARM product | Desktop Data UDP 4: FARM product
ddi-udp-5	8892/udp	0.000000	# Desktop Data UDP 4: FARM product
ddi-tcp-6	8893/tcp	0.000000	# ddi-udp-6 | Desktop Data TCP 5: NewsEDGE/Web application | Desktop Data UDP 5: NewsEDGE/Web application
ddi-udp-6	8893/udp	0.000000	# Desktop Data UDP 5: NewsEDGE/Web application
ddi-tcp-7	8894/tcp	0.000000	# ddi-udp-7 | Desktop Data TCP 6: COAL application | Desktop Data UDP 6: COAL application
ddi-udp-7	8894/udp	0.000000	# Desktop Data UDP 6: COAL application
unknown	8896/udp	0.000330
unknown	8898/tcp	0.000076
ospf-lite	8899/tcp	0.000608
ospf-lite	8899/udp	0.000330
jmb-cds1	8900/tcp	0.000076	# JMB-CDS 1
jmb-cds1	8900/udp	0.001321	# JMB-CDS 1
jmb-cds2	8901/tcp	0.000000	# JMB-CDS 2
jmb-cds2	8901/udp	0.000330	# JMB-CDS 2
unknown	8907/udp	0.000330
dpp	8908/tcp	0.000000	# WFA Device Provisioning Protocol
manyone-http	8910/tcp	0.000000
manyone-http	8910/udp	0.000330
manyone-xml	8911/tcp	0.000000
manyone-xml	8911/udp	0.000000
wcbackup	8912/tcp	0.000000	# Windows Client Backup
wcbackup	8912/udp	0.000000	# Windows Client Backup
dragonfly	8913/tcp	0.000000	# Dragonfly System Service
dragonfly	8913/udp	0.000000	# Dragonfly System Service
unknown	8919/udp	0.000330
unknown	8924/udp	0.000661
unknown	8925/tcp	0.000076
unknown	8929/udp	0.000330
unknown	8933/udp	0.000330
unknown	8934/udp	0.000661
twds	8937/tcp	0.000000	# Transaction Warehouse Data Service
unknown	8938/udp	0.000330
unknown	8939/udp	0.000330
ub-dns-control	8953/tcp	0.000000	# unbound dns nameserver control
cumulus-admin	8954/tcp	0.000076	# Cumulus Admin Port
cumulus-admin	8954/udp	0.000000	# Cumulus Admin Port
unknown	8959/udp	0.000330
unknown	8964/udp	0.000330
unknown	8966/udp	0.000330
unknown	8971/udp	0.000330
unknown	8976/udp	0.000330
unknown	8979/udp	0.000661
nod-provider	8980/tcp	0.000076	# Network of Devices Provider
nod-client	8981/tcp	0.000000	# Network of Devices Client
unknown	8987/tcp	0.000152
sunwebadmins	8989/tcp	0.000000	# Sun Web Server SSL Admin Service
sunwebadmins	8989/udp	0.000000	# Sun Web Server SSL Admin Service
http-wmap	8990/tcp	0.000000	# webmail HTTP service
http-wmap	8990/udp	0.000000	# webmail HTTP service
https-wmap	8991/tcp	0.000000	# webmail HTTPS service
https-wmap	8991/udp	0.000000	# webmail HTTPS service
unknown	8994/tcp	0.000380
unknown	8996/tcp	0.000152
oracle-ms-ens	8997/tcp	0.000000	# Oracle Messaging Server Event Notification Service
canto-roboflow	8998/tcp	0.000000	# Canto RoboFlow Control
unknown	8998/udp	0.000661
bctp	8999/tcp	0.000076	# Brodos Crypto Trade Protocol
bctp	8999/udp	0.000000	# Brodos Crypto Trade Protocol
cslistener	9000/tcp	0.002129
cslistener	9000/udp	0.001652
tor-orport	9001/tcp	0.001216	# etlservicemgr | Tor ORPort | ETL Service Manager
etlservicemgr	9001/udp	0.001652	# ETL Service Manager
dynamid	9002/tcp	0.000380	# DynamID authentication
dynamid	9002/udp	0.000661	# DynamID authentication
unknown	9003/tcp	0.000228
unknown	9004/tcp	0.000076
golem	9005/tcp	0.000076	# Golem Inter-System RPC
unknown	9006/udp	0.000330
ogs-client	9007/tcp	0.000000	# Open Grid Services Client
ogs-client	9007/udp	0.000000	# Open Grid Services Client
ogs-server	9008/tcp	0.000000	# Open Grid Services Server
pichat	9009/tcp	0.000456	# Pichat Server
pichat	9009/udp	0.000000	# Pichat Server
sdr	9010/tcp	0.000380	# Secure Data Replicator Protocol
d-star	9011/tcp	0.000380	# D-Star Routing digital voice+data for amateur radio
unknown	9011/udp	0.000330
unknown	9013/tcp	0.000076
unknown	9017/udp	0.000330
tambora	9020/tcp	0.000076
tambora	9020/udp	0.001982
panagolin-ident	9021/tcp	0.000076	# Pangolin Identification
panagolin-ident	9021/udp	0.000000	# Pangolin Identification
paragent	9022/tcp	0.000076	# PrivateArk Remote Agent
paragent	9022/udp	0.000000	# PrivateArk Remote Agent
swa-1	9023/tcp	0.000000	# Secure Web Access - 1
swa-1	9023/udp	0.000000	# Secure Web Access - 1
swa-2	9024/tcp	0.000000	# Secure Web Access - 2
swa-2	9024/udp	0.000000	# Secure Web Access - 2
swa-3	9025/tcp	0.000000	# Secure Web Access - 3
swa-3	9025/udp	0.000000	# Secure Web Access - 3
swa-4	9026/tcp	0.000000	# Secure Web Access - 4
swa-4	9026/udp	0.000000	# Secure Web Access - 4
unknown	9027/udp	0.000330
unknown	9028/udp	0.000330
unknown	9034/udp	0.000330
unknown	9037/tcp	0.000076
tor-trans	9040/tcp	0.000301	# Tor TransPort, www.torproject.org
unknown	9041/udp	0.000330
unknown	9044/tcp	0.000076
tor-socks	9050/tcp	0.000703	# versiera | Tor SocksPort, www.torproject.org | Versiera Agent Listener
tor-control	9051/tcp	0.000025	# fio-cmgmt | Tor ControlPort, www.torproject.org | Fusion-io Central Manager Service
unknown	9053/udp	0.000991
unknown	9055/udp	0.000330
CardWeb-IO	9060/tcp	0.000000	# CardWeb-RT | CardWeb request-response I/O exchange | CardWeb realtime device data
unknown	9061/tcp	0.000076
unknown	9061/udp	0.000330
unknown	9064/udp	0.000330
unknown	9065/tcp	0.000076
unknown	9070/udp	0.000330
unknown	9071/tcp	0.000608
unknown	9079/udp	0.000661
glrpc	9080/tcp	0.000380	# Groove GLRPC
glrpc	9080/udp	0.000330	# Groove GLRPC
cisco-aqos	9081/tcp	0.000228	# Required for Adaptive Quality of Service
lcs-ap	9082/sctp	0.000000	# LCS Application Protocol
emc-pp-mgmtsvc	9083/tcp	0.000000	# EMC PowerPath Mgmt Service
aurora	9084/sctp	0.000000	# IBM AURORA Performance Visualizer
aurora	9084/tcp	0.000076	# IBM AURORA Performance Visualizer
aurora	9084/udp	0.000000	# IBM AURORA Performance Visualizer
ibm-rsyscon	9085/tcp	0.000000	# IBM Remote System Console
ibm-rsyscon	9085/udp	0.000330	# IBM Remote System Console
net2display	9086/tcp	0.000000	# Vesa Net2Display
net2display	9086/udp	0.000330	# Vesa Net2Display
classic	9087/tcp	0.000000	# Classic Data Server
classic	9087/udp	0.000000	# Classic Data Server
sqlexec	9088/tcp	0.000000	# IBM Informix SQL Interface
sqlexec	9088/udp	0.000330	# IBM Informix SQL Interface
sqlexec-ssl	9089/tcp	0.000000	# IBM Informix SQL Interface - Encrypted
sqlexec-ssl	9089/udp	0.000330	# IBM Informix SQL Interface - Encrypted
zeus-admin	9090/tcp	0.002747	# websm | Zeus admin server | WebSM
websm	9090/udp	0.000000
xmltec-xmlmail	9091/tcp	0.000304
xmltec-xmlmail	9091/udp	0.000330
XmlIpcRegSvc	9092/tcp	0.000000	# Xml-Ipc Server Reg
XmlIpcRegSvc	9092/udp	0.000000	# Xml-Ipc Server Reg
copycat	9093/tcp	0.000000	# Copycat database replication service
unknown	9098/tcp	0.000152
unknown	9098/udp	0.000330
unknown	9099/tcp	0.000228
jetdirect	9100/tcp	0.003287	# pdl-datastream | hp-pdl-datastr | HP JetDirect card | PDL Data Streaming Port | Printer PDL Data Stream
hp-pdl-datastr	9100/udp	0.000000	# PDL Data Streaming Port
jetdirect	9101/tcp	0.000602	# bacula-dir | HP JetDirect card | Bacula Director
bacula-dir	9101/udp	0.000330	# Bacula Director
jetdirect	9102/tcp	0.002133	# bacula-fd | HP JetDirect card. Also used (and officially registered for) Bacula File Daemon (an open source backup system) | Bacula File Daemon
bacula-fd	9102/udp	0.000000	# Bacula File Daemon
jetdirect	9103/tcp	0.000188	# bacula-sd | HP JetDirect card | Bacula Storage Daemon
bacula-sd	9103/udp	0.002313	# Bacula Storage Daemon
jetdirect	9104/tcp	0.000050	# peerwire | HP JetDirect card | PeerWire
peerwire	9104/udp	0.000000
jetdirect	9105/tcp	0.000038	# xadmin | HP JetDirect card | Xadmin Control Service
xadmin	9105/udp	0.000000	# Xadmin Control Service
jetdirect	9106/tcp	0.000038	# astergate-disc | astergate | HP JetDirect card | Astergate Control Service | Astergate Discovery Service
astergate-disc	9106/udp	0.000000	# Astergate Discovery Service
jetdirect	9107/tcp	0.000038	# astergatefax | HP JetDirect card | AstergateFax Control Service
unknown	9110/tcp	0.000304
unknown	9110/udp	0.000661
DragonIDSConsole	9111/tcp	0.000251	# hexxorecore | Dragon IDS Console | Multiple Purpose, Distributed Message Bus
unknown	9114/udp	0.000330
mxit	9119/tcp	0.000000	# MXit Instant Messaging
mxit	9119/udp	0.000000	# MXit Instant Messaging
grcmp	9122/tcp	0.000000	# Global Relay compliant mobile instant messaging protocol
grcp	9123/tcp	0.000000	# Global Relay compliant instant messaging protocol
unknown	9124/udp	0.000330
unknown	9125/tcp	0.000076
unknown	9128/tcp	0.000076
unknown	9129/udp	0.000330
unknown	9130/tcp	0.000076
dddp	9131/tcp	0.000076	# Dynamic Device Discovery
dddp	9131/udp	0.000330	# Dynamic Device Discovery
unknown	9133/tcp	0.000076
unknown	9136/udp	0.000330
unknown	9140/udp	0.000330
unknown	9146/udp	0.000330
ms-sql2000	9152/tcp	0.000125
unknown	9154/udp	0.000661
unknown	9156/udp	0.000661
unknown	9159/udp	0.000330
apani1	9160/tcp	0.000076
apani1	9160/udp	0.000000
apani2	9161/tcp	0.000076
apani2	9161/udp	0.000000
apani3	9162/tcp	0.000000
apani3	9162/udp	0.000000
apani4	9163/tcp	0.000000
apani4	9163/udp	0.000000
apani5	9164/tcp	0.000000
apani5	9164/udp	0.000330
unknown	9168/udp	0.000330
unknown	9170/tcp	0.000076
unknown	9170/udp	0.000661
unknown	9176/udp	0.000330
unknown	9183/tcp	0.000076
unknown	9184/udp	0.000330
unknown	9186/udp	0.000330
sun-as-jpda	9191/tcp	0.000152	# Sun AppSvr JPDA
sun-as-jpda	9191/udp	0.000000	# Sun AppSvr JPDA
unknown	9196/udp	0.000330
unknown	9197/tcp	0.000152
unknown	9198/tcp	0.000152
unknown	9199/udp	0.001982
wap-wsp	9200/tcp	0.000228	# WAP connectionless session services | WAP connectionless session service
wap-wsp	9200/udp	0.007268	# WAP connectionless session services
wap-wsp-wtp	9201/tcp	0.000000	# WAP session service
wap-wsp-wtp	9201/udp	0.000000	# WAP session service
wap-wsp-s	9202/tcp	0.000076	# WAP secure connectionless session service
wap-wsp-s	9202/udp	0.000000	# WAP secure connectionless session service
wap-wsp-wtp-s	9203/tcp	0.000000	# WAP secure session service
wap-wsp-wtp-s	9203/udp	0.000000	# WAP secure session service
wap-vcard	9204/tcp	0.000000	# WAP vCard
wap-vcard	9204/udp	0.000000	# WAP vCard
wap-vcal	9205/tcp	0.000000	# WAP vCal
wap-vcal	9205/udp	0.000000	# WAP vCal
wap-vcard-s	9206/tcp	0.000000	# WAP vCard Secure
wap-vcard-s	9206/udp	0.000661	# WAP vCard Secure
wap-vcal-s	9207/tcp	0.000532	# WAP vCal Secure
wap-vcal-s	9207/udp	0.000330	# WAP vCal Secure
rjcdb-vcards	9208/tcp	0.000000	# rjcdb vCard
rjcdb-vcards	9208/udp	0.000000	# rjcdb vCard
almobile-system	9209/tcp	0.000000	# ALMobile System Service
almobile-system	9209/udp	0.000000	# ALMobile System Service
oma-mlp	9210/tcp	0.000076	# OMA Mobile Location Protocol
oma-mlp	9210/udp	0.000000	# OMA Mobile Location Protocol
oma-mlp-s	9211/tcp	0.000076	# OMA Mobile Location Protocol Secure
oma-mlp-s	9211/udp	0.000330	# OMA Mobile Location Protocol Secure
serverviewdbms	9212/tcp	0.000000	# Server View dbms access [January 2005] | Server View dbms access
serverviewdbms	9212/udp	0.000000	# Server View dbms access [January 2005]
serverstart	9213/tcp	0.000000	# ServerStart RemoteControl [August 2005] | ServerStart RemoteControl
serverstart	9213/udp	0.000000	# ServerStart RemoteControl [August 2005]
ipdcesgbs	9214/tcp	0.000000	# IPDC ESG BootstrapService
ipdcesgbs	9214/udp	0.000330	# IPDC ESG BootstrapService
insis	9215/tcp	0.000000	# Integrated Setup and Install Service
insis	9215/udp	0.000000	# Integrated Setup and Install Service
acme	9216/tcp	0.000000	# Aionex Communication Management Engine
acme	9216/udp	0.000000	# Aionex Communication Management Engine
fsc-port	9217/tcp	0.000000	# FSC Communication Port
fsc-port	9217/udp	0.000000	# FSC Communication Port
unknown	9218/udp	0.000330
unknown	9220/tcp	0.000380
teamcoherence	9222/tcp	0.000000	# QSC Team Coherence
teamcoherence	9222/udp	0.000330	# QSC Team Coherence
unknown	9226/udp	0.000330
unknown	9227/udp	0.000330
unknown	9228/udp	0.000330
unknown	9229/udp	0.000661
unknown	9232/udp	0.000330
unknown	9234/udp	0.000330
unknown	9238/udp	0.000330
unknown	9245/udp	0.000330
unknown	9251/udp	0.000330
mon	9255/tcp	0.000000	# Manager On Network
mon	9255/udp	0.000000	# Manager On Network
unknown	9258/udp	0.000330
unknown	9261/udp	0.000330
unknown	9268/udp	0.000330
unknown	9269/udp	0.000330
unknown	9271/udp	0.000330
traingpsdata	9277/tcp	0.000000	# GPS Data transmitted from train to ground network
pegasus	9278/tcp	0.000000	# Pegasus GPS Platform
pegasus	9278/udp	0.000000	# Pegasus GPS Platform
pegasus-ctl	9279/tcp	0.000000	# Pegaus GPS System Control Interface
pegasus-ctl	9279/udp	0.000000	# Pegaus GPS System Control Interface
pgps	9280/tcp	0.000000	# Predicted GPS
pgps	9280/udp	0.000000	# Predicted GPS
swtp-port1	9281/tcp	0.000000	# SofaWare transport port 1
swtp-port1	9281/udp	0.000000	# SofaWare transport port 1
swtp-port2	9282/tcp	0.000000	# SofaWare transport port 2
swtp-port2	9282/udp	0.000000	# SofaWare transport port 2
callwaveiam	9283/tcp	0.000000
callwaveiam	9283/udp	0.000000
visd	9284/tcp	0.000000	# VERITAS Information Serve
visd	9284/udp	0.000000	# VERITAS Information Serve
n2h2server	9285/tcp	0.000000	# N2H2 Filter Service Port
n2h2server	9285/udp	0.000330	# N2H2 Filter Service Port
n2receive	9286/tcp	0.000000	# n2 monitoring receiver
cumulus	9287/tcp	0.000076
cumulus	9287/udp	0.000000
unknown	9288/udp	0.000330
unknown	9289/udp	0.000330
unknown	9290/tcp	0.000380
unknown	9290/udp	0.000330
armtechdaemon	9292/tcp	0.000000	# ArmTech Daemon
armtechdaemon	9292/udp	0.000000	# ArmTech Daemon
storview	9293/tcp	0.000000	# StorView Client
storview	9293/udp	0.000000	# StorView Client
armcenterhttp	9294/tcp	0.000000	# ARMCenter http Service
armcenterhttp	9294/udp	0.000000	# ARMCenter http Service
armcenterhttps	9295/tcp	0.000000	# ARMCenter https Service
armcenterhttps	9295/udp	0.000000	# ARMCenter https Service
vrace	9300/tcp	0.000076	# Virtual Racing Service
vrace	9300/udp	0.000330	# Virtual Racing Service
unknown	9301/udp	0.000330
unknown	9302/udp	0.000330
sphinxql	9306/tcp	0.000000	# Sphinx search server (MySQL listener)
sapms	9310/tcp	0.000000	# SAP Message Server
unknown	9310/udp	0.000661
sphinxapi	9312/tcp	0.000000	# Sphinx search server
unknown	9314/udp	0.000330
secure-ts	9318/tcp	0.000000	# PKIX TimeStamp over TLS
secure-ts	9318/udp	0.000000	# PKIX TimeStamp over TLS
guibase	9321/tcp	0.000000
guibase	9321/udp	0.000000
unknown	9322/udp	0.000330
unknown	9326/udp	0.000330
litecoin	9333/tcp	0.000076	# Litecoin crypto currency - https://litecoin.info/Litecoin.conf
unknown	9336/udp	0.000330
unknown	9338/udp	0.000330
gnmi-gnoi	9339/tcp	0.000000	# gRPC Network Mgmt/Operations Interface
gribi	9340/tcp	0.000000	# gRPC Routing Information Base Interface
mpidcmgr	9343/tcp	0.000076
mpidcmgr	9343/udp	0.000000
mphlpdmc	9344/tcp	0.000000
mphlpdmc	9344/udp	0.000000
rancher	9345/tcp	0.000000	# Rancher Agent
ctechlicensing	9346/tcp	0.000000	# C Tech Licensing
ctechlicensing	9346/udp	0.000000	# C Tech Licensing
unknown	9349/udp	0.000330
unknown	9351/tcp	0.000076
unknown	9351/udp	0.000330
unknown	9352/udp	0.000330
unknown	9354/udp	0.000330
unknown	9361/udp	0.000330
unknown	9364/tcp	0.000076
unknown	9364/udp	0.000330
unknown	9365/udp	0.000330
unknown	9366/udp	0.000330
unknown	9370/udp	0.001321
unknown	9372/udp	0.000330
fjdmimgr	9374/tcp	0.000000
fjdmimgr	9374/udp	0.000000
boxp	9380/tcp	0.000000	# Brivs! Open Extensible Protocol
boxp	9380/udp	0.000000	# Brivs! Open Extensible Protocol
unknown	9383/udp	0.000330
d2dconfig	9387/tcp	0.000000	# D2D Configuration Service
d2ddatatrans	9388/tcp	0.000000	# D2D Data Transfer Service
unknown	9388/udp	0.000330
adws	9389/tcp	0.000000	# Active Directory Web Services
otp	9390/tcp	0.000000	# OpenVAS Transfer Protocol
unknown	9391/udp	0.000330
fjinvmgr	9396/tcp	0.000000
fjinvmgr	9396/udp	0.000330
mpidcagt	9397/tcp	0.000000
mpidcagt	9397/udp	0.000330
sec-t4net-srv	9400/tcp	0.000076	# Samsung Twain for Network Server
sec-t4net-srv	9400/udp	0.000000	# Samsung Twain for Network Server
sec-t4net-clt	9401/tcp	0.000000	# Samsung Twain for Network Client
sec-t4net-clt	9401/udp	0.000000	# Samsung Twain for Network Client
sec-pc2fax-srv	9402/tcp	0.000000	# Samsung PC2FAX for Network Server
sec-pc2fax-srv	9402/udp	0.000000	# Samsung PC2FAX for Network Server
unknown	9407/udp	0.000330
unknown	9409/tcp	0.000152
unknown	9415/tcp	0.000760
unknown	9416/udp	0.000661
git	9418/tcp	0.000228	# Git revision control system | git pack transfer service
git	9418/udp	0.000000	# git pack transfer service
unknown	9420/udp	0.000330
unknown	9424/udp	0.000330
unknown	9431/udp	0.000330
unknown	9432/udp	0.000330
unknown	9433/udp	0.000330
tungsten-https	9443/tcp	0.000152	# WSO2 Tungsten HTTPS
tungsten-https	9443/udp	0.000000	# WSO2 Tungsten HTTPS
wso2esb-console	9444/tcp	0.000152	# WSO2 ESB Administration Console HTTPS
wso2esb-console	9444/udp	0.000000	# WSO2 ESB Administration Console HTTPS
mindarray-ca	9445/tcp	0.000000	# MindArray Systems Console Agent
sntlkeyssrvr	9450/tcp	0.000000	# Sentinel Keys Server
sntlkeyssrvr	9450/udp	0.000000	# Sentinel Keys Server
unknown	9453/udp	0.000330
unknown	9454/tcp	0.000076
unknown	9462/udp	0.000330
unknown	9464/tcp	0.000076
unknown	9471/udp	0.000330
unknown	9478/tcp	0.000076
unknown	9485/tcp	0.000380
unknown	9493/tcp	0.000076
unknown	9497/udp	0.000330
ismserver	9500/tcp	0.000380
ismserver	9500/udp	0.000000
unknown	9501/tcp	0.000152
unknown	9502/tcp	0.000380
unknown	9502/udp	0.000330
unknown	9503/tcp	0.000380
unknown	9513/tcp	0.000076
unknown	9513/udp	0.000330
unknown	9519/udp	0.000330
unknown	9521/udp	0.000330
sma-spw	9522/tcp	0.000000	# SMA Speedwire
unknown	9524/udp	0.000330
unknown	9527/tcp	0.000076
unknown	9528/udp	0.000330
unknown	9534/udp	0.000330
man	9535/tcp	0.000790	# mngsuite | Management Suite Remote Control
man	9535/udp	0.000560
laes-bf	9536/tcp	0.000000	# Surveillance buffering function
laes-bf	9536/udp	0.000000	# Surveillance buffering function
unknown	9538/udp	0.000330
unknown	9547/udp	0.000330
trispen-sra	9555/tcp	0.000000	# Trispen Secure Remote Access
trispen-sra	9555/udp	0.000000	# Trispen Secure Remote Access
p4runtime	9559/tcp	0.000000	# P4Runtime gRPC Service
unknown	9559/udp	0.000330
unknown	9560/udp	0.000330
unknown	9565/udp	0.000330
unknown	9567/udp	0.000330
unknown	9575/tcp	0.000228
unknown	9578/udp	0.000330
unknown	9583/tcp	0.000076
unknown	9589/udp	0.000661
ldgateway	9592/tcp	0.000076	# LANDesk Gateway
ldgateway	9592/udp	0.000000	# LANDesk Gateway
cba8	9593/tcp	0.000760	# LANDesk Management Agent (cba8)
cba8	9593/udp	0.000330	# LANDesk Management Agent (cba8)
msgsys	9594/tcp	0.000760	# Message System
msgsys	9594/udp	0.000000	# Message System
pds	9595/tcp	0.000760	# Ping Discovery System | Ping Discovery Service
pds	9595/udp	0.000991	# Ping Discovery System
mercury-disc	9596/tcp	0.000000	# Mercury Discovery
mercury-disc	9596/udp	0.000000	# Mercury Discovery
pd-admin	9597/tcp	0.000000	# PD Administration
pd-admin	9597/udp	0.000000	# PD Administration
vscp	9598/tcp	0.000000	# Very Simple Ctrl Protocol
vscp	9598/udp	0.000330	# Very Simple Ctrl Protocol
robix	9599/tcp	0.000000
robix	9599/udp	0.000661
micromuse-ncpw	9600/tcp	0.000152
micromuse-ncpw	9600/udp	0.000000
unknown	9605/udp	0.000330
streamcomm-ds	9612/tcp	0.000000	# StreamComm User Directory
streamcomm-ds	9612/udp	0.000000	# StreamComm User Directory
unknown	9613/tcp	0.000076
iadt-tls	9614/tcp	0.000000	# iADT Protocol over TLS
erunbook_agent	9616/tcp	0.000076	# erunbook-agent | eRunbook Agent
erunbook_server	9617/tcp	0.000000	# erunbook-server | eRunbook Server
unknown	9617/udp	0.000330
condor	9618/tcp	0.000380	# Condor Collector Service
condor	9618/udp	0.000000	# Condor Collector Service
unknown	9619/tcp	0.000076
unknown	9620/tcp	0.000076
unknown	9620/udp	0.000661
unknown	9621/tcp	0.000152
unknown	9622/udp	0.000330
unknown	9627/udp	0.000330
odbcpathway	9628/tcp	0.000076	# ODBC Pathway Service
odbcpathway	9628/udp	0.000000	# ODBC Pathway Service
uniport	9629/tcp	0.000000	# UniPort SSO Controller
uniport	9629/udp	0.000000	# UniPort SSO Controller
peoctlr	9630/tcp	0.000000	# Peovica Controller
peocoll	9631/tcp	0.000000	# Peovica Collector
mc-comm	9632/tcp	0.000000	# Mobile-C Communications
mc-comm	9632/udp	0.000000	# Mobile-C Communications
unknown	9637/udp	0.000330
unknown	9638/udp	0.000661
pqsflows	9640/tcp	0.000000	# ProQueSys Flows Service
unknown	9643/tcp	0.000152
unknown	9645/udp	0.000330
unknown	9648/tcp	0.000076
unknown	9651/udp	0.000330
unknown	9654/tcp	0.000076
unknown	9654/udp	0.000330
unknown	9657/udp	0.000330
unknown	9661/tcp	0.000076
unknown	9665/tcp	0.000076
zoomcp	9666/tcp	0.000304	# Zoom Control Panel Game Server Management
xmms2	9667/tcp	0.000076	# Cross-platform Music Multiplexing System
xmms2	9667/udp	0.000000	# Cross-platform Music Multiplexing System
tec5-sdctp	9668/tcp	0.000000	# tec5 Spectral Device Control Protocol
tec5-sdctp	9668/udp	0.000000	# tec5 Spectral Device Control Protocol
unknown	9670/udp	0.000330
unknown	9673/tcp	0.000152
unknown	9674/tcp	0.000076
unknown	9679/tcp	0.000076
unknown	9680/tcp	0.000076
unknown	9683/tcp	0.000076
unknown	9687/udp	0.000330
unknown	9688/udp	0.000330
unknown	9692/udp	0.000330
client-wakeup	9694/tcp	0.000076	# T-Mobile Client Wakeup Message
client-wakeup	9694/udp	0.000000	# T-Mobile Client Wakeup Message
ccnx	9695/tcp	0.000000	# Content Centric Networking
ccnx	9695/udp	0.000661	# Content Centric Networking
unknown	9699/udp	0.000330
board-roar	9700/tcp	0.000076	# Board M.I.T. Service
board-roar	9700/udp	0.000000	# Board M.I.T. Service
unknown	9716/udp	0.000661
unknown	9722/udp	0.000330
unknown	9725/udp	0.000330
unknown	9726/udp	0.000330
unknown	9729/udp	0.000330
unknown	9730/udp	0.000330
unknown	9735/udp	0.000330
unknown	9740/udp	0.000991
unknown	9744/udp	0.000330
unknown	9745/tcp	0.000076
l5nas-parchan	9747/tcp	0.000000	# L5NAS Parallel Channel
l5nas-parchan	9747/udp	0.000000	# L5NAS Parallel Channel
board-voip	9750/tcp	0.000000	# Board M.I.T. Synchronous Collaboration
board-voip	9750/udp	0.000661	# Board M.I.T. Synchronous Collaboration
unknown	9751/udp	0.000330
rasadv	9753/tcp	0.000000
rasadv	9753/udp	0.000000
tungsten-http	9762/tcp	0.000000	# WSO2 Tungsten HTTP
tungsten-http	9762/udp	0.000000	# WSO2 Tungsten HTTP
unknown	9769/udp	0.000330
unknown	9771/udp	0.000330
unknown	9777/tcp	0.000076
unknown	9779/udp	0.000330
unknown	9782/udp	0.000330
unknown	9783/udp	0.000330
unknown	9790/udp	0.000330
unknown	9797/udp	0.000330
davsrc	9800/tcp	0.000000	# WebDav Source Port
davsrc	9800/udp	0.000000	# WebDav Source Port
sstp-2	9801/tcp	0.000000	# Sakura Script Transfer Protocol-2
sstp-2	9801/udp	0.000000	# Sakura Script Transfer Protocol-2
davsrcs	9802/tcp	0.000000	# WebDAV Source TLS/SSL
davsrcs	9802/udp	0.000330	# WebDAV Source TLS/SSL
unknown	9804/udp	0.000330
unknown	9812/tcp	0.000076
unknown	9814/tcp	0.000076
unknown	9814/udp	0.000330
unknown	9815/tcp	0.000152
unknown	9815/udp	0.000330
unknown	9818/udp	0.000330
unknown	9823/tcp	0.000076
unknown	9823/udp	0.000330
unknown	9825/tcp	0.000076
unknown	9825/udp	0.000330
unknown	9826/tcp	0.000076
unknown	9827/udp	0.000330
unknown	9830/tcp	0.000076
unknown	9834/udp	0.000330
unknown	9842/udp	0.000330
unknown	9844/tcp	0.000076
unknown	9847/udp	0.000330
unknown	9849/udp	0.000330
unknown	9851/udp	0.000330
unknown	9859/udp	0.000330
unknown	9869/udp	0.000661
sapv1	9875/tcp	0.000076	# Session Announcement v1
sapv1	9875/udp	0.000000	# Session Announcement v1
sd	9876/tcp	0.000602	# Session Director
sd	9876/udp	0.004498	# Session Director
x510	9877/tcp	0.000304	# The X.510 wrapper protocol
unknown	9877/udp	0.001652
kca-service	9878/tcp	0.000228	# The KX509 Kerberized Certificate Issuance Protocol in Use in 2012
unknown	9884/udp	0.000330
unknown	9887/udp	0.000330
cyborg-systems	9888/tcp	0.000000	# CYBORG Systems
cyborg-systems	9888/udp	0.000000	# CYBORG Systems
gt-proxy	9889/tcp	0.000000	# Port for Cable network related data proxy or repeater
gt-proxy	9889/udp	0.000000	# Port for Cable network related data proxy or repeater
unknown	9890/udp	0.000991
unknown	9893/udp	0.000330
unknown	9894/udp	0.000330
unknown	9897/udp	0.000661
monkeycom	9898/tcp	0.000228
monkeycom	9898/udp	0.000000
sctp-tunneling	9899/sctp	0.000000	# SCTP Tunneling (misconfiguration) | SCTP TUNNELING
sctp-tunneling	9899/tcp	0.000000	# SCTP TUNNELING
sctp-tunneling	9899/udp	0.000000	# SCTP Tunneling
iua	9900/sctp	0.000000
iua	9900/tcp	0.000380
iua	9900/udp	0.000000
enrp-sctp	9901/sctp	0.000000	# enrp | ENRP server channel | enrp server channel
unknown	9901/tcp	0.000076
enrp	9901/udp	0.000000	# ENRP server channel
enrp-sctp-tls	9902/sctp	0.000000	# ENRP/TLS server channel | enrp/tls server channel
multicast-ping	9903/tcp	0.000000	# Multicast Ping Protocol
unknown	9908/tcp	0.000076
domaintime	9909/tcp	0.000076
domaintime	9909/udp	0.000000
unknown	9910/tcp	0.000076
sype-transport	9911/tcp	0.000076	# SYPECom Transport Protocol
sype-transport	9911/udp	0.000000	# SYPECom Transport Protocol
unknown	9912/tcp	0.000076
unknown	9912/udp	0.000330
unknown	9914/tcp	0.000152
unknown	9915/tcp	0.000076
unknown	9917/tcp	0.000228
unknown	9919/tcp	0.000076
unknown	9921/udp	0.000661
xybrid-cloud	9925/tcp	0.000000	# XYBRID Cloud
nping-echo	9929/tcp	0.000163	# Nping echo server mode - https://nmap.org/book/nping-man-echo-mode.html - The port frequency is made up to keep it (barely) in top 1000 TCP
unknown	9941/tcp	0.000152
unknown	9943/tcp	0.000304
unknown	9944/tcp	0.000304
unknown	9945/udp	0.000330
unknown	9947/udp	0.000330
apc-9950	9950/tcp	0.000076	# APC 9950
apc-9950	9950/udp	0.002643	# APC 9950
apc-9951	9951/tcp	0.000000	# APC 9951
apc-9951	9951/udp	0.000000	# APC 9951
apc-9952	9952/tcp	0.000000	# APC 9952
apc-9952	9952/udp	0.000330	# APC 9952
acis	9953/tcp	0.000000	# 9953
acis	9953/udp	0.000000	# 9953
hinp	9954/tcp	0.000000	# HaloteC Instrument Network Protocol
alljoyn-stm	9955/tcp	0.000000	# alljoyn-mcm | Contact Port for AllJoyn standard messaging | Contact Port for AllJoyn multiplexed constrained messaging
alljoyn	9956/tcp	0.000000	# Alljoyn Name Service
odnsp	9966/tcp	0.000000	# OKI Data Network Setting Protocol
odnsp	9966/udp	0.000000	# OKI Data Network Setting Protocol
unknown	9968/tcp	0.000380
unknown	9971/tcp	0.000076
unknown	9975/tcp	0.000076
unknown	9975/udp	0.000330
xybrid-rt	9978/tcp	0.000000	# XYBRID RT Server
visweather	9979/tcp	0.000076	# Valley Information Systems Weather station data
pumpkindb	9981/tcp	0.000000	# Event sourcing database engine with a built-in programming language
dsm-scm-target	9987/tcp	0.000000	# DSM/SCM Target Interface
dsm-scm-target	9987/udp	0.000000	# DSM/SCM Target Interface
nsesrvr	9988/tcp	0.000152	# Software Essentials Secure HTTP server
osm-appsrvr	9990/tcp	0.000076	# OSM Applet Server
osm-appsrvr	9990/udp	0.000000	# OSM Applet Server
issa	9991/tcp	0.000063	# osm-oev | ISS System Scanner Agent | OSM Event Server
osm-oev	9991/udp	0.000000	# OSM Event Server
issc	9992/tcp	0.000138	# palace-1 | ISS System Scanner Console | OnLive-1
palace-1	9992/udp	0.000000	# OnLive-1
palace-2	9993/tcp	0.000000	# OnLive-2
palace-2	9993/udp	0.000000	# OnLive-2
palace-3	9994/tcp	0.000000	# OnLive-3
palace-3	9994/udp	0.000000	# OnLive-3
palace-4	9995/tcp	0.000076
palace-4	9995/udp	0.000000
palace-5	9996/tcp	0.000000
palace-5	9996/udp	0.000000
palace-6	9997/tcp	0.000000
palace-6	9997/udp	0.000000
distinct32	9998/tcp	0.000304
distinct32	9998/udp	0.000330
abyss	9999/tcp	0.004441	# Abyss web server remote web management interface | distinct
distinct	9999/udp	0.000330
snet-sensor-mgmt	10000/tcp	0.011692	# ndmp | SecureNet Pro Sensor https management server or apple airport admin | Network Data Management Protocol
ndmp	10000/udp	0.007598	# Network Data Management Protocol
scp-config	10001/tcp	0.001292	# SCP Configuration
scp-config	10001/udp	0.000000	# SCP Configuration
documentum	10002/tcp	0.000380	# EMC-Documentum Content Server Product
documentum	10002/udp	0.000000	# EMC-Documentum Content Server Product
documentum_s	10003/tcp	0.000228	# documentum-s | EMC-Documentum Content Server Product
documentum_s	10003/udp	0.000000	# EMC-Documentum Content Server Product
emcrmirccd	10004/tcp	0.000304	# EMC Replication Manager Client
stel	10005/tcp	0.000151	# emcrmird | Secure telnet | EMC Replication Manager Server
netapp-sync	10006/tcp	0.000076	# Sync replication protocol among different NetApp platforms
mvs-capacity	10007/tcp	0.000076	# MVS Capacity
mvs-capacity	10007/udp	0.000661	# MVS Capacity
octopus	10008/tcp	0.000152	# Octopus Multiplexer
octopus	10008/udp	0.000000	# Octopus Multiplexer
swdtp-sv	10009/tcp	0.000228	# Systemwalker Desktop Patrol
swdtp-sv	10009/udp	0.000000	# Systemwalker Desktop Patrol
rxapi	10010/tcp	0.002889	# ooRexx rxapi services
unknown	10011/tcp	0.000152
unknown	10011/udp	0.000661
unknown	10012/tcp	0.000380
unknown	10018/tcp	0.000076
unknown	10018/udp	0.000330
unknown	10019/tcp	0.000076
abb-hw	10020/tcp	0.000076	# Hardware configuration and maintenance
unknown	10021/udp	0.000330
unknown	10022/tcp	0.000152
cefd-vmp	10023/tcp	0.000152	# Comtech EF-Data's Vipersat Management Protocol
unknown	10024/tcp	0.000380
unknown	10025/tcp	0.000380
unknown	10028/udp	0.000330
unknown	10031/udp	0.000330
unknown	10034/tcp	0.000152
unknown	10035/tcp	0.000076
unknown	10040/udp	0.000330
unknown	10042/tcp	0.000076
unknown	10045/tcp	0.000076
zabbix-agent	10050/tcp	0.000000	# Zabbix Agent
zabbix-agent	10050/udp	0.000000	# Zabbix Agent
zabbix-trapper	10051/tcp	0.000000	# Zabbix Trapper
zabbix-trapper	10051/udp	0.000000	# Zabbix Trapper
unknown	10053/udp	0.000330
qptlmd	10055/tcp	0.000000	# Quantapoint FLEXlm Licensing Service
unknown	10056/udp	0.000330
unknown	10058/tcp	0.000152
unknown	10058/udp	0.000330
unknown	10061/udp	0.000330
unknown	10064/tcp	0.000076
unknown	10066/udp	0.000661
unknown	10076/udp	0.000661
unknown	10077/udp	0.000330
amanda	10080/tcp	0.000000
amanda	10080/udp	0.005585	# Amanda Backup Util
famdc	10081/tcp	0.000000	# FAM Archive Server
famdc	10081/udp	0.000991	# FAM Archive Server
amandaidx	10082/tcp	0.000213	# Amanda indexing
amidxtape	10083/tcp	0.000125	# Amanda tape indexing
unknown	10084/udp	0.000330
unknown	10089/udp	0.000330
unknown	10093/tcp	0.000076
unknown	10099/udp	0.000330
itap-ddtp	10100/tcp	0.000000	# VERITAS ITAP DDTP
itap-ddtp	10100/udp	0.000000	# VERITAS ITAP DDTP
ezmeeting-2	10101/tcp	0.000076	# eZmeeting
ezmeeting-2	10101/udp	0.000000	# eZmeeting
ezproxy-2	10102/tcp	0.000000	# eZproxy
ezproxy-2	10102/udp	0.000000	# eZproxy
ezrelay	10103/tcp	0.000000
ezrelay	10103/udp	0.000000
swdtp	10104/tcp	0.000000	# Systemwalker Desktop Patrol
swdtp	10104/udp	0.000000	# Systemwalker Desktop Patrol
bctp-server	10107/tcp	0.000000	# VERITAS BCTP, server
bctp-server	10107/udp	0.000000	# VERITAS BCTP, server
nmea-0183	10110/tcp	0.000000	# NMEA-0183 Navigational Data
nmea-0183	10110/udp	0.000330	# NMEA-0183 Navigational Data
nmea-onenet	10111/tcp	0.000000	# NMEA OneNet multicast messaging
unknown	10112/udp	0.000330
netiq-endpoint	10113/tcp	0.000000	# NetIQ Endpoint
netiq-endpoint	10113/udp	0.000000	# NetIQ Endpoint
netiq-qcheck	10114/tcp	0.000000	# NetIQ Qcheck
netiq-qcheck	10114/udp	0.000330	# NetIQ Qcheck
netiq-endpt	10115/tcp	0.000076	# NetIQ Endpoint
netiq-endpt	10115/udp	0.000000	# NetIQ Endpoint
netiq-voipa	10116/tcp	0.000000	# NetIQ VoIP Assessor
netiq-voipa	10116/udp	0.000000	# NetIQ VoIP Assessor
iqrm	10117/tcp	0.000000	# NetIQ IQCResource Managament Svc
iqrm	10117/udp	0.000000	# NetIQ IQCResource Managament Svc
cimple	10125/tcp	0.000000	# HotLink CIMple REST API
bmc-perf-sd	10128/tcp	0.000000	# BMC-PERFORM-SERVICE DAEMON
bmc-perf-sd	10128/udp	0.000000	# BMC-PERFORM-SERVICE DAEMON
bmc-gms	10129/tcp	0.000000	# BMC General Manager Server
unknown	10131/udp	0.000330
unknown	10143/udp	0.000330
unknown	10152/udp	0.000330
qb-db-server	10160/tcp	0.000152	# QB Database Server
qb-db-server	10160/udp	0.000000	# QB Database Server
snmptls	10161/tcp	0.000000	# snmpdtls | SNMP-TLS | SNMP-DTLS
snmpdtls	10161/udp	0.000000	# SNMP-DTLS
snmptls-trap	10162/tcp	0.000000	# snmpdtls-trap | SNMP-Trap-TLS | SNMP-Trap-DTLS
snmpdtls-trap	10162/udp	0.000330	# SNMP-Trap-DTLS
unknown	10169/udp	0.000330
unknown	10180/tcp	0.000228
unknown	10185/udp	0.000330
unknown	10186/udp	0.000330
unknown	10189/udp	0.000330
unknown	10194/udp	0.000330
trisoap	10200/tcp	0.000000	# Trigence AE Soap Service
trisoap	10200/udp	0.000000	# Trigence AE Soap Service
rsms	10201/tcp	0.000000	# rscs | Remote Server Management Service | Remote Server Control and Test Service
rscs	10201/udp	0.000000	# Remote Server Control and Test Service
unknown	10212/udp	0.000330
unknown	10214/udp	0.000330
unknown	10215/tcp	0.000228
unknown	10218/udp	0.000330
unknown	10219/udp	0.000330
unknown	10227/udp	0.000330
unknown	10238/tcp	0.000076
unknown	10239/udp	0.000330
unknown	10243/tcp	0.000684
unknown	10245/tcp	0.000076
unknown	10246/tcp	0.000076
unknown	10248/udp	0.000330
apollo-relay	10252/tcp	0.000000	# Apollo Relay Port
apollo-relay	10252/udp	0.000000	# Apollo Relay Port
eapol-relay	10253/tcp	0.000000	# Relay of EAPOL frames
unknown	10255/tcp	0.000076
axis-wimp-port	10260/tcp	0.000000	# Axis WIMP Port
axis-wimp-port	10260/udp	0.000330	# Axis WIMP Port
tile-ml	10261/tcp	0.000000	# Tile remote machine learning
unknown	10261/udp	0.000330
unknown	10268/udp	0.000661
unknown	10280/tcp	0.000076
unknown	10284/udp	0.000330
unknown	10286/udp	0.000330
blocks	10288/tcp	0.000000
blocks	10288/udp	0.000000
unknown	10289/udp	0.000330
unknown	10290/udp	0.000330
unknown	10302/udp	0.000991
unknown	10303/udp	0.000330
unknown	10309/udp	0.000330
unknown	10310/udp	0.000330
unknown	10312/udp	0.000330
unknown	10313/udp	0.000330
unknown	10316/udp	0.000330
unknown	10317/udp	0.000330
cosir	10321/tcp	0.000000	# Computer Op System Information Report
unknown	10322/udp	0.000330
unknown	10324/udp	0.000330
unknown	10337/udp	0.000330
unknown	10338/tcp	0.000076
unknown	10339/udp	0.000330
unknown	10341/udp	0.000330
unknown	10343/udp	0.000661
unknown	10347/tcp	0.000076
unknown	10355/udp	0.000330
unknown	10357/tcp	0.000076
unknown	10363/udp	0.000330
unknown	10369/udp	0.000661
unknown	10374/udp	0.000330
unknown	10378/udp	0.000330
unknown	10381/udp	0.000330
unknown	10386/udp	0.000330
unknown	10387/tcp	0.000076
unknown	10390/udp	0.000330
unknown	10397/udp	0.000330
unknown	10399/udp	0.000330
unknown	10409/udp	0.000661
unknown	10412/udp	0.000330
unknown	10414/tcp	0.000076
unknown	10416/udp	0.000330
unknown	10420/udp	0.000330
unknown	10431/udp	0.000330
unknown	10433/udp	0.000330
bngsync	10439/tcp	0.000000	# BalanceNG session table synchronization protocol
unknown	10439/udp	0.000330
cirrossp	10443/tcp	0.000076	# CirrosSP Workstation Communication
unknown	10445/udp	0.000661
unknown	10450/udp	0.000330
unknown	10454/udp	0.000330
unknown	10477/udp	0.000330
unknown	10484/udp	0.000991
unknown	10490/udp	0.000661
unknown	10492/udp	0.000330
unknown	10494/tcp	0.000076
unknown	10498/udp	0.000330
unknown	10499/udp	0.000330
hip-nat-t	10500/tcp	0.000076	# HIP NAT-Traversal
hip-nat-t	10500/udp	0.000000	# HIP NAT-Traversal
unknown	10503/udp	0.000330
unknown	10506/udp	0.000330
unknown	10509/tcp	0.000076
unknown	10510/udp	0.000330
unknown	10511/udp	0.000330
unknown	10517/udp	0.000661
unknown	10525/udp	0.000661
unknown	10529/tcp	0.000076
unknown	10529/udp	0.000330
unknown	10535/tcp	0.000076
unknown	10536/udp	0.000330
unknown	10538/udp	0.000330
MOS-lower	10540/tcp	0.000000	# MOS Media Object Metadata Port
MOS-lower	10540/udp	0.000330	# MOS Media Object Metadata Port
MOS-upper	10541/tcp	0.000000	# MOS Running Order Port
MOS-upper	10541/udp	0.000000	# MOS Running Order Port
MOS-aux	10542/tcp	0.000000	# MOS Low Priority Port
MOS-aux	10542/udp	0.000000	# MOS Low Priority Port
MOS-soap	10543/tcp	0.000000	# MOS SOAP Default Port
MOS-soap	10543/udp	0.000330	# MOS SOAP Default Port
MOS-soap-opt	10544/tcp	0.000000	# MOS SOAP Optional Port
MOS-soap-opt	10544/udp	0.000000	# MOS SOAP Optional Port
unknown	10545/udp	0.000330
serverdocs	10548/tcp	0.000000	# Apple Document Sharing Service
unknown	10550/tcp	0.000076
unknown	10551/tcp	0.000076
unknown	10552/tcp	0.000076
unknown	10553/tcp	0.000076
unknown	10553/udp	0.000330
unknown	10554/tcp	0.000076
unknown	10554/udp	0.000330
unknown	10555/tcp	0.000076
unknown	10556/tcp	0.000076
unknown	10562/udp	0.000330
unknown	10564/udp	0.000330
unknown	10565/tcp	0.000076
unknown	10566/tcp	0.000380
unknown	10567/tcp	0.000076
unknown	10575/udp	0.000330
unknown	10581/udp	0.000330
unknown	10582/udp	0.000330
unknown	10583/udp	0.000991
unknown	10584/udp	0.000330
unknown	10587/udp	0.000330
unknown	10593/udp	0.000330
unknown	10601/tcp	0.000076
unknown	10602/tcp	0.000076
unknown	10613/udp	0.000330
unknown	10615/udp	0.000330
unknown	10616/tcp	0.000380
unknown	10617/tcp	0.000380
unknown	10621/tcp	0.000380
unknown	10621/udp	0.000330
unknown	10626/tcp	0.000380
unknown	10628/tcp	0.000380
unknown	10628/udp	0.000661
unknown	10629/tcp	0.000380
printopia	10631/tcp	0.000000	# Printopia Serve
unknown	10633/udp	0.000330
unknown	10635/udp	0.000330
unknown	10639/udp	0.000330
unknown	10640/udp	0.000330
unknown	10641/udp	0.000330
unknown	10645/udp	0.000330
unknown	10650/udp	0.000330
unknown	10653/udp	0.000661
unknown	10660/udp	0.000330
unknown	10666/udp	0.000661
unknown	10671/udp	0.000330
unknown	10694/udp	0.000330
unknown	10699/tcp	0.000076
unknown	10715/udp	0.000330
unknown	10718/udp	0.000330
unknown	10733/udp	0.000330
unknown	10738/udp	0.000330
unknown	10744/udp	0.000330
unknown	10754/tcp	0.000076
unknown	10754/udp	0.000330
unknown	10760/udp	0.000330
unknown	10767/udp	0.000330
unknown	10776/udp	0.000330
unknown	10778/tcp	0.000304
unknown	10784/udp	0.000330
unknown	10790/udp	0.000330
unknown	10795/udp	0.000330
gap	10800/tcp	0.000000	# Gestor de Acaparamiento para Pocket PCs
gap	10800/udp	0.000000	# Gestor de Acaparamiento para Pocket PCs
unknown	10804/udp	0.000330
lpdg	10805/tcp	0.000000	# LUCIA Pareja Data Group
lpdg	10805/udp	0.000000	# LUCIA Pareja Data Group
unknown	10806/udp	0.000330
nbd	10809/tcp	0.000000	# Linux Network Block Device
unknown	10809/udp	0.000330
nmc-disc	10810/tcp	0.000000	# Nuance Mobile Care Discovery
nmc-disc	10810/udp	0.000330	# Nuance Mobile Care Discovery
unknown	10812/udp	0.000330
unknown	10815/udp	0.000330
unknown	10823/udp	0.000330
unknown	10825/udp	0.000991
unknown	10827/udp	0.000661
unknown	10835/udp	0.000330
unknown	10836/udp	0.000330
unknown	10842/tcp	0.000076
unknown	10845/udp	0.000661
unknown	10851/udp	0.000330
unknown	10852/tcp	0.000076
helix	10860/tcp	0.000000	# Helix Client/Server
helix	10860/udp	0.000330	# Helix Client/Server
unknown	10862/udp	0.000661
unknown	10872/udp	0.000330
unknown	10873/tcp	0.000152
unknown	10876/udp	0.000330
unknown	10878/tcp	0.000076
bveapi	10880/tcp	0.000000	# BVEssentials HTTP API
unknown	10887/udp	0.000330
unknown	10893/udp	0.000330
unknown	10900/tcp	0.000076
unknown	10900/udp	0.000330
unknown	10903/udp	0.000330
unknown	10906/udp	0.000330
unknown	10916/udp	0.000330
unknown	10923/udp	0.000330
octopustentacle	10933/tcp	0.000000	# Listen port used by the Octopus Deploy Tentacle deployment agent
unknown	10942/udp	0.000330
unknown	10963/udp	0.000330
unknown	10967/udp	0.000330
unknown	10971/udp	0.000330
unknown	10981/udp	0.000330
rmiaux	10990/tcp	0.000000	# Auxiliary RMI Port
rmiaux	10990/udp	0.000330	# Auxiliary RMI Port
unknown	10991/udp	0.000330
unknown	10995/udp	0.000330
unknown	10998/udp	0.000330
irisa	11000/tcp	0.000076
irisa	11000/udp	0.000000
metasys	11001/tcp	0.000076
metasys	11001/udp	0.000000
unknown	11002/udp	0.000330
unknown	11003/tcp	0.000076
unknown	11003/udp	0.000330
unknown	11007/tcp	0.000076
unknown	11019/tcp	0.000076
unknown	11026/tcp	0.000076
unknown	11030/udp	0.000330
unknown	11031/tcp	0.000076
unknown	11032/tcp	0.000076
unknown	11032/udp	0.000330
unknown	11033/tcp	0.000076
unknown	11033/udp	0.000330
unknown	11034/udp	0.000330
unknown	11039/udp	0.000330
unknown	11054/udp	0.000330
unknown	11063/udp	0.000661
unknown	11064/udp	0.000330
unknown	11068/udp	0.000330
unknown	11069/udp	0.000330
unknown	11074/udp	0.000330
unknown	11084/udp	0.000330
unknown	11089/tcp	0.000076
unknown	11093/udp	0.000330
weave	11095/tcp	0.000000	# Nest device-to-device and device-to-service application protocol
unknown	11100/tcp	0.000076
origo-sync	11103/tcp	0.000000	# OrigoDB Server Sync Interface
unknown	11103/udp	0.000330
netapp-icmgmt	11104/tcp	0.000000	# NetApp Intercluster Management
netapp-icdata	11105/tcp	0.000000	# NetApp Intercluster Data
sgi-lk	11106/tcp	0.000000	# SGI LK Licensing service
sgi-lk	11106/udp	0.000000	# SGI LK Licensing service
myq-termlink	11108/tcp	0.000000	# Hardware Terminals Discovery and Low-Level Communication Protocol
sgi-dmfmgr	11109/tcp	0.000000	# Data migration facility Manager (DMF) is a browser based interface to DMF
sgi-soap	11110/tcp	0.000380	# Data migration facility (DMF) SOAP is a web server protocol to support remote access to DMF
vce	11111/tcp	0.000228	# Viral Computing Environment (VCE)
vce	11111/udp	0.000000	# Viral Computing Environment (VCE)
dicom	11112/tcp	0.000000
dicom	11112/udp	0.000000
unknown	11120/udp	0.000330
unknown	11124/udp	0.000330
unknown	11131/udp	0.000330
unknown	11137/udp	0.000661
unknown	11138/udp	0.000661
unknown	11139/udp	0.000330
unknown	11149/udp	0.000330
unknown	11156/udp	0.000661
unknown	11157/udp	0.000661
suncacao-snmp	11161/tcp	0.000000	# sun cacao snmp access point
suncacao-snmp	11161/udp	0.000000	# sun cacao snmp access point
suncacao-jmxmp	11162/tcp	0.000000	# sun cacao JMX-remoting access point
suncacao-jmxmp	11162/udp	0.000330	# sun cacao JMX-remoting access point
suncacao-rmi	11163/tcp	0.000000	# sun cacao rmi registry access point
suncacao-rmi	11163/udp	0.000000	# sun cacao rmi registry access point
suncacao-csa	11164/tcp	0.000000	# sun cacao command-streaming access point
suncacao-csa	11164/udp	0.000000	# sun cacao command-streaming access point
suncacao-websvc	11165/tcp	0.000000	# sun cacao web service access point
suncacao-websvc	11165/udp	0.000000	# sun cacao web service access point
snss	11171/tcp	0.000000	# Surgical Notes Security Service Discovery (SNSS)
snss	11171/udp	0.000000	# Surgical Notes Security Service Discovery (SNSS)
oemcacao-jmxmp	11172/tcp	0.000000	# OEM cacao JMX-remoting access point
t5-straton	11173/tcp	0.000000	# Straton Runtime Programing
oemcacao-rmi	11174/tcp	0.000000	# OEM cacao rmi registry access point
unknown	11174/udp	0.000330
oemcacao-websvc	11175/tcp	0.000000	# OEM cacao web service access point
unknown	11175/udp	0.000330
unknown	11179/udp	0.000330
unknown	11180/tcp	0.000076
unknown	11181/udp	0.000330
unknown	11182/udp	0.000661
unknown	11183/udp	0.000330
unknown	11200/tcp	0.000076
smsqp	11201/tcp	0.000000
smsqp	11201/udp	0.000000
dcsl-backup	11202/tcp	0.000000	# DCSL Network Backup Services
unknown	11205/udp	0.000330
wifree	11208/tcp	0.000000	# WiFree Service
wifree	11208/udp	0.000000	# WiFree Service
memcache	11211/tcp	0.000000	# Memory cache service
memcache	11211/udp	0.000000	# Memory cache service
unknown	11214/udp	0.000330
unknown	11222/udp	0.000330
unknown	11223/udp	0.000330
unknown	11224/tcp	0.000076
unknown	11225/udp	0.000330
unknown	11226/udp	0.000330
unknown	11228/udp	0.000330
unknown	11232/udp	0.000330
xcompute	11235/tcp	0.000000	# numerical systems messaging
unknown	11236/udp	0.000330
unknown	11238/udp	0.000330
unknown	11241/udp	0.000330
unknown	11249/udp	0.000330
unknown	11250/tcp	0.000076
unknown	11251/udp	0.000330
unknown	11255/udp	0.000330
unknown	11271/udp	0.000991
unknown	11277/udp	0.000330
unknown	11285/udp	0.000330
unknown	11287/udp	0.000991
unknown	11288/tcp	0.000076
unknown	11296/tcp	0.000076
unknown	11297/udp	0.000330
unknown	11302/udp	0.000330
imip	11319/tcp	0.000000
imip	11319/udp	0.000000
imip-channels	11320/tcp	0.000000	# IMIP Channels Port
imip-channels	11320/udp	0.000000	# IMIP Channels Port
arena-server	11321/tcp	0.000000	# Arena Server Listen
arena-server	11321/udp	0.000000	# Arena Server Listen
unknown	11342/udp	0.000330
unknown	11346/udp	0.000330
unknown	11354/udp	0.000330
unknown	11361/udp	0.000330
unknown	11364/udp	0.000661
atm-uhas	11367/tcp	0.000000	# ATM UHAS
atm-uhas	11367/udp	0.000000	# ATM UHAS
pksd	11371/tcp	0.000038	# hkp | PGP Public Key Server | OpenPGP HTTP Keyserver
hkp	11371/udp	0.000000	# OpenPGP HTTP Keyserver
unknown	11373/udp	0.000330
unknown	11375/udp	0.000330
unknown	11389/udp	0.000330
unknown	11400/udp	0.000330
unknown	11401/tcp	0.000076
unknown	11406/udp	0.000330
unknown	11412/udp	0.000330
unknown	11421/udp	0.000330
unknown	11423/udp	0.000330
unknown	11425/udp	0.000661
lsdp	11430/tcp	0.000000	# Lenbrook Service Discovery Protocol
unknown	11449/udp	0.000661
unknown	11452/udp	0.000330
unknown	11455/udp	0.000330
unknown	11468/udp	0.000330
unknown	11487/udp	0.003634
asgcypresstcps	11489/tcp	0.000000	# ASG Cypress Secure Only
unknown	11490/udp	0.000330
unknown	11494/udp	0.000330
unknown	11496/udp	0.000330
unknown	11503/udp	0.000330
unknown	11504/udp	0.000330
unknown	11506/udp	0.000330
unknown	11519/udp	0.000330
unknown	11523/udp	0.000330
unknown	11528/udp	0.000330
unknown	11536/udp	0.000330
unknown	11540/udp	0.000330
unknown	11543/udp	0.000330
unknown	11546/udp	0.000330
unknown	11552/tcp	0.000076
unknown	11567/udp	0.000661
unknown	11568/udp	0.000330
unknown	11571/udp	0.000330
unknown	11574/udp	0.000330
unknown	11579/udp	0.000330
unknown	11587/udp	0.000330
unknown	11590/udp	0.000330
unknown	11593/udp	0.000330
unknown	11599/udp	0.000330
tempest-port	11600/tcp	0.000000	# Tempest Protocol Port
tempest-port	11600/udp	0.000000	# Tempest Protocol Port
unknown	11603/udp	0.000330
unknown	11605/udp	0.000330
unknown	11606/udp	0.000330
unknown	11611/udp	0.000330
unknown	11613/udp	0.000330
unknown	11616/udp	0.000330
unknown	11618/udp	0.000991
unknown	11620/udp	0.000330
emc-xsw-dconfig	11623/tcp	0.000000	# EMC XtremSW distributed config
unknown	11625/udp	0.000330
unknown	11628/udp	0.000330
unknown	11634/udp	0.000330
unknown	11635/udp	0.000330
unknown	11641/udp	0.000330
unknown	11648/udp	0.000330
unknown	11649/udp	0.000330
unknown	11661/udp	0.000330
unknown	11666/udp	0.000330
unknown	11681/udp	0.000330
unknown	11688/udp	0.000330
unknown	11689/udp	0.000330
unknown	11696/udp	0.000330
unknown	11697/tcp	0.000076
unknown	11698/udp	0.000330
unknown	11701/udp	0.000330
unknown	11710/udp	0.000330
unknown	11711/udp	0.000330
h323callsigalt	11720/tcp	0.000000	# h323 Call Signal Alternate | H.323 Call Control Signalling Alternate
h323callsigalt	11720/udp	0.000661	# h323 Call Signal Alternate
unknown	11721/udp	0.000330
emc-xsw-dcache	11723/tcp	0.000000	# EMC XtremSW distributed cache
unknown	11723/udp	0.000661
unknown	11735/tcp	0.000076
unknown	11739/udp	0.000330
intrepid-ssl	11751/tcp	0.000000	# Intrepid SSL
intrepid-ssl	11751/udp	0.000000	# Intrepid SSL
unknown	11761/udp	0.000330
unknown	11767/udp	0.000330
unknown	11774/udp	0.000330
unknown	11777/udp	0.000330
unknown	11779/udp	0.000330
unknown	11785/udp	0.000661
unknown	11788/udp	0.000330
lanschool	11796/tcp	0.000000	# lanschool-mpt | Lanschool Multipoint
unknown	11800/udp	0.000330
unknown	11810/udp	0.000330
unknown	11813/tcp	0.000076
unknown	11820/udp	0.000330
unknown	11822/udp	0.000330
unknown	11835/udp	0.000330
unknown	11837/udp	0.000330
unknown	11839/udp	0.000330
unknown	11860/udp	0.000330
unknown	11862/tcp	0.000076
unknown	11862/udp	0.000330
unknown	11863/tcp	0.000076
unknown	11863/udp	0.000330
unknown	11872/udp	0.000661
unknown	11875/udp	0.000330
xoraya	11876/tcp	0.000000	# X2E Xoraya Multichannel protocol
xoraya	11876/udp	0.000000	# X2E Xoraya Multichannel protocol
x2e-disc	11877/tcp	0.000000	# X2E service discovery protocol
x2e-disc	11877/udp	0.000000	# X2E service discovery protocol
unknown	11878/udp	0.000661
unknown	11891/udp	0.000330
unknown	11892/udp	0.000330
unknown	11898/udp	0.000330
unknown	11900/udp	0.000330
unknown	11906/udp	0.000330
unknown	11907/udp	0.000330
unknown	11914/udp	0.000330
unknown	11917/udp	0.000330
unknown	11921/udp	0.000330
unknown	11929/udp	0.000330
unknown	11940/tcp	0.000076
unknown	11940/udp	0.000330
unknown	11945/udp	0.000330
unknown	11947/udp	0.000330
unknown	11948/udp	0.000330
unknown	11953/udp	0.000330
unknown	11962/udp	0.000330
unknown	11963/udp	0.000330
sysinfo-sp	11967/tcp	0.000380	# SysInfo Service Protocol | SysInfo Sercice Protocol
sysinfo-sp	11967/udp	0.000000	# SysInfo Sercice Protocol
unknown	11970/udp	0.000661
tibsd	11971/tcp	0.000000	# TiBS Service
unknown	11973/udp	0.000330
unknown	11978/udp	0.000330
unknown	11982/udp	0.000330
unknown	11988/udp	0.000330
unknown	11991/udp	0.000330
wmereceiving	11997/sctp	0.000000	# WorldMailExpress
unknown	11997/udp	0.000330
wmedistribution	11998/sctp	0.000000	# WorldMailExpress
unknown	11998/udp	0.000330
wmereporting	11999/sctp	0.000000	# WorldMailExpress
unknown	11999/udp	0.000330
cce4x	12000/tcp	0.000427	# entextxid | ClearCommerce Engine 4.x (www.clearcommerce.com) | IBM Enterprise Extender SNA XID Exchange
entextxid	12000/udp	0.000661	# IBM Enterprise Extender SNA XID Exchange
entextnetwk	12001/tcp	0.000076	# IBM Enterprise Extender SNA COS Network Priority
entextnetwk	12001/udp	0.000661	# IBM Enterprise Extender SNA COS Network Priority
entexthigh	12002/tcp	0.000076	# IBM Enterprise Extender SNA COS High Priority
entexthigh	12002/udp	0.000661	# IBM Enterprise Extender SNA COS High Priority
entextmed	12003/tcp	0.000000	# IBM Enterprise Extender SNA COS Medium Priority
entextmed	12003/udp	0.000991	# IBM Enterprise Extender SNA COS Medium Priority
entextlow	12004/tcp	0.000000	# IBM Enterprise Extender SNA COS Low Priority
entextlow	12004/udp	0.000661	# IBM Enterprise Extender SNA COS Low Priority
dbisamserver1	12005/tcp	0.000076	# DBISAM Database Server - Regular
dbisamserver1	12005/udp	0.000000	# DBISAM Database Server - Regular
dbisamserver2	12006/tcp	0.000152	# DBISAM Database Server - Admin
dbisamserver2	12006/udp	0.000000	# DBISAM Database Server - Admin
accuracer	12007/tcp	0.000000	# Accuracer Database System ñ Server | Accuracer Database System Server
accuracer	12007/udp	0.000330	# Accuracer Database System ñ Server
accuracer-dbms	12008/tcp	0.000000	# Accuracer Database System ñ Admin | Accuracer Database System Admin
accuracer-dbms	12008/udp	0.000000	# Accuracer Database System ñ Admin
ghvpn	12009/tcp	0.000076	# Green Hills VPN
edbsrvr	12010/tcp	0.000000	# ElevateDB Server
vipera	12012/tcp	0.000000	# Vipera Messaging Service
vipera	12012/udp	0.000000	# Vipera Messaging Service
vipera-ssl	12013/tcp	0.000000	# Vipera Messaging Service over SSL Communication
vipera-ssl	12013/udp	0.000000	# Vipera Messaging Service over SSL Communication
unknown	12017/udp	0.000330
unknown	12019/tcp	0.000076
unknown	12021/tcp	0.000152
unknown	12026/udp	0.000330
unknown	12031/tcp	0.000076
unknown	12034/tcp	0.000076
unknown	12034/udp	0.000661
unknown	12041/udp	0.000330
unknown	12048/udp	0.000330
unknown	12059/tcp	0.000152
unknown	12059/udp	0.000330
unknown	12060/udp	0.000330
unknown	12063/udp	0.000330
unknown	12066/udp	0.000330
unknown	12074/udp	0.000330
unknown	12077/tcp	0.000076
unknown	12080/tcp	0.000076
unknown	12088/udp	0.000330
unknown	12090/tcp	0.000076
unknown	12090/udp	0.000330
unknown	12096/tcp	0.000076
unknown	12096/udp	0.000330
unknown	12097/tcp	0.000076
unknown	12099/udp	0.000330
unknown	12101/udp	0.000330
unknown	12108/udp	0.000330
rets-ssl	12109/tcp	0.000000	# RETS over SSL
rets-ssl	12109/udp	0.000000	# RETS over SSL
unknown	12111/udp	0.000330
unknown	12115/udp	0.000330
nupaper-ss	12121/tcp	0.000076	# NuPaper Session Service
nupaper-ss	12121/udp	0.000000	# NuPaper Session Service
unknown	12128/udp	0.000330
unknown	12132/tcp	0.000076
unknown	12137/tcp	0.000076
unknown	12140/udp	0.000330
unknown	12146/tcp	0.000076
unknown	12146/udp	0.000330
unknown	12149/udp	0.000330
unknown	12156/tcp	0.000076
unknown	12162/udp	0.000330
unknown	12166/udp	0.000330
cawas	12168/tcp	0.000000	# CA Web Access Service
cawas	12168/udp	0.000000	# CA Web Access Service
unknown	12170/udp	0.000330
unknown	12171/tcp	0.000076
hivep	12172/tcp	0.000000
hivep	12172/udp	0.000000
unknown	12173/udp	0.000661
unknown	12174/tcp	0.000228
unknown	12185/udp	0.000330
unknown	12190/udp	0.000330
unknown	12192/tcp	0.000076
unknown	12195/udp	0.000661
unknown	12199/udp	0.000330
unknown	12200/udp	0.000330
unknown	12205/udp	0.000330
unknown	12208/udp	0.000991
unknown	12210/udp	0.000330
unknown	12215/tcp	0.000152
unknown	12218/udp	0.000330
unknown	12222/udp	0.000330
unknown	12225/tcp	0.000076
unknown	12239/udp	0.000330
unknown	12240/tcp	0.000076
unknown	12240/udp	0.000330
unknown	12243/tcp	0.000076
unknown	12247/udp	0.000330
unknown	12250/udp	0.000330
unknown	12251/tcp	0.000076
unknown	12259/udp	0.000330
unknown	12262/tcp	0.000152
unknown	12265/tcp	0.000228
unknown	12267/udp	0.000330
unknown	12268/udp	0.000661
unknown	12271/tcp	0.000076
unknown	12274/udp	0.000330
unknown	12275/tcp	0.000076
unknown	12282/udp	0.000330
unknown	12287/udp	0.000330
unknown	12296/tcp	0.000076
linogridengine	12300/tcp	0.000000	# LinoGrid Engine
linogridengine	12300/udp	0.000000	# LinoGrid Engine
rads	12302/tcp	0.000000	# Remote Administration Daemon (RAD) is a system service that offers secure, remote, programmatic access to Solaris system configuration and run-time state
unknown	12302/udp	0.000330
unknown	12304/udp	0.000661
unknown	12306/udp	0.000661
unknown	12313/udp	0.000330
warehouse-sss	12321/tcp	0.000000	# Warehouse Monitoring Syst SSS
warehouse-sss	12321/udp	0.000661	# Warehouse Monitoring Syst SSS
warehouse	12322/tcp	0.000000	# Warehouse Monitoring Syst
warehouse	12322/udp	0.000000	# Warehouse Monitoring Syst
unknown	12340/tcp	0.000076
unknown	12342/udp	0.000330
netbus	12345/tcp	0.000527	# italk | NetBus backdoor trojan or Trend Micro Office Scan | Italk Chat System
italk	12345/udp	0.000000	# Italk Chat System
netbus	12346/tcp	0.000088	# NetBus backdoor trojan
unknown	12346/udp	0.000330
unknown	12352/udp	0.000330
unknown	12357/udp	0.000330
unknown	12361/udp	0.000330
unknown	12369/udp	0.000330
unknown	12374/udp	0.000330
unknown	12375/udp	0.000330
unknown	12376/udp	0.000330
unknown	12378/udp	0.000330
unknown	12380/tcp	0.000152
unknown	12397/udp	0.000330
unknown	12400/udp	0.000330
unknown	12401/udp	0.000330
unknown	12406/udp	0.000330
unknown	12414/tcp	0.000076
unknown	12432/udp	0.000330
unknown	12434/udp	0.000330
unknown	12435/udp	0.000330
unknown	12444/udp	0.000330
unknown	12447/udp	0.000661
unknown	12449/udp	0.000330
unknown	12452/tcp	0.000152
unknown	12459/udp	0.000330
unknown	12469/udp	0.000661
unknown	12472/udp	0.000661
unknown	12473/udp	0.000330
unknown	12478/udp	0.000330
unknown	12480/udp	0.000330
unknown	12484/udp	0.000330
unknown	12496/udp	0.000330
unknown	12504/udp	0.000330
unknown	12517/udp	0.000330
unknown	12525/udp	0.000661
unknown	12534/udp	0.000330
unknown	12535/udp	0.000330
unknown	12537/udp	0.000330
carb-repl-ctrl	12546/tcp	0.000000	# Carbonite Server Replication Control
unknown	12562/udp	0.000330
unknown	12568/udp	0.000330
unknown	12571/udp	0.000330
unknown	12578/udp	0.000661
unknown	12592/udp	0.000330
unknown	12593/udp	0.000330
unknown	12599/udp	0.000330
unknown	12601/udp	0.000330
unknown	12602/udp	0.000661
unknown	12604/udp	0.000330
unknown	12613/udp	0.000330
unknown	12616/udp	0.000330
unknown	12618/udp	0.000330
unknown	12622/udp	0.000330
unknown	12623/udp	0.000330
unknown	12625/udp	0.000330
unknown	12639/udp	0.000330
unknown	12640/udp	0.000330
unknown	12641/udp	0.000330
unknown	12650/udp	0.000661
unknown	12672/udp	0.000330
unknown	12682/udp	0.000330
unknown	12699/tcp	0.000076
unknown	12700/udp	0.000330
unknown	12702/tcp	0.000076
unknown	12706/udp	0.000330
unknown	12708/udp	0.000330
unknown	12712/udp	0.000330
unknown	12714/udp	0.000330
unknown	12718/udp	0.000330
unknown	12720/udp	0.000330
unknown	12730/udp	0.000330
unknown	12748/udp	0.000330
tsaf	12753/tcp	0.000000	# tsaf port
tsaf	12753/udp	0.000000	# tsaf port
unknown	12764/udp	0.000330
unknown	12766/tcp	0.000076
unknown	12774/udp	0.000330
unknown	12775/udp	0.000330
unknown	12786/udp	0.000330
unknown	12789/udp	0.000330
unknown	12793/udp	0.000330
unknown	12796/udp	0.000330
unknown	12800/udp	0.000330
unknown	12804/udp	0.000330
unknown	12805/udp	0.000330
unknown	12807/udp	0.000330
unknown	12814/udp	0.000330
unknown	12825/udp	0.000330
unknown	12828/udp	0.000330
unknown	12836/udp	0.000330
unknown	12838/udp	0.000330
unknown	12839/udp	0.000330
unknown	12845/udp	0.000330
unknown	12854/udp	0.000661
unknown	12858/udp	0.000330
netperf	12865/tcp	0.000076	# control port for the netperf benchmark
unknown	12873/udp	0.000661
unknown	12883/udp	0.000330
unknown	12889/udp	0.000330
unknown	12890/udp	0.000330
unknown	12891/tcp	0.000076
unknown	12892/tcp	0.000076
unknown	12902/udp	0.000330
unknown	12905/udp	0.000330
unknown	12906/udp	0.000330
unknown	12918/udp	0.000330
unknown	12924/udp	0.000330
unknown	12931/udp	0.000330
unknown	12933/udp	0.000661
unknown	12940/udp	0.000330
unknown	12953/udp	0.000330
unknown	12955/tcp	0.000076
unknown	12961/udp	0.000330
unknown	12962/tcp	0.000076
unknown	12964/udp	0.000330
unknown	12966/udp	0.000330
unknown	12967/udp	0.000330
unknown	12970/udp	0.000330
unknown	12972/udp	0.000330
unknown	12974/udp	0.000330
unknown	12977/udp	0.000330
unknown	12986/udp	0.000661
unknown	12991/udp	0.000661
unknown	12993/udp	0.000330
unknown	12994/udp	0.000330
unknown	12999/udp	0.000330
unknown	13000/udp	0.000330
unknown	13001/udp	0.000330
unknown	13002/udp	0.000661
unknown	13005/udp	0.000330
unknown	13010/udp	0.000330
unknown	13013/udp	0.000330
unknown	13017/tcp	0.000076
unknown	13020/udp	0.000330
unknown	13027/udp	0.000330
unknown	13046/udp	0.000330
unknown	13058/udp	0.000330
unknown	13059/udp	0.000330
unknown	13063/udp	0.000330
unknown	13064/udp	0.000330
unknown	13071/udp	0.000330
unknown	13092/udp	0.000330
unknown	13093/tcp	0.000076
unknown	13095/udp	0.000330
unknown	13098/udp	0.000330
unknown	13102/udp	0.000330
unknown	13109/udp	0.000330
unknown	13123/udp	0.000330
unknown	13130/tcp	0.000076
unknown	13132/tcp	0.000076
unknown	13134/udp	0.000330
unknown	13140/tcp	0.000076
unknown	13140/udp	0.000330
unknown	13142/tcp	0.000076
unknown	13149/tcp	0.000076
unknown	13149/udp	0.000330
unknown	13151/udp	0.000330
unknown	13155/udp	0.000661
i-zipqd	13160/tcp	0.000000
i-zipqd	13160/udp	0.000330
unknown	13164/udp	0.000661
unknown	13167/tcp	0.000076
unknown	13171/udp	0.000330
unknown	13173/udp	0.000330
unknown	13188/tcp	0.000076
unknown	13189/udp	0.000330
unknown	13192/tcp	0.000076
unknown	13192/udp	0.000330
unknown	13193/tcp	0.000076
unknown	13194/tcp	0.000076
unknown	13194/udp	0.000330
unknown	13203/udp	0.000330
bcslogc	13216/tcp	0.000000	# Black Crow Software application logging
bcslogc	13216/udp	0.000330	# Black Crow Software application logging
rs-pias	13217/tcp	0.000000	# R&S Proxy Installation Assistant Service
rs-pias	13217/udp	0.000000	# R&S Proxy Installation Assistant Service
emc-vcas-tcp	13218/tcp	0.000000	# emc-vcas-udp | EMC Virtual CAS Service | EMV Virtual CAS Service Discovery
emc-vcas-udp	13218/udp	0.000000	# EMV Virtual CAS Service Discovery
unknown	13220/udp	0.000330
unknown	13222/udp	0.000330
powwow-client	13223/tcp	0.000000	# PowWow Client
powwow-client	13223/udp	0.000000	# PowWow Client
powwow-server	13224/tcp	0.000000	# PowWow Server
powwow-server	13224/udp	0.000000	# PowWow Server
unknown	13227/udp	0.000330
unknown	13229/tcp	0.000076
unknown	13231/udp	0.000330
unknown	13237/udp	0.000330
unknown	13238/udp	0.000330
unknown	13248/udp	0.000330
unknown	13250/tcp	0.000076
unknown	13250/udp	0.000330
unknown	13254/udp	0.000330
unknown	13261/tcp	0.000076
unknown	13264/tcp	0.000076
unknown	13265/tcp	0.000076
unknown	13265/udp	0.000330
unknown	13266/udp	0.000661
unknown	13273/udp	0.000330
unknown	13277/udp	0.000330
unknown	13280/udp	0.000330
unknown	13291/udp	0.000661
unknown	13295/udp	0.000330
unknown	13298/udp	0.000330
unknown	13299/udp	0.000661
unknown	13306/tcp	0.000076
unknown	13307/udp	0.000330
unknown	13312/udp	0.000661
unknown	13318/tcp	0.000076
unknown	13319/udp	0.000330
unknown	13323/udp	0.000330
unknown	13330/udp	0.000330
unknown	13340/tcp	0.000076
unknown	13344/udp	0.000330
unknown	13345/udp	0.000330
unknown	13347/udp	0.000330
unknown	13359/tcp	0.000076
unknown	13366/udp	0.000330
unknown	13378/udp	0.000661
unknown	13384/udp	0.000330
unknown	13387/udp	0.000330
unknown	13396/udp	0.000330
doip-data	13400/tcp	0.000000	# doip-disc | DoIP Data | DoIP Discovery
unknown	13402/udp	0.000661
unknown	13419/udp	0.000661
unknown	13420/udp	0.000330
unknown	13424/udp	0.000330
unknown	13428/udp	0.000330
unknown	13429/udp	0.000991
unknown	13445/udp	0.000330
unknown	13451/udp	0.000330
unknown	13454/udp	0.000330
unknown	13456/tcp	0.000380
unknown	13466/udp	0.000330
unknown	13469/udp	0.000330
unknown	13474/udp	0.000661
unknown	13476/udp	0.000661
unknown	13495/udp	0.000330
unknown	13499/udp	0.000330
unknown	13501/udp	0.000330
unknown	13502/tcp	0.000076
unknown	13511/udp	0.000330
unknown	13517/udp	0.000330
unknown	13520/udp	0.000330
unknown	13524/udp	0.000330
unknown	13526/udp	0.000330
unknown	13528/udp	0.000330
unknown	13534/udp	0.000330
unknown	13539/udp	0.000661
unknown	13540/udp	0.000330
unknown	13543/udp	0.000661
unknown	13552/udp	0.000661
unknown	13557/udp	0.000991
unknown	13558/udp	0.000330
unknown	13564/udp	0.000330
unknown	13565/udp	0.000330
unknown	13570/udp	0.000661
unknown	13571/udp	0.000661
unknown	13580/tcp	0.000076
unknown	13583/udp	0.000330
unknown	13584/udp	0.000330
unknown	13591/udp	0.000330
unknown	13612/udp	0.000330
unknown	13614/udp	0.000330
unknown	13620/udp	0.000330
unknown	13623/udp	0.000330
unknown	13627/udp	0.000661
unknown	13630/udp	0.000330
unknown	13641/udp	0.000330
unknown	13648/udp	0.000330
unknown	13653/udp	0.000330
unknown	13659/udp	0.000330
unknown	13661/udp	0.000330
unknown	13663/udp	0.000661
unknown	13664/udp	0.000330
unknown	13666/udp	0.000330
unknown	13667/udp	0.000330
unknown	13668/udp	0.000330
unknown	13686/udp	0.000661
unknown	13688/udp	0.000330
unknown	13691/udp	0.000330
unknown	13695/tcp	0.000076
unknown	13699/udp	0.000661
netbackup	13701/tcp	0.000013	# vmd           server
unknown	13701/udp	0.000661
netbackup	13702/tcp	0.000000	# ascd          server
netbackup	13705/tcp	0.000000	# tl8cd         server
netbackup	13706/tcp	0.000000	# odld          server
unknown	13707/udp	0.000330
netbackup	13708/tcp	0.000000	# vtlcd         server
netbackup	13709/tcp	0.000000	# ts8d          server
netbackup	13710/tcp	0.000000	# tc8d          server
netbackup	13711/tcp	0.000000	# server
netbackup	13712/tcp	0.000000	# tc4d          server
unknown	13712/udp	0.000330
netbackup	13713/tcp	0.000025	# tl4d          server
unknown	13713/udp	0.000330
netbackup	13714/tcp	0.000013	# tsdd          server
netbackup	13715/tcp	0.000013	# tshd          server
netbackup	13716/tcp	0.000000	# tlmd          server
unknown	13716/udp	0.000330
netbackup	13717/tcp	0.000000	# tlhcd         server
netbackup	13718/tcp	0.000013	# lmfcd         server
netbackup	13720/tcp	0.000038	# bprd | bprd          server | BPRD Protocol (VERITAS NetBackup)
bprd	13720/udp	0.000000	# BPRD Protocol (VERITAS NetBackup)
netbackup	13721/tcp	0.000013	# bpdbm | bpdbm         server | BPDBM Protocol (VERITAS NetBackup)
bpdbm	13721/udp	0.000000	# BPDBM Protocol (VERITAS NetBackup)
netbackup	13722/tcp	0.000314	# bpjava-msvc | bpjava-msvc   client | BP Java MSVC Protocol
bpjava-msvc	13722/udp	0.000330	# BP Java MSVC Protocol
unknown	13723/tcp	0.000076
vnetd	13724/tcp	0.000152	# Veritas Network Utility
vnetd	13724/udp	0.000000	# Veritas Network Utility
unknown	13727/udp	0.000330
unknown	13730/tcp	0.000076
unknown	13734/udp	0.000330
unknown	13742/udp	0.000330
unknown	13743/udp	0.000330
unknown	13747/udp	0.000661
unknown	13757/udp	0.000330
unknown	13760/udp	0.000330
unknown	13762/udp	0.000330
unknown	13766/tcp	0.000076
unknown	13770/udp	0.000330
unknown	13773/udp	0.000330
netbackup	13782/tcp	0.000728	# bpcd | bpcd          client | VERITAS NetBackup
bpcd	13782/udp	0.000000	# VERITAS NetBackup
netbackup	13783/tcp	0.000389	# vopied | vopied        client | VOPIED Protocol
vopied	13783/udp	0.000000	# VOPIED Protocol
unknown	13784/tcp	0.000076
nbdb	13785/tcp	0.000000	# NetBackup Database
nbdb	13785/udp	0.000000	# NetBackup Database
nomdb	13786/tcp	0.000000	# Veritas-nomdb
nomdb	13786/udp	0.000000	# Veritas-nomdb
unknown	13790/udp	0.000330
unknown	13799/udp	0.000661
unknown	13806/udp	0.000330
unknown	13808/udp	0.000330
unknown	13814/udp	0.000330
dsmcc-config	13818/tcp	0.000000	# DSMCC Config
dsmcc-config	13818/udp	0.000000	# DSMCC Config
dsmcc-session	13819/tcp	0.000000	# DSMCC Session Messages
dsmcc-session	13819/udp	0.000000	# DSMCC Session Messages
dsmcc-passthru	13820/tcp	0.000000	# DSMCC Pass-Thru Messages
dsmcc-passthru	13820/udp	0.000000	# DSMCC Pass-Thru Messages
dsmcc-download	13821/tcp	0.000000	# DSMCC Download Protocol
dsmcc-download	13821/udp	0.000000	# DSMCC Download Protocol
dsmcc-ccp	13822/tcp	0.000000	# DSMCC Channel Change Protocol
dsmcc-ccp	13822/udp	0.000000	# DSMCC Channel Change Protocol
bmdss	13823/tcp	0.000000	# Blackmagic Design Streaming Server
a-trust-rpc	13832/tcp	0.000000	# Certificate Management and Issuing
unknown	13835/udp	0.000330
unknown	13846/tcp	0.000076
unknown	13850/udp	0.000330
unknown	13851/udp	0.000330
unknown	13855/udp	0.000330
unknown	13856/udp	0.000661
unknown	13862/udp	0.000330
unknown	13865/udp	0.000661
unknown	13876/udp	0.000661
unknown	13881/udp	0.000330
unknown	13883/udp	0.000330
unknown	13890/udp	0.000330
unknown	13892/udp	0.000330
ucontrol	13894/tcp	0.000000	# Ultimate Control communication protocol
unknown	13899/tcp	0.000076
unknown	13900/udp	0.000330
unknown	13905/udp	0.000661
unknown	13910/udp	0.000330
unknown	13911/udp	0.000330
unknown	13913/udp	0.000330
unknown	13914/udp	0.000661
unknown	13923/udp	0.000330
unknown	13925/udp	0.000661
dta-systems	13929/tcp	0.000000	# D-TA SYSTEMS
dta-systems	13929/udp	0.000000	# D-TA SYSTEMS
medevolve	13930/tcp	0.000000	# MedEvolve Port Requester
unknown	13931/udp	0.000330
unknown	13935/udp	0.000330
unknown	13943/udp	0.000330
unknown	13944/udp	0.000330
unknown	13950/udp	0.000330
unknown	13957/udp	0.000330
unknown	13962/udp	0.000330
unknown	13965/udp	0.000330
unknown	13967/udp	0.000330
unknown	13971/udp	0.000330
unknown	13974/udp	0.000330
unknown	13976/udp	0.000330
unknown	13977/udp	0.000330
unknown	13986/udp	0.000330
unknown	13989/udp	0.000330
unknown	13992/udp	0.000330
unknown	13996/udp	0.000330
scotty-ft	14000/tcp	0.000380	# SCOTTY High-Speed Filetransfer
scotty-ft	14000/udp	0.000000	# SCOTTY High-Speed Filetransfer
sua	14001/sctp	0.000000	# De-Registered
sua	14001/tcp	0.000076
sua	14001/udp	0.000000	# De-Registered (2001 June 06)
scotty-disc	14002/tcp	0.000000	# Discovery of a SCOTTY hardware codec board
unknown	14006/udp	0.000330
sage-best-com1	14033/tcp	0.000000	# sage Best! Config Server 1
sage-best-com1	14033/udp	0.000000	# sage Best! Config Server 1
sage-best-com2	14034/tcp	0.000000	# sage Best! Config Server 2
sage-best-com2	14034/udp	0.000330	# sage Best! Config Server 2
unknown	14035/udp	0.000330
unknown	14047/udp	0.000330
unknown	14052/udp	0.000330
unknown	14062/udp	0.000330
unknown	14063/udp	0.000330
unknown	14070/udp	0.000330
unknown	14085/udp	0.000330
unknown	14087/udp	0.000330
unknown	14094/udp	0.000330
unknown	14134/udp	0.000330
unknown	14135/udp	0.000330
bo2k	14141/tcp	0.000038	# vcs-app | Back Orifice 2K BoPeep mouse/keyboard input | VCS Application
vcs-app	14141/udp	0.000000	# VCS Application
icpp	14142/tcp	0.000000	# IceWall Cert Protocol
icpp	14142/udp	0.000000	# IceWall Cert Protocol
icpps	14143/tcp	0.000000	# IceWall Cert Protocol over TLS
unknown	14144/udp	0.000330
gcm-app	14145/tcp	0.000000	# GCM Application
gcm-app	14145/udp	0.000000	# GCM Application
unknown	14146/udp	0.000330
unknown	14147/tcp	0.000076
vrts-tdd	14149/tcp	0.000000	# Veritas Traffic Director
vrts-tdd	14149/udp	0.000000	# Veritas Traffic Director
vcscmd	14150/tcp	0.000000	# Veritas Cluster Server Command Server
unknown	14150/udp	0.000330
unknown	14151/udp	0.000330
vad	14154/tcp	0.000000	# Veritas Application Director
vad	14154/udp	0.000000	# Veritas Application Director
unknown	14156/udp	0.000330
unknown	14158/udp	0.000330
unknown	14159/udp	0.000330
unknown	14162/udp	0.000330
unknown	14169/udp	0.000661
unknown	14181/udp	0.000991
unknown	14183/udp	0.000330
unknown	14188/udp	0.000330
unknown	14189/udp	0.000330
unknown	14195/udp	0.000661
unknown	14197/udp	0.000330
unknown	14202/udp	0.000661
unknown	14203/udp	0.000330
unknown	14210/udp	0.000330
unknown	14212/udp	0.000330
unknown	14215/udp	0.000330
unknown	14216/udp	0.000330
unknown	14218/tcp	0.000076
unknown	14219/udp	0.000330
unknown	14220/udp	0.000661
unknown	14229/udp	0.000330
unknown	14232/udp	0.000330
unknown	14233/udp	0.000330
unknown	14235/udp	0.000330
unknown	14237/tcp	0.000076
unknown	14238/tcp	0.000532
unknown	14241/udp	0.000661
unknown	14245/udp	0.000330
unknown	14246/udp	0.000330
unknown	14247/udp	0.000330
cps	14250/tcp	0.000000	# Fencing Server
cps	14250/udp	0.000000	# Fencing Server
unknown	14252/udp	0.000330
unknown	14254/tcp	0.000076
unknown	14281/udp	0.000661
unknown	14284/udp	0.000330
unknown	14286/udp	0.000661
unknown	14290/udp	0.000661
unknown	14295/udp	0.000330
unknown	14305/udp	0.000330
unknown	14309/udp	0.000330
unknown	14310/udp	0.000330
unknown	14327/udp	0.000330
unknown	14334/udp	0.000330
unknown	14339/udp	0.000330
unknown	14341/udp	0.000661
unknown	14343/udp	0.000330
unknown	14346/udp	0.000330
unknown	14356/udp	0.000661
unknown	14360/udp	0.000330
unknown	14361/udp	0.000330
unknown	14368/udp	0.000330
unknown	14370/udp	0.000330
unknown	14373/udp	0.000330
unknown	14385/udp	0.000330
unknown	14388/udp	0.000661
unknown	14395/udp	0.000330
unknown	14403/udp	0.000330
unknown	14404/udp	0.000330
unknown	14405/udp	0.000330
unknown	14413/udp	0.000330
ca-web-update	14414/tcp	0.000000	# CA eTrust Web Update Service
ca-web-update	14414/udp	0.000000	# CA eTrust Web Update Service
unknown	14418/tcp	0.000076
unknown	14425/udp	0.000330
unknown	14428/udp	0.000330
unknown	14429/udp	0.000330
unknown	14441/tcp	0.000228
unknown	14442/tcp	0.000380
unknown	14443/tcp	0.000076
unknown	14444/tcp	0.000076
unknown	14446/udp	0.000330
unknown	14457/udp	0.000330
unknown	14458/udp	0.000330
unknown	14472/udp	0.000330
unknown	14476/udp	0.000330
unknown	14481/udp	0.000330
unknown	14487/udp	0.000661
unknown	14488/udp	0.000330
unknown	14494/udp	0.000330
unknown	14499/udp	0.000991
xpra	14500/tcp	0.000000	# xpra network protocol
unknown	14507/udp	0.000330
unknown	14512/udp	0.000330
unknown	14513/udp	0.000330
unknown	14524/udp	0.000330
unknown	14527/udp	0.000330
unknown	14532/udp	0.000330
unknown	14534/tcp	0.000076
unknown	14535/udp	0.000330
unknown	14536/udp	0.000330
unknown	14538/udp	0.000330
unknown	14545/tcp	0.000076
unknown	14570/udp	0.000330
unknown	14575/udp	0.000330
unknown	14578/udp	0.000330
unknown	14589/udp	0.000330
unknown	14595/udp	0.000330
unknown	14600/udp	0.000330
unknown	14604/udp	0.000330
unknown	14614/udp	0.000330
unknown	14616/udp	0.000330
unknown	14622/udp	0.000330
unknown	14632/udp	0.000330
unknown	14634/udp	0.000330
unknown	14637/udp	0.000330
unknown	14644/udp	0.000330
unknown	14651/udp	0.000330
unknown	14664/udp	0.000330
unknown	14665/udp	0.000330
unknown	14668/udp	0.000330
unknown	14670/udp	0.000330
unknown	14671/udp	0.000330
unknown	14672/udp	0.000330
unknown	14679/udp	0.000661
unknown	14687/udp	0.000330
unknown	14693/tcp	0.000076
unknown	14693/udp	0.000330
unknown	14700/udp	0.000330
unknown	14701/udp	0.000330
unknown	14719/udp	0.000330
unknown	14720/udp	0.000330
unknown	14725/udp	0.000330
unknown	14726/udp	0.000330
unknown	14732/udp	0.000330
unknown	14733/tcp	0.000076
unknown	14749/udp	0.000330
unknown	14753/udp	0.000330
unknown	14756/udp	0.000330
unknown	14771/udp	0.000661
unknown	14777/udp	0.000330
unknown	14783/udp	0.000330
unknown	14790/udp	0.000330
unknown	14799/udp	0.000330
unknown	14808/udp	0.000661
unknown	14822/udp	0.000330
unknown	14827/tcp	0.000076
unknown	14834/udp	0.000330
unknown	14837/udp	0.000330
unknown	14858/udp	0.000330
unknown	14864/udp	0.000330
unknown	14875/udp	0.000330
unknown	14882/udp	0.000330
unknown	14888/udp	0.000330
unknown	14889/udp	0.000661
unknown	14891/tcp	0.000076
unknown	14892/udp	0.000330
unknown	14916/tcp	0.000076
unknown	14916/udp	0.000330
unknown	14922/udp	0.000661
unknown	14928/udp	0.000330
unknown	14934/udp	0.000330
hde-lcesrvr-1	14936/tcp	0.000000
hde-lcesrvr-1	14936/udp	0.000000
hde-lcesrvr-2	14937/tcp	0.000000
hde-lcesrvr-2	14937/udp	0.000661
unknown	14944/udp	0.000330
unknown	14946/udp	0.000661
unknown	14959/udp	0.000330
unknown	14964/udp	0.000330
unknown	14966/udp	0.000330
unknown	14972/udp	0.000330
unknown	14978/udp	0.000330
unknown	14982/udp	0.000330
unknown	14991/udp	0.000661
unknown	14998/udp	0.000330
hydap	15000/tcp	0.001064	# Hypack Hydrographic Software Packages Data Acquisition | Hypack Data Aquisition
hydap	15000/udp	0.000000	# Hypack Hydrographic Software Packages Data Acquisition
unknown	15001/tcp	0.000152
onep-tls	15002/tcp	0.000380	# Open Network Environment TLS
unknown	15003/tcp	0.000380
unknown	15003/udp	0.000330
unknown	15004/tcp	0.000228
unknown	15005/tcp	0.000076
unknown	15006/udp	0.000330
unknown	15009/udp	0.000330
unknown	15015/udp	0.000330
unknown	15022/udp	0.000330
unknown	15041/udp	0.000661
unknown	15044/udp	0.000330
unknown	15050/tcp	0.000076
unknown	15053/udp	0.000991
unknown	15055/udp	0.000661
unknown	15057/udp	0.000330
unknown	15058/udp	0.000330
unknown	15067/udp	0.000661
unknown	15085/udp	0.000330
unknown	15086/udp	0.000661
unknown	15093/udp	0.000330
unknown	15100/udp	0.000330
unknown	15107/udp	0.000330
unknown	15109/udp	0.000330
unknown	15117/udp	0.000330
v2g-secc	15118/tcp	0.000000	# v2g Supply Equipment Communication Controller Discovery Protocol
unknown	15118/udp	0.000330
unknown	15122/udp	0.000330
unknown	15123/udp	0.000661
unknown	15124/udp	0.000661
unknown	15125/udp	0.000330
swgps	15126/tcp	0.000000	# Nortel Java S/WGPS Global Payment Solutions for US credit card authorizations
unknown	15131/udp	0.000330
unknown	15133/udp	0.000330
unknown	15138/udp	0.000991
unknown	15141/udp	0.000330
unknown	15145/tcp	0.000076
unknown	15147/udp	0.000330
unknown	15149/udp	0.000661
bo2k	15151/tcp	0.000013	# Back Orifice 2K BoPeep video output
unknown	15172/udp	0.000330
unknown	15173/udp	0.000330
unknown	15179/udp	0.000330
unknown	15184/udp	0.000330
unknown	15186/udp	0.000661
unknown	15189/udp	0.000330
unknown	15190/tcp	0.000076
unknown	15191/tcp	0.000076
unknown	15199/udp	0.000330
unknown	15200/udp	0.000330
unknown	15214/udp	0.000330
unknown	15220/udp	0.000330
unknown	15222/udp	0.000330
unknown	15230/udp	0.000330
unknown	15239/udp	0.000330
unknown	15240/udp	0.000330
unknown	15242/udp	0.000330
unknown	15243/udp	0.000330
unknown	15251/udp	0.000330
unknown	15260/udp	0.000330
unknown	15265/udp	0.000330
unknown	15267/udp	0.000661
unknown	15274/udp	0.000330
unknown	15275/tcp	0.000076
unknown	15277/udp	0.000330
unknown	15283/udp	0.000330
unknown	15284/udp	0.000330
unknown	15286/udp	0.000330
unknown	15288/udp	0.000330
unknown	15290/udp	0.000661
unknown	15293/udp	0.000330
unknown	15295/udp	0.000330
unknown	15298/udp	0.000330
unknown	15300/udp	0.000330
unknown	15302/udp	0.000330
unknown	15308/udp	0.000330
unknown	15311/udp	0.000330
unknown	15317/tcp	0.000076
unknown	15328/udp	0.000330
unknown	15336/udp	0.000330
unknown	15344/tcp	0.000076
xpilot	15345/tcp	0.000000	# XPilot Contact Port
xpilot	15345/udp	0.000000	# XPilot Contact Port
unknown	15350/udp	0.000330
unknown	15359/udp	0.000330
unknown	15360/udp	0.000661
unknown	15361/udp	0.000661
3link	15363/tcp	0.000000	# 3Link Negotiation
3link	15363/udp	0.000330	# 3Link Negotiation
unknown	15367/udp	0.000330
unknown	15374/udp	0.000330
unknown	15375/udp	0.000330
unknown	15377/udp	0.000330
unknown	15381/udp	0.000661
unknown	15389/udp	0.000330
unknown	15395/udp	0.000330
unknown	15402/tcp	0.000152
unknown	15419/udp	0.000330
unknown	15422/udp	0.000330
unknown	15444/udp	0.000330
unknown	15448/tcp	0.000076
unknown	15448/udp	0.000330
unknown	15449/udp	0.000661
unknown	15468/udp	0.000330
unknown	15473/udp	0.000330
unknown	15477/udp	0.000330
unknown	15479/udp	0.000330
unknown	15483/udp	0.000330
unknown	15491/udp	0.000330
unknown	15506/udp	0.000330
unknown	15507/udp	0.000330
unknown	15509/udp	0.000330
unknown	15514/udp	0.000661
unknown	15519/udp	0.000330
unknown	15524/udp	0.000330
unknown	15529/udp	0.000330
unknown	15536/udp	0.000330
unknown	15540/udp	0.000330
unknown	15549/udp	0.000330
unknown	15550/tcp	0.000076
cisco-snat	15555/tcp	0.000000	# Cisco Stateful NAT
cisco-snat	15555/udp	0.000000	# Cisco Stateful NAT
unknown	15559/udp	0.000330
unknown	15563/udp	0.000330
unknown	15572/udp	0.000330
unknown	15589/udp	0.000330
unknown	15606/udp	0.000330
unknown	15610/udp	0.000330
unknown	15616/udp	0.000330
unknown	15617/udp	0.000330
unknown	15621/udp	0.000661
unknown	15625/udp	0.000330
unknown	15631/tcp	0.000076
unknown	15635/udp	0.000330
unknown	15645/tcp	0.000076
unknown	15646/tcp	0.000076
unknown	15648/udp	0.000661
unknown	15649/udp	0.000330
unknown	15657/udp	0.000330
bex-xr	15660/tcp	0.000380	# Backup Express Restore Server
bex-xr	15660/udp	0.000000	# Backup Express Restore Server
unknown	15670/tcp	0.000076
unknown	15670/udp	0.000330
unknown	15677/tcp	0.000076
unknown	15677/udp	0.000330
unknown	15687/udp	0.000330
unknown	15696/udp	0.000330
unknown	15698/udp	0.000330
unknown	15701/udp	0.000330
unknown	15704/udp	0.000330
unknown	15711/udp	0.000330
unknown	15718/udp	0.000330
unknown	15722/tcp	0.000076
unknown	15722/udp	0.000330
unknown	15730/tcp	0.000076
unknown	15733/udp	0.000661
unknown	15735/udp	0.000330
ptp	15740/tcp	0.000000	# Picture Transfer Protocol
ptp	15740/udp	0.000000	# Picture Transfer Protocol
unknown	15742/tcp	0.000304
unknown	15749/udp	0.000330
unknown	15752/udp	0.000330
unknown	15754/udp	0.000661
unknown	15758/tcp	0.000076
unknown	15777/udp	0.000330
unknown	15782/udp	0.000330
unknown	15785/udp	0.000330
unknown	15798/udp	0.000330
unknown	15803/udp	0.000661
unknown	15804/udp	0.000330
unknown	15811/udp	0.000330
unknown	15814/udp	0.000661
unknown	15816/udp	0.000330
unknown	15829/udp	0.000330
unknown	15831/udp	0.000661
unknown	15833/udp	0.000330
unknown	15840/udp	0.000330
unknown	15846/udp	0.000330
unknown	15854/udp	0.000330
unknown	15871/udp	0.000330
unknown	15888/udp	0.000330
unknown	15891/udp	0.000330
unknown	15894/udp	0.000330
unknown	15895/udp	0.000330
unknown	15900/udp	0.000330
unknown	15915/tcp	0.000076
unknown	15916/udp	0.000330
unknown	15917/udp	0.000330
unknown	15934/udp	0.000330
unknown	15950/udp	0.000330
unknown	15953/udp	0.000330
unknown	15955/udp	0.000330
unknown	15960/udp	0.000330
unknown	15966/udp	0.000661
unknown	15969/udp	0.000661
2ping	15998/tcp	0.000000	# 2ping Bi-Directional Ping Service
2ping	15998/udp	0.000000	# 2ping Bi-Directional Ping Service
programmar	15999/tcp	0.000000	# ProGrammar Enterprise
unknown	15999/udp	0.000330
fmsas	16000/tcp	0.000228	# Administration Server Access
fmsascon	16001/tcp	0.000380	# Administration Server Connector
gsms	16002/tcp	0.000000	# GoodSync Mediation Service
alfin	16003/tcp	0.000000	# Automation and Control by REGULACE.ORG
alfin	16003/udp	0.000000	# Automation and Control by REGULACE.ORG
unknown	16012/tcp	0.000304
unknown	16013/udp	0.000330
unknown	16016/tcp	0.000380
unknown	16018/tcp	0.000380
jwpc	16020/tcp	0.000000	# Filemaker Java Web Publishing Core
jwpc-bin	16021/tcp	0.000000	# Filemaker Java Web Publishing Core Binary
unknown	16023/udp	0.000330
unknown	16027/udp	0.000330
unknown	16030/udp	0.000330
unknown	16031/udp	0.000330
unknown	16035/udp	0.000330
unknown	16045/udp	0.000330
unknown	16046/udp	0.000330
unknown	16048/tcp	0.000076
unknown	16055/udp	0.000330
unknown	16057/udp	0.000330
unknown	16062/udp	0.000330
unknown	16066/udp	0.000661
unknown	16067/udp	0.000330
unknown	16072/udp	0.000330
osxwebadmin	16080/tcp	0.000251	# Apple OS X WebAdmin
unknown	16080/udp	0.000330
unknown	16085/udp	0.000330
unknown	16086/udp	0.001321
unknown	16094/udp	0.000330
unknown	16098/udp	0.000330
unknown	16100/udp	0.000330
unknown	16103/udp	0.000330
unknown	16108/udp	0.000661
unknown	16109/udp	0.000330
unknown	16113/tcp	0.000228
unknown	16113/udp	0.000330
unknown	16115/udp	0.000330
unknown	16116/udp	0.000330
unknown	16121/udp	0.000330
unknown	16122/udp	0.000330
unknown	16130/udp	0.000330
unknown	16134/udp	0.000330
unknown	16139/udp	0.000330
unknown	16141/udp	0.000330
unknown	16155/udp	0.000661
unknown	16159/udp	0.000661
sun-sea-port	16161/tcp	0.000076	# Solaris SEA Port
sun-sea-port	16161/udp	0.000000	# Solaris SEA Port
solaris-audit	16162/tcp	0.000000	# Solaris Audit - secure remote audit log
unknown	16163/udp	0.000330
unknown	16178/udp	0.000330
unknown	16187/udp	0.000330
unknown	16189/udp	0.000330
unknown	16195/udp	0.000330
unknown	16208/udp	0.000330
unknown	16209/udp	0.000330
unknown	16210/udp	0.000330
unknown	16212/udp	0.000330
unknown	16222/udp	0.000330
unknown	16226/udp	0.000661
unknown	16228/udp	0.000330
unknown	16231/udp	0.000330
unknown	16233/udp	0.000330
unknown	16241/udp	0.000330
unknown	16242/udp	0.000330
unknown	16257/udp	0.000330
unknown	16262/udp	0.000330
unknown	16263/udp	0.000661
unknown	16268/udp	0.000330
unknown	16270/tcp	0.000076
unknown	16273/tcp	0.000076
unknown	16273/udp	0.000330
unknown	16283/tcp	0.000076
unknown	16283/udp	0.000330
unknown	16286/tcp	0.000076
unknown	16289/udp	0.000330
unknown	16297/tcp	0.000076
unknown	16297/udp	0.000330
unknown	16298/udp	0.000330
unknown	16306/udp	0.000330
etb4j	16309/tcp	0.000000
etb4j	16309/udp	0.000000
pduncs	16310/tcp	0.000000	# Policy Distribute, Update Notification
pduncs	16310/udp	0.000000	# Policy Distribute, Update Notification
pdefmns	16311/tcp	0.000000	# Policy definition and update management
pdefmns	16311/udp	0.000000	# Policy definition and update management
unknown	16312/udp	0.000661
unknown	16316/udp	0.000330
unknown	16326/udp	0.000330
unknown	16327/udp	0.000330
unknown	16331/udp	0.000330
unknown	16334/udp	0.000661
unknown	16342/udp	0.000330
unknown	16349/tcp	0.000076
unknown	16355/udp	0.000330
unknown	16359/udp	0.000330
netserialext1	16360/tcp	0.000000	# Network Serial Extension Ports One
netserialext1	16360/udp	0.000000	# Network Serial Extension Ports One
netserialext2	16361/tcp	0.000000	# Network Serial Extension Ports Two
netserialext2	16361/udp	0.000330	# Network Serial Extension Ports Two
netserialext3	16367/tcp	0.000000	# Network Serial Extension Ports Three
netserialext3	16367/udp	0.000000	# Network Serial Extension Ports Three
netserialext4	16368/tcp	0.000000	# Network Serial Extension Ports Four
netserialext4	16368/udp	0.000000	# Network Serial Extension Ports Four
unknown	16372/tcp	0.000076
unknown	16376/udp	0.000330
unknown	16378/udp	0.000330
unknown	16382/udp	0.000330
connected	16384/tcp	0.000000	# Connected Corp
connected	16384/udp	0.000000	# Connected Corp
rdgs	16385/tcp	0.000000	# Reliable Datagram Sockets
unknown	16386/udp	0.000654
unknown	16387/udp	0.000654
unknown	16390/udp	0.000654
unknown	16392/udp	0.000654
unknown	16395/udp	0.000654
unknown	16398/udp	0.000654
unknown	16400/udp	0.000654
unknown	16402/udp	0.001961
unknown	16403/udp	0.000654
unknown	16405/udp	0.000654
unknown	16410/udp	0.000654
unknown	16413/udp	0.000654
unknown	16416/udp	0.000654
unknown	16420/udp	0.001307
unknown	16421/udp	0.000654
unknown	16424/udp	0.000654
unknown	16429/udp	0.000654
unknown	16430/udp	0.001961
unknown	16431/udp	0.000654
unknown	16433/udp	0.001307
unknown	16435/udp	0.000654
unknown	16439/udp	0.000654
unknown	16441/udp	0.000654
overnet	16444/tcp	0.000025	# Overnet file sharing
overnet	16444/udp	0.000726	# Overnet file sharing
unknown	16449/udp	0.001307
unknown	16452/udp	0.000654
unknown	16453/udp	0.000654
unknown	16455/udp	0.000654
unknown	16462/udp	0.000654
unknown	16463/udp	0.000654
unknown	16464/tcp	0.000076
unknown	16464/udp	0.000654
unknown	16465/udp	0.000654
unknown	16469/udp	0.000654
unknown	16470/udp	0.000654
unknown	16475/udp	0.000654
unknown	16476/udp	0.000654
unknown	16480/udp	0.000654
unknown	16482/udp	0.000654
unknown	16484/udp	0.000654
unknown	16496/udp	0.000654
unknown	16497/udp	0.000654
unknown	16498/udp	0.001307
unknown	16502/udp	0.000654
unknown	16503/udp	0.001307
unknown	16512/udp	0.000654
unknown	16518/udp	0.000654
unknown	16521/udp	0.000654
unknown	16527/udp	0.000654
unknown	16532/udp	0.000654
unknown	16536/udp	0.000654
unknown	16537/udp	0.000654
unknown	16540/udp	0.000654
unknown	16541/udp	0.000654
unknown	16542/udp	0.000654
unknown	16545/udp	0.001307
unknown	16548/udp	0.001307
unknown	16552/udp	0.000654
unknown	16555/udp	0.000654
unknown	16556/udp	0.000654
unknown	16557/udp	0.000654
unknown	16562/udp	0.000654
unknown	16564/udp	0.000654
unknown	16565/udp	0.000654
unknown	16570/udp	0.000654
unknown	16573/udp	0.001307
unknown	16577/udp	0.000654
unknown	16578/udp	0.000654
unknown	16581/udp	0.000654
unknown	16582/udp	0.000654
unknown	16585/udp	0.000654
unknown	16596/udp	0.000654
unknown	16597/udp	0.000654
unknown	16601/udp	0.000654
unknown	16606/udp	0.000654
unknown	16607/udp	0.000654
unknown	16609/udp	0.000654
unknown	16611/udp	0.000654
unknown	16613/udp	0.000654
unknown	16618/udp	0.000654
xoms	16619/tcp	0.000000	# X509 Objects Management Service
unknown	16619/udp	0.000654
unknown	16620/udp	0.000654
unknown	16623/udp	0.000654
unknown	16624/udp	0.000654
unknown	16633/udp	0.000654
unknown	16641/udp	0.000654
unknown	16648/udp	0.000654
unknown	16649/udp	0.000654
unknown	16654/udp	0.000654
axon-tunnel	16665/tcp	0.000000	# Reliable multipath data transport for high latencies
vtp	16666/tcp	0.000000	# Vidder Tunnel Protocol
unknown	16669/udp	0.000654
unknown	16671/udp	0.000654
unknown	16673/udp	0.000654
unknown	16674/udp	0.001307
unknown	16676/udp	0.000654
unknown	16680/udp	0.003268
unknown	16684/udp	0.000654
unknown	16686/udp	0.000654
unknown	16696/udp	0.000654
unknown	16697/udp	0.001307
unknown	16700/udp	0.001307
unknown	16704/udp	0.000654
unknown	16705/tcp	0.000152
unknown	16708/udp	0.001307
unknown	16709/udp	0.000654
unknown	16711/udp	0.001307
unknown	16714/udp	0.000654
unknown	16716/udp	0.000654
unknown	16719/udp	0.000654
unknown	16723/tcp	0.000076
unknown	16723/udp	0.000654
unknown	16724/tcp	0.000076
unknown	16725/tcp	0.000076
unknown	16728/udp	0.000654
unknown	16731/udp	0.000654
unknown	16732/udp	0.000654
unknown	16736/udp	0.000654
unknown	16739/udp	0.001307
unknown	16742/udp	0.000654
unknown	16743/udp	0.000654
unknown	16746/udp	0.000654
unknown	16747/udp	0.000654
unknown	16748/udp	0.000654
unknown	16749/udp	0.000654
unknown	16754/udp	0.000654
unknown	16761/udp	0.000654
unknown	16762/udp	0.000654
unknown	16766/udp	0.001307
unknown	16768/udp	0.000654
unknown	16779/udp	0.001307
unknown	16786/udp	0.001307
unknown	16787/udp	0.000654
unknown	16788/udp	0.000654
cadsisvr	16789/tcp	0.000000	# This server provides callable services to mainframe External Security Managers from any TCP/IP platform
unknown	16789/udp	0.000654
unknown	16791/udp	0.000654
unknown	16795/udp	0.000654
unknown	16797/tcp	0.000076
unknown	16797/udp	0.000654
unknown	16800/tcp	0.000152
unknown	16806/udp	0.000654
unknown	16816/udp	0.001307
unknown	16824/udp	0.000654
unknown	16828/udp	0.000654
unknown	16829/udp	0.001307
unknown	16832/udp	0.002614
unknown	16838/udp	0.001307
unknown	16839/udp	0.001307
unknown	16845/tcp	0.000076
unknown	16849/udp	0.000654
unknown	16851/tcp	0.000152
unknown	16851/udp	0.000654
unknown	16862/udp	0.001307
unknown	16864/udp	0.000654
unknown	16875/udp	0.000654
unknown	16877/udp	0.000654
unknown	16879/udp	0.000654
unknown	16888/udp	0.000654
unknown	16890/udp	0.000654
unknown	16892/udp	0.000654
unknown	16896/udp	0.001307
unknown	16897/udp	0.000654
newbay-snc-mc	16900/tcp	0.000076	# Newbay Mobile Client Update Service
newbay-snc-mc	16900/udp	0.000000	# Newbay Mobile Client Update Service
unknown	16901/tcp	0.000076
unknown	16908/udp	0.000654
unknown	16912/udp	0.001307
unknown	16913/udp	0.000654
unknown	16918/udp	0.001961
unknown	16919/udp	0.001307
unknown	16921/udp	0.000654
unknown	16924/udp	0.000654
unknown	16926/udp	0.000654
unknown	16937/udp	0.000654
unknown	16938/udp	0.001307
unknown	16939/udp	0.001307
unknown	16944/udp	0.000654
unknown	16946/udp	0.000654
unknown	16947/udp	0.002614
unknown	16948/udp	0.001307
sgcip	16950/tcp	0.000000	# Simple Generic Client Interface Protocol
sgcip	16950/udp	0.000000	# Simple Generic Client Interface Protocol
unknown	16951/udp	0.000654
unknown	16954/udp	0.000654
unknown	16955/udp	0.000654
unknown	16957/udp	0.000654
subseven	16959/tcp	0.000000	# Subseven trojan
unknown	16968/udp	0.000654
unknown	16970/udp	0.001307
unknown	16971/udp	0.000654
unknown	16972/udp	0.001307
unknown	16974/udp	0.001307
unknown	16976/udp	0.000654
unknown	16985/udp	0.000654
unknown	16990/udp	0.000654
intel-rci-mp	16991/tcp	0.000000
intel-rci-mp	16991/udp	0.000000
amt-soap-http	16992/tcp	0.000760	# Intel(R) AMT SOAP/HTTP
amt-soap-http	16992/udp	0.000000	# Intel(R) AMT SOAP/HTTP
amt-soap-https	16993/tcp	0.000760	# Intel(R) AMT SOAP/HTTPS
amt-soap-https	16993/udp	0.000000	# Intel(R) AMT SOAP/HTTPS
amt-redir-tcp	16994/tcp	0.000000	# Intel(R) AMT Redirection/TCP
amt-redir-tcp	16994/udp	0.000000	# Intel(R) AMT Redirection/TCP
amt-redir-tls	16995/tcp	0.000000	# Intel(R) AMT Redirection/TLS
amt-redir-tls	16995/udp	0.000000	# Intel(R) AMT Redirection/TLS
unknown	16997/udp	0.000654
unknown	17001/udp	0.000654
unknown	17003/udp	0.000654
unknown	17005/udp	0.000654
unknown	17006/udp	0.001307
isode-dua	17007/tcp	0.000013
isode-dua	17007/udp	0.000591
ncpu	17010/tcp	0.000000	# Plan 9 cpu port
unknown	17010/udp	0.000654
unknown	17011/udp	0.000654
unknown	17012/udp	0.000654
unknown	17016/tcp	0.000076
unknown	17017/tcp	0.000076
unknown	17018/udp	0.001307
unknown	17023/udp	0.000654
unknown	17028/udp	0.000654
unknown	17032/udp	0.000654
unknown	17046/udp	0.000654
unknown	17048/udp	0.000654
unknown	17049/udp	0.000654
unknown	17053/udp	0.000654
unknown	17054/udp	0.000654
unknown	17061/udp	0.000654
unknown	17063/udp	0.000654
unknown	17064/udp	0.000654
unknown	17065/udp	0.000654
unknown	17068/udp	0.000654
unknown	17070/tcp	0.000076
unknown	17077/udp	0.001307
unknown	17082/udp	0.000654
unknown	17083/udp	0.000654
unknown	17089/tcp	0.000076
unknown	17091/udp	0.001961
unknown	17093/udp	0.000654
unknown	17095/udp	0.000654
unknown	17101/udp	0.001307
unknown	17108/udp	0.000654
unknown	17115/udp	0.000654
unknown	17126/udp	0.000654
unknown	17129/tcp	0.000076
unknown	17133/udp	0.000654
unknown	17137/udp	0.000654
unknown	17143/udp	0.000654
unknown	17145/udp	0.000654
unknown	17146/udp	0.001307
unknown	17147/udp	0.000654
unknown	17151/udp	0.000654
unknown	17153/udp	0.000654
unknown	17161/udp	0.000654
unknown	17172/udp	0.000654
unknown	17174/udp	0.000654
unknown	17179/udp	0.000654
unknown	17182/udp	0.000654
vestasdlp	17184/tcp	0.000000	# Vestas Data Layer Protocol
unknown	17184/udp	0.001307
soundsvirtual	17185/tcp	0.000000	# Sounds Virtual
wdbrpc	17185/udp	0.013395	# vxWorks WDB remote debugging ONCRPC
unknown	17188/udp	0.000654
unknown	17189/udp	0.000654
unknown	17190/udp	0.000654
unknown	17195/udp	0.000654
unknown	17199/udp	0.000654
unknown	17203/udp	0.000654
unknown	17205/udp	0.001307
unknown	17207/udp	0.001307
unknown	17212/udp	0.000654
unknown	17213/udp	0.000654
unknown	17216/udp	0.000654
chipper	17219/tcp	0.000000
chipper	17219/udp	0.001307
avtp	17220/tcp	0.000000	# IEEE 1722 Transport Protocol for Time Sensitive Applications
unknown	17220/udp	0.000654
avdecc	17221/tcp	0.000000	# IEEE 1722.1 AVB Discovery, Enumeration, Connection management, and Control
cpsp	17222/tcp	0.000000	# Control Plane Synchronization Protocol (SPSP)
isa100-gci	17223/tcp	0.000000	# ISA100 GCI is a service utilizing a common interface between an ISA100 Wireless gateway and a client application
trdp-pd	17224/tcp	0.000000	# Train Realtime Data Protocol (TRDP) Process Data
unknown	17224/udp	0.000654
trdp-md	17225/tcp	0.000000	# Train Realtime Data Protocol (TRDP) Message Data
unknown	17225/udp	0.000654
unknown	17229/udp	0.000654
integrius-stp	17234/tcp	0.000000	# Integrius Secure Tunnel Protocol
integrius-stp	17234/udp	0.000000	# Integrius Secure Tunnel Protocol
ssh-mgmt	17235/tcp	0.000000	# SSH Tectia Manager
ssh-mgmt	17235/udp	0.000654	# SSH Tectia Manager
unknown	17236/udp	0.001307
unknown	17237/udp	0.001307
unknown	17245/udp	0.000654
unknown	17246/udp	0.000654
unknown	17249/udp	0.000654
unknown	17251/tcp	0.000076
unknown	17252/udp	0.000654
unknown	17255/tcp	0.000076
unknown	17263/udp	0.000654
unknown	17264/udp	0.000654
unknown	17265/udp	0.000654
unknown	17269/udp	0.000654
unknown	17272/udp	0.000654
unknown	17273/udp	0.000654
unknown	17275/udp	0.000654
unknown	17281/udp	0.000654
unknown	17282/udp	0.001307
unknown	17284/udp	0.000654
unknown	17286/udp	0.000654
unknown	17295/udp	0.000654
unknown	17297/udp	0.000654
unknown	17299/udp	0.000654
kuang2	17300/tcp	0.000013	# Kuang2 backdoor
unknown	17300/udp	0.000654
unknown	17302/udp	0.001307
unknown	17313/udp	0.000654
unknown	17320/udp	0.000654
unknown	17321/udp	0.001307
unknown	17324/udp	0.000654
unknown	17331/udp	0.001307
unknown	17332/udp	0.001307
unknown	17336/udp	0.000654
unknown	17338/udp	0.001307
unknown	17340/udp	0.000654
unknown	17341/udp	0.000654
unknown	17342/udp	0.000654
unknown	17343/udp	0.000654
unknown	17344/udp	0.000654
unknown	17348/udp	0.000654
unknown	17350/udp	0.000654
unknown	17354/udp	0.000654
unknown	17359/udp	0.001307
unknown	17372/udp	0.000654
unknown	17376/udp	0.000654
unknown	17378/udp	0.000654
unknown	17389/udp	0.000654
unknown	17393/udp	0.000654
unknown	17394/udp	0.000654
unknown	17396/udp	0.000654
unknown	17397/udp	0.000654
unknown	17401/udp	0.000654
unknown	17406/udp	0.000654
unknown	17407/udp	0.000654
unknown	17409/tcp	0.000076
unknown	17409/udp	0.000654
unknown	17412/udp	0.000654
unknown	17413/tcp	0.000076
unknown	17417/udp	0.001307
unknown	17418/udp	0.000654
unknown	17423/udp	0.001307
unknown	17424/udp	0.001307
unknown	17444/udp	0.000654
unknown	17445/udp	0.000654
unknown	17449/udp	0.000654
unknown	17455/udp	0.001961
unknown	17459/udp	0.001961
unknown	17468/udp	0.001307
unknown	17475/udp	0.000654
unknown	17477/udp	0.000654
unknown	17479/udp	0.000654
unknown	17482/udp	0.000654
unknown	17484/udp	0.000654
unknown	17487/udp	0.001307
unknown	17488/udp	0.000654
unknown	17490/udp	0.001307
unknown	17491/udp	0.000654
unknown	17492/udp	0.000654
unknown	17493/udp	0.000654
unknown	17494/udp	0.001307
unknown	17495/udp	0.000654
unknown	17499/udp	0.000654
db-lsp	17500/tcp	0.000076	# db-lsp-disc | Dropbox LanSync Protocol | Dropbox LanSync Discovery
db-lsp-disc	17500/udp	0.000000	# Dropbox LanSync Discovery
unknown	17501/udp	0.000654
unknown	17505/udp	0.001307
unknown	17511/udp	0.000654
unknown	17514/udp	0.000654
unknown	17519/udp	0.000654
unknown	17520/udp	0.000654
unknown	17526/udp	0.000654
unknown	17528/udp	0.000654
unknown	17533/udp	0.001307
unknown	17534/udp	0.000654
unknown	17546/udp	0.000654
unknown	17548/udp	0.000654
unknown	17549/udp	0.001307
unknown	17550/udp	0.000654
unknown	17553/udp	0.000654
ailith	17555/tcp	0.000000	# Ailith management of routers
unknown	17559/udp	0.000654
unknown	17563/udp	0.000654
unknown	17566/udp	0.000654
unknown	17567/udp	0.000654
unknown	17573/udp	0.001961
unknown	17580/udp	0.001307
unknown	17585/udp	0.001307
unknown	17586/udp	0.000654
unknown	17587/udp	0.000654
unknown	17592/udp	0.001307
unknown	17594/udp	0.000654
unknown	17595/tcp	0.000152
unknown	17599/udp	0.000654
unknown	17605/udp	0.001307
unknown	17607/udp	0.000654
unknown	17609/udp	0.000654
unknown	17610/udp	0.000654
unknown	17614/udp	0.000654
unknown	17615/udp	0.001961
unknown	17616/udp	0.001961
unknown	17618/udp	0.000654
unknown	17627/udp	0.000654
unknown	17629/udp	0.001307
unknown	17635/udp	0.000654
unknown	17638/udp	0.001307
unknown	17644/udp	0.000654
unknown	17645/udp	0.000654
unknown	17650/udp	0.000654
unknown	17654/udp	0.000654
unknown	17658/udp	0.000654
unknown	17663/udp	0.001307
unknown	17667/udp	0.000654
unknown	17668/udp	0.000654
unknown	17669/udp	0.000654
unknown	17673/udp	0.001307
unknown	17674/udp	0.001307
unknown	17675/udp	0.000654
unknown	17679/udp	0.000654
unknown	17680/udp	0.000654
unknown	17682/udp	0.000654
unknown	17683/udp	0.001307
unknown	17688/udp	0.000654
unknown	17693/udp	0.000654
unknown	17696/udp	0.000654
unknown	17698/udp	0.000654
unknown	17700/tcp	0.000076
unknown	17700/udp	0.000654
unknown	17701/tcp	0.000076
unknown	17701/udp	0.000654
unknown	17702/tcp	0.000076
unknown	17707/udp	0.000654
unknown	17712/udp	0.000654
unknown	17713/udp	0.000654
unknown	17715/tcp	0.000076
unknown	17720/udp	0.000654
unknown	17726/udp	0.001307
ea	17729/tcp	0.000000	# Eclipse Aviation
ea	17729/udp	0.000000	# Eclipse Aviation
unknown	17731/udp	0.000654
unknown	17734/udp	0.000654
unknown	17735/udp	0.000654
unknown	17737/udp	0.000654
unknown	17739/udp	0.000654
unknown	17740/udp	0.000654
unknown	17748/udp	0.000654
zep	17754/tcp	0.000000	# Encap. ZigBee Packets
zep	17754/udp	0.001307	# Encap. ZigBee Packets
zigbee-ip	17755/tcp	0.000000	# ZigBee IP Transport Service
zigbee-ip	17755/udp	0.000654	# ZigBee IP Transport Service
zigbee-ips	17756/tcp	0.000000	# ZigBee IP Transport Secure Service
zigbee-ips	17756/udp	0.000654	# ZigBee IP Transport Secure Service
unknown	17757/udp	0.000654
unknown	17762/udp	0.001307
unknown	17766/udp	0.000654
unknown	17769/udp	0.000654
unknown	17770/udp	0.000654
unknown	17775/udp	0.000654
sw-orion	17777/tcp	0.000000	# SolarWinds Orion
unknown	17778/udp	0.000654
unknown	17787/udp	0.001307
unknown	17788/udp	0.000654
unknown	17796/udp	0.000654
unknown	17798/udp	0.000654
unknown	17800/udp	0.000654
unknown	17801/tcp	0.000076
unknown	17802/tcp	0.000076
unknown	17814/udp	0.001307
unknown	17816/udp	0.000654
unknown	17818/udp	0.000654
unknown	17820/udp	0.000654
unknown	17823/udp	0.001307
unknown	17824/udp	0.001307
unknown	17828/udp	0.000654
unknown	17836/udp	0.001307
unknown	17837/udp	0.000654
unknown	17845/udp	0.001307
unknown	17848/udp	0.000654
unknown	17849/udp	0.000654
unknown	17852/udp	0.000654
unknown	17860/tcp	0.000076
unknown	17863/udp	0.000654
unknown	17865/udp	0.000654
unknown	17866/udp	0.000654
unknown	17867/tcp	0.000076
unknown	17867/udp	0.000654
unknown	17877/tcp	0.000228
unknown	17880/udp	0.000654
unknown	17883/udp	0.000654
unknown	17885/udp	0.000654
unknown	17886/udp	0.000654
unknown	17887/udp	0.000654
unknown	17888/udp	0.001961
unknown	17889/udp	0.000654
unknown	17893/udp	0.000654
unknown	17895/udp	0.000654
unknown	17899/udp	0.000654
unknown	17900/udp	0.000654
unknown	17901/udp	0.000654
unknown	17903/udp	0.000654
unknown	17905/udp	0.000654
unknown	17924/udp	0.000654
unknown	17931/udp	0.000654
unknown	17939/udp	0.001961
unknown	17943/udp	0.000654
unknown	17946/udp	0.001307
unknown	17950/udp	0.000654
unknown	17953/udp	0.000654
unknown	17964/udp	0.000654
unknown	17966/udp	0.000654
unknown	17969/tcp	0.000076
unknown	17982/udp	0.000654
unknown	17985/tcp	0.000076
unknown	17987/udp	0.000654
unknown	17988/tcp	0.000380
unknown	17988/udp	0.000654
unknown	17989/udp	0.001961
unknown	17993/udp	0.000654
unknown	17996/udp	0.000654
unknown	17997/tcp	0.000076
biimenu	18000/tcp	0.000138	# Beckman Instruments, Inc.
biimenu	18000/udp	0.000541	# Beckman Instruments, Inc.
unknown	18003/udp	0.000654
unknown	18004/udp	0.001961
unknown	18005/udp	0.000654
unknown	18012/tcp	0.000076
unknown	18012/udp	0.000654
unknown	18013/udp	0.000654
unknown	18015/tcp	0.000076
unknown	18018/tcp	0.000152
unknown	18021/udp	0.000654
unknown	18023/udp	0.000654
unknown	18025/udp	0.000654
unknown	18038/udp	0.000654
unknown	18040/tcp	0.000228
unknown	18042/udp	0.000654
unknown	18052/udp	0.000654
unknown	18053/udp	0.000654
unknown	18066/udp	0.000654
unknown	18069/udp	0.000654
unknown	18074/udp	0.000654
unknown	18075/udp	0.000654
unknown	18080/tcp	0.000076
unknown	18081/udp	0.001307
unknown	18088/udp	0.000654
unknown	18089/udp	0.000654
unknown	18093/udp	0.000654
unknown	18097/udp	0.000654
unknown	18098/udp	0.000654
unknown	18100/udp	0.000654
unknown	18101/tcp	0.000228
unknown	18103/udp	0.000654
radpdf	18104/tcp	0.000000	# RAD PDF Service
unknown	18113/udp	0.001307
unknown	18117/udp	0.000654
unknown	18120/udp	0.000654
unknown	18130/udp	0.000654
unknown	18131/udp	0.000654
unknown	18134/udp	0.001307
racf	18136/tcp	0.000000	# z/OS Resource Access Control Facility
unknown	18136/udp	0.000654
unknown	18145/udp	0.000654
unknown	18148/tcp	0.000076
unknown	18150/udp	0.000654
unknown	18154/udp	0.000654
unknown	18156/udp	0.001307
unknown	18161/udp	0.000654
unknown	18163/udp	0.000654
unknown	18164/udp	0.000654
unknown	18165/udp	0.000654
unknown	18166/udp	0.000654
unknown	18174/udp	0.000654
unknown	18179/udp	0.000654
opsec-cvp	18181/tcp	0.000025	# Check Point OPSEC | OPSEC CVP
opsec-cvp	18181/udp	0.000000	# OPSEC CVP
opsec-ufp	18182/tcp	0.000038	# Check Point OPSEC | OPSEC UFP
opsec-ufp	18182/udp	0.000654	# OPSEC UFP
opsec-sam	18183/tcp	0.000025	# Check Point OPSEC | OPSEC SAM
opsec-sam	18183/udp	0.000654	# OPSEC SAM
opsec-lea	18184/tcp	0.000038	# Check Point OPSEC | OPSEC LEA
opsec-lea	18184/udp	0.000000	# OPSEC LEA
opsec-omi	18185/tcp	0.000000	# Check Point OPSEC | OPSEC OMI
opsec-omi	18185/udp	0.000000	# OPSEC OMI
ohsc	18186/tcp	0.000000	# Occupational Health SC | Occupational Health Sc
ohsc	18186/udp	0.000000	# Occupational Health Sc
opsec-ela	18187/tcp	0.000013	# Check Point OPSEC | OPSEC ELA
opsec-ela	18187/udp	0.000000	# OPSEC ELA
unknown	18189/udp	0.000654
unknown	18193/udp	0.000654
unknown	18202/udp	0.000654
unknown	18203/udp	0.000654
unknown	18208/udp	0.000654
unknown	18214/udp	0.000654
unknown	18215/udp	0.000654
unknown	18225/udp	0.000654
unknown	18228/udp	0.001307
unknown	18231/tcp	0.000076
unknown	18231/udp	0.000654
unknown	18234/udp	0.001961
unknown	18236/udp	0.000654
unknown	18240/udp	0.000654
checkpoint-rtm	18241/tcp	0.000000	# Check Point RTM
checkpoint-rtm	18241/udp	0.000000	# Check Point RTM
iclid	18242/tcp	0.000000	# Checkpoint router monitoring
clusterxl	18243/tcp	0.000000	# Checkpoint router state backup
unknown	18250/udp	0.001307
unknown	18252/udp	0.000654
unknown	18255/udp	0.001307
unknown	18256/udp	0.000654
unknown	18258/udp	0.001307
unknown	18259/udp	0.000654
unknown	18261/udp	0.000654
gv-pf	18262/tcp	0.000000	# GV NetConfig Service
gv-pf	18262/udp	0.000654	# GV NetConfig Service
unknown	18264/tcp	0.000152
unknown	18273/udp	0.000654
unknown	18275/udp	0.000654
unknown	18284/udp	0.000654
unknown	18287/udp	0.000654
unknown	18289/udp	0.000654
unknown	18296/udp	0.000654
unknown	18297/udp	0.000654
unknown	18301/udp	0.000654
unknown	18306/udp	0.000654
unknown	18308/udp	0.000654
unknown	18309/udp	0.000654
unknown	18318/udp	0.000654
unknown	18319/udp	0.001307
unknown	18323/udp	0.000654
unknown	18324/udp	0.000654
unknown	18327/udp	0.000654
unknown	18328/udp	0.000654
unknown	18331/udp	0.001961
bitcoin	18333/tcp	0.000076	# Bitcoin crypto currency - https://en.bitcoin.it/wiki/Running_Bitcoin
unknown	18336/tcp	0.000076
unknown	18337/tcp	0.000076
unknown	18343/udp	0.000654
unknown	18344/udp	0.000654
unknown	18346/udp	0.000654
unknown	18348/udp	0.000654
unknown	18354/udp	0.000654
unknown	18355/udp	0.000654
unknown	18360/udp	0.001961
unknown	18362/udp	0.000654
unknown	18365/udp	0.000654
unknown	18369/udp	0.000654
unknown	18373/udp	0.001307
unknown	18380/tcp	0.000076
unknown	18384/udp	0.000654
unknown	18393/udp	0.000654
unknown	18396/udp	0.000654
unknown	18398/udp	0.000654
unknown	18402/udp	0.000654
unknown	18415/udp	0.000654
unknown	18417/udp	0.000654
unknown	18420/udp	0.000654
unknown	18423/udp	0.000654
unknown	18428/udp	0.000654
unknown	18433/udp	0.000654
unknown	18438/udp	0.000654
unknown	18439/tcp	0.000076
unknown	18440/udp	0.000654
unknown	18446/udp	0.000654
unknown	18447/udp	0.000654
unknown	18448/udp	0.000654
unknown	18449/udp	0.002614
unknown	18456/udp	0.000654
unknown	18462/udp	0.000654
ac-cluster	18463/tcp	0.000000	# AC Cluster
ac-cluster	18463/udp	0.000000	# AC Cluster
unknown	18471/udp	0.000654
unknown	18476/udp	0.000654
unknown	18477/udp	0.000654
unknown	18485/udp	0.001307
unknown	18487/udp	0.000654
unknown	18488/udp	0.000654
unknown	18493/udp	0.000654
unknown	18495/udp	0.000654
unknown	18497/udp	0.000654
unknown	18498/udp	0.000654
unknown	18501/udp	0.000654
unknown	18503/udp	0.000654
unknown	18505/tcp	0.000076
unknown	18508/udp	0.000654
heythings	18516/tcp	0.000000	# HeyThings Device communicate service
unknown	18517/tcp	0.000076
unknown	18517/udp	0.000654
unknown	18525/udp	0.000654
unknown	18529/udp	0.000654
unknown	18531/udp	0.000654
unknown	18536/udp	0.000654
unknown	18543/udp	0.001307
unknown	18551/udp	0.000654
unknown	18560/udp	0.000654
unknown	18561/udp	0.000654
unknown	18564/udp	0.000654
unknown	18566/udp	0.000654
unknown	18569/tcp	0.000076
unknown	18572/udp	0.000654
unknown	18573/udp	0.000654
unknown	18577/udp	0.000654
unknown	18581/udp	0.000654
unknown	18582/udp	0.001961
unknown	18593/udp	0.000654
unknown	18605/udp	0.001307
unknown	18606/udp	0.000654
unknown	18611/udp	0.000654
unknown	18612/udp	0.000654
unknown	18615/udp	0.000654
unknown	18617/udp	0.001307
unknown	18621/udp	0.000654
unknown	18622/udp	0.000654
unknown	18623/udp	0.000654
unknown	18625/udp	0.000654
unknown	18626/udp	0.000654
unknown	18628/udp	0.000654
unknown	18630/udp	0.000654
unknown	18632/udp	0.000654
rds-ib	18634/tcp	0.000000	# Reliable Datagram Service
rds-ib	18634/udp	0.000000	# Reliable Datagram Service
rds-ip	18635/tcp	0.000000	# Reliable Datagram Service over IP
rds-ip	18635/udp	0.000000	# Reliable Datagram Service over IP
unknown	18640/udp	0.000654
unknown	18651/udp	0.000654
unknown	18652/udp	0.000654
unknown	18654/udp	0.000654
unknown	18655/udp	0.000654
unknown	18656/udp	0.000654
unknown	18666/udp	0.001307
vdmmesh	18668/tcp	0.000000	# vdmmesh-disc | Manufacturing Execution Systems Mesh Communication
unknown	18668/udp	0.000654
unknown	18669/tcp	0.000076
unknown	18669/udp	0.001307
unknown	18674/udp	0.000654
unknown	18676/udp	0.001307
unknown	18677/udp	0.000654
unknown	18679/udp	0.000654
unknown	18683/udp	0.001307
unknown	18684/udp	0.000654
unknown	18685/udp	0.000654
unknown	18686/udp	0.000654
unknown	18692/udp	0.000654
unknown	18701/udp	0.000654
unknown	18703/udp	0.000654
unknown	18705/udp	0.000654
unknown	18709/udp	0.000654
unknown	18715/udp	0.000654
unknown	18717/udp	0.000654
unknown	18720/udp	0.000654
unknown	18723/udp	0.000654
unknown	18725/udp	0.000654
unknown	18730/udp	0.000654
unknown	18735/udp	0.000654
unknown	18739/udp	0.000654
unknown	18746/udp	0.000654
unknown	18754/udp	0.000654
unknown	18758/udp	0.000654
unknown	18759/udp	0.000654
unknown	18762/udp	0.000654
unknown	18763/udp	0.000654
unknown	18764/udp	0.000654
unknown	18766/udp	0.000654
ique	18769/tcp	0.000000	# IQue Protocol
ique	18769/udp	0.000654	# IQue Protocol
unknown	18772/udp	0.000654
unknown	18791/udp	0.000654
unknown	18796/udp	0.000654
unknown	18797/udp	0.000654
unknown	18801/udp	0.000654
unknown	18806/udp	0.000654
unknown	18807/udp	0.001307
unknown	18812/udp	0.000654
unknown	18817/udp	0.000654
unknown	18818/udp	0.001307
unknown	18821/udp	0.001307
unknown	18826/udp	0.000654
unknown	18828/udp	0.000654
unknown	18830/udp	0.001307
unknown	18831/udp	0.000654
unknown	18832/udp	0.001307
unknown	18834/udp	0.000654
unknown	18835/udp	0.001961
unknown	18836/udp	0.000654
unknown	18846/udp	0.000654
unknown	18851/udp	0.000654
unknown	18855/udp	0.000654
unknown	18856/udp	0.000654
unknown	18857/udp	0.000654
unknown	18862/udp	0.000654
unknown	18864/udp	0.000654
unknown	18865/udp	0.000654
unknown	18869/udp	0.001307
unknown	18872/udp	0.000654
unknown	18874/tcp	0.000076
unknown	18877/udp	0.000654
infotos	18881/tcp	0.000000
infotos	18881/udp	0.000000
unknown	18883/udp	0.001307
unknown	18884/udp	0.000654
unknown	18887/tcp	0.000076
unknown	18887/udp	0.000654
apc-necmp	18888/tcp	0.000000	# APCNECMP
apc-necmp	18888/udp	0.001307	# APCNECMP
unknown	18894/udp	0.000654
unknown	18898/udp	0.000654
unknown	18901/udp	0.000654
unknown	18903/udp	0.000654
unknown	18905/udp	0.000654
unknown	18907/udp	0.000654
unknown	18909/udp	0.000654
unknown	18910/tcp	0.000076
unknown	18915/udp	0.000654
unknown	18924/udp	0.000654
unknown	18926/udp	0.000654
unknown	18928/udp	0.000654
unknown	18929/udp	0.000654
unknown	18935/udp	0.000654
unknown	18944/udp	0.000654
unknown	18949/udp	0.000654
unknown	18954/udp	0.000654
unknown	18958/udp	0.001307
unknown	18959/udp	0.000654
unknown	18962/tcp	0.000076
unknown	18966/udp	0.000654
unknown	18968/udp	0.000654
unknown	18971/udp	0.000654
unknown	18973/udp	0.000654
unknown	18976/udp	0.000654
unknown	18980/udp	0.001961
unknown	18985/udp	0.001307
unknown	18986/udp	0.000654
unknown	18987/udp	0.001307
unknown	18988/tcp	0.000304
unknown	18991/udp	0.001307
unknown	18994/udp	0.001307
unknown	18995/udp	0.000654
unknown	18996/udp	0.001307
unknown	18997/udp	0.000654
igrid	19000/tcp	0.000000	# iGrid Server
igrid	19000/udp	0.000000	# iGrid Server
unknown	19003/udp	0.000654
scintilla	19007/tcp	0.000000	# Scintilla protocol for device services
unknown	19007/udp	0.000654
unknown	19010/tcp	0.000076
unknown	19010/udp	0.000654
unknown	19015/udp	0.000654
unknown	19017/udp	0.001961
unknown	19018/udp	0.000654
j-link	19020/tcp	0.000000	# J-Link TCP/IP Protocol
unknown	19020/udp	0.000654
unknown	19021/udp	0.000654
unknown	19022/udp	0.001307
unknown	19024/udp	0.000654
unknown	19037/udp	0.000654
unknown	19038/udp	0.000654
unknown	19039/udp	0.001961
unknown	19042/udp	0.000654
unknown	19047/udp	0.001307
unknown	19050/udp	0.000654
unknown	19056/udp	0.000654
unknown	19060/udp	0.000654
unknown	19061/udp	0.000654
unknown	19063/udp	0.000654
unknown	19065/udp	0.000654
unknown	19074/udp	0.000654
unknown	19075/udp	0.001307
unknown	19078/udp	0.000654
unknown	19083/udp	0.000654
unknown	19084/udp	0.000654
unknown	19092/udp	0.000654
unknown	19096/udp	0.001307
unknown	19097/udp	0.000654
unknown	19101/tcp	0.000380
unknown	19106/udp	0.000654
unknown	19111/udp	0.000654
unknown	19113/udp	0.000654
unknown	19117/udp	0.000654
unknown	19119/udp	0.000654
unknown	19120/udp	0.002614
unknown	19128/udp	0.000654
unknown	19130/tcp	0.000076
unknown	19130/udp	0.001961
unknown	19133/udp	0.000654
unknown	19137/udp	0.000654
unknown	19139/udp	0.000654
unknown	19140/udp	0.001307
unknown	19141/udp	0.001307
unknown	19145/udp	0.000654
unknown	19147/udp	0.000654
gkrellm	19150/tcp	0.000013	# GKrellM remote system activity meter daemon
unknown	19154/udp	0.001307
unknown	19161/udp	0.001307
unknown	19163/udp	0.000654
unknown	19165/udp	0.001961
unknown	19166/udp	0.000654
unknown	19171/udp	0.000654
unknown	19175/udp	0.000654
unknown	19181/udp	0.001307
unknown	19183/udp	0.000654
unknown	19184/udp	0.000654
unknown	19185/udp	0.000654
unknown	19190/udp	0.000654
opsec-uaa	19191/tcp	0.000000	# OPSEC UAA
opsec-uaa	19191/udp	0.000000	# OPSEC UAA
unknown	19193/udp	0.001307
ua-secureagent	19194/tcp	0.000000	# UserAuthority SecureAgent
ua-secureagent	19194/udp	0.000000	# UserAuthority SecureAgent
unknown	19195/udp	0.000654
unknown	19197/udp	0.001961
unknown	19200/tcp	0.000076
unknown	19200/udp	0.000654
unknown	19201/tcp	0.000076
unknown	19202/udp	0.000654
unknown	19207/udp	0.000654
unknown	19208/udp	0.000654
unknown	19209/udp	0.000654
unknown	19210/udp	0.000654
unknown	19219/udp	0.000654
cora	19220/tcp	0.000000	# cora-disc | Client Connection Management and Data Exchange Service | Discovery for Client Connection Management and Data Exchange Service
unknown	19220/udp	0.000654
unknown	19222/udp	0.001307
unknown	19227/udp	0.001307
unknown	19229/udp	0.000654
unknown	19233/udp	0.000654
unknown	19234/udp	0.000654
unknown	19236/udp	0.000654
unknown	19239/udp	0.000654
unknown	19246/udp	0.000654
unknown	19255/udp	0.000654
unknown	19260/udp	0.000654
unknown	19263/udp	0.000654
unknown	19269/udp	0.000654
unknown	19273/udp	0.001307
unknown	19279/udp	0.000654
unknown	19281/udp	0.000654
keysrvr	19283/tcp	0.000304	# Key Server for SASSAFRAS
keysrvr	19283/udp	0.004575	# Key Server for SASSAFRAS
unknown	19284/udp	0.000654
unknown	19289/udp	0.000654
unknown	19293/udp	0.000654
unknown	19294/udp	0.001961
unknown	19300/udp	0.000654
unknown	19310/udp	0.000654
unknown	19313/udp	0.000654
keyshadow	19315/tcp	0.000304	# Key Shadow for SASSAFRAS
keyshadow	19315/udp	0.001307	# Key Shadow for SASSAFRAS
unknown	19316/udp	0.000654
unknown	19322/udp	0.001961
unknown	19328/udp	0.000654
unknown	19331/udp	0.000654
unknown	19332/udp	0.001961
litecoin	19333/tcp	0.000076	# Litecoin crypto currency testnet - https://litecoin.info/Litecoin.conf
unknown	19333/udp	0.000654
unknown	19336/udp	0.000654
unknown	19340/udp	0.000654
unknown	19341/udp	0.000654
unknown	19350/tcp	0.000228
unknown	19350/udp	0.000654
unknown	19351/udp	0.000654
unknown	19352/udp	0.000654
unknown	19353/tcp	0.000076
unknown	19364/udp	0.000654
unknown	19367/udp	0.000654
unknown	19371/udp	0.000654
unknown	19374/udp	0.001307
unknown	19378/udp	0.000654
unknown	19383/udp	0.000654
unknown	19384/udp	0.000654
unknown	19385/udp	0.000654
unknown	19391/udp	0.000654
unknown	19394/udp	0.000654
mtrgtrans	19398/tcp	0.000000
mtrgtrans	19398/udp	0.000000
unknown	19403/tcp	0.000076
hp-sco	19410/tcp	0.000000
hp-sco	19410/udp	0.000000
hp-sca	19411/tcp	0.000000
hp-sca	19411/udp	0.000000
hp-sessmon	19412/tcp	0.000000
hp-sessmon	19412/udp	0.000000
unknown	19413/udp	0.000654
unknown	19415/udp	0.001307
unknown	19416/udp	0.000654
unknown	19424/udp	0.000654
unknown	19425/udp	0.000654
unknown	19427/udp	0.000654
unknown	19429/udp	0.000654
unknown	19433/udp	0.000654
unknown	19434/udp	0.000654
unknown	19440/udp	0.000654
unknown	19442/udp	0.000654
unknown	19446/udp	0.000654
unknown	19447/udp	0.000654
unknown	19451/udp	0.000654
unknown	19459/udp	0.000654
unknown	19462/udp	0.000654
unknown	19464/tcp	0.000076
unknown	19464/udp	0.000654
unknown	19479/udp	0.000654
unknown	19482/udp	0.001307
unknown	19489/udp	0.001961
unknown	19499/udp	0.000654
unknown	19500/udp	0.001307
unknown	19501/tcp	0.000076
unknown	19501/udp	0.000654
unknown	19503/udp	0.002614
unknown	19504/udp	0.001307
unknown	19505/udp	0.000654
unknown	19506/udp	0.000654
unknown	19508/udp	0.000654
unknown	19514/udp	0.000654
unknown	19522/udp	0.000654
unknown	19524/udp	0.000654
unknown	19529/udp	0.000654
unknown	19530/udp	0.000654
fxuptp	19539/tcp	0.000000
fxuptp	19539/udp	0.000654
sxuptp	19540/tcp	0.000000
sxuptp	19540/udp	0.000000
jcp	19541/tcp	0.000000	# JCP Client
jcp	19541/udp	0.001307	# JCP Client
unknown	19542/udp	0.000654
unknown	19544/udp	0.000654
unknown	19545/udp	0.000654
unknown	19561/udp	0.000654
unknown	19578/udp	0.000654
unknown	19582/udp	0.000654
unknown	19584/udp	0.000654
unknown	19587/udp	0.000654
unknown	19591/udp	0.000654
unknown	19595/udp	0.000654
unknown	19600/udp	0.001961
unknown	19605/udp	0.001307
unknown	19607/udp	0.000654
unknown	19610/udp	0.000654
unknown	19612/tcp	0.000076
unknown	19613/udp	0.000654
unknown	19614/udp	0.000654
unknown	19616/udp	0.002614
unknown	19617/udp	0.000654
unknown	19618/udp	0.000654
unknown	19624/udp	0.001307
unknown	19625/udp	0.001307
unknown	19627/udp	0.000654
unknown	19629/udp	0.000654
unknown	19632/udp	0.001307
unknown	19634/tcp	0.000076
unknown	19637/udp	0.000654
unknown	19639/udp	0.001307
unknown	19641/udp	0.000654
unknown	19642/udp	0.000654
unknown	19644/udp	0.000654
unknown	19647/udp	0.001307
unknown	19648/udp	0.000654
unknown	19650/udp	0.001307
unknown	19652/udp	0.000654
unknown	19658/udp	0.000654
unknown	19659/udp	0.000654
unknown	19660/udp	0.001307
unknown	19662/udp	0.001307
unknown	19663/udp	0.001307
unknown	19664/udp	0.000654
unknown	19667/udp	0.000654
unknown	19672/udp	0.000654
unknown	19678/udp	0.000654
unknown	19682/udp	0.003922
unknown	19683/udp	0.001307
unknown	19685/udp	0.000654
unknown	19687/udp	0.001961
unknown	19688/udp	0.000654
unknown	19695/udp	0.001307
unknown	19701/udp	0.000654
unknown	19704/udp	0.000654
unknown	19707/udp	0.001307
unknown	19711/udp	0.000654
unknown	19715/tcp	0.000076
unknown	19717/udp	0.001307
unknown	19718/udp	0.001307
unknown	19719/udp	0.001307
unknown	19722/udp	0.001307
unknown	19724/udp	0.000654
unknown	19728/udp	0.001307
unknown	19730/udp	0.000654
unknown	19734/udp	0.000654
unknown	19736/udp	0.000654
unknown	19739/udp	0.000654
unknown	19747/udp	0.000654
unknown	19753/udp	0.000654
unknown	19754/udp	0.000654
unknown	19756/udp	0.000654
unknown	19757/udp	0.000654
unknown	19761/udp	0.000654
unknown	19764/udp	0.000654
unknown	19773/udp	0.000654
unknown	19780/tcp	0.000304
unknown	19780/udp	0.000654
unknown	19781/udp	0.000654
unknown	19783/udp	0.000654
mle	19788/tcp	0.000000	# Mesh Link Establishment
unknown	19789/udp	0.001307
faircom-db	19790/tcp	0.000000	# FairCom Database
unknown	19790/udp	0.000654
unknown	19791/udp	0.000654
unknown	19792/udp	0.001307
unknown	19797/udp	0.000654
unknown	19799/udp	0.000654
unknown	19801/tcp	0.000380
unknown	19808/udp	0.000654
unknown	19816/udp	0.000654
unknown	19817/udp	0.000654
unknown	19819/udp	0.000654
unknown	19823/udp	0.000654
unknown	19827/udp	0.000654
unknown	19829/udp	0.000654
unknown	19836/udp	0.000654
unknown	19837/udp	0.000654
unknown	19842/tcp	0.000380
unknown	19850/udp	0.000654
unknown	19851/udp	0.000654
unknown	19852/tcp	0.000076
unknown	19852/udp	0.000654
unknown	19856/udp	0.000654
unknown	19859/udp	0.000654
unknown	19860/udp	0.000654
unknown	19868/udp	0.000654
unknown	19869/udp	0.000654
unknown	19870/udp	0.000654
unknown	19873/udp	0.000654
unknown	19875/udp	0.000654
unknown	19880/udp	0.000654
unknown	19882/udp	0.000654
unknown	19887/udp	0.000654
unknown	19892/udp	0.000654
unknown	19897/udp	0.000654
unknown	19900/tcp	0.000152
unknown	19903/udp	0.000654
unknown	19906/udp	0.000654
unknown	19911/udp	0.000654
unknown	19912/udp	0.000654
unknown	19917/udp	0.000654
unknown	19921/udp	0.000654
unknown	19926/udp	0.000654
unknown	19933/udp	0.001961
unknown	19935/udp	0.001307
unknown	19936/udp	0.001307
unknown	19940/udp	0.000654
unknown	19954/udp	0.000654
unknown	19956/udp	0.001307
unknown	19959/udp	0.000654
unknown	19966/udp	0.000654
unknown	19967/udp	0.000654
unknown	19968/udp	0.000654
unknown	19977/udp	0.000654
unknown	19984/udp	0.000654
unknown	19988/udp	0.000654
unknown	19989/udp	0.000654
unknown	19995/tcp	0.000076
unknown	19995/udp	0.001307
unknown	19996/tcp	0.000076
unknown	19997/udp	0.000654
iec-104-sec	19998/tcp	0.000000	# IEC 60870-5-104 process control - secure
unknown	19998/udp	0.001307
dnp-sec	19999/tcp	0.000000	# Distributed Network Protocol - Secure | Distributed Network Protocol - secured
dnp-sec	19999/udp	0.000000	# Distributed Network Protocol - Secure
dnp	20000/tcp	0.000380	# Distributed Network Protocol
dnp	20000/udp	0.000000
microsan	20001/tcp	0.000076
microsan	20001/udp	0.000000
commtact-http	20002/tcp	0.000152	# Commtact HTTP
commtact-http	20002/udp	0.000000	# Commtact HTTP
commtact-https	20003/tcp	0.000000	# Commtact HTTPS
commtact-https	20003/udp	0.001307	# Commtact HTTPS
unknown	20004/udp	0.001961
btx	20005/tcp	0.000401	# openwebnet | xcept4 (Interacts with German Telekom's CEPT videotext service) | OpenWebNet protocol for electric network
openwebnet	20005/udp	0.000654	# OpenWebNet protocol for electric network
unknown	20006/udp	0.000654
unknown	20008/udp	0.000654
unknown	20011/tcp	0.000076
ss-idi-disc	20012/tcp	0.000000	# Samsung Interdevice Interaction discovery
ss-idi-disc	20012/udp	0.000000	# Samsung Interdevice Interaction discovery
ss-idi	20013/tcp	0.000000	# Samsung Interdevice Interaction
opendeploy	20014/tcp	0.000000	# OpenDeploy Listener
opendeploy	20014/udp	0.000000	# OpenDeploy Listener
unknown	20015/udp	0.000654
unknown	20017/tcp	0.000076
unknown	20019/udp	0.002614
unknown	20021/tcp	0.000076
unknown	20022/udp	0.000654
unknown	20024/udp	0.000654
unknown	20027/udp	0.000654
unknown	20031/tcp	0.000380
bakbonenetvault	20031/udp	0.025490	# BakBone NetVault primary communications port
unknown	20032/tcp	0.000076
nburn_id	20034/tcp	0.000000	# nburn-id | NetBurner ID Port
nburn_id	20034/udp	0.000654	# NetBurner ID Port
unknown	20039/tcp	0.000076
unknown	20039/udp	0.000654
unknown	20041/udp	0.000654
unknown	20045/udp	0.000654
tmophl7mts	20046/tcp	0.000000	# TMOP HL7 Message Transfer Service
tmophl7mts	20046/udp	0.000000	# TMOP HL7 Message Transfer Service
mountd	20048/tcp	0.000000	# NFS mount protocol
mountd	20048/udp	0.000654	# NFS mount protocol
nfsrdma	20049/sctp	0.000000	# Network File System (NFS) over RDMA
nfsrdma	20049/tcp	0.000000	# Network File System (NFS) over RDMA
nfsrdma	20049/udp	0.000000	# Network File System (NFS) over RDMA
unknown	20052/tcp	0.000076
unknown	20055/udp	0.000654
unknown	20056/udp	0.000654
avesterra	20057/tcp	0.000000	# AvesTerra Hypergraph Transfer Protocol (HGTP)
unknown	20062/udp	0.000654
unknown	20065/udp	0.000654
unknown	20069/udp	0.000654
unknown	20071/udp	0.000654
unknown	20076/tcp	0.000076
unknown	20076/udp	0.000654
unknown	20079/udp	0.000654
unknown	20080/tcp	0.000076
unknown	20081/udp	0.000654
unknown	20082/udp	0.001307
unknown	20083/udp	0.000654
unknown	20085/tcp	0.000076
unknown	20085/udp	0.000654
unknown	20089/tcp	0.000076
unknown	20089/udp	0.000654
unknown	20091/udp	0.000654
unknown	20095/udp	0.000654
unknown	20099/udp	0.000654
unknown	20102/tcp	0.000076
unknown	20103/udp	0.000654
unknown	20104/udp	0.000654
unknown	20106/tcp	0.000076
unknown	20107/udp	0.000654
unknown	20110/udp	0.000654
unknown	20111/tcp	0.000076
unknown	20117/udp	0.001307
unknown	20118/tcp	0.000076
unknown	20120/udp	0.001307
unknown	20125/tcp	0.000076
unknown	20125/udp	0.000654
unknown	20126/udp	0.002614
unknown	20127/tcp	0.000076
unknown	20129/udp	0.001307
unknown	20132/udp	0.000654
unknown	20133/udp	0.000654
unknown	20146/udp	0.001307
unknown	20147/tcp	0.000076
unknown	20150/udp	0.000654
unknown	20154/udp	0.001307
unknown	20156/udp	0.000654
unknown	20158/udp	0.000654
unknown	20160/udp	0.000654
unknown	20161/udp	0.000654
unknown	20162/udp	0.000654
unknown	20164/udp	0.001307
unknown	20165/udp	0.000654
tolfab	20167/tcp	0.000000	# TOLfab Data Change
tolfab	20167/udp	0.000000	# TOLfab Data Change
unknown	20169/udp	0.000654
unknown	20171/udp	0.000654
unknown	20173/udp	0.000654
unknown	20175/udp	0.000654
unknown	20176/udp	0.000654
unknown	20179/tcp	0.000076
unknown	20180/tcp	0.000076
unknown	20181/udp	0.000654
unknown	20184/udp	0.000654
unknown	20190/udp	0.000654
unknown	20194/udp	0.000654
unknown	20197/udp	0.000654
ipdtp-port	20202/tcp	0.000000	# IPD Tunneling Port
ipdtp-port	20202/udp	0.000000	# IPD Tunneling Port
unknown	20204/udp	0.000654
unknown	20206/udp	0.001307
unknown	20217/udp	0.001307
unknown	20221/tcp	0.000380
unknown	20221/udp	0.000654
ipulse-ics	20222/tcp	0.000380
ipulse-ics	20222/udp	0.000654
unknown	20223/tcp	0.000076
unknown	20223/udp	0.000654
unknown	20224/tcp	0.000076
unknown	20224/udp	0.000654
unknown	20225/tcp	0.000076
unknown	20226/tcp	0.000076
unknown	20226/udp	0.000654
unknown	20227/tcp	0.000076
unknown	20228/tcp	0.000076
unknown	20228/udp	0.000654
unknown	20229/udp	0.000654
unknown	20239/udp	0.000654
unknown	20243/udp	0.000654
unknown	20244/udp	0.000654
unknown	20249/udp	0.001307
unknown	20253/udp	0.000654
unknown	20254/udp	0.000654
unknown	20258/udp	0.000654
unknown	20260/udp	0.000654
unknown	20262/udp	0.001307
unknown	20276/udp	0.000654
unknown	20279/udp	0.001307
unknown	20280/tcp	0.000076
unknown	20280/udp	0.000654
unknown	20281/udp	0.000654
unknown	20284/udp	0.000654
unknown	20287/udp	0.000654
unknown	20288/udp	0.001307
unknown	20292/udp	0.000654
unknown	20297/udp	0.000654
unknown	20300/udp	0.000654
unknown	20306/udp	0.000654
unknown	20309/udp	0.001307
unknown	20313/udp	0.001307
unknown	20316/udp	0.000654
unknown	20326/udp	0.001307
unknown	20339/udp	0.000654
unknown	20340/udp	0.000654
unknown	20353/udp	0.000654
unknown	20355/udp	0.000654
unknown	20357/udp	0.000654
unknown	20358/udp	0.000654
unknown	20359/udp	0.001961
unknown	20360/udp	0.001307
unknown	20364/udp	0.000654
unknown	20366/udp	0.001307
unknown	20369/udp	0.000654
unknown	20370/udp	0.000654
unknown	20380/udp	0.001307
unknown	20381/udp	0.000654
unknown	20389/udp	0.002614
unknown	20392/udp	0.000654
unknown	20396/udp	0.000654
unknown	20409/udp	0.001307
unknown	20411/udp	0.001307
unknown	20423/udp	0.001307
unknown	20424/udp	0.001307
unknown	20425/udp	0.001307
unknown	20426/udp	0.000654
unknown	20432/udp	0.000654
unknown	20437/udp	0.000654
unknown	20439/udp	0.000654
unknown	20443/udp	0.000654
unknown	20444/udp	0.000654
unknown	20445/udp	0.001307
unknown	20449/udp	0.001307
unknown	20450/udp	0.000654
unknown	20452/udp	0.000654
unknown	20453/udp	0.000654
unknown	20464/udp	0.001307
unknown	20465/udp	0.001307
unknown	20469/udp	0.000654
unknown	20470/udp	0.000654
unknown	20473/tcp	0.000076
unknown	20473/udp	0.000654
unknown	20475/udp	0.000654
emwavemsg	20480/tcp	0.000000	# emWave Message Service
emwavemsg	20480/udp	0.000000	# emWave Message Service
unknown	20481/udp	0.000654
unknown	20483/udp	0.000654
unknown	20485/udp	0.000654
unknown	20487/udp	0.000654
unknown	20488/udp	0.000654
unknown	20489/udp	0.000654
unknown	20497/udp	0.000654
unknown	20500/udp	0.000654
unknown	20506/udp	0.000654
unknown	20513/udp	0.000654
unknown	20516/udp	0.000654
unknown	20517/udp	0.000654
unknown	20518/udp	0.001307
unknown	20522/udp	0.001307
unknown	20525/udp	0.001307
unknown	20526/udp	0.000654
unknown	20527/udp	0.000654
unknown	20530/udp	0.000654
unknown	20533/udp	0.000654
unknown	20537/udp	0.000654
unknown	20540/udp	0.001307
unknown	20541/udp	0.000654
unknown	20543/udp	0.000654
unknown	20544/udp	0.000654
unknown	20545/udp	0.000654
unknown	20548/udp	0.000654
unknown	20551/udp	0.000654
unknown	20555/udp	0.000654
unknown	20560/udp	0.001307
unknown	20561/udp	0.000654
unknown	20563/udp	0.000654
unknown	20564/udp	0.000654
unknown	20569/udp	0.000654
unknown	20584/udp	0.000654
unknown	20585/udp	0.000654
unknown	20590/udp	0.000654
unknown	20591/udp	0.000654
unknown	20608/udp	0.000654
unknown	20611/udp	0.000654
unknown	20619/udp	0.000654
unknown	20621/udp	0.000654
unknown	20625/udp	0.000654
unknown	20626/udp	0.000654
unknown	20635/udp	0.000654
unknown	20641/udp	0.000654
unknown	20646/udp	0.000654
unknown	20660/udp	0.000654
unknown	20665/udp	0.001307
track	20670/tcp	0.000000
track	20670/udp	0.000000
unknown	20671/udp	0.000654
unknown	20673/udp	0.000654
unknown	20675/udp	0.000654
unknown	20677/udp	0.000654
unknown	20678/udp	0.001307
unknown	20679/udp	0.001307
unknown	20680/udp	0.000654
unknown	20681/udp	0.000654
unknown	20687/udp	0.000654
unknown	20688/udp	0.000654
unknown	20689/udp	0.000654
unknown	20691/udp	0.000654
unknown	20696/udp	0.000654
unknown	20700/udp	0.000654
unknown	20702/udp	0.000654
unknown	20710/udp	0.001307
unknown	20712/udp	0.000654
unknown	20713/udp	0.000654
unknown	20717/udp	0.001307
unknown	20719/udp	0.000654
unknown	20723/udp	0.000654
unknown	20725/udp	0.000654
unknown	20733/udp	0.000654
unknown	20734/tcp	0.000076
unknown	20734/udp	0.000654
unknown	20736/udp	0.000654
unknown	20739/udp	0.000654
unknown	20741/udp	0.000654
unknown	20742/udp	0.001307
unknown	20743/udp	0.000654
unknown	20747/udp	0.000654
unknown	20748/udp	0.000654
unknown	20749/udp	0.000654
unknown	20752/udp	0.001307
unknown	20758/udp	0.000654
unknown	20759/udp	0.000654
unknown	20762/udp	0.001307
unknown	20765/udp	0.000654
unknown	20771/udp	0.000654
unknown	20780/udp	0.000654
unknown	20785/udp	0.000654
unknown	20791/udp	0.001307
unknown	20795/udp	0.000654
unknown	20796/udp	0.000654
unknown	20805/udp	0.000654
crtech-nlm	20810/tcp	0.000000	# CRTech NLM
unknown	20812/udp	0.000654
unknown	20815/udp	0.000654
unknown	20816/udp	0.000654
unknown	20817/udp	0.001307
unknown	20819/udp	0.000654
unknown	20822/udp	0.000654
unknown	20825/udp	0.000654
unknown	20826/udp	0.000654
unknown	20828/tcp	0.000760
unknown	20830/udp	0.000654
unknown	20831/udp	0.000654
unknown	20833/udp	0.000654
unknown	20842/udp	0.001307
unknown	20848/udp	0.001307
unknown	20851/udp	0.001307
unknown	20852/udp	0.000654
unknown	20858/udp	0.000654
unknown	20861/udp	0.000654
unknown	20863/udp	0.000654
unknown	20865/udp	0.001307
unknown	20868/udp	0.000654
unknown	20872/udp	0.001307
unknown	20876/udp	0.001307
unknown	20878/udp	0.000654
unknown	20880/udp	0.000654
unknown	20881/udp	0.000654
unknown	20882/udp	0.000654
unknown	20883/tcp	0.000076
unknown	20884/udp	0.001307
unknown	20892/udp	0.000654
unknown	20896/udp	0.000654
unknown	20897/udp	0.000654
unknown	20905/udp	0.000654
unknown	20908/udp	0.000654
unknown	20913/udp	0.000654
unknown	20915/udp	0.000654
unknown	20919/udp	0.001307
unknown	20921/udp	0.000654
unknown	20924/udp	0.000654
unknown	20926/udp	0.000654
unknown	20927/udp	0.000654
unknown	20932/udp	0.000654
unknown	20934/tcp	0.000076
unknown	20940/tcp	0.000076
unknown	20940/udp	0.000654
unknown	20942/udp	0.000654
unknown	20959/udp	0.000654
unknown	20966/udp	0.000654
unknown	20970/udp	0.000654
unknown	20974/udp	0.000654
unknown	20983/udp	0.000654
unknown	20987/udp	0.000654
unknown	20989/udp	0.000654
unknown	20990/tcp	0.000076
unknown	20990/udp	0.000654
unknown	20994/udp	0.000654
athand-mmp	20999/tcp	0.000000	# At Hand MMP | AT Hand MMP
athand-mmp	20999/udp	0.000000	# AT Hand MMP
irtrans	21000/tcp	0.000000	# IRTrans Control
irtrans	21000/udp	0.001307	# IRTrans Control
unknown	21007/udp	0.000654
notezilla-lan	21010/tcp	0.000000	# Notezilla.Lan Server
unknown	21011/tcp	0.000076
unknown	21016/udp	0.001307
unknown	21019/udp	0.000654
unknown	21030/udp	0.000654
unknown	21060/udp	0.001307
unknown	21062/udp	0.000654
unknown	21071/udp	0.000654
unknown	21077/udp	0.000654
unknown	21078/tcp	0.000076
unknown	21083/udp	0.001307
unknown	21084/udp	0.000654
unknown	21103/udp	0.000654
unknown	21104/udp	0.001307
unknown	21105/udp	0.000654
unknown	21111/udp	0.001307
unknown	21117/udp	0.000654
unknown	21121/udp	0.000654
unknown	21123/udp	0.000654
unknown	21124/udp	0.000654
unknown	21128/udp	0.000654
unknown	21131/udp	0.001961
unknown	21152/udp	0.000654
unknown	21157/udp	0.000654
unknown	21159/udp	0.000654
unknown	21166/udp	0.000654
unknown	21167/udp	0.001307
unknown	21168/udp	0.000654
unknown	21170/udp	0.000654
unknown	21180/udp	0.000654
unknown	21185/udp	0.000654
unknown	21186/udp	0.001307
unknown	21187/udp	0.000654
unknown	21188/udp	0.000654
unknown	21192/udp	0.000654
unknown	21193/udp	0.000654
unknown	21194/udp	0.000654
unknown	21195/udp	0.000654
memcachedb	21201/tcp	0.000076
unknown	21201/udp	0.000654
unknown	21202/udp	0.000654
unknown	21204/udp	0.000654
unknown	21206/udp	0.001307
unknown	21207/udp	0.001307
unknown	21209/udp	0.000654
trinket-agent	21212/tcp	0.000000	# Distributed artificial intelligence
unknown	21212/udp	0.001961
cohesity-agent	21213/tcp	0.000000	# Cohesity backup agents
unknown	21214/udp	0.000654
unknown	21215/udp	0.000654
aigairserver	21221/tcp	0.000000	# Services for Air Server
unknown	21225/udp	0.000654
unknown	21231/udp	0.000654
unknown	21233/udp	0.000654
unknown	21235/udp	0.000654
unknown	21239/udp	0.000654
unknown	21241/udp	0.000654
unknown	21244/udp	0.000654
unknown	21247/udp	0.001307
unknown	21253/udp	0.000654
unknown	21261/udp	0.001961
unknown	21270/udp	0.000654
unknown	21280/udp	0.000654
unknown	21282/udp	0.001307
unknown	21284/udp	0.000654
unknown	21292/udp	0.000654
unknown	21297/udp	0.000654
unknown	21298/udp	0.001961
unknown	21299/udp	0.000654
unknown	21303/udp	0.001307
unknown	21304/udp	0.000654
unknown	21310/udp	0.000654
unknown	21312/udp	0.000654
unknown	21313/udp	0.000654
unknown	21318/udp	0.001307
unknown	21320/udp	0.001307
unknown	21331/udp	0.000654
unknown	21333/udp	0.001307
unknown	21334/udp	0.000654
unknown	21337/udp	0.000654
unknown	21344/udp	0.001307
unknown	21347/udp	0.000654
unknown	21350/udp	0.000654
unknown	21354/udp	0.001961
unknown	21358/udp	0.001307
unknown	21360/udp	0.001307
unknown	21364/udp	0.001307
unknown	21366/udp	0.001307
unknown	21368/udp	0.000654
unknown	21372/udp	0.000654
unknown	21375/udp	0.000654
unknown	21376/udp	0.000654
unknown	21377/udp	0.000654
unknown	21383/udp	0.002614
unknown	21385/udp	0.000654
unknown	21387/udp	0.000654
unknown	21393/udp	0.000654
unknown	21395/udp	0.000654
unknown	21397/udp	0.000654
unknown	21399/udp	0.000654
unknown	21405/udp	0.001307
unknown	21407/udp	0.000654
unknown	21434/udp	0.000654
unknown	21440/udp	0.000654
unknown	21446/udp	0.000654
unknown	21452/udp	0.000654
unknown	21454/udp	0.001307
unknown	21456/udp	0.000654
unknown	21461/udp	0.000654
unknown	21468/udp	0.001307
unknown	21469/udp	0.000654
unknown	21471/udp	0.000654
unknown	21472/udp	0.000654
unknown	21473/tcp	0.000076
unknown	21473/udp	0.000654
unknown	21476/udp	0.001307
unknown	21478/udp	0.000654
unknown	21483/udp	0.000654
unknown	21498/udp	0.000654
unknown	21501/udp	0.000654
unknown	21506/udp	0.000654
unknown	21507/udp	0.000654
unknown	21511/udp	0.000654
unknown	21514/udp	0.001307
unknown	21521/udp	0.000654
unknown	21524/udp	0.001307
unknown	21525/udp	0.001307
unknown	21547/udp	0.000654
unknown	21550/udp	0.000654
rdm-tfs	21553/tcp	0.000000	# Raima RDM TFS
unknown	21553/udp	0.000654
dfserver	21554/tcp	0.000000	# MineScape Design File Server
dfserver	21554/udp	0.000000	# MineScape Design File Server
unknown	21556/udp	0.001307
unknown	21564/udp	0.000654
unknown	21566/udp	0.001307
unknown	21567/udp	0.000654
unknown	21568/udp	0.001307
unknown	21571/tcp	0.000380
unknown	21572/udp	0.000654
unknown	21576/udp	0.001307
unknown	21588/udp	0.000654
vofr-gateway	21590/tcp	0.000000	# VoFR Gateway
vofr-gateway	21590/udp	0.000000	# VoFR Gateway
unknown	21599/udp	0.000654
unknown	21609/udp	0.001307
unknown	21611/udp	0.000654
unknown	21616/udp	0.000654
unknown	21620/udp	0.000654
unknown	21621/udp	0.001961
unknown	21624/udp	0.000654
unknown	21625/udp	0.001307
unknown	21629/udp	0.000654
unknown	21631/tcp	0.000076
unknown	21634/tcp	0.000076
unknown	21640/udp	0.000654
unknown	21644/udp	0.001307
unknown	21647/udp	0.000654
unknown	21649/udp	0.001307
unknown	21654/udp	0.000654
unknown	21655/udp	0.001307
unknown	21662/udp	0.000654
unknown	21663/udp	0.001307
unknown	21665/udp	0.000654
unknown	21666/udp	0.000654
unknown	21667/udp	0.000654
unknown	21669/udp	0.000654
unknown	21671/udp	0.000654
unknown	21674/udp	0.001307
unknown	21679/udp	0.000654
unknown	21680/udp	0.000654
unknown	21682/udp	0.000654
unknown	21684/udp	0.000654
unknown	21685/udp	0.000654
unknown	21686/udp	0.000654
unknown	21689/udp	0.000654
unknown	21698/udp	0.001307
unknown	21702/udp	0.001307
unknown	21703/udp	0.000654
unknown	21706/udp	0.000654
unknown	21708/udp	0.000654
unknown	21710/udp	0.001307
unknown	21716/udp	0.000654
unknown	21726/udp	0.000654
unknown	21728/tcp	0.000076
unknown	21738/udp	0.000654
unknown	21742/udp	0.001307
unknown	21752/udp	0.000654
unknown	21756/udp	0.000654
unknown	21759/udp	0.000654
unknown	21765/udp	0.000654
unknown	21768/udp	0.000654
unknown	21771/udp	0.000654
unknown	21775/udp	0.000654
unknown	21780/udp	0.001307
unknown	21784/udp	0.001307
unknown	21785/udp	0.000654
unknown	21786/udp	0.000654
unknown	21792/tcp	0.000152
unknown	21794/udp	0.000654
tvpm	21800/tcp	0.000000	# TVNC Pro Multiplexing
tvpm	21800/udp	0.001307	# TVNC Pro Multiplexing
sal	21801/tcp	0.000000	# Safe AutoLogon
unknown	21803/udp	0.001961
unknown	21804/udp	0.000654
unknown	21805/udp	0.000654
unknown	21806/udp	0.000654
unknown	21814/udp	0.000654
unknown	21819/udp	0.000654
unknown	21825/udp	0.000654
unknown	21830/udp	0.000654
unknown	21834/udp	0.001307
unknown	21835/udp	0.000654
unknown	21842/udp	0.001307
webphone	21845/tcp	0.000000
webphone	21845/udp	0.000000
netspeak-is	21846/tcp	0.000000	# NetSpeak Corp. Directory Services
netspeak-is	21846/udp	0.000000	# NetSpeak Corp. Directory Services
netspeak-cs	21847/tcp	0.000000	# NetSpeak Corp. Connection Services
netspeak-cs	21847/udp	0.001307	# NetSpeak Corp. Connection Services
netspeak-acd	21848/tcp	0.000000	# NetSpeak Corp. Automatic Call Distribution
netspeak-acd	21848/udp	0.000000	# NetSpeak Corp. Automatic Call Distribution
netspeak-cps	21849/tcp	0.000000	# NetSpeak Corp. Credit Processing System
netspeak-cps	21849/udp	0.000000	# NetSpeak Corp. Credit Processing System
unknown	21851/udp	0.000654
unknown	21852/udp	0.000654
unknown	21854/udp	0.000654
unknown	21858/udp	0.000654
unknown	21865/udp	0.000654
unknown	21868/udp	0.001307
unknown	21880/udp	0.000654
unknown	21881/udp	0.000654
unknown	21885/udp	0.000654
unknown	21888/udp	0.000654
unknown	21891/tcp	0.000076
unknown	21892/udp	0.000654
unknown	21895/udp	0.000654
unknown	21898/udp	0.001307
unknown	21899/udp	0.000654
unknown	21900/udp	0.000654
unknown	21902/udp	0.001961
unknown	21908/udp	0.000654
unknown	21915/tcp	0.000076
unknown	21919/udp	0.000654
unknown	21920/udp	0.000654
unknown	21923/udp	0.001307
unknown	21927/udp	0.000654
unknown	21930/udp	0.000654
unknown	21934/udp	0.000654
unknown	21935/udp	0.000654
unknown	21936/udp	0.000654
unknown	21939/udp	0.000654
unknown	21940/udp	0.000654
unknown	21941/udp	0.000654
unknown	21946/udp	0.000654
unknown	21948/udp	0.001307
unknown	21964/udp	0.000654
unknown	21967/udp	0.001307
unknown	21968/udp	0.000654
unknown	21974/udp	0.000654
unknown	21978/udp	0.000654
unknown	21982/udp	0.000654
unknown	21994/udp	0.000654
unknown	21995/udp	0.000654
unknown	21996/udp	0.000654
unknown	21999/udp	0.000654
snapenetio	22000/tcp	0.000000
snapenetio	22000/udp	0.000000
optocontrol	22001/tcp	0.000000
optocontrol	22001/udp	0.000000
optohost002	22002/tcp	0.000000	# Opto Host Port 2
optohost002	22002/udp	0.000000	# Opto Host Port 2
optohost003	22003/tcp	0.000000	# Opto Host Port 3
optohost003	22003/udp	0.000000	# Opto Host Port 3
optohost004	22004/tcp	0.000000	# Opto Host Port 4
optohost004	22004/udp	0.000000	# Opto Host Port 4
optohost004	22005/tcp	0.000000	# Opto Host Port 5
optohost004	22005/udp	0.000000	# Opto Host Port 5
unknown	22006/udp	0.000654
unknown	22007/udp	0.000654
unknown	22011/udp	0.000654
unknown	22014/udp	0.000654
unknown	22016/udp	0.000654
unknown	22017/udp	0.000654
unknown	22019/udp	0.000654
unknown	22022/tcp	0.000076
unknown	22027/udp	0.000654
unknown	22029/udp	0.001307
unknown	22031/udp	0.000654
unknown	22032/udp	0.000654
unknown	22035/udp	0.000654
unknown	22041/udp	0.000654
unknown	22042/udp	0.000654
unknown	22043/udp	0.001307
unknown	22045/udp	0.001307
unknown	22053/udp	0.001307
unknown	22055/udp	0.001961
unknown	22062/udp	0.000654
unknown	22063/tcp	0.000076
unknown	22063/udp	0.000654
unknown	22068/udp	0.000654
unknown	22069/udp	0.000654
unknown	22072/udp	0.000654
unknown	22079/udp	0.000654
unknown	22084/udp	0.000654
unknown	22090/udp	0.000654
unknown	22092/udp	0.000654
unknown	22094/udp	0.000654
unknown	22098/udp	0.000654
unknown	22099/udp	0.000654
unknown	22100/tcp	0.000076
unknown	22102/udp	0.000654
unknown	22104/udp	0.000654
unknown	22105/udp	0.001307
unknown	22109/udp	0.001307
unknown	22111/udp	0.000654
unknown	22112/udp	0.000654
unknown	22115/udp	0.000654
unknown	22123/udp	0.001307
unknown	22124/udp	0.001307
dcap	22125/tcp	0.000076	# dCache Access Protocol
gsidcap	22128/tcp	0.000076	# GSI dCache Access Protocol
unknown	22130/udp	0.000654
unknown	22131/udp	0.000654
unknown	22146/udp	0.001307
unknown	22147/udp	0.000654
unknown	22148/udp	0.000654
unknown	22159/udp	0.000654
unknown	22163/udp	0.000654
unknown	22169/udp	0.000654
unknown	22171/udp	0.000654
unknown	22172/udp	0.000654
unknown	22174/udp	0.000654
unknown	22176/udp	0.000654
unknown	22177/tcp	0.000076
unknown	22178/udp	0.000654
unknown	22190/udp	0.000654
unknown	22200/tcp	0.000076
unknown	22203/udp	0.000654
unknown	22215/udp	0.001307
unknown	22218/udp	0.000654
unknown	22221/udp	0.000654
easyengine	22222/tcp	0.000152	# EasyEngine is CLI tool to manage WordPress Sites on Nginx server
unknown	22223/tcp	0.000076
unknown	22227/udp	0.000654
unknown	22230/udp	0.000654
unknown	22232/udp	0.000654
unknown	22233/udp	0.000654
unknown	22239/udp	0.000654
unknown	22242/udp	0.000654
unknown	22248/udp	0.000654
unknown	22249/udp	0.000654
unknown	22252/udp	0.001307
unknown	22256/udp	0.000654
unknown	22260/udp	0.000654
unknown	22261/udp	0.000654
unknown	22266/udp	0.000654
unknown	22267/udp	0.000654
unknown	22268/udp	0.000654
wnn6	22273/tcp	0.000075	# Wnn6 (Japanese input)
wnn6	22273/udp	0.000000
unknown	22275/udp	0.000654
unknown	22277/udp	0.000654
unknown	22278/udp	0.000654
unknown	22279/udp	0.000654
unknown	22287/udp	0.000654
unknown	22288/udp	0.001307
wnn6_Cn	22289/tcp	0.000000	# Wnn6 (Chinese input)
unknown	22290/tcp	0.000076
unknown	22290/udp	0.000654
unknown	22291/udp	0.000654
unknown	22292/udp	0.001307
unknown	22293/udp	0.000654
unknown	22294/udp	0.000654
unknown	22296/udp	0.000654
unknown	22297/udp	0.000654
unknown	22300/udp	0.000654
unknown	22304/udp	0.000654
wnn6_Kr	22305/tcp	0.000000	# cis | Wnn6 (Korean input) | CompactIS Tunnel
cis	22305/udp	0.000000	# CompactIS Tunnel
unknown	22316/udp	0.000654
unknown	22318/udp	0.000654
wnn6_Tw	22321/tcp	0.000000	# Wnn6 (Taiwanse input)
unknown	22324/udp	0.001307
showcockpit-net	22333/tcp	0.000000	# ShowCockpit Networking
unknown	22333/udp	0.000654
shrewd-control	22335/tcp	0.000000	# shrewd-stream | Initium Labs Security and Automation Control | Initium Labs Security and Automation Streaming
unknown	22339/udp	0.000654
unknown	22340/udp	0.000654
unknown	22341/tcp	0.000076
unknown	22341/udp	0.001961
cis-secure	22343/tcp	0.000000	# CompactIS Secure Tunnel
cis-secure	22343/udp	0.000000	# CompactIS Secure Tunnel
unknown	22344/udp	0.000654
WibuKey	22347/tcp	0.000000	# WibuKey Standard WkLan
WibuKey	22347/udp	0.000654	# WibuKey Standard WkLan
CodeMeter	22350/tcp	0.000076	# CodeMeter Standard
CodeMeter	22350/udp	0.000654	# CodeMeter Standard
codemeter-cmwan	22351/tcp	0.000000	# TPC/IP requests of copy protection software to a server
unknown	22356/udp	0.001307
unknown	22360/udp	0.000654
unknown	22362/udp	0.000654
unknown	22366/udp	0.000654
unknown	22368/udp	0.000654
hpnpd	22370/tcp	0.000000	# Hewlett-Packard Network Printer daemon
hpnpd	22370/udp	0.000726	# Hewlett-Packard Network Printer daemon
unknown	22371/udp	0.000654
unknown	22373/udp	0.000654
unknown	22374/udp	0.000654
unknown	22375/udp	0.000654
unknown	22376/udp	0.001307
unknown	22377/udp	0.001307
unknown	22380/udp	0.000654
unknown	22381/udp	0.001307
unknown	22382/udp	0.000654
unknown	22386/udp	0.000654
unknown	22388/udp	0.000654
unknown	22406/udp	0.000654
unknown	22408/udp	0.000654
unknown	22412/udp	0.000654
unknown	22413/udp	0.000654
unknown	22415/udp	0.000654
unknown	22417/udp	0.001307
unknown	22418/udp	0.000654
unknown	22422/udp	0.000654
unknown	22430/udp	0.000654
unknown	22435/udp	0.000654
unknown	22438/udp	0.001307
unknown	22440/udp	0.000654
unknown	22441/udp	0.000654
unknown	22444/udp	0.000654
unknown	22445/udp	0.000654
unknown	22450/udp	0.000654
unknown	22454/udp	0.000654
unknown	22458/udp	0.000654
unknown	22459/udp	0.000654
unknown	22461/udp	0.000654
unknown	22467/udp	0.000654
unknown	22471/udp	0.000654
unknown	22475/udp	0.000654
unknown	22481/udp	0.001307
unknown	22492/udp	0.000654
unknown	22494/udp	0.001307
unknown	22495/udp	0.001307
unknown	22499/udp	0.000654
unknown	22502/udp	0.000654
unknown	22505/udp	0.001307
unknown	22506/udp	0.000654
unknown	22507/udp	0.000654
unknown	22518/udp	0.000654
unknown	22519/udp	0.000654
unknown	22522/udp	0.001307
unknown	22526/udp	0.001307
unknown	22528/udp	0.000654
caldsoft-backup	22537/tcp	0.000000	# CaldSoft Backup server file transfer
unknown	22539/udp	0.000654
unknown	22540/udp	0.000654
unknown	22542/udp	0.000654
unknown	22543/udp	0.000654
unknown	22544/udp	0.000654
unknown	22547/udp	0.001307
unknown	22549/udp	0.000654
unknown	22554/udp	0.000654
vocaltec-wconf	22555/tcp	0.000076	# vocaltec-phone | Vocaltec Web Conference | Vocaltec Internet Phone
vocaltec-phone	22555/udp	0.000000	# Vocaltec Internet Phone
unknown	22556/udp	0.000654
unknown	22558/udp	0.000654
unknown	22563/tcp	0.000076
unknown	22564/udp	0.000654
unknown	22565/udp	0.000654
unknown	22571/udp	0.001307
unknown	22574/udp	0.000654
unknown	22585/udp	0.001307
unknown	22586/udp	0.000654
unknown	22589/udp	0.000654
unknown	22590/udp	0.000654
unknown	22593/udp	0.001307
unknown	22595/udp	0.000654
unknown	22596/udp	0.000654
unknown	22597/udp	0.001307
unknown	22600/udp	0.000654
unknown	22609/udp	0.000654
unknown	22611/udp	0.001307
unknown	22617/udp	0.000654
unknown	22618/udp	0.000654
unknown	22619/udp	0.000654
unknown	22626/udp	0.001307
unknown	22633/udp	0.000654
unknown	22639/udp	0.000654
unknown	22640/udp	0.000654
unknown	22643/udp	0.000654
unknown	22647/udp	0.000654
unknown	22662/udp	0.000654
unknown	22667/udp	0.000654
unknown	22677/udp	0.001307
unknown	22684/udp	0.000654
unknown	22691/udp	0.000654
unknown	22692/udp	0.001961
unknown	22695/udp	0.001961
unknown	22701/udp	0.000654
unknown	22703/udp	0.000654
unknown	22710/udp	0.000654
unknown	22711/tcp	0.000076
unknown	22711/udp	0.000654
unknown	22713/udp	0.000654
unknown	22714/udp	0.000654
unknown	22719/tcp	0.000076
unknown	22720/udp	0.000654
unknown	22721/udp	0.000654
unknown	22724/udp	0.000654
unknown	22725/udp	0.000654
unknown	22726/udp	0.000654
unknown	22727/tcp	0.000076
unknown	22732/udp	0.001307
unknown	22733/udp	0.000654
unknown	22735/udp	0.000654
unknown	22736/udp	0.001307
unknown	22739/udp	0.001961
unknown	22740/udp	0.000654
unknown	22746/udp	0.000654
unknown	22747/udp	0.000654
unknown	22748/udp	0.000654
unknown	22750/udp	0.000654
unknown	22758/udp	0.000654
unknown	22762/udp	0.001307
talikaserver	22763/tcp	0.000000	# Talika Main Server
talikaserver	22763/udp	0.000000	# Talika Main Server
unknown	22764/udp	0.000654
unknown	22766/udp	0.000654
unknown	22769/tcp	0.000076
unknown	22773/udp	0.000654
unknown	22776/udp	0.001307
unknown	22779/udp	0.000654
unknown	22784/udp	0.000654
unknown	22785/udp	0.000654
unknown	22787/udp	0.000654
unknown	22793/udp	0.000654
unknown	22799/udp	0.001961
aws-brf	22800/tcp	0.000000	# Telerate Information Platform LAN
aws-brf	22800/udp	0.000000	# Telerate Information Platform LAN
unknown	22806/udp	0.000654
unknown	22807/udp	0.000654
unknown	22810/udp	0.000654
unknown	22811/udp	0.000654
unknown	22815/udp	0.000654
unknown	22825/udp	0.000654
unknown	22828/udp	0.000654
unknown	22832/udp	0.000654
unknown	22839/udp	0.000654
unknown	22843/udp	0.001307
unknown	22844/udp	0.000654
unknown	22846/udp	0.002614
unknown	22847/udp	0.000654
unknown	22852/udp	0.001307
unknown	22853/udp	0.001307
unknown	22855/udp	0.000654
unknown	22857/udp	0.000654
unknown	22862/udp	0.001307
unknown	22864/udp	0.000654
unknown	22872/udp	0.000654
unknown	22876/udp	0.000654
unknown	22879/udp	0.000654
unknown	22881/udp	0.000654
unknown	22882/tcp	0.000076
unknown	22883/udp	0.000654
unknown	22886/udp	0.000654
unknown	22891/udp	0.000654
unknown	22894/udp	0.000654
unknown	22898/udp	0.000654
unknown	22902/udp	0.001307
unknown	22903/udp	0.000654
unknown	22909/udp	0.000654
unknown	22914/udp	0.001961
unknown	22928/udp	0.000654
unknown	22931/udp	0.000654
unknown	22934/udp	0.000654
unknown	22935/udp	0.000654
unknown	22936/udp	0.000654
unknown	22939/tcp	0.000380
unknown	22939/udp	0.000654
unknown	22940/udp	0.000654
unknown	22945/udp	0.001307
unknown	22947/udp	0.000654
unknown	22949/udp	0.000654
brf-gw	22951/tcp	0.000000	# Telerate Information Platform WAN
brf-gw	22951/udp	0.000000	# Telerate Information Platform WAN
unknown	22954/udp	0.000654
unknown	22955/udp	0.000654
unknown	22959/tcp	0.000076
unknown	22959/udp	0.000654
unknown	22962/udp	0.000654
unknown	22964/udp	0.000654
unknown	22968/udp	0.000654
unknown	22969/tcp	0.000076
unknown	22969/udp	0.000654
unknown	22978/udp	0.000654
unknown	22979/udp	0.000654
unknown	22982/udp	0.000654
unknown	22986/udp	0.003922
unknown	22988/udp	0.000654
unknown	22991/udp	0.001307
unknown	22994/udp	0.000654
unknown	22996/udp	0.002614
inovaport1	23000/tcp	0.000000	# Inova LightLink Server Type 1
inovaport1	23000/udp	0.000654	# Inova LightLink Server Type 1
inovaport2	23001/tcp	0.000000	# Inova LightLink Server Type 2
inovaport2	23001/udp	0.000000	# Inova LightLink Server Type 2
inovaport3	23002/tcp	0.000000	# Inova LightLink Server Type 3
inovaport3	23002/udp	0.000000	# Inova LightLink Server Type 3
inovaport4	23003/tcp	0.000000	# Inova LightLink Server Type 4
inovaport4	23003/udp	0.000000	# Inova LightLink Server Type 4
inovaport5	23004/tcp	0.000000	# Inova LightLink Server Type 5
inovaport5	23004/udp	0.000000	# Inova LightLink Server Type 5
inovaport6	23005/tcp	0.000000	# Inova LightLink Server Type 6
inovaport6	23005/udp	0.000000	# Inova LightLink Server Type 6
unknown	23006/udp	0.000654
unknown	23008/udp	0.000654
unknown	23013/udp	0.000654
unknown	23017/tcp	0.000076
unknown	23017/udp	0.000654
unknown	23021/udp	0.000654
unknown	23022/udp	0.000654
unknown	23027/udp	0.001307
unknown	23033/udp	0.000654
unknown	23040/tcp	0.000076
unknown	23040/udp	0.001961
unknown	23041/udp	0.000654
unknown	23042/udp	0.000654
unknown	23045/udp	0.000654
unknown	23052/tcp	0.000152
gntp	23053/tcp	0.000000	# Generic Notification Transport Protocol
unknown	23055/udp	0.000654
unknown	23059/udp	0.001307
unknown	23066/udp	0.000654
unknown	23073/udp	0.001307
unknown	23074/udp	0.000654
unknown	23076/udp	0.000654
unknown	23077/udp	0.000654
unknown	23080/udp	0.000654
unknown	23082/udp	0.000654
unknown	23084/udp	0.000654
unknown	23088/udp	0.000654
unknown	23089/udp	0.000654
unknown	23092/udp	0.000654
unknown	23093/udp	0.000654
unknown	23095/udp	0.000654
unknown	23102/udp	0.000654
unknown	23108/udp	0.001307
unknown	23111/udp	0.000654
unknown	23116/udp	0.000654
unknown	23117/udp	0.000654
unknown	23123/udp	0.000654
unknown	23131/udp	0.000654
unknown	23139/udp	0.000654
unknown	23143/udp	0.000654
unknown	23146/udp	0.000654
unknown	23147/udp	0.000654
unknown	23148/udp	0.000654
unknown	23150/udp	0.000654
unknown	23152/udp	0.001307
unknown	23153/udp	0.000654
unknown	23161/udp	0.001307
unknown	23162/udp	0.001307
unknown	23170/udp	0.001307
unknown	23172/udp	0.000654
unknown	23176/udp	0.001961
unknown	23177/udp	0.000654
unknown	23179/udp	0.000654
unknown	23180/udp	0.000654
unknown	23182/udp	0.000654
unknown	23183/udp	0.000654
unknown	23184/udp	0.001307
unknown	23186/udp	0.000654
unknown	23189/udp	0.000654
unknown	23193/udp	0.000654
unknown	23202/udp	0.001307
unknown	23203/udp	0.000654
unknown	23209/udp	0.000654
unknown	23219/tcp	0.000076
unknown	23223/udp	0.000654
unknown	23228/tcp	0.000076
unknown	23230/udp	0.001307
unknown	23236/udp	0.000654
unknown	23238/udp	0.000654
unknown	23256/udp	0.001307
unknown	23257/udp	0.000654
unknown	23258/udp	0.000654
unknown	23262/udp	0.000654
unknown	23265/udp	0.000654
unknown	23268/udp	0.000654
unknown	23270/tcp	0.000076
s102	23272/tcp	0.000000	# S102 application
s102	23272/udp	0.000000	# S102 application
unknown	23280/udp	0.000654
unknown	23281/udp	0.000654
unknown	23283/udp	0.000654
unknown	23289/udp	0.000654
5afe-dir	23294/tcp	0.000000	# 5afe-disc | 5AFE SDN Directory | 5AFE SDN Directory discovery
unknown	23296/tcp	0.000076
unknown	23298/udp	0.000654
unknown	23307/udp	0.000654
unknown	23320/udp	0.000654
unknown	23322/udp	0.001307
unknown	23323/udp	0.000654
unknown	23324/udp	0.000654
unknown	23327/udp	0.001307
unknown	23330/udp	0.000654
elxmgmt	23333/tcp	0.000000	# Emulex HBAnyware Remote Management
elxmgmt	23333/udp	0.000000	# Emulex HBAnyware Remote Management
unknown	23334/udp	0.000654
unknown	23337/udp	0.001307
unknown	23341/udp	0.001307
unknown	23342/tcp	0.000076
unknown	23344/udp	0.000654
unknown	23347/udp	0.000654
unknown	23350/udp	0.000654
unknown	23351/udp	0.000654
unknown	23352/udp	0.000654
unknown	23354/udp	0.001961
unknown	23356/udp	0.000654
unknown	23360/udp	0.000654
unknown	23363/udp	0.001307
unknown	23374/udp	0.001307
unknown	23378/udp	0.000654
unknown	23380/udp	0.000654
unknown	23382/tcp	0.000076
unknown	23386/udp	0.000654
unknown	23390/udp	0.000654
unknown	23393/udp	0.000654
unknown	23394/udp	0.000654
unknown	23395/udp	0.000654
unknown	23396/udp	0.000654
unknown	23399/udp	0.001307
novar-dbase	23400/tcp	0.000000	# Novar Data
novar-dbase	23400/udp	0.000654	# Novar Data
novar-alarm	23401/tcp	0.000000	# Novar Alarm
novar-alarm	23401/udp	0.000000	# Novar Alarm
novar-global	23402/tcp	0.000000	# Novar Global
novar-global	23402/udp	0.000000	# Novar Global
unknown	23406/udp	0.000654
unknown	23419/udp	0.000654
unknown	23421/udp	0.001307
unknown	23423/udp	0.000654
unknown	23425/udp	0.000654
unknown	23426/udp	0.001307
unknown	23428/udp	0.001307
unknown	23430/tcp	0.000076
unknown	23430/udp	0.001307
unknown	23436/udp	0.000654
unknown	23438/udp	0.000654
unknown	23440/udp	0.000654
unknown	23441/udp	0.000654
unknown	23445/udp	0.000654
unknown	23451/tcp	0.000076
unknown	23455/udp	0.000654
aequus	23456/tcp	0.000000	# Aequus Service
unknown	23456/udp	0.000654
aequus-alt	23457/tcp	0.000000	# Aequus Service Mgmt
unknown	23468/udp	0.000654
unknown	23469/udp	0.000654
unknown	23470/udp	0.000654
unknown	23471/udp	0.000654
unknown	23477/udp	0.000654
unknown	23480/udp	0.000654
unknown	23495/udp	0.001307
unknown	23497/udp	0.000654
unknown	23502/tcp	0.000760
unknown	23504/udp	0.001307
unknown	23509/udp	0.000654
unknown	23513/udp	0.000654
unknown	23519/udp	0.000654
unknown	23522/udp	0.001307
unknown	23524/udp	0.000654
unknown	23526/udp	0.000654
unknown	23529/udp	0.000654
unknown	23531/udp	0.001961
unknown	23532/udp	0.000654
unknown	23536/udp	0.000654
unknown	23537/udp	0.000654
unknown	23542/udp	0.000654
areaguard-neo	23546/tcp	0.000000	# AreaGuard Neo - WebServer
unknown	23547/udp	0.001307
unknown	23550/udp	0.000654
unknown	23552/udp	0.000654
unknown	23553/udp	0.000654
unknown	23557/udp	0.001961
unknown	23563/udp	0.000654
unknown	23567/udp	0.000654
unknown	23568/udp	0.000654
unknown	23571/udp	0.000654
unknown	23575/udp	0.000654
unknown	23578/udp	0.000654
unknown	23583/udp	0.000654
unknown	23585/udp	0.001307
unknown	23586/udp	0.001307
unknown	23592/udp	0.000654
unknown	23595/udp	0.000654
unknown	23602/udp	0.000654
unknown	23606/udp	0.000654
unknown	23608/udp	0.001961
unknown	23610/udp	0.000654
unknown	23615/udp	0.000654
unknown	23619/udp	0.000654
unknown	23624/udp	0.000654
unknown	23632/udp	0.000654
unknown	23633/udp	0.001307
unknown	23635/udp	0.000654
unknown	23638/udp	0.001307
unknown	23648/udp	0.000654
unknown	23649/udp	0.000654
unknown	23651/udp	0.000654
unknown	23657/udp	0.000654
unknown	23663/udp	0.000654
unknown	23675/udp	0.000654
unknown	23678/udp	0.000654
unknown	23679/udp	0.001961
unknown	23682/udp	0.000654
unknown	23689/udp	0.000654
unknown	23691/udp	0.000654
unknown	23693/udp	0.000654
unknown	23694/udp	0.000654
unknown	23695/udp	0.000654
unknown	23696/udp	0.000654
unknown	23698/udp	0.001307
unknown	23704/udp	0.001307
unknown	23709/udp	0.000654
unknown	23714/udp	0.001307
unknown	23715/udp	0.000654
unknown	23718/udp	0.000654
unknown	23719/udp	0.000654
unknown	23723/tcp	0.000076
unknown	23726/udp	0.000654
unknown	23728/udp	0.000654
unknown	23730/udp	0.000654
unknown	23734/udp	0.000654
unknown	23739/udp	0.000654
unknown	23740/udp	0.000654
unknown	23745/udp	0.001307
unknown	23746/udp	0.000654
unknown	23752/udp	0.000654
unknown	23755/udp	0.001307
unknown	23757/udp	0.000654
unknown	23758/udp	0.001307
unknown	23761/udp	0.000654
unknown	23768/udp	0.000654
unknown	23770/udp	0.000654
unknown	23771/udp	0.000654
unknown	23778/udp	0.000654
unknown	23781/udp	0.001961
unknown	23783/udp	0.000654
unknown	23786/udp	0.000654
unknown	23789/udp	0.000654
unknown	23791/udp	0.000654
unknown	23792/udp	0.000654
unknown	23794/udp	0.000654
unknown	23796/tcp	0.000152
unknown	23796/udp	0.000654
unknown	23807/udp	0.000654
unknown	23813/udp	0.000654
unknown	23814/udp	0.000654
unknown	23816/udp	0.000654
unknown	23835/udp	0.000654
unknown	23837/udp	0.000654
unknown	23840/udp	0.000654
unknown	23841/udp	0.000654
unknown	23854/udp	0.000654
unknown	23856/udp	0.000654
unknown	23857/udp	0.000654
unknown	23859/udp	0.000654
unknown	23863/udp	0.000654
unknown	23865/udp	0.001307
unknown	23875/udp	0.000654
unknown	23877/udp	0.000654
unknown	23884/udp	0.000654
unknown	23885/udp	0.000654
unknown	23887/tcp	0.000076
unknown	23888/udp	0.000654
unknown	23891/udp	0.000654
unknown	23904/udp	0.000654
unknown	23907/udp	0.000654
unknown	23909/udp	0.000654
unknown	23916/udp	0.000654
unknown	23930/udp	0.000654
unknown	23936/udp	0.000654
unknown	23940/udp	0.001307
unknown	23945/udp	0.000654
unknown	23946/udp	0.001307
unknown	23949/udp	0.000654
unknown	23951/udp	0.001307
unknown	23953/tcp	0.000076
unknown	23953/udp	0.000654
unknown	23963/udp	0.000654
unknown	23964/udp	0.000654
unknown	23965/udp	0.001961
unknown	23969/udp	0.000654
unknown	23980/udp	0.001961
unknown	23981/udp	0.000654
unknown	23983/udp	0.000654
unknown	23985/udp	0.000654
unknown	23986/udp	0.000654
unknown	23987/udp	0.000654
unknown	23988/udp	0.000654
unknown	23989/udp	0.000654
unknown	23990/udp	0.000654
unknown	23993/udp	0.000654
med-ltp	24000/tcp	0.000000
med-ltp	24000/udp	0.000000
med-fsp-rx	24001/tcp	0.000000
med-fsp-rx	24001/udp	0.000000
med-fsp-tx	24002/tcp	0.000000
med-fsp-tx	24002/udp	0.000000
med-supp	24003/tcp	0.000000
med-supp	24003/udp	0.000000
med-ovw	24004/tcp	0.000000
med-ovw	24004/udp	0.000654
med-ci	24005/tcp	0.000000
med-ci	24005/udp	0.000654
med-net-svc	24006/tcp	0.000000
med-net-svc	24006/udp	0.000000
unknown	24007/udp	0.001961
unknown	24008/udp	0.001307
unknown	24012/udp	0.000654
unknown	24013/udp	0.001307
unknown	24014/udp	0.000654
unknown	24016/udp	0.000654
unknown	24021/udp	0.001307
unknown	24022/udp	0.000654
unknown	24029/udp	0.000654
unknown	24031/udp	0.000654
unknown	24032/udp	0.001307
unknown	24033/udp	0.000654
unknown	24042/udp	0.000654
unknown	24056/udp	0.000654
unknown	24061/udp	0.000654
unknown	24063/udp	0.001307
unknown	24066/udp	0.000654
unknown	24069/udp	0.000654
unknown	24070/udp	0.000654
unknown	24075/udp	0.000654
unknown	24076/udp	0.000654
unknown	24092/udp	0.000654
unknown	24093/udp	0.001307
unknown	24096/udp	0.000654
unknown	24098/udp	0.001307
unknown	24104/udp	0.001307
unknown	24105/udp	0.000654
unknown	24107/udp	0.001307
unknown	24108/udp	0.000654
unknown	24111/udp	0.000654
unknown	24113/udp	0.001307
unknown	24121/udp	0.000654
unknown	24127/udp	0.000654
unknown	24129/udp	0.000654
unknown	24134/udp	0.000654
unknown	24139/udp	0.000654
unknown	24148/udp	0.000654
unknown	24151/udp	0.000654
unknown	24154/udp	0.000654
unknown	24155/udp	0.001307
unknown	24157/udp	0.000654
unknown	24158/udp	0.001307
unknown	24159/udp	0.000654
unknown	24160/udp	0.000654
unknown	24162/udp	0.000654
unknown	24165/udp	0.000654
unknown	24168/udp	0.000654
unknown	24172/udp	0.001307
unknown	24181/udp	0.000654
unknown	24187/udp	0.000654
unknown	24188/udp	0.000654
unknown	24201/udp	0.000654
unknown	24207/udp	0.000654
unknown	24212/udp	0.001307
unknown	24216/udp	0.000654
unknown	24218/tcp	0.000076
unknown	24226/udp	0.000654
unknown	24232/udp	0.000654
unknown	24233/udp	0.000654
unknown	24234/udp	0.000654
unknown	24236/udp	0.000654
unknown	24241/udp	0.000654
filesphere	24242/tcp	0.000000
filesphere	24242/udp	0.001307
unknown	24245/udp	0.000654
unknown	24247/udp	0.000654
vista-4gl	24249/tcp	0.000000	# Vista 4GL
vista-4gl	24249/udp	0.000000	# Vista 4GL
unknown	24250/udp	0.000654
unknown	24257/udp	0.000654
unknown	24262/udp	0.000654
unknown	24263/udp	0.000654
unknown	24265/udp	0.001307
unknown	24266/udp	0.000654
unknown	24268/udp	0.000654
unknown	24271/udp	0.001307
unknown	24272/udp	0.000654
unknown	24273/udp	0.000654
unknown	24274/udp	0.000654
unknown	24276/udp	0.000654
unknown	24277/udp	0.000654
unknown	24279/udp	0.001961
unknown	24291/udp	0.000654
unknown	24300/udp	0.000654
unknown	24302/udp	0.000654
unknown	24306/udp	0.001307
unknown	24309/udp	0.000654
ild	24321/tcp	0.000000	# Isolv Local Directory
ild	24321/udp	0.000000	# Isolv Local Directory
hid	24322/tcp	0.000000	# Transport of Human Interface Device data streams
vrmg-ip	24323/tcp	0.000000	# Verimag mobile class protocol over TCP
unknown	24323/udp	0.000654
unknown	24324/udp	0.000654
unknown	24326/udp	0.000654
unknown	24342/udp	0.000654
unknown	24346/udp	0.000654
unknown	24353/udp	0.000654
unknown	24355/udp	0.000654
unknown	24356/udp	0.000654
unknown	24360/udp	0.000654
unknown	24362/udp	0.000654
unknown	24363/udp	0.000654
unknown	24366/udp	0.000654
unknown	24373/udp	0.000654
unknown	24374/udp	0.000654
intel_rci	24386/tcp	0.000000	# intel-rci | Intel RCI
intel_rci	24386/udp	0.000000	# Intel RCI
unknown	24388/udp	0.001307
unknown	24392/tcp	0.000076
unknown	24394/udp	0.000654
unknown	24397/udp	0.000654
unknown	24398/udp	0.000654
unknown	24404/udp	0.000654
unknown	24406/udp	0.000654
unknown	24409/udp	0.000654
unknown	24412/udp	0.000654
unknown	24413/udp	0.000654
unknown	24416/tcp	0.000076
unknown	24418/udp	0.001307
unknown	24419/udp	0.001307
unknown	24420/udp	0.000654
unknown	24427/udp	0.000654
unknown	24428/udp	0.000654
unknown	24431/udp	0.000654
unknown	24432/udp	0.000654
unknown	24433/udp	0.000654
unknown	24440/udp	0.000654
unknown	24443/udp	0.000654
unknown	24444/tcp	0.000304
unknown	24444/udp	0.001307
unknown	24449/udp	0.000654
unknown	24452/udp	0.000654
unknown	24456/udp	0.000654
unknown	24460/udp	0.000654
unknown	24462/udp	0.000654
unknown	24463/udp	0.000654
tonidods	24465/tcp	0.000000	# Tonido Domain Server
tonidods	24465/udp	0.000000	# Tonido Domain Server
unknown	24466/udp	0.000654
unknown	24467/udp	0.000654
unknown	24482/udp	0.000654
unknown	24489/udp	0.000654
unknown	24490/udp	0.000654
unknown	24496/udp	0.001307
unknown	24497/udp	0.000654
unknown	24500/udp	0.000654
unknown	24505/udp	0.000654
unknown	24508/udp	0.000654
unknown	24509/udp	0.000654
unknown	24511/udp	0.001961
unknown	24512/udp	0.000654
unknown	24518/udp	0.000654
unknown	24524/udp	0.000654
unknown	24527/udp	0.000654
unknown	24528/udp	0.001307
unknown	24538/udp	0.000654
unknown	24539/udp	0.001307
unknown	24552/tcp	0.000076
binkp	24554/tcp	0.000076
binkp	24554/udp	0.000000
unknown	24555/udp	0.000654
unknown	24560/udp	0.000654
unknown	24562/udp	0.000654
unknown	24564/udp	0.000654
unknown	24567/udp	0.000654
unknown	24573/udp	0.000654
bilobit	24577/tcp	0.000000	# bilobit-update | bilobit Service | bilobit Service Update
unknown	24580/udp	0.000654
unknown	24582/udp	0.000654
unknown	24584/udp	0.000654
unknown	24594/udp	0.001961
unknown	24595/udp	0.000654
unknown	24606/udp	0.001961
unknown	24610/udp	0.000654
unknown	24611/udp	0.000654
unknown	24616/tcp	0.000076
unknown	24616/udp	0.000654
unknown	24620/udp	0.000654
unknown	24622/udp	0.000654
unknown	24626/udp	0.000654
unknown	24627/udp	0.000654
unknown	24636/udp	0.000654
unknown	24639/udp	0.001307
unknown	24642/udp	0.000654
unknown	24644/udp	0.001961
unknown	24645/udp	0.000654
unknown	24650/udp	0.000654
unknown	24652/udp	0.000654
unknown	24655/udp	0.001307
unknown	24656/udp	0.000654
unknown	24657/udp	0.000654
unknown	24658/udp	0.001307
unknown	24665/udp	0.001307
sdtvwcam	24666/tcp	0.000000	# Service used by SmarDTV to communicate between a CAM and a second screen application
unknown	24668/udp	0.000654
canditv	24676/tcp	0.000000	# Canditv Message Service
canditv	24676/udp	0.000000	# Canditv Message Service
flashfiler	24677/tcp	0.000000
flashfiler	24677/udp	0.000654
proactivate	24678/tcp	0.000000	# Turbopower Proactivate
proactivate	24678/udp	0.000000	# Turbopower Proactivate
unknown	24679/udp	0.000654
tcc-http	24680/tcp	0.000000	# TCC User HTTP Service
tcc-http	24680/udp	0.000654	# TCC User HTTP Service
unknown	24681/udp	0.000654
unknown	24684/udp	0.000654
unknown	24685/udp	0.000654
unknown	24686/udp	0.000654
unknown	24689/udp	0.001307
unknown	24692/udp	0.000654
unknown	24693/udp	0.001307
unknown	24696/udp	0.000654
unknown	24705/udp	0.000654
unknown	24706/udp	0.001307
unknown	24716/udp	0.000654
unknown	24722/udp	0.000654
unknown	24723/udp	0.000654
unknown	24725/udp	0.001307
unknown	24731/udp	0.001307
unknown	24732/udp	0.000654
unknown	24735/udp	0.000654
unknown	24737/udp	0.000654
unknown	24739/udp	0.000654
unknown	24740/udp	0.000654
unknown	24741/udp	0.001307
cslg	24754/tcp	0.000000	# Citrix StorageLink Gateway
unknown	24756/udp	0.001307
unknown	24761/udp	0.000654
unknown	24763/udp	0.000654
unknown	24767/udp	0.000654
unknown	24773/udp	0.000654
unknown	24779/udp	0.000654
unknown	24781/udp	0.000654
unknown	24782/udp	0.000654
unknown	24783/udp	0.000654
unknown	24790/udp	0.000654
unknown	24794/udp	0.000654
unknown	24795/udp	0.000654
unknown	24796/udp	0.000654
unknown	24798/udp	0.000654
unknown	24800/tcp	0.000380
unknown	24800/udp	0.001307
unknown	24802/udp	0.000654
unknown	24805/udp	0.000654
unknown	24811/udp	0.000654
unknown	24818/udp	0.001307
unknown	24822/udp	0.000654
unknown	24824/udp	0.000654
unknown	24825/udp	0.000654
unknown	24828/udp	0.000654
unknown	24831/udp	0.000654
unknown	24837/udp	0.001307
unknown	24840/udp	0.000654
unknown	24841/udp	0.000654
unknown	24843/udp	0.000654
unknown	24844/udp	0.000654
unknown	24848/udp	0.000654
assoc-disc	24850/tcp	0.000000	# Device Association Discovery
unknown	24852/udp	0.000654
unknown	24854/udp	0.001961
unknown	24862/udp	0.000654
unknown	24865/udp	0.000654
unknown	24867/udp	0.000654
unknown	24869/udp	0.000654
unknown	24870/udp	0.000654
unknown	24871/udp	0.000654
unknown	24874/udp	0.000654
unknown	24875/udp	0.001307
unknown	24878/udp	0.000654
unknown	24882/udp	0.000654
unknown	24883/udp	0.000654
unknown	24890/udp	0.000654
unknown	24893/udp	0.000654
unknown	24899/udp	0.000654
unknown	24905/udp	0.000654
unknown	24910/udp	0.001961
unknown	24911/udp	0.001307
unknown	24916/udp	0.001307
find	24922/tcp	0.000000	# Find Identification of Network Devices
find	24922/udp	0.000000	# Find Identification of Network Devices
unknown	24926/udp	0.000654
unknown	24932/udp	0.000654
unknown	24936/udp	0.000654
unknown	24939/udp	0.000654
unknown	24941/udp	0.001307
unknown	24943/udp	0.000654
unknown	24945/udp	0.001307
unknown	24946/udp	0.000654
unknown	24950/udp	0.001307
unknown	24956/udp	0.000654
unknown	24957/udp	0.000654
unknown	24958/udp	0.000654
unknown	24963/udp	0.000654
unknown	24973/udp	0.000654
unknown	24980/udp	0.000654
unknown	24982/udp	0.000654
unknown	24983/udp	0.000654
unknown	24993/udp	0.000654
unknown	24995/udp	0.000654
unknown	24999/tcp	0.000076
icl-twobase1	25000/tcp	0.000076
icl-twobase1	25000/udp	0.000000
icl-twobase2	25001/tcp	0.000076
icl-twobase2	25001/udp	0.000000
icl-twobase3	25002/tcp	0.000000
icl-twobase3	25002/udp	0.000000
icl-twobase4	25003/tcp	0.000000
icl-twobase4	25003/udp	0.001961
icl-twobase5	25004/tcp	0.000000
icl-twobase5	25004/udp	0.000000
icl-twobase6	25005/tcp	0.000000
icl-twobase6	25005/udp	0.000000
icl-twobase7	25006/tcp	0.000000
icl-twobase7	25006/udp	0.000000
icl-twobase8	25007/tcp	0.000000
icl-twobase8	25007/udp	0.000000
icl-twobase9	25008/tcp	0.000000
icl-twobase9	25008/udp	0.000000
icl-twobase10	25009/tcp	0.000000
icl-twobase10	25009/udp	0.000000
unknown	25011/udp	0.000654
unknown	25017/udp	0.000654
unknown	25018/udp	0.000654
unknown	25019/udp	0.000654
unknown	25020/udp	0.000654
unknown	25025/udp	0.000654
unknown	25028/udp	0.000654
unknown	25029/udp	0.000654
unknown	25030/udp	0.000654
unknown	25036/udp	0.001307
unknown	25040/udp	0.001307
unknown	25043/udp	0.000654
unknown	25052/udp	0.000654
unknown	25067/udp	0.000654
unknown	25069/udp	0.000654
unknown	25074/udp	0.000654
unknown	25078/udp	0.000654
unknown	25080/udp	0.000654
unknown	25081/udp	0.000654
unknown	25082/udp	0.000654
unknown	25086/udp	0.000654
unknown	25091/udp	0.000654
unknown	25093/udp	0.000654
db2c-tls	25100/tcp	0.000000	# IBM Db2 Client Interface - Encrypted
unknown	25102/udp	0.000654
unknown	25103/udp	0.000654
unknown	25104/udp	0.000654
unknown	25107/udp	0.000654
unknown	25115/udp	0.000654
unknown	25127/udp	0.000654
unknown	25129/udp	0.000654
unknown	25135/udp	0.001307
unknown	25137/udp	0.000654
unknown	25147/udp	0.000654
unknown	25150/udp	0.000654
unknown	25153/udp	0.000654
unknown	25155/udp	0.000654
unknown	25157/udp	0.001961
unknown	25158/udp	0.000654
unknown	25159/udp	0.000654
unknown	25160/udp	0.000654
unknown	25163/udp	0.000654
unknown	25168/udp	0.000654
unknown	25169/udp	0.001307
unknown	25170/udp	0.001307
unknown	25173/udp	0.000654
unknown	25174/tcp	0.000076
unknown	25180/udp	0.000654
unknown	25183/udp	0.000654
unknown	25184/udp	0.000654
unknown	25185/udp	0.000654
unknown	25191/udp	0.000654
unknown	25192/udp	0.000654
unknown	25197/udp	0.000654
unknown	25202/udp	0.000654
unknown	25204/udp	0.000654
unknown	25205/udp	0.000654
unknown	25211/udp	0.000654
unknown	25212/udp	0.001307
unknown	25214/udp	0.000654
unknown	25215/udp	0.000654
unknown	25217/udp	0.000654
unknown	25228/udp	0.000654
unknown	25230/udp	0.000654
unknown	25235/udp	0.000654
unknown	25237/udp	0.000654
unknown	25240/udp	0.001961
unknown	25241/udp	0.000654
unknown	25243/udp	0.000654
unknown	25244/udp	0.000654
unknown	25248/udp	0.001307
unknown	25249/udp	0.001307
unknown	25251/udp	0.000654
unknown	25258/udp	0.000654
unknown	25260/tcp	0.000076
unknown	25262/tcp	0.000076
unknown	25266/udp	0.001307
unknown	25267/udp	0.000654
unknown	25268/udp	0.000654
unknown	25271/udp	0.001307
unknown	25274/udp	0.000654
unknown	25280/udp	0.001961
unknown	25286/udp	0.000654
unknown	25288/tcp	0.000076
unknown	25288/udp	0.000654
unknown	25290/udp	0.001307
unknown	25301/udp	0.000654
unknown	25302/udp	0.000654
unknown	25304/udp	0.000654
unknown	25309/udp	0.000654
unknown	25314/udp	0.000654
unknown	25321/udp	0.000654
unknown	25327/tcp	0.000076
unknown	25331/udp	0.001307
unknown	25332/udp	0.001307
unknown	25337/udp	0.001961
unknown	25338/udp	0.000654
unknown	25343/udp	0.000654
unknown	25348/udp	0.000654
unknown	25353/udp	0.000654
unknown	25364/udp	0.000654
unknown	25366/udp	0.001307
unknown	25369/udp	0.000654
unknown	25374/udp	0.000654
unknown	25375/udp	0.002614
unknown	25378/udp	0.000654
unknown	25385/udp	0.001307
unknown	25390/udp	0.000654
unknown	25394/udp	0.000654
unknown	25395/udp	0.000654
unknown	25396/udp	0.000654
unknown	25397/udp	0.000654
unknown	25398/udp	0.000654
unknown	25399/udp	0.000654
unknown	25402/udp	0.001307
unknown	25416/udp	0.000654
unknown	25418/udp	0.000654
unknown	25421/udp	0.000654
unknown	25428/udp	0.000654
unknown	25432/udp	0.000654
unknown	25439/udp	0.000654
unknown	25442/udp	0.000654
unknown	25443/udp	0.000654
unknown	25445/tcp	0.000076
unknown	25446/udp	0.000654
unknown	25451/udp	0.000654
unknown	25453/udp	0.000654
unknown	25455/udp	0.000654
unknown	25460/udp	0.000654
unknown	25462/udp	0.001961
unknown	25466/udp	0.001307
rna	25471/tcp	0.000000	# RNSAP User Adaptation for Iurh
unknown	25473/tcp	0.000076
unknown	25474/udp	0.000654
unknown	25480/udp	0.000654
unknown	25483/udp	0.000654
unknown	25486/tcp	0.000076
unknown	25488/udp	0.001307
unknown	25492/udp	0.000654
unknown	25493/udp	0.000654
unknown	25498/udp	0.001307
unknown	25499/udp	0.000654
unknown	25502/udp	0.000654
unknown	25509/udp	0.000654
unknown	25514/udp	0.001307
unknown	25515/udp	0.000654
unknown	25521/udp	0.001307
unknown	25522/udp	0.000654
unknown	25523/udp	0.000654
unknown	25524/udp	0.000654
unknown	25533/udp	0.000654
unknown	25534/udp	0.000654
unknown	25537/udp	0.000654
unknown	25538/udp	0.001307
unknown	25540/udp	0.000654
unknown	25541/udp	0.001961
unknown	25542/udp	0.000654
unknown	25544/udp	0.001307
unknown	25546/udp	0.001961
unknown	25560/udp	0.001307
unknown	25564/udp	0.000654
minecraft	25565/tcp	0.000076	# A video game - http://en.wikipedia.org/wiki/Minecraft
unknown	25567/udp	0.000654
unknown	25568/udp	0.000654
unknown	25569/udp	0.000654
unknown	25572/udp	0.000654
unknown	25573/udp	0.000654
unknown	25574/udp	0.000654
sauterdongle	25576/tcp	0.000000	# Sauter Dongle
unknown	25579/udp	0.001307
unknown	25586/udp	0.001307
unknown	25588/udp	0.000654
unknown	25590/udp	0.000654
unknown	25591/udp	0.000654
unknown	25592/udp	0.000654
unknown	25594/udp	0.000654
unknown	25600/udp	0.001307
unknown	25603/udp	0.000654
idtp	25604/tcp	0.000000	# Identifier Tracing Protocol
unknown	25611/udp	0.000654
unknown	25617/udp	0.000654
unknown	25618/udp	0.000654
unknown	25624/udp	0.001307
unknown	25627/udp	0.001307
unknown	25628/udp	0.001307
unknown	25630/udp	0.000654
unknown	25636/udp	0.000654
unknown	25641/udp	0.000654
unknown	25642/udp	0.000654
unknown	25643/udp	0.000654
unknown	25644/udp	0.000654
unknown	25652/udp	0.001307
unknown	25658/udp	0.000654
unknown	25659/udp	0.000654
unknown	25666/udp	0.000654
unknown	25667/udp	0.000654
unknown	25670/udp	0.001307
unknown	25677/udp	0.000654
unknown	25687/udp	0.000654
unknown	25703/tcp	0.000076
unknown	25706/udp	0.000654
unknown	25709/udp	0.001961
unknown	25710/udp	0.000654
unknown	25712/udp	0.000654
unknown	25715/udp	0.001307
unknown	25716/udp	0.000654
unknown	25717/tcp	0.000076
unknown	25723/udp	0.000654
unknown	25724/udp	0.000654
unknown	25730/udp	0.000654
unknown	25731/udp	0.000654
unknown	25733/udp	0.001307
unknown	25734/tcp	0.000380
unknown	25735/tcp	0.000228
unknown	25735/udp	0.000654
unknown	25744/udp	0.000654
unknown	25751/udp	0.000654
unknown	25756/udp	0.001307
unknown	25763/udp	0.000654
unknown	25767/udp	0.000654
unknown	25768/udp	0.000654
unknown	25778/udp	0.001307
unknown	25790/udp	0.000654
vocaltec-hos	25793/tcp	0.000000	# Vocaltec Address Server
vocaltec-hos	25793/udp	0.000654	# Vocaltec Address Server
unknown	25794/udp	0.000654
unknown	25798/udp	0.000654
unknown	25799/udp	0.000654
unknown	25815/udp	0.000654
unknown	25823/udp	0.000654
unknown	25826/udp	0.001307
unknown	25827/udp	0.000654
unknown	25832/udp	0.000654
unknown	25833/udp	0.000654
unknown	25841/udp	0.000654
unknown	25847/tcp	0.000076
unknown	25849/udp	0.000654
unknown	25851/udp	0.001307
unknown	25853/udp	0.000654
unknown	25857/udp	0.000654
unknown	25868/udp	0.001307
unknown	25875/udp	0.001307
unknown	25879/udp	0.000654
unknown	25881/udp	0.000654
unknown	25887/udp	0.000654
unknown	25894/udp	0.000654
unknown	25896/udp	0.000654
tasp-net	25900/tcp	0.000000	# TASP Network Comm
tasp-net	25900/udp	0.000000	# TASP Network Comm
niobserver	25901/tcp	0.000000
niobserver	25901/udp	0.000654
nilinkanalyst	25902/tcp	0.000000
nilinkanalyst	25902/udp	0.000000
niprobe	25903/tcp	0.000000
niprobe	25903/udp	0.000000
unknown	25909/udp	0.001307
unknown	25910/udp	0.000654
unknown	25913/udp	0.001307
unknown	25921/udp	0.000654
unknown	25925/udp	0.001307
unknown	25928/udp	0.000654
unknown	25929/udp	0.000654
unknown	25931/udp	0.001961
unknown	25940/udp	0.000654
unknown	25944/udp	0.000654
unknown	25949/udp	0.000654
unknown	25950/udp	0.000654
unknown	25951/udp	0.000654
bf-game	25954/tcp	0.000000	# Bitfighter game server
bf-master	25955/tcp	0.000000	# Bitfighter master server
unknown	25956/udp	0.001307
unknown	25958/udp	0.000654
unknown	25968/udp	0.000654
unknown	25969/udp	0.000654
unknown	25975/udp	0.000654
unknown	25980/udp	0.000654
unknown	25985/udp	0.000654
unknown	25987/udp	0.000654
unknown	25988/udp	0.000654
unknown	25989/udp	0.000654
unknown	25992/udp	0.001307
unknown	25993/udp	0.000654
quake	26000/tcp	0.000152
quake	26000/udp	0.000490	# Quake game server
unknown	26001/tcp	0.000076
unknown	26002/udp	0.000654
unknown	26005/udp	0.000654
unknown	26007/tcp	0.000076
unknown	26013/udp	0.000654
unknown	26020/udp	0.000654
unknown	26021/udp	0.000654
unknown	26026/udp	0.001307
unknown	26030/udp	0.000654
unknown	26031/udp	0.001307
unknown	26033/udp	0.000654
unknown	26035/udp	0.000654
unknown	26036/udp	0.000654
unknown	26039/udp	0.000654
unknown	26040/udp	0.000654
unknown	26048/udp	0.000654
unknown	26050/udp	0.000654
unknown	26052/udp	0.001307
unknown	26055/udp	0.000654
unknown	26057/udp	0.000654
unknown	26058/udp	0.000654
unknown	26062/udp	0.000654
unknown	26066/udp	0.000654
unknown	26067/udp	0.000654
unknown	26073/udp	0.000654
unknown	26078/udp	0.000654
unknown	26079/udp	0.001307
unknown	26080/udp	0.000654
unknown	26089/udp	0.000654
unknown	26090/udp	0.000654
unknown	26095/udp	0.000654
unknown	26100/udp	0.000654
unknown	26103/udp	0.001307
unknown	26107/udp	0.000654
unknown	26110/udp	0.000654
unknown	26116/udp	0.000654
unknown	26119/udp	0.000654
unknown	26121/udp	0.000654
unknown	26123/udp	0.001307
unknown	26127/udp	0.000654
unknown	26130/udp	0.000654
unknown	26131/udp	0.000654
scscp	26133/tcp	0.000000	# Symbolic Computation Software Composability Protocol
scscp	26133/udp	0.000000	# Symbolic Computation Software Composability Protocol
unknown	26134/udp	0.000654
unknown	26137/udp	0.000654
unknown	26141/udp	0.000654
unknown	26147/udp	0.000654
unknown	26157/udp	0.000654
unknown	26158/udp	0.000654
unknown	26163/udp	0.000654
unknown	26164/udp	0.000654
unknown	26171/udp	0.001307
unknown	26172/udp	0.000654
unknown	26175/udp	0.000654
unknown	26179/udp	0.000654
unknown	26181/udp	0.000654
unknown	26183/udp	0.000654
unknown	26187/udp	0.000654
unknown	26189/udp	0.000654
unknown	26191/udp	0.001307
unknown	26196/udp	0.001307
unknown	26198/udp	0.000654
unknown	26201/udp	0.000654
unknown	26203/udp	0.000654
unknown	26204/udp	0.001307
unknown	26205/udp	0.000654
unknown	26207/udp	0.000654
wnn6_DS	26208/tcp	0.000025	# Wnn6 (Dserver) | wnn6-ds
wnn6-ds	26208/udp	0.000000
unknown	26211/udp	0.000654
unknown	26214/tcp	0.000228
unknown	26219/udp	0.001307
unknown	26225/udp	0.000654
unknown	26239/udp	0.001307
unknown	26243/udp	0.001307
unknown	26254/udp	0.001307
cockroach	26257/tcp	0.000000	# CockroachDB
ezproxy	26260/tcp	0.000000
ezproxy	26260/udp	0.000000
ezmeeting	26261/tcp	0.000000
ezmeeting	26261/udp	0.000000
k3software-svr	26262/tcp	0.000000	# K3 Software-Server
k3software-svr	26262/udp	0.000000	# K3 Software-Server
k3software-cli	26263/tcp	0.000000	# K3 Software-Client
k3software-cli	26263/udp	0.000000	# K3 Software-Client
unknown	26270/udp	0.000654
unknown	26273/udp	0.000654
unknown	26275/udp	0.000654
unknown	26279/udp	0.000654
unknown	26283/udp	0.000654
unknown	26284/udp	0.001307
unknown	26286/udp	0.001307
unknown	26289/udp	0.001307
unknown	26291/udp	0.000654
unknown	26296/udp	0.000654
unknown	26299/udp	0.000654
unknown	26304/udp	0.000654
unknown	26311/udp	0.000654
unknown	26318/udp	0.000654
unknown	26325/udp	0.000654
unknown	26337/udp	0.001307
unknown	26338/udp	0.000654
unknown	26339/udp	0.000654
unknown	26340/tcp	0.000076
unknown	26340/udp	0.001307
unknown	26356/udp	0.000654
unknown	26362/udp	0.000654
unknown	26364/udp	0.000654
unknown	26367/udp	0.000654
unknown	26369/udp	0.000654
unknown	26372/udp	0.000654
unknown	26376/udp	0.000654
unknown	26381/udp	0.001307
unknown	26384/udp	0.000654
unknown	26388/udp	0.001307
unknown	26395/udp	0.000654
unknown	26397/udp	0.000654
unknown	26401/udp	0.001307
unknown	26407/udp	0.001961
unknown	26409/udp	0.000654
unknown	26411/udp	0.000654
unknown	26413/udp	0.000654
unknown	26415/udp	0.001961
unknown	26416/udp	0.000654
unknown	26417/tcp	0.000076
unknown	26417/udp	0.000654
unknown	26418/udp	0.000654
unknown	26420/udp	0.001307
unknown	26423/udp	0.001307
unknown	26431/udp	0.001307
unknown	26432/udp	0.000654
unknown	26434/udp	0.001307
unknown	26436/udp	0.000654
unknown	26439/udp	0.000654
unknown	26442/udp	0.000654
unknown	26448/udp	0.000654
unknown	26451/udp	0.000654
unknown	26452/udp	0.001307
unknown	26466/udp	0.000654
unknown	26470/tcp	0.000152
unknown	26473/udp	0.000654
unknown	26477/udp	0.000654
unknown	26481/udp	0.000654
unknown	26482/udp	0.000654
unknown	26484/udp	0.000654
exoline-tcp	26486/tcp	0.000000	# exoline-udp | EXOline-UDP
exoline-udp	26486/udp	0.000000
exoconfig	26487/tcp	0.000000
exoconfig	26487/udp	0.000000
exonet	26489/tcp	0.000000
exonet	26489/udp	0.000000
unknown	26491/udp	0.000654
unknown	26493/udp	0.001307
unknown	26497/udp	0.000654
unknown	26507/udp	0.001307
unknown	26508/udp	0.000654
unknown	26509/udp	0.000654
unknown	26512/udp	0.001307
unknown	26522/udp	0.000654
unknown	26523/udp	0.000654
unknown	26529/udp	0.000654
unknown	26531/udp	0.001307
unknown	26532/udp	0.000654
unknown	26536/udp	0.000654
unknown	26538/udp	0.000654
unknown	26541/udp	0.000654
unknown	26549/udp	0.001307
unknown	26556/udp	0.000654
unknown	26563/udp	0.000654
unknown	26573/udp	0.000654
unknown	26575/udp	0.000654
unknown	26578/udp	0.000654
unknown	26579/udp	0.000654
unknown	26585/udp	0.000654
unknown	26587/udp	0.000654
unknown	26594/udp	0.000654
unknown	26596/udp	0.000654
unknown	26618/udp	0.000654
unknown	26621/udp	0.000654
unknown	26622/udp	0.000654
unknown	26628/udp	0.000654
unknown	26631/udp	0.000654
unknown	26639/udp	0.000654
unknown	26641/udp	0.000654
unknown	26645/udp	0.001307
unknown	26649/udp	0.000654
unknown	26651/udp	0.000654
unknown	26654/udp	0.000654
unknown	26655/udp	0.000654
unknown	26664/udp	0.000654
unknown	26665/udp	0.000654
unknown	26666/udp	0.000654
unknown	26668/udp	0.000654
unknown	26669/tcp	0.000076
unknown	26673/udp	0.000654
unknown	26674/udp	0.000654
unknown	26678/udp	0.000654
unknown	26679/udp	0.000654
unknown	26681/udp	0.000654
unknown	26683/udp	0.000654
unknown	26685/udp	0.000654
unknown	26689/udp	0.000654
unknown	26690/udp	0.000654
unknown	26691/udp	0.000654
unknown	26692/udp	0.000654
unknown	26695/udp	0.000654
unknown	26698/udp	0.001307
unknown	26699/udp	0.000654
unknown	26702/udp	0.000654
unknown	26705/udp	0.001307
unknown	26706/udp	0.000654
unknown	26708/udp	0.000654
unknown	26714/udp	0.000654
unknown	26718/udp	0.000654
unknown	26720/udp	0.001961
unknown	26724/udp	0.000654
unknown	26725/udp	0.000654
unknown	26742/udp	0.001307
unknown	26746/udp	0.000654
unknown	26747/udp	0.000654
unknown	26753/udp	0.000654
unknown	26754/udp	0.000654
unknown	26760/udp	0.000654
unknown	26761/udp	0.000654
unknown	26765/udp	0.001307
unknown	26771/udp	0.001307
unknown	26775/udp	0.000654
unknown	26776/udp	0.000654
unknown	26786/udp	0.000654
unknown	26792/udp	0.000654
unknown	26794/udp	0.000654
unknown	26795/udp	0.001307
unknown	26796/udp	0.001307
unknown	26801/udp	0.000654
unknown	26803/udp	0.000654
unknown	26805/udp	0.000654
unknown	26806/udp	0.000654
unknown	26810/udp	0.000654
unknown	26814/udp	0.000654
unknown	26819/udp	0.001307
unknown	26823/udp	0.001307
unknown	26829/udp	0.000654
unknown	26830/udp	0.000654
unknown	26839/udp	0.000654
unknown	26841/udp	0.000654
unknown	26842/udp	0.000654
unknown	26843/udp	0.001307
unknown	26845/udp	0.001307
unknown	26847/udp	0.000654
unknown	26857/udp	0.000654
unknown	26859/udp	0.000654
unknown	26860/udp	0.000654
unknown	26861/udp	0.000654
unknown	26866/udp	0.001307
unknown	26868/udp	0.001307
unknown	26872/udp	0.001961
unknown	26875/udp	0.000654
unknown	26876/udp	0.000654
unknown	26878/udp	0.001307
unknown	26881/udp	0.000654
unknown	26882/udp	0.000654
unknown	26884/udp	0.000654
unknown	26888/udp	0.001307
unknown	26891/udp	0.000654
unknown	26896/udp	0.000654
unknown	26899/udp	0.000654
hexen2	26900/udp	0.001166	# Hexen 2 game server
unknown	26903/udp	0.000654
unknown	26906/udp	0.000654
unknown	26914/udp	0.000654
unknown	26916/udp	0.000654
unknown	26919/udp	0.000654
unknown	26926/udp	0.000654
unknown	26932/udp	0.000654
unknown	26934/udp	0.000654
unknown	26937/udp	0.000654
unknown	26941/udp	0.000654
unknown	26944/udp	0.000654
unknown	26949/udp	0.001307
unknown	26951/udp	0.000654
unknown	26953/udp	0.000654
unknown	26955/udp	0.000654
unknown	26958/udp	0.000654
unknown	26960/udp	0.000654
unknown	26963/udp	0.000654
unknown	26966/udp	0.001961
unknown	26970/udp	0.000654
unknown	26972/tcp	0.000076
unknown	26973/udp	0.001307
unknown	26977/udp	0.000654
unknown	26979/udp	0.000654
unknown	26982/udp	0.001307
unknown	26983/udp	0.000654
unknown	26988/udp	0.000654
unknown	26994/udp	0.001307
unknown	26996/udp	0.001307
unknown	26998/udp	0.001307
flexlm0	27000/tcp	0.000640	# FlexLM license manager additional ports
flex-lm	27000/udp	0.000000	# FLEX LM (1-10)
flexlm1	27001/tcp	0.000075	# FlexLM license manager additional ports
flex-lm	27001/udp	0.000000	# FLEX LM (1-10)
flexlm2	27002/tcp	0.000013	# FlexLM license manager additional ports
flex-lm	27002/udp	0.001307	# FLEX LM (1-10)
flexlm3	27003/tcp	0.000013	# FlexLM license manager additional ports
flex-lm	27003/udp	0.000654	# FLEX LM (1-10)
flexlm4	27004/tcp	0.000000	# FlexLM license manager additional ports
flex-lm	27004/udp	0.000000	# FLEX LM (1-10)
flexlm5	27005/tcp	0.000013	# FlexLM license manager additional ports
flex-lm	27005/udp	0.000000	# FLEX LM (1-10)
flexlm6	27006/tcp	0.000000	# FlexLM license manager additional ports
flex-lm	27006/udp	0.000000	# FLEX LM (1-10)
flexlm7	27007/tcp	0.000013	# FlexLM license manager additional ports
flex-lm	27007/udp	0.001307	# FLEX LM (1-10)
flexlm8	27008/tcp	0.000000	# FlexLM license manager additional ports
flex-lm	27008/udp	0.000000	# FLEX LM (1-10)
flexlm9	27009/tcp	0.000013	# FlexLM license manager additional ports
flex-lm	27009/udp	0.000000	# FLEX LM (1-10)
flexlm10	27010/tcp	0.000063	# flex-lmadmin | FlexLM license manager additional ports | A protocol for managing license services
unknown	27010/udp	0.001307
unknown	27014/udp	0.000654
unknown	27015/tcp	0.000076
halflife	27015/udp	0.002432	# Half-life game server
unknown	27016/tcp	0.000076
mongod	27017/tcp	0.000076	# mongodb | http://docs.mongodb.org/manual/reference/default-mongodb-port/ | Mongo database system
unknown	27017/udp	0.001307
mongod	27018/tcp	0.000076	# http://docs.mongodb.org/manual/reference/default-mongodb-port/
unknown	27018/udp	0.000654
mongod	27019/tcp	0.000076	# http://docs.mongodb.org/manual/reference/default-mongodb-port/
unknown	27020/udp	0.000654
unknown	27025/udp	0.001307
unknown	27027/udp	0.001307
unknown	27029/udp	0.000654
unknown	27032/udp	0.000654
unknown	27036/udp	0.000654
unknown	27038/udp	0.000654
unknown	27042/udp	0.000654
unknown	27046/udp	0.000654
unknown	27048/udp	0.000654
unknown	27049/udp	0.000654
unknown	27055/tcp	0.000076
unknown	27057/udp	0.000654
unknown	27058/udp	0.001307
unknown	27061/udp	0.000654
unknown	27062/udp	0.000654
unknown	27064/udp	0.001307
unknown	27072/udp	0.001307
unknown	27074/tcp	0.000076
unknown	27075/tcp	0.000076
unknown	27075/udp	0.000654
unknown	27076/udp	0.000654
unknown	27078/udp	0.001307
unknown	27079/udp	0.001307
unknown	27085/udp	0.001307
unknown	27087/tcp	0.000076
unknown	27087/udp	0.000654
unknown	27088/udp	0.000654
unknown	27089/udp	0.000654
unknown	27094/udp	0.000654
unknown	27095/udp	0.001307
unknown	27098/udp	0.000654
unknown	27100/udp	0.000654
unknown	27101/udp	0.000654
unknown	27104/udp	0.000654
unknown	27110/udp	0.001307
unknown	27118/udp	0.000654
unknown	27133/udp	0.001307
unknown	27139/udp	0.000654
unknown	27144/udp	0.000654
unknown	27147/udp	0.000654
unknown	27148/udp	0.000654
unknown	27150/udp	0.001307
unknown	27157/udp	0.000654
unknown	27169/udp	0.000654
unknown	27172/udp	0.000654
unknown	27174/udp	0.000654
unknown	27175/udp	0.000654
unknown	27179/udp	0.001307
unknown	27180/udp	0.001307
unknown	27182/udp	0.001307
unknown	27192/udp	0.000654
unknown	27195/udp	0.002614
unknown	27196/udp	0.000654
unknown	27200/udp	0.001307
unknown	27202/udp	0.000654
unknown	27204/tcp	0.000076
unknown	27209/udp	0.001307
unknown	27212/udp	0.000654
unknown	27221/udp	0.000654
unknown	27223/udp	0.000654
unknown	27227/udp	0.000654
unknown	27228/udp	0.000654
unknown	27230/udp	0.000654
unknown	27232/udp	0.000654
unknown	27237/udp	0.000654
unknown	27249/udp	0.000654
unknown	27258/udp	0.000654
unknown	27259/udp	0.000654
unknown	27263/udp	0.001307
unknown	27268/udp	0.000654
unknown	27270/udp	0.000654
unknown	27271/udp	0.001307
unknown	27272/udp	0.001307
unknown	27274/udp	0.000654
unknown	27280/udp	0.000654
unknown	27285/udp	0.000654
unknown	27286/udp	0.000654
unknown	27287/udp	0.001307
unknown	27289/udp	0.000654
unknown	27290/udp	0.000654
unknown	27291/udp	0.000654
unknown	27298/udp	0.000654
unknown	27300/udp	0.000654
unknown	27310/udp	0.000654
unknown	27313/udp	0.000654
unknown	27316/tcp	0.000076
unknown	27323/udp	0.000654
unknown	27330/udp	0.000654
unknown	27331/udp	0.000654
unknown	27340/udp	0.000654
imagepump	27345/tcp	0.000000
imagepump	27345/udp	0.000000
mdcs-scheduler	27350/tcp	0.000076	# MATLAB Job Scheduler
unknown	27351/tcp	0.000076
unknown	27352/tcp	0.000304
unknown	27353/tcp	0.000304
unknown	27355/tcp	0.000304
unknown	27355/udp	0.000654
unknown	27356/tcp	0.000228
unknown	27357/tcp	0.000152
unknown	27358/udp	0.000654
unknown	27364/udp	0.000654
unknown	27366/udp	0.000654
unknown	27368/udp	0.000654
unknown	27372/tcp	0.000076
unknown	27373/udp	0.000654
subseven	27374/tcp	0.000050	# Subseven Windows trojan
unknown	27381/udp	0.000654
unknown	27391/udp	0.000654
unknown	27395/udp	0.000654
unknown	27397/udp	0.000654
unknown	27398/udp	0.000654
unknown	27408/udp	0.000654
unknown	27410/udp	0.000654
unknown	27414/udp	0.001307
unknown	27416/udp	0.001307
unknown	27424/udp	0.000654
unknown	27433/udp	0.000654
unknown	27436/udp	0.000654
unknown	27437/udp	0.001307
unknown	27438/udp	0.000654
jesmsjc	27442/tcp	0.000000	# Job controller service
jesmsjc	27442/udp	0.000000	# Job controller service
Trinoo_Bcast	27444/udp	0.001554	# Trinoo distributed attack tool Master
unknown	27445/udp	0.000654
unknown	27449/udp	0.000654
unknown	27454/udp	0.000654
unknown	27455/udp	0.000654
unknown	27464/udp	0.000654
unknown	27465/udp	0.000654
unknown	27466/udp	0.001307
unknown	27470/udp	0.000654
unknown	27471/udp	0.000654
unknown	27473/udp	0.001961
unknown	27475/udp	0.000654
unknown	27476/udp	0.000654
unknown	27482/udp	0.001961
unknown	27487/udp	0.001307
unknown	27493/udp	0.000654
quakeworld	27500/udp	0.000980	# Quake world
unknown	27501/udp	0.000654
kopek-httphead	27504/tcp	0.000000	# Kopek HTTP Head Port
kopek-httphead	27504/udp	0.000000	# Kopek HTTP Head Port
unknown	27507/udp	0.000654
unknown	27510/udp	0.000654
unknown	27512/udp	0.000654
unknown	27521/tcp	0.000076
unknown	27525/udp	0.000654
unknown	27532/udp	0.000654
unknown	27533/udp	0.000654
unknown	27537/tcp	0.000076
unknown	27537/udp	0.000654
unknown	27538/udp	0.001307
unknown	27547/udp	0.001307
unknown	27548/udp	0.000654
unknown	27556/udp	0.000654
unknown	27561/udp	0.001307
unknown	27563/udp	0.000654
unknown	27564/udp	0.000654
unknown	27566/udp	0.000654
unknown	27573/udp	0.001307
unknown	27575/udp	0.000654
unknown	27579/udp	0.001307
unknown	27581/udp	0.000654
unknown	27584/udp	0.000654
unknown	27586/udp	0.000654
unknown	27587/udp	0.000654
unknown	27588/udp	0.000654
unknown	27593/udp	0.000654
unknown	27597/udp	0.000654
unknown	27599/udp	0.000654
unknown	27600/udp	0.001307
unknown	27602/udp	0.000654
unknown	27606/udp	0.001307
unknown	27608/udp	0.000654
unknown	27617/udp	0.000654
unknown	27621/udp	0.000654
unknown	27622/udp	0.000654
unknown	27624/udp	0.000654
unknown	27626/udp	0.000654
unknown	27630/udp	0.000654
unknown	27631/udp	0.000654
unknown	27636/udp	0.000654
unknown	27637/udp	0.000654
unknown	27662/udp	0.000654
unknown	27663/udp	0.000654
Trinoo_Master	27665/tcp	0.000038	# Trinoo distributed attack tool Master server control port
unknown	27666/udp	0.001307
unknown	27669/udp	0.000654
unknown	27672/udp	0.000654
unknown	27673/udp	0.001307
unknown	27677/udp	0.000654
unknown	27678/udp	0.001307
unknown	27680/udp	0.000654
unknown	27682/udp	0.001307
unknown	27687/udp	0.000654
unknown	27688/udp	0.000654
unknown	27689/udp	0.000654
unknown	27690/udp	0.000654
unknown	27693/udp	0.000654
unknown	27694/udp	0.000654
unknown	27696/udp	0.001307
unknown	27698/udp	0.000654
unknown	27700/udp	0.000654
unknown	27702/udp	0.000654
unknown	27703/udp	0.000654
unknown	27705/udp	0.000654
unknown	27707/udp	0.001961
unknown	27708/udp	0.001307
unknown	27711/udp	0.001307
unknown	27712/udp	0.000654
unknown	27713/udp	0.000654
unknown	27714/udp	0.000654
unknown	27715/tcp	0.000380
unknown	27715/udp	0.000654
unknown	27718/udp	0.001307
unknown	27720/udp	0.000654
unknown	27721/udp	0.000654
unknown	27722/udp	0.001307
unknown	27729/udp	0.000654
unknown	27733/udp	0.000654
unknown	27735/udp	0.000654
unknown	27741/udp	0.000654
unknown	27742/udp	0.000654
unknown	27745/udp	0.000654
unknown	27750/udp	0.001307
unknown	27755/udp	0.000654
unknown	27756/udp	0.000654
unknown	27760/udp	0.000654
unknown	27767/udp	0.000654
unknown	27769/udp	0.000654
unknown	27770/tcp	0.000076
unknown	27775/udp	0.000654
unknown	27781/udp	0.000654
ars-vista	27782/tcp	0.000000	# ARS VISTA Application
ars-vista	27782/udp	0.000000	# ARS VISTA Application
unknown	27783/udp	0.000654
unknown	27785/udp	0.000654
unknown	27786/udp	0.000654
unknown	27788/udp	0.000654
unknown	27792/udp	0.000654
unknown	27801/udp	0.000654
unknown	27803/udp	0.000654
unknown	27815/udp	0.000654
unknown	27817/udp	0.000654
unknown	27818/udp	0.000654
unknown	27822/udp	0.000654
unknown	27826/udp	0.000654
unknown	27828/udp	0.000654
unknown	27829/udp	0.000654
unknown	27830/udp	0.000654
unknown	27832/udp	0.000654
unknown	27833/udp	0.000654
unknown	27836/udp	0.000654
unknown	27838/udp	0.000654
unknown	27849/udp	0.000654
unknown	27850/udp	0.000654
unknown	27853/udp	0.001307
unknown	27856/udp	0.000654
unknown	27859/udp	0.000654
unknown	27860/udp	0.000654
unknown	27861/udp	0.001307
unknown	27863/udp	0.000654
unknown	27867/udp	0.000654
unknown	27869/udp	0.000654
unknown	27872/udp	0.000654
astrolink	27876/tcp	0.000000	# Astrolink Protocol
unknown	27876/udp	0.000654
unknown	27884/udp	0.000654
unknown	27887/udp	0.000654
unknown	27892/udp	0.003268
unknown	27895/udp	0.001307
unknown	27899/udp	0.001961
unknown	27900/udp	0.000654
unknown	27902/udp	0.000654
unknown	27905/udp	0.000654
quake2	27910/udp	0.000760	# Quake 2 game server
unknown	27912/udp	0.000654
unknown	27916/udp	0.000654
unknown	27918/udp	0.000654
unknown	27919/udp	0.001307
unknown	27931/udp	0.000654
unknown	27939/udp	0.000654
unknown	27940/udp	0.000654
unknown	27944/udp	0.000654
unknown	27949/udp	0.001307
unknown	27951/udp	0.000654
unknown	27952/udp	0.000654
unknown	27954/udp	0.000654
unknown	27958/udp	0.000654
unknown	27959/udp	0.000654
quake3	27960/udp	0.000726	# Quake 3 Arena Server
unknown	27967/udp	0.000654
unknown	27969/udp	0.001307
unknown	27970/udp	0.000654
unknown	27972/udp	0.000654
unknown	27973/udp	0.001307
unknown	27974/udp	0.000654
unknown	27979/udp	0.000654
unknown	27983/udp	0.000654
unknown	27984/udp	0.000654
unknown	27992/udp	0.000654
unknown	27994/udp	0.000654
unknown	27996/udp	0.000654
tw-auth-key	27999/tcp	0.000000	# TW Authentication/Key Distribution and | Attribute Certificate Services
tw-auth-key	27999/udp	0.000000	# Attribute Certificate Services
nxlmd	28000/tcp	0.000000	# NX License Manager
nxlmd	28000/udp	0.000000	# NX License Manager
pqsp	28001/tcp	0.000000	# PQ Service
unknown	28005/udp	0.000654
gruber-cashreg	28010/tcp	0.000000	# Gruber cash registry protocol
unknown	28011/udp	0.001307
rethinkdb	28015/tcp	0.000076
mongod	28017/tcp	0.000076	# http://docs.mongodb.org/manual/reference/default-mongodb-port/
unknown	28019/udp	0.000654
unknown	28020/udp	0.000654
unknown	28021/udp	0.000654
unknown	28028/udp	0.000654
unknown	28029/udp	0.000654
unknown	28034/udp	0.001307
unknown	28036/udp	0.000654
unknown	28043/udp	0.000654
unknown	28045/udp	0.000654
unknown	28051/udp	0.000654
unknown	28054/udp	0.000654
unknown	28058/udp	0.000654
unknown	28059/udp	0.000654
unknown	28064/udp	0.000654
unknown	28070/udp	0.001307
unknown	28071/udp	0.001307
unknown	28072/udp	0.000654
unknown	28074/udp	0.000654
unknown	28077/udp	0.000654
unknown	28078/udp	0.000654
thor-engine	28080/tcp	0.000000	# thor/server - ML engine
unknown	28080/udp	0.001307
unknown	28089/udp	0.000654
unknown	28091/udp	0.001307
unknown	28094/udp	0.000654
unknown	28096/udp	0.000654
unknown	28097/udp	0.000654
unknown	28098/udp	0.001307
unknown	28105/udp	0.001307
unknown	28107/udp	0.001307
unknown	28108/udp	0.000654
unknown	28109/udp	0.000654
unknown	28112/udp	0.000654
unknown	28114/tcp	0.000076
unknown	28116/udp	0.000654
a27-ran-ran	28119/tcp	0.000000	# A27 cdma2000 RAN Management
unknown	28120/udp	0.000654
unknown	28121/udp	0.000654
unknown	28122/udp	0.001961
unknown	28124/udp	0.000654
unknown	28129/udp	0.001307
unknown	28141/udp	0.000654
unknown	28142/tcp	0.000076
unknown	28142/udp	0.000654
unknown	28144/udp	0.000654
unknown	28145/udp	0.000654
unknown	28148/udp	0.000654
unknown	28154/udp	0.000654
unknown	28155/udp	0.000654
unknown	28172/udp	0.001307
unknown	28178/udp	0.000654
unknown	28182/udp	0.000654
unknown	28183/udp	0.000654
unknown	28190/udp	0.001307
unknown	28195/udp	0.000654
unknown	28197/udp	0.000654
voxelstorm	28200/tcp	0.000000	# VoxelStorm game server
unknown	28200/udp	0.000654
unknown	28201/tcp	0.000380
unknown	28203/udp	0.000654
unknown	28211/tcp	0.000152
unknown	28211/udp	0.001307
unknown	28212/udp	0.000654
unknown	28213/udp	0.000654
unknown	28215/udp	0.000654
unknown	28218/udp	0.000654
unknown	28219/udp	0.000654
unknown	28220/udp	0.001307
unknown	28221/udp	0.000654
unknown	28222/udp	0.001307
unknown	28230/udp	0.000654
unknown	28237/udp	0.000654
unknown	28239/udp	0.000654
siemensgsm	28240/tcp	0.000000	# Siemens GSM
siemensgsm	28240/udp	0.000000	# Siemens GSM
unknown	28242/udp	0.000654
unknown	28243/udp	0.000654
unknown	28246/udp	0.000654
unknown	28247/udp	0.001307
unknown	28248/udp	0.000654
unknown	28251/udp	0.000654
unknown	28257/udp	0.000654
unknown	28263/udp	0.001307
unknown	28265/udp	0.000654
unknown	28271/udp	0.000654
unknown	28283/udp	0.000654
unknown	28292/udp	0.000654
unknown	28295/udp	0.001307
unknown	28298/udp	0.000654
unknown	28301/udp	0.000654
unknown	28303/udp	0.000654
unknown	28307/udp	0.000654
unknown	28309/udp	0.000654
unknown	28311/udp	0.000654
unknown	28315/udp	0.000654
unknown	28317/udp	0.000654
unknown	28322/udp	0.000654
unknown	28327/udp	0.000654
unknown	28334/udp	0.000654
unknown	28335/udp	0.000654
unknown	28344/udp	0.001307
unknown	28345/udp	0.000654
unknown	28348/udp	0.000654
unknown	28349/udp	0.001307
unknown	28353/udp	0.000654
unknown	28356/udp	0.000654
unknown	28366/udp	0.000654
unknown	28367/udp	0.000654
unknown	28369/udp	0.001961
unknown	28374/tcp	0.000076
unknown	28377/udp	0.000654
unknown	28378/udp	0.000654
unknown	28380/udp	0.000654
unknown	28386/udp	0.000654
unknown	28387/udp	0.001307
unknown	28391/udp	0.000654
unknown	28392/udp	0.000654
unknown	28393/udp	0.000654
unknown	28396/udp	0.000654
unknown	28401/udp	0.000654
unknown	28411/udp	0.000654
unknown	28417/udp	0.000654
unknown	28419/udp	0.000654
unknown	28421/udp	0.000654
unknown	28422/udp	0.000654
unknown	28425/udp	0.000654
unknown	28427/udp	0.000654
unknown	28428/udp	0.000654
unknown	28433/udp	0.000654
unknown	28434/udp	0.000654
unknown	28437/udp	0.000654
unknown	28438/udp	0.001307
unknown	28440/udp	0.001307
unknown	28441/udp	0.000654
unknown	28445/udp	0.001307
unknown	28455/udp	0.000654
unknown	28464/udp	0.000654
unknown	28465/udp	0.001961
unknown	28466/udp	0.000654
unknown	28469/udp	0.000654
unknown	28471/udp	0.000654
unknown	28472/udp	0.000654
unknown	28476/udp	0.001307
unknown	28477/udp	0.000654
unknown	28483/udp	0.000654
unknown	28484/udp	0.000654
unknown	28485/udp	0.001307
unknown	28488/udp	0.000654
unknown	28493/udp	0.001961
unknown	28506/udp	0.000654
unknown	28513/udp	0.000654
unknown	28521/udp	0.000654
unknown	28525/udp	0.001307
unknown	28529/udp	0.000654
unknown	28530/udp	0.000654
unknown	28534/udp	0.000654
unknown	28537/udp	0.000654
unknown	28543/udp	0.001961
unknown	28544/udp	0.000654
unknown	28545/udp	0.000654
unknown	28547/udp	0.002614
unknown	28556/udp	0.000654
unknown	28561/udp	0.000654
unknown	28567/tcp	0.000076
unknown	28575/udp	0.000654
unknown	28584/udp	0.001307
unknown	28586/udp	0.000654
unknown	28587/udp	0.000654
bosswave	28589/tcp	0.000000	# Building operating system services wide area verified exchange
unknown	28597/udp	0.000654
unknown	28607/udp	0.000654
unknown	28609/udp	0.001307
unknown	28610/udp	0.000654
unknown	28617/udp	0.000654
unknown	28618/udp	0.000654
unknown	28620/udp	0.000654
unknown	28625/udp	0.000654
unknown	28630/udp	0.001307
unknown	28633/udp	0.000654
unknown	28638/udp	0.000654
unknown	28640/udp	0.001307
unknown	28641/udp	0.001961
unknown	28642/udp	0.000654
unknown	28643/udp	0.000654
unknown	28644/udp	0.000654
unknown	28645/udp	0.001307
unknown	28649/udp	0.000654
unknown	28654/udp	0.000654
unknown	28660/udp	0.000654
unknown	28661/udp	0.000654
unknown	28663/udp	0.001307
unknown	28664/udp	0.001307
unknown	28673/udp	0.000654
unknown	28674/udp	0.001307
unknown	28675/udp	0.000654
unknown	28682/udp	0.000654
unknown	28685/udp	0.000654
unknown	28689/udp	0.000654
unknown	28692/udp	0.001307
unknown	28696/udp	0.000654
unknown	28697/udp	0.000654
unknown	28700/udp	0.000654
unknown	28705/udp	0.000654
unknown	28706/udp	0.001307
unknown	28707/udp	0.001307
unknown	28708/udp	0.000654
unknown	28717/tcp	0.000076
unknown	28719/udp	0.001307
unknown	28723/udp	0.000654
unknown	28725/udp	0.001307
unknown	28728/udp	0.000654
unknown	28729/udp	0.000654
unknown	28730/udp	0.000654
unknown	28734/udp	0.000654
unknown	28736/udp	0.000654
unknown	28737/udp	0.000654
unknown	28741/udp	0.000654
unknown	28744/udp	0.000654
unknown	28745/udp	0.001307
unknown	28746/udp	0.001307
unknown	28748/udp	0.000654
unknown	28750/udp	0.000654
unknown	28752/udp	0.000654
unknown	28754/udp	0.000654
unknown	28755/udp	0.000654
unknown	28765/udp	0.000654
unknown	28769/udp	0.000654
unknown	28772/udp	0.000654
unknown	28775/udp	0.000654
unknown	28776/udp	0.000654
unknown	28778/udp	0.000654
unknown	28779/udp	0.000654
unknown	28780/udp	0.000654
unknown	28785/udp	0.000654
unknown	28797/udp	0.000654
unknown	28800/udp	0.000654
unknown	28803/udp	0.001307
unknown	28808/udp	0.001307
unknown	28810/udp	0.000654
unknown	28811/udp	0.000654
unknown	28813/udp	0.000654
unknown	28815/udp	0.001307
unknown	28816/udp	0.000654
unknown	28822/udp	0.000654
unknown	28826/udp	0.000654
unknown	28827/udp	0.000654
unknown	28830/udp	0.000654
unknown	28836/udp	0.000654
unknown	28837/udp	0.000654
unknown	28839/udp	0.000654
unknown	28840/udp	0.001961
unknown	28845/udp	0.000654
unknown	28847/udp	0.000654
unknown	28850/tcp	0.000076
unknown	28851/tcp	0.000076
unknown	28851/udp	0.000654
unknown	28854/udp	0.000654
unknown	28855/udp	0.000654
unknown	28856/udp	0.000654
unknown	28858/udp	0.000654
unknown	28865/udp	0.000654
unknown	28875/udp	0.000654
unknown	28876/udp	0.000654
unknown	28877/udp	0.000654
unknown	28879/udp	0.000654
unknown	28880/udp	0.000654
unknown	28883/udp	0.000654
unknown	28885/udp	0.000654
unknown	28887/udp	0.000654
unknown	28888/udp	0.000654
unknown	28892/udp	0.001307
unknown	28893/udp	0.000654
unknown	28895/udp	0.000654
unknown	28896/udp	0.000654
unknown	28898/udp	0.000654
unknown	28900/udp	0.000654
unknown	28902/udp	0.000654
unknown	28905/udp	0.000654
unknown	28906/udp	0.000654
heretic2	28910/udp	0.000524	# Heretic 2 game server
unknown	28917/udp	0.000654
unknown	28919/udp	0.000654
unknown	28920/udp	0.000654
unknown	28924/tcp	0.000076
unknown	28924/udp	0.000654
unknown	28927/udp	0.000654
unknown	28931/udp	0.001307
unknown	28932/udp	0.000654
unknown	28933/udp	0.001307
unknown	28934/udp	0.000654
unknown	28938/udp	0.000654
unknown	28940/udp	0.000654
unknown	28943/udp	0.000654
unknown	28944/udp	0.001307
unknown	28945/udp	0.000654
unknown	28946/udp	0.000654
unknown	28952/udp	0.000654
unknown	28953/udp	0.000654
unknown	28954/udp	0.000654
unknown	28958/udp	0.000654
unknown	28965/udp	0.001307
unknown	28966/udp	0.000654
unknown	28967/tcp	0.000076
unknown	28967/udp	0.000654
unknown	28969/udp	0.000654
unknown	28973/udp	0.001961
unknown	28976/udp	0.000654
unknown	28979/udp	0.000654
unknown	28992/udp	0.000654
unknown	28995/udp	0.001307
unknown	28997/udp	0.000654
saltd-licensing	29000/tcp	0.000000	# Siemens Licensing Server
unknown	29000/udp	0.000654
unknown	29007/udp	0.000654
unknown	29008/udp	0.000654
unknown	29010/udp	0.000654
unknown	29013/udp	0.000654
unknown	29014/udp	0.000654
rethinkdb	29015/tcp	0.000076
unknown	29022/udp	0.000654
unknown	29026/udp	0.000654
unknown	29030/udp	0.001307
unknown	29032/udp	0.000654
unknown	29036/udp	0.000654
unknown	29039/udp	0.000654
unknown	29045/tcp	0.000076
unknown	29045/udp	0.000654
unknown	29046/udp	0.000654
unknown	29048/udp	0.001307
unknown	29052/udp	0.000654
unknown	29053/udp	0.000654
unknown	29054/udp	0.001307
unknown	29056/udp	0.000654
unknown	29058/udp	0.000654
unknown	29061/udp	0.000654
unknown	29069/udp	0.000654
unknown	29070/udp	0.000654
unknown	29078/udp	0.001961
unknown	29082/udp	0.001307
unknown	29084/udp	0.000654
unknown	29087/udp	0.000654
unknown	29095/udp	0.000654
unknown	29105/udp	0.000654
unknown	29112/udp	0.000654
unknown	29114/udp	0.000654
unknown	29115/udp	0.000654
sgsap	29118/sctp	0.000000	# SGsAP in 3GPP
unknown	29121/udp	0.000654
unknown	29126/udp	0.000654
unknown	29129/udp	0.001307
unknown	29134/udp	0.000654
unknown	29135/udp	0.001307
unknown	29137/udp	0.000654
unknown	29142/udp	0.001307
unknown	29149/udp	0.000654
unknown	29150/udp	0.001307
unknown	29152/tcp	0.000076
unknown	29153/udp	0.001307
unknown	29162/udp	0.001307
unknown	29163/udp	0.000654
otmp	29167/tcp	0.000000	# ObTools Message Protocol
otmp	29167/udp	0.000000	# ObTools Message Protocol
sbcap	29168/sctp	0.000000	# SBcAP in 3GPP
unknown	29168/udp	0.001307
iuhsctpassoc	29169/sctp	0.000000	# HNBAP and RUA Common Association
unknown	29172/udp	0.000654
unknown	29177/udp	0.000654
unknown	29180/udp	0.001307
unknown	29183/udp	0.000654
unknown	29185/udp	0.000654
unknown	29186/udp	0.000654
unknown	29195/udp	0.000654
unknown	29196/udp	0.000654
unknown	29199/udp	0.000654
unknown	29200/udp	0.001307
unknown	29201/udp	0.000654
unknown	29203/udp	0.000654
unknown	29207/udp	0.000654
unknown	29211/udp	0.000654
unknown	29218/udp	0.000654
unknown	29220/udp	0.000654
unknown	29224/udp	0.000654
unknown	29230/udp	0.001307
unknown	29238/udp	0.000654
unknown	29239/udp	0.000654
unknown	29243/tcp	0.000076
unknown	29243/udp	0.001961
unknown	29248/udp	0.000654
unknown	29249/udp	0.000654
unknown	29256/udp	0.001961
unknown	29257/udp	0.000654
unknown	29259/udp	0.000654
unknown	29268/udp	0.000654
unknown	29272/udp	0.000654
unknown	29273/udp	0.000654
unknown	29276/udp	0.001307
unknown	29277/udp	0.000654
unknown	29278/udp	0.000654
unknown	29280/udp	0.000654
unknown	29281/udp	0.000654
unknown	29283/udp	0.000654
unknown	29284/udp	0.000654
unknown	29286/udp	0.000654
unknown	29298/udp	0.000654
unknown	29305/udp	0.000654
unknown	29308/udp	0.000654
unknown	29312/udp	0.000654
unknown	29315/udp	0.000654
unknown	29317/udp	0.000654
unknown	29319/udp	0.001307
unknown	29323/udp	0.000654
unknown	29324/udp	0.000654
unknown	29327/udp	0.000654
unknown	29329/udp	0.000654
unknown	29331/udp	0.000654
unknown	29333/udp	0.001307
unknown	29335/udp	0.000654
unknown	29342/udp	0.000654
unknown	29352/udp	0.000654
unknown	29355/udp	0.000654
unknown	29357/udp	0.001307
unknown	29364/udp	0.000654
unknown	29366/udp	0.000654
unknown	29368/udp	0.000654
unknown	29375/udp	0.000654
unknown	29376/udp	0.000654
unknown	29380/udp	0.000654
unknown	29390/udp	0.000654
unknown	29393/udp	0.000654
unknown	29396/udp	0.000654
unknown	29397/udp	0.000654
unknown	29398/udp	0.000654
unknown	29400/udp	0.001307
unknown	29401/udp	0.001307
unknown	29403/udp	0.000654
unknown	29406/udp	0.000654
unknown	29407/udp	0.000654
unknown	29408/udp	0.000654
unknown	29410/udp	0.001307
unknown	29414/udp	0.000654
unknown	29415/udp	0.000654
unknown	29420/udp	0.000654
unknown	29426/udp	0.001307
unknown	29427/udp	0.000654
unknown	29432/udp	0.000654
unknown	29435/udp	0.000654
unknown	29442/udp	0.000654
unknown	29444/udp	0.001307
unknown	29447/udp	0.000654
unknown	29448/udp	0.000654
unknown	29449/udp	0.001307
unknown	29453/udp	0.001307
unknown	29457/udp	0.000654
unknown	29461/udp	0.001307
unknown	29465/udp	0.000654
unknown	29467/udp	0.000654
unknown	29471/udp	0.000654
unknown	29474/udp	0.000654
unknown	29476/udp	0.000654
unknown	29480/udp	0.000654
unknown	29486/udp	0.000654
unknown	29488/udp	0.000654
unknown	29494/udp	0.000654
unknown	29499/udp	0.000654
unknown	29503/udp	0.001307
unknown	29506/udp	0.000654
unknown	29507/tcp	0.000076
unknown	29508/udp	0.000654
unknown	29512/udp	0.000654
unknown	29514/udp	0.000654
unknown	29518/udp	0.000654
unknown	29520/udp	0.000654
unknown	29522/udp	0.001307
unknown	29523/udp	0.000654
unknown	29525/udp	0.000654
unknown	29533/udp	0.000654
unknown	29534/udp	0.001307
unknown	29541/udp	0.001307
unknown	29554/udp	0.001307
unknown	29559/udp	0.000654
unknown	29562/udp	0.000654
unknown	29564/udp	0.001307
unknown	29570/udp	0.000654
unknown	29572/udp	0.000654
unknown	29577/udp	0.000654
unknown	29581/udp	0.001307
unknown	29582/udp	0.000654
unknown	29583/udp	0.000654
unknown	29585/udp	0.000654
unknown	29587/udp	0.000654
unknown	29588/udp	0.000654
unknown	29589/udp	0.000654
unknown	29595/udp	0.001307
unknown	29600/udp	0.000654
unknown	29604/udp	0.000654
unknown	29607/udp	0.000654
unknown	29613/udp	0.001307
unknown	29615/udp	0.000654
unknown	29616/udp	0.000654
unknown	29618/udp	0.000654
unknown	29630/udp	0.000654
unknown	29632/udp	0.000654
unknown	29639/udp	0.000654
unknown	29642/udp	0.000654
unknown	29647/udp	0.000654
unknown	29652/udp	0.000654
unknown	29659/udp	0.000654
unknown	29665/udp	0.000654
unknown	29667/udp	0.000654
unknown	29672/tcp	0.000152
unknown	29673/udp	0.000654
unknown	29677/udp	0.000654
unknown	29680/udp	0.000654
unknown	29681/udp	0.000654
unknown	29682/udp	0.000654
unknown	29694/udp	0.000654
unknown	29700/udp	0.000654
unknown	29701/udp	0.000654
unknown	29709/udp	0.001307
unknown	29712/udp	0.000654
unknown	29715/udp	0.000654
unknown	29729/udp	0.000654
unknown	29731/udp	0.000654
unknown	29733/udp	0.000654
unknown	29737/udp	0.000654
unknown	29742/udp	0.000654
unknown	29747/udp	0.000654
unknown	29749/udp	0.000654
unknown	29752/udp	0.000654
unknown	29753/udp	0.000654
unknown	29754/udp	0.000654
unknown	29756/udp	0.000654
unknown	29759/udp	0.000654
unknown	29761/udp	0.000654
unknown	29771/udp	0.000654
unknown	29773/udp	0.000654
unknown	29780/udp	0.000654
unknown	29782/udp	0.000654
unknown	29785/udp	0.000654
unknown	29787/udp	0.000654
unknown	29788/udp	0.000654
unknown	29794/udp	0.001307
unknown	29796/udp	0.000654
unknown	29802/udp	0.000654
unknown	29809/udp	0.000654
unknown	29810/tcp	0.000076
unknown	29810/udp	0.001961
unknown	29811/udp	0.000654
unknown	29812/udp	0.000654
unknown	29816/udp	0.000654
unknown	29823/udp	0.002614
unknown	29829/udp	0.000654
unknown	29831/tcp	0.000152
unknown	29833/udp	0.000654
unknown	29834/udp	0.001307
unknown	29840/udp	0.000654
unknown	29842/udp	0.000654
unknown	29843/udp	0.001307
unknown	29846/udp	0.000654
unknown	29852/udp	0.000654
unknown	29854/udp	0.000654
unknown	29858/udp	0.000654
unknown	29860/udp	0.000654
unknown	29863/udp	0.000654
unknown	29864/udp	0.000654
unknown	29867/udp	0.000654
unknown	29869/udp	0.000654
unknown	29876/udp	0.000654
unknown	29878/udp	0.000654
unknown	29883/udp	0.000654
unknown	29886/udp	0.001307
unknown	29894/udp	0.001307
unknown	29901/udp	0.000654
unknown	29903/udp	0.000654
unknown	29905/udp	0.000654
unknown	29907/udp	0.000654
unknown	29911/udp	0.000654
unknown	29914/udp	0.000654
unknown	29915/udp	0.000654
unknown	29926/udp	0.000654
unknown	29927/udp	0.000654
unknown	29930/udp	0.000654
unknown	29932/udp	0.000654
unknown	29949/udp	0.000654
unknown	29956/udp	0.000654
unknown	29961/udp	0.001307
unknown	29964/udp	0.001307
unknown	29967/udp	0.000654
unknown	29970/udp	0.000654
unknown	29977/udp	0.001961
unknown	29978/udp	0.000654
unknown	29980/udp	0.000654
unknown	29981/udp	0.001307
unknown	29987/udp	0.000654
unknown	29988/udp	0.000654
bingbang	29999/tcp	0.000000	# data exchange protocol for IEC61850 in wind power plants
ndmps	30000/tcp	0.000380	# Secure Network Data Management Protocol
unknown	30000/udp	0.000654
pago-services1	30001/tcp	0.000076	# Pago Services 1
pago-services1	30001/udp	0.000000	# Pago Services 1
pago-services2	30002/tcp	0.000000	# Pago Services 2
pago-services2	30002/udp	0.000000	# Pago Services 2
amicon-fpsu-ra	30003/tcp	0.000000	# Amicon FPSU-IP Remote Administration
amicon-fpsu-s	30004/tcp	0.000000	# Amicon FPSU-IP VPN
unknown	30005/tcp	0.000152
unknown	30006/udp	0.000654
unknown	30008/udp	0.000654
unknown	30015/udp	0.000654
unknown	30018/udp	0.000654
unknown	30020/udp	0.000654
unknown	30027/udp	0.000654
unknown	30031/udp	0.000654
unknown	30034/udp	0.001307
unknown	30036/udp	0.000654
unknown	30041/udp	0.000654
unknown	30046/udp	0.000654
unknown	30048/udp	0.000654
unknown	30055/udp	0.001307
unknown	30059/udp	0.000654
unknown	30063/udp	0.000654
unknown	30066/udp	0.000654
unknown	30067/udp	0.001307
unknown	30085/udp	0.001307
unknown	30086/udp	0.000654
unknown	30087/tcp	0.000076
unknown	30093/udp	0.001307
rwp	30100/tcp	0.000000	# Remote Window Protocol
unknown	30108/udp	0.000654
unknown	30113/udp	0.000654
unknown	30123/udp	0.000654
unknown	30126/udp	0.000654
unknown	30130/udp	0.000654
unknown	30131/udp	0.000654
unknown	30132/udp	0.000654
unknown	30134/udp	0.001307
unknown	30135/udp	0.000654
unknown	30139/udp	0.000654
unknown	30144/udp	0.000654
unknown	30148/udp	0.000654
unknown	30150/udp	0.000654
unknown	30154/udp	0.001307
unknown	30168/udp	0.000654
unknown	30170/udp	0.000654
unknown	30172/udp	0.000654
unknown	30175/udp	0.000654
unknown	30179/udp	0.000654
unknown	30181/udp	0.000654
unknown	30182/udp	0.000654
unknown	30184/udp	0.000654
unknown	30188/udp	0.000654
unknown	30193/udp	0.000654
unknown	30194/udp	0.000654
unknown	30195/tcp	0.000076
unknown	30209/udp	0.001307
unknown	30211/udp	0.000654
unknown	30212/udp	0.000654
unknown	30214/udp	0.001307
unknown	30230/udp	0.000654
unknown	30234/udp	0.000654
unknown	30235/udp	0.000654
unknown	30236/udp	0.000654
unknown	30239/udp	0.000654
unknown	30241/udp	0.000654
unknown	30244/udp	0.000654
unknown	30245/udp	0.000654
unknown	30246/udp	0.000654
unknown	30252/udp	0.000654
unknown	30254/udp	0.000654
unknown	30256/udp	0.001307
unknown	30258/udp	0.000654
kingdomsonline	30260/tcp	0.000000	# Kingdoms Online (CraigAvenue)
kingdomsonline	30260/udp	0.001307	# Kingdoms Online (CraigAvenue)
unknown	30263/udp	0.001961
unknown	30267/udp	0.000654
unknown	30286/udp	0.000654
unknown	30293/udp	0.000654
unknown	30295/udp	0.000654
unknown	30298/udp	0.000654
unknown	30299/tcp	0.000076
unknown	30299/udp	0.001307
unknown	30300/udp	0.000654
unknown	30303/udp	0.002614
unknown	30305/udp	0.000654
unknown	30306/udp	0.000654
unknown	30309/udp	0.000654
unknown	30310/udp	0.000654
unknown	30318/udp	0.000654
unknown	30330/udp	0.000654
unknown	30331/udp	0.000654
unknown	30335/udp	0.000654
unknown	30338/udp	0.000654
unknown	30341/udp	0.000654
unknown	30348/udp	0.001307
unknown	30350/udp	0.000654
unknown	30359/udp	0.000654
unknown	30365/udp	0.002614
unknown	30378/udp	0.000654
unknown	30381/udp	0.000654
unknown	30383/udp	0.000654
unknown	30394/udp	0.000654
unknown	30398/udp	0.000654
gs-realtime	30400/tcp	0.000000	# GroundStar RealTime System
unknown	30400/udp	0.000654
unknown	30411/udp	0.000654
unknown	30416/udp	0.000654
unknown	30418/udp	0.000654
unknown	30419/udp	0.000654
unknown	30420/udp	0.000654
unknown	30423/udp	0.000654
unknown	30424/udp	0.000654
unknown	30428/udp	0.000654
unknown	30430/udp	0.000654
unknown	30433/udp	0.000654
unknown	30434/udp	0.000654
unknown	30453/udp	0.000654
unknown	30454/udp	0.000654
unknown	30457/udp	0.000654
unknown	30461/udp	0.001307
unknown	30462/udp	0.000654
unknown	30463/udp	0.000654
unknown	30464/udp	0.000654
unknown	30465/udp	0.001307
unknown	30467/udp	0.000654
unknown	30468/udp	0.000654
unknown	30470/udp	0.000654
unknown	30472/udp	0.000654
unknown	30473/udp	0.001307
unknown	30474/udp	0.001307
unknown	30475/udp	0.000654
unknown	30477/udp	0.001307
unknown	30478/udp	0.000654
unknown	30481/udp	0.000654
unknown	30483/udp	0.000654
unknown	30491/udp	0.000654
unknown	30492/udp	0.000654
unknown	30493/udp	0.000654
unknown	30495/udp	0.000654
unknown	30496/udp	0.000654
unknown	30500/udp	0.000654
unknown	30501/udp	0.000654
unknown	30511/udp	0.000654
unknown	30512/udp	0.001307
unknown	30514/udp	0.000654
unknown	30516/udp	0.000654
unknown	30518/udp	0.000654
unknown	30519/tcp	0.000076
unknown	30521/udp	0.000654
unknown	30522/udp	0.000654
unknown	30526/udp	0.001307
unknown	30529/udp	0.000654
unknown	30533/udp	0.001307
unknown	30536/udp	0.000654
unknown	30539/udp	0.000654
unknown	30544/udp	0.001961
unknown	30550/udp	0.000654
unknown	30555/udp	0.000654
unknown	30564/udp	0.000654
unknown	30566/udp	0.000654
unknown	30568/udp	0.000654
unknown	30575/udp	0.000654
unknown	30578/udp	0.001307
unknown	30583/udp	0.001307
unknown	30587/udp	0.000654
unknown	30588/udp	0.000654
unknown	30592/udp	0.000654
unknown	30599/tcp	0.000076
unknown	30601/udp	0.000654
unknown	30609/udp	0.000654
unknown	30612/udp	0.001307
unknown	30619/udp	0.000654
unknown	30622/udp	0.001307
unknown	30623/udp	0.000654
unknown	30624/udp	0.000654
unknown	30627/udp	0.000654
unknown	30637/udp	0.000654
unknown	30644/tcp	0.000076
unknown	30644/udp	0.000654
unknown	30646/udp	0.000654
unknown	30648/udp	0.000654
unknown	30650/udp	0.000654
unknown	30651/udp	0.000654
unknown	30656/udp	0.001961
unknown	30657/udp	0.000654
unknown	30658/udp	0.000654
unknown	30659/tcp	0.000076
unknown	30660/udp	0.000654
unknown	30661/udp	0.001307
unknown	30662/udp	0.000654
unknown	30664/udp	0.000654
unknown	30665/udp	0.000654
unknown	30669/udp	0.001307
unknown	30670/udp	0.000654
unknown	30672/udp	0.000654
unknown	30682/udp	0.000654
unknown	30687/udp	0.000654
unknown	30688/udp	0.000654
unknown	30689/udp	0.000654
unknown	30697/udp	0.001961
unknown	30698/udp	0.001307
unknown	30701/udp	0.000654
unknown	30702/udp	0.000654
unknown	30704/tcp	0.000152
unknown	30704/udp	0.001961
unknown	30705/tcp	0.000076
unknown	30710/udp	0.000654
unknown	30712/udp	0.000654
unknown	30713/udp	0.000654
unknown	30718/tcp	0.000380
unknown	30718/udp	0.007190
unknown	30719/udp	0.000654
unknown	30723/udp	0.000654
unknown	30725/udp	0.000654
unknown	30729/udp	0.000654
unknown	30734/udp	0.000654
unknown	30737/udp	0.000654
unknown	30738/udp	0.000654
unknown	30741/udp	0.000654
unknown	30746/udp	0.000654
unknown	30754/udp	0.000654
unknown	30755/udp	0.000654
unknown	30757/udp	0.001307
unknown	30762/udp	0.000654
unknown	30765/udp	0.000654
unknown	30772/udp	0.000654
unknown	30780/udp	0.000654
unknown	30782/udp	0.000654
unknown	30783/udp	0.000654
unknown	30784/udp	0.000654
unknown	30785/udp	0.001307
unknown	30789/udp	0.001307
unknown	30795/udp	0.000654
unknown	30796/udp	0.000654
unknown	30803/udp	0.001307
unknown	30805/udp	0.000654
unknown	30808/udp	0.000654
unknown	30819/udp	0.000654
unknown	30820/udp	0.000654
unknown	30823/udp	0.000654
unknown	30824/udp	0.001307
unknown	30825/udp	0.000654
unknown	30826/udp	0.000654
unknown	30827/udp	0.000654
unknown	30828/udp	0.000654
samsung-disc	30832/tcp	0.000000	# Samsung Convergence Discovery Protocol
unknown	30833/udp	0.000654
unknown	30837/udp	0.000654
unknown	30838/udp	0.000654
unknown	30841/udp	0.000654
unknown	30849/udp	0.000654
unknown	30851/udp	0.000654
unknown	30856/udp	0.001307
unknown	30867/udp	0.000654
unknown	30869/udp	0.001307
unknown	30875/udp	0.001307
unknown	30876/udp	0.000654
unknown	30880/udp	0.001307
unknown	30881/udp	0.000654
unknown	30886/udp	0.000654
unknown	30892/udp	0.000654
unknown	30893/udp	0.000654
unknown	30894/udp	0.000654
unknown	30896/tcp	0.000076
unknown	30897/udp	0.000654
unknown	30906/udp	0.000654
unknown	30908/udp	0.000654
unknown	30909/udp	0.001307
unknown	30910/udp	0.000654
unknown	30912/udp	0.000654
unknown	30918/udp	0.000654
unknown	30919/udp	0.000654
unknown	30924/udp	0.000654
unknown	30926/udp	0.000654
unknown	30930/udp	0.001307
unknown	30931/udp	0.000654
unknown	30932/udp	0.001307
unknown	30942/udp	0.000654
unknown	30943/udp	0.001307
unknown	30945/udp	0.000654
unknown	30951/tcp	0.000228
unknown	30951/udp	0.000654
unknown	30955/udp	0.000654
unknown	30958/udp	0.000654
unknown	30959/udp	0.000654
unknown	30965/udp	0.000654
unknown	30967/udp	0.000654
unknown	30972/udp	0.000654
unknown	30975/udp	0.001961
unknown	30982/udp	0.000654
unknown	30984/udp	0.000654
unknown	30986/udp	0.000654
unknown	30990/udp	0.000654
unknown	30996/udp	0.001307
ovobs	30999/tcp	0.000000	# OpenView Service Desk Client
ovobs	30999/udp	0.000000	# OpenView Service Desk Client
unknown	31001/udp	0.000654
unknown	31005/udp	0.000654
unknown	31015/udp	0.000654
ka-sddp	31016/tcp	0.000000	# ka-kdp | Kollective Agent Secure Distributed Delivery Protocol | Kollective Agent Kollective Delivery Protocol
autotrac-acp	31020/tcp	0.000000	# Autotrac ACP 245
unknown	31020/udp	0.000654
unknown	31022/udp	0.000654
unknown	31028/udp	0.000654
yawn	31029/tcp	0.000000	# YaWN - Yet Another Windows Notifier
yawn	31029/udp	0.000000	# YaWN - Yet Another Windows Notifier
unknown	31030/udp	0.000654
unknown	31033/tcp	0.000076
unknown	31034/udp	0.001307
unknown	31036/udp	0.001307
unknown	31038/tcp	0.000380
unknown	31048/udp	0.000654
unknown	31049/udp	0.001307
unknown	31051/udp	0.001307
unknown	31052/udp	0.000654
unknown	31054/udp	0.000654
unknown	31058/tcp	0.000076
unknown	31058/udp	0.000654
unknown	31059/udp	0.001961
unknown	31068/udp	0.000654
unknown	31069/udp	0.000654
unknown	31072/tcp	0.000076
unknown	31072/udp	0.000654
unknown	31073/udp	0.002614
unknown	31076/udp	0.000654
unknown	31078/udp	0.000654
unknown	31080/udp	0.000654
unknown	31082/udp	0.001307
unknown	31083/udp	0.000654
unknown	31084/udp	0.001307
unknown	31085/udp	0.000654
unknown	31088/udp	0.000654
unknown	31089/udp	0.000654
unknown	31100/udp	0.000654
unknown	31105/udp	0.000654
unknown	31109/udp	0.001961
unknown	31112/udp	0.001307
unknown	31115/udp	0.001307
unknown	31119/udp	0.000654
unknown	31127/udp	0.000654
unknown	31129/udp	0.000654
unknown	31133/udp	0.001307
unknown	31134/udp	0.001307
unknown	31137/udp	0.001307
unknown	31141/udp	0.000654
unknown	31146/udp	0.000654
unknown	31150/udp	0.000654
unknown	31155/udp	0.001307
unknown	31162/udp	0.001307
unknown	31176/udp	0.000654
unknown	31180/udp	0.001307
unknown	31187/udp	0.000654
unknown	31189/udp	0.001961
unknown	31192/udp	0.000654
unknown	31195/udp	0.001961
unknown	31198/udp	0.000654
unknown	31199/udp	0.001307
unknown	31202/udp	0.001307
unknown	31204/udp	0.000654
unknown	31209/udp	0.000654
unknown	31211/udp	0.000654
unknown	31212/udp	0.000654
unknown	31215/udp	0.000654
unknown	31217/udp	0.000654
unknown	31218/udp	0.000654
unknown	31230/udp	0.000654
unknown	31234/udp	0.000654
unknown	31237/udp	0.000654
unknown	31238/udp	0.000654
unknown	31240/udp	0.000654
unknown	31242/udp	0.000654
unknown	31247/udp	0.000654
unknown	31248/udp	0.000654
unknown	31249/udp	0.000654
unknown	31252/udp	0.000654
unknown	31254/udp	0.000654
unknown	31257/udp	0.000654
unknown	31258/udp	0.000654
unknown	31261/udp	0.001307
unknown	31266/udp	0.001307
unknown	31267/udp	0.001307
unknown	31268/udp	0.000654
unknown	31271/udp	0.000654
unknown	31273/udp	0.000654
unknown	31275/udp	0.000654
unknown	31279/udp	0.000654
unknown	31284/udp	0.001307
unknown	31288/udp	0.000654
unknown	31292/udp	0.000654
unknown	31293/udp	0.000654
unknown	31299/udp	0.000654
unknown	31301/udp	0.000654
unknown	31309/udp	0.000654
unknown	31314/udp	0.000654
unknown	31318/udp	0.000654
unknown	31324/udp	0.000654
unknown	31325/udp	0.000654
unknown	31326/udp	0.000654
unknown	31333/udp	0.000654
unknown	31334/udp	0.001307
Trinoo_Register	31335/udp	0.001706	# Trinoo distributed attack tool Bcast Daemon registration port
unknown	31336/udp	0.000654
Elite	31337/tcp	0.000163	# eldim | Sometimes interesting stuff can be found here | eldim is a secure file upload proxy
BackOrifice	31337/udp	0.011469	# cDc Back Orifice remote admin tool
unknown	31339/tcp	0.000076
unknown	31340/udp	0.000654
unknown	31343/udp	0.001307
unknown	31347/udp	0.000654
unknown	31350/udp	0.001307
unknown	31352/udp	0.001307
unknown	31354/udp	0.000654
unknown	31358/udp	0.000654
unknown	31361/udp	0.001307
unknown	31362/udp	0.000654
unknown	31365/udp	0.001961
unknown	31366/udp	0.000654
unknown	31371/udp	0.000654
unknown	31386/tcp	0.000076
unknown	31386/udp	0.000654
unknown	31391/udp	0.000654
unknown	31392/udp	0.000654
unknown	31398/udp	0.000654
pace-licensed	31400/tcp	0.000000	# PACE license server
unknown	31404/udp	0.001307
unknown	31412/udp	0.001307
unknown	31414/udp	0.000654
unknown	31415/udp	0.000654
boinc	31416/tcp	0.000075	# xqosd | BOINC Client Control | XQoS network monitor
xqosd	31416/udp	0.000000	# XQoS network monitor
unknown	31421/udp	0.000654
unknown	31422/udp	0.000654
unknown	31423/udp	0.000654
unknown	31424/udp	0.000654
unknown	31428/udp	0.001307
unknown	31429/udp	0.000654
unknown	31432/udp	0.000654
unknown	31438/tcp	0.000076
unknown	31439/udp	0.000654
unknown	31451/udp	0.000654
unknown	31453/udp	0.000654
unknown	31454/udp	0.000654
tetrinet	31457/tcp	0.000000	# TetriNET Protocol
tetrinet	31457/udp	0.000000	# TetriNET Protocol
unknown	31459/udp	0.000654
unknown	31460/udp	0.000654
unknown	31470/udp	0.000654
unknown	31481/udp	0.001307
unknown	31487/udp	0.000654
unknown	31493/udp	0.000654
unknown	31495/udp	0.000654
unknown	31506/udp	0.000654
unknown	31509/udp	0.000654
unknown	31510/udp	0.000654
unknown	31518/udp	0.000654
unknown	31520/udp	0.001307
unknown	31521/udp	0.001307
unknown	31522/tcp	0.000076
unknown	31527/udp	0.000654
unknown	31532/udp	0.000654
unknown	31543/udp	0.000654
unknown	31544/udp	0.000654
unknown	31545/udp	0.000654
unknown	31548/udp	0.000654
unknown	31557/udp	0.000654
unknown	31558/udp	0.000654
unknown	31560/udp	0.001307
unknown	31563/udp	0.000654
unknown	31564/udp	0.000654
unknown	31565/udp	0.000654
unknown	31566/udp	0.000654
unknown	31569/udp	0.001307
unknown	31577/udp	0.000654
unknown	31579/udp	0.000654
unknown	31584/udp	0.001307
unknown	31593/udp	0.000654
unknown	31594/udp	0.000654
unknown	31595/udp	0.000654
unknown	31596/udp	0.000654
unknown	31597/udp	0.000654
unknown	31598/udp	0.000654
unknown	31599/udp	0.001307
unknown	31600/udp	0.000654
unknown	31601/udp	0.000654
unknown	31602/udp	0.001307
unknown	31606/udp	0.000654
unknown	31609/udp	0.001307
unknown	31615/udp	0.000654
unknown	31617/udp	0.000654
lm-mon	31620/tcp	0.000000	# lm mon
lm-mon	31620/udp	0.000000	# lm mon
unknown	31624/udp	0.000654
unknown	31625/udp	0.001961
unknown	31626/udp	0.000654
unknown	31643/udp	0.000654
unknown	31648/udp	0.000654
unknown	31651/udp	0.000654
unknown	31653/udp	0.000654
unknown	31655/udp	0.000654
unknown	31657/tcp	0.000076
unknown	31657/udp	0.000654
unknown	31660/udp	0.000654
unknown	31663/udp	0.000654
unknown	31668/udp	0.000654
unknown	31669/udp	0.000654
unknown	31670/udp	0.000654
unknown	31671/udp	0.000654
unknown	31673/udp	0.001307
unknown	31678/udp	0.000654
unknown	31679/udp	0.000654
unknown	31681/udp	0.002614
unknown	31683/udp	0.000654
dsx_monitor	31685/tcp	0.000000	# dsx-monitor | DS Expert Monitor
unknown	31692/udp	0.001307
unknown	31703/udp	0.000654
unknown	31705/udp	0.000654
unknown	31709/udp	0.000654
unknown	31712/udp	0.000654
unknown	31720/udp	0.001307
unknown	31723/udp	0.000654
diagd	31727/tcp	0.000152
unknown	31727/udp	0.000654
unknown	31728/tcp	0.000076
unknown	31729/udp	0.000654
unknown	31731/udp	0.001961
unknown	31732/udp	0.001307
unknown	31733/udp	0.000654
unknown	31735/udp	0.001307
unknown	31736/udp	0.000654
unknown	31737/udp	0.000654
unknown	31739/udp	0.000654
unknown	31743/udp	0.001307
unknown	31749/udp	0.000654
unknown	31750/udp	0.001307
unknown	31752/udp	0.000654
unknown	31757/udp	0.000654
unknown	31759/udp	0.000654
unknown	31763/udp	0.000654
gamesmith-port	31765/tcp	0.000000	# GameSmith Port
gamesmith-port	31765/udp	0.000000	# GameSmith Port
unknown	31776/udp	0.000654
unknown	31778/udp	0.000654
unknown	31779/udp	0.000654
unknown	31782/udp	0.000654
unknown	31783/udp	0.001307
unknown	31792/udp	0.001307
unknown	31794/udp	0.001307
unknown	31798/udp	0.000654
unknown	31803/udp	0.001307
unknown	31813/udp	0.000654
unknown	31817/udp	0.000654
unknown	31818/udp	0.000654
unknown	31819/udp	0.000654
unknown	31821/udp	0.000654
unknown	31822/udp	0.000654
unknown	31825/udp	0.000654
unknown	31827/udp	0.000654
unknown	31833/udp	0.000654
unknown	31834/udp	0.000654
unknown	31842/udp	0.000654
unknown	31844/udp	0.000654
unknown	31847/udp	0.000654
unknown	31852/udp	0.001307
unknown	31853/udp	0.000654
unknown	31854/udp	0.000654
unknown	31861/udp	0.000654
unknown	31869/udp	0.000654
unknown	31870/udp	0.000654
unknown	31872/udp	0.000654
unknown	31877/udp	0.000654
unknown	31878/udp	0.000654
unknown	31882/udp	0.001307
unknown	31887/udp	0.001307
unknown	31891/udp	0.002614
unknown	31892/udp	0.000654
unknown	31894/udp	0.000654
unknown	31898/udp	0.000654
unknown	31899/udp	0.000654
unknown	31901/udp	0.000654
unknown	31906/udp	0.000654
unknown	31918/udp	0.001307
unknown	31920/udp	0.000654
unknown	31921/udp	0.000654
unknown	31922/udp	0.000654
unknown	31928/udp	0.000654
unknown	31929/udp	0.000654
unknown	31934/udp	0.000654
unknown	31939/udp	0.000654
unknown	31940/udp	0.000654
iceedcp_tx	31948/tcp	0.000000	# iceedcp-tx | Embedded Device Configuration Protocol TX
iceedcp_tx	31948/udp	0.000000	# Embedded Device Configuration Protocol TX
iceedcp_rx	31949/tcp	0.000000	# iceedcp-rx | Embedded Device Configuration Protocol RX
iceedcp_rx	31949/udp	0.000000	# Embedded Device Configuration Protocol RX
unknown	31950/udp	0.000654
unknown	31963/udp	0.001307
unknown	31966/udp	0.000654
unknown	31967/udp	0.000654
unknown	31968/udp	0.000654
unknown	31972/udp	0.000654
unknown	31974/udp	0.000654
unknown	31979/udp	0.000654
unknown	31981/udp	0.000654
unknown	31992/udp	0.000654
unknown	31997/udp	0.000654
unknown	31999/udp	0.001307
unknown	32005/udp	0.000654
unknown	32006/tcp	0.000076
unknown	32006/udp	0.000654
unknown	32007/udp	0.000654
unknown	32010/udp	0.000654
unknown	32011/udp	0.000654
unknown	32018/udp	0.000654
unknown	32022/tcp	0.000076
unknown	32024/udp	0.000654
unknown	32025/udp	0.000654
unknown	32031/tcp	0.000076
unknown	32033/udp	0.000654
iracinghelper	32034/tcp	0.000000	# iRacing helper service
iracinghelper	32034/udp	0.000000	# iRacing helper service
unknown	32035/udp	0.000654
unknown	32039/udp	0.000654
unknown	32040/udp	0.000654
unknown	32044/udp	0.001307
unknown	32046/udp	0.000654
unknown	32048/udp	0.000654
unknown	32053/udp	0.001307
unknown	32059/udp	0.000654
unknown	32064/udp	0.000654
unknown	32065/udp	0.000654
unknown	32066/udp	0.001307
unknown	32068/udp	0.000654
unknown	32072/udp	0.000654
unknown	32079/udp	0.000654
unknown	32081/udp	0.000654
unknown	32084/udp	0.000654
unknown	32088/tcp	0.000076
unknown	32090/udp	0.000654
unknown	32091/udp	0.000654
unknown	32092/udp	0.000654
unknown	32094/udp	0.000654
unknown	32102/tcp	0.000076
unknown	32105/udp	0.000654
unknown	32106/udp	0.000654
unknown	32107/udp	0.000654
unknown	32109/udp	0.000654
unknown	32117/udp	0.000654
unknown	32124/udp	0.001307
unknown	32127/udp	0.000654
unknown	32129/udp	0.001307
unknown	32132/udp	0.001307
unknown	32161/udp	0.000654
unknown	32162/udp	0.000654
unknown	32163/udp	0.000654
unknown	32167/udp	0.000654
unknown	32172/udp	0.000654
unknown	32174/udp	0.000654
unknown	32176/udp	0.000654
unknown	32178/udp	0.000654
unknown	32180/udp	0.000654
unknown	32185/udp	0.001307
unknown	32186/udp	0.000654
unknown	32187/udp	0.000654
unknown	32188/udp	0.000654
unknown	32190/udp	0.000654
unknown	32195/udp	0.000654
unknown	32198/udp	0.000654
unknown	32200/tcp	0.000076
unknown	32201/udp	0.000654
unknown	32202/udp	0.000654
unknown	32204/udp	0.000654
unknown	32210/udp	0.000654
unknown	32216/udp	0.001307
unknown	32217/udp	0.000654
unknown	32219/tcp	0.000076
unknown	32219/udp	0.001307
unknown	32221/udp	0.000654
unknown	32222/udp	0.000654
unknown	32223/udp	0.000654
unknown	32225/udp	0.000654
unknown	32228/udp	0.000654
unknown	32231/udp	0.000654
unknown	32245/udp	0.000654
unknown	32248/udp	0.000654
t1distproc60	32249/tcp	0.000000	# T1 Distributed Processor
t1distproc60	32249/udp	0.000000	# T1 Distributed Processor
unknown	32251/udp	0.000654
unknown	32259/udp	0.000654
unknown	32260/tcp	0.000076
unknown	32261/tcp	0.000076
unknown	32262/udp	0.001307
unknown	32264/udp	0.000654
unknown	32268/udp	0.000654
unknown	32270/udp	0.000654
unknown	32272/udp	0.000654
unknown	32273/udp	0.001307
unknown	32274/udp	0.000654
unknown	32276/udp	0.000654
unknown	32277/udp	0.000654
unknown	32281/udp	0.000654
unknown	32282/udp	0.000654
unknown	32289/udp	0.000654
unknown	32291/udp	0.000654
unknown	32295/udp	0.000654
unknown	32297/udp	0.000654
unknown	32305/udp	0.000654
unknown	32306/udp	0.000654
unknown	32309/udp	0.000654
unknown	32313/udp	0.000654
unknown	32316/udp	0.000654
unknown	32317/udp	0.000654
unknown	32319/udp	0.000654
unknown	32323/udp	0.000654
unknown	32326/udp	0.001307
unknown	32329/udp	0.000654
unknown	32338/udp	0.000654
unknown	32339/udp	0.000654
unknown	32342/udp	0.000654
unknown	32345/udp	0.001961
unknown	32349/udp	0.000654
unknown	32352/udp	0.001307
unknown	32355/udp	0.000654
unknown	32359/udp	0.001307
unknown	32360/udp	0.000654
unknown	32364/udp	0.000654
unknown	32368/udp	0.001307
unknown	32369/udp	0.000654
unknown	32377/udp	0.000654
unknown	32378/udp	0.000654
unknown	32379/udp	0.000654
unknown	32382/udp	0.001307
unknown	32385/udp	0.001961
unknown	32389/udp	0.000654
unknown	32391/udp	0.000654
unknown	32398/udp	0.000654
plex	32400/tcp	0.000000	# Plex multimedia
unknown	32404/udp	0.001307
unknown	32406/udp	0.000654
unknown	32409/udp	0.000654
unknown	32412/udp	0.000654
unknown	32415/udp	0.001307
unknown	32422/udp	0.001307
unknown	32423/udp	0.000654
unknown	32425/udp	0.001307
unknown	32426/udp	0.000654
unknown	32428/udp	0.000654
unknown	32429/udp	0.000654
unknown	32430/udp	0.001307
unknown	32433/udp	0.000654
unknown	32435/udp	0.000654
unknown	32436/udp	0.000654
unknown	32439/udp	0.000654
unknown	32440/udp	0.000654
unknown	32444/udp	0.000654
unknown	32446/udp	0.001307
unknown	32447/udp	0.000654
unknown	32449/udp	0.000654
unknown	32454/udp	0.000654
unknown	32465/udp	0.000654
unknown	32466/udp	0.000654
unknown	32468/udp	0.000654
unknown	32469/udp	0.001307
unknown	32473/udp	0.000654
unknown	32474/udp	0.000654
unknown	32478/udp	0.000654
unknown	32479/udp	0.001307
unknown	32482/udp	0.000654
apm-link	32483/tcp	0.000000	# Access Point Manager Link
apm-link	32483/udp	0.000654	# Access Point Manager Link
unknown	32484/udp	0.000654
unknown	32487/udp	0.000654
unknown	32488/udp	0.000654
unknown	32495/udp	0.001307
unknown	32496/udp	0.000654
unknown	32499/udp	0.001307
unknown	32503/udp	0.000654
unknown	32506/udp	0.001307
unknown	32508/udp	0.000654
unknown	32511/udp	0.000654
unknown	32512/udp	0.000654
unknown	32518/udp	0.000654
unknown	32523/udp	0.000654
unknown	32524/udp	0.000654
unknown	32528/udp	0.001961
unknown	32532/udp	0.000654
unknown	32546/udp	0.001307
unknown	32550/udp	0.000654
unknown	32553/udp	0.000654
unknown	32558/udp	0.000654
unknown	32560/udp	0.000654
unknown	32564/udp	0.000654
unknown	32566/udp	0.000654
unknown	32571/udp	0.000654
unknown	32574/udp	0.000654
unknown	32575/udp	0.000654
unknown	32576/udp	0.000654
unknown	32577/udp	0.000654
unknown	32578/udp	0.000654
unknown	32583/udp	0.000654
unknown	32592/udp	0.000654
unknown	32595/udp	0.000654
unknown	32597/udp	0.000654
unknown	32598/udp	0.000654
unknown	32607/udp	0.001307
unknown	32611/udp	0.001307
unknown	32612/udp	0.000654
unknown	32617/udp	0.000654
unknown	32618/udp	0.000654
unknown	32629/udp	0.000654
unknown	32631/udp	0.000654
unknown	32632/udp	0.000654
unknown	32634/udp	0.000654
sec-ntb-clnt	32635/tcp	0.000000	# SecureNotebook-CLNT
sec-ntb-clnt	32635/udp	0.000000	# SecureNotebook-CLNT
DMExpress	32636/tcp	0.000000
DMExpress	32636/udp	0.000000
unknown	32637/udp	0.000654
unknown	32639/udp	0.000654
unknown	32641/udp	0.000654
unknown	32642/udp	0.000654
unknown	32644/udp	0.000654
unknown	32652/udp	0.000654
unknown	32656/udp	0.000654
unknown	32664/udp	0.000654
unknown	32669/udp	0.000654
unknown	32674/udp	0.000654
unknown	32675/udp	0.000654
unknown	32676/udp	0.000654
unknown	32682/udp	0.000654
unknown	32685/udp	0.000654
unknown	32687/udp	0.000654
unknown	32693/udp	0.000654
unknown	32706/udp	0.000654
unknown	32714/udp	0.000654
unknown	32723/udp	0.000654
unknown	32727/udp	0.001307
unknown	32731/udp	0.000654
unknown	32734/udp	0.000654
unknown	32736/udp	0.000654
unknown	32742/udp	0.000654
unknown	32743/udp	0.000654
unknown	32744/udp	0.000654
unknown	32748/udp	0.000654
unknown	32750/udp	0.001307
unknown	32760/udp	0.001307
unknown	32764/tcp	0.000076
unknown	32765/tcp	0.000076
filenet-powsrm	32767/tcp	0.000076	# FileNet BPM WS-ReliableMessaging Client
filenet-powsrm	32767/udp	0.000000	# FileNet BPM WS-ReliableMessaging Client
filenet-tms	32768/tcp	0.009199	# Filenet TMS
omad	32768/udp	0.044407	# OpenMosix Autodiscovery Daemon
filenet-rpc	32769/tcp	0.000760	# Filenet RPC
filenet-rpc	32769/udp	0.007768	# Filenet RPC
sometimes-rpc3	32770/tcp	0.000903	# filenet-nch | Sometimes an RPC port on my Solaris box | Filenet NCH
sometimes-rpc4	32770/udp	0.006745	# Sometimes an RPC port on my Solaris box
sometimes-rpc5	32771/tcp	0.001367	# filenet-rmi | Sometimes an RPC port on my Solaris box (rusersd) | FileNET RMI | FileNet RMI
sometimes-rpc6	32771/udp	0.008490	# Sometimes an RPC port on my Solaris box (rusersd)
sometimes-rpc7	32772/tcp	0.000891	# filenet-pa | Sometimes an RPC port on my Solaris box (status) | FileNET Process Analyzer
sometimes-rpc8	32772/udp	0.005352	# Sometimes an RPC port on my Solaris box (status)
sometimes-rpc9	32773/tcp	0.000602	# filenet-cm | Sometimes an RPC port on my Solaris box (rquotad) | FileNET Component Manager
sometimes-rpc10	32773/udp	0.003238	# Sometimes an RPC port on my Solaris box (rquotad)
sometimes-rpc11	32774/tcp	0.000602	# filenet-re | Sometimes an RPC port on my Solaris box (rusersd) | FileNET Rules Engine
sometimes-rpc12	32774/udp	0.002819	# Sometimes an RPC port on my Solaris box (rusersd)
sometimes-rpc13	32775/tcp	0.000427	# filenet-pch | Sometimes an RPC port on my Solaris box (status) | Performance Clearinghouse
sometimes-rpc14	32775/udp	0.002668	# Sometimes an RPC port on my Solaris box (status)
sometimes-rpc15	32776/tcp	0.000364	# filenet-peior | Sometimes an RPC port on my Solaris box (sprayd) | FileNET BPM IOR
sometimes-rpc16	32776/udp	0.002013	# Sometimes an RPC port on my Solaris box (sprayd)
sometimes-rpc17	32777/tcp	0.000301	# filenet-obrok | Sometimes an RPC port on my Solaris box (walld) | FileNet BPM CORBA
sometimes-rpc18	32777/udp	0.002282	# Sometimes an RPC port on my Solaris box (walld)
sometimes-rpc19	32778/tcp	0.000289	# Sometimes an RPC port on my Solaris box (rstatd)
sometimes-rpc20	32778/udp	0.001577	# Sometimes an RPC port on my Solaris box (rstatd)
sometimes-rpc21	32779/tcp	0.000301	# Sometimes an RPC port on my Solaris box
sometimes-rpc22	32779/udp	0.002584	# Sometimes an RPC port on my Solaris box
sometimes-rpc23	32780/tcp	0.000263	# Sometimes an RPC port on my Solaris box
sometimes-rpc24	32780/udp	0.001812	# Sometimes an RPC port on my Solaris box
unknown	32781/tcp	0.000380
unknown	32782/tcp	0.000380
unknown	32783/tcp	0.000228
unknown	32784/tcp	0.000304
unknown	32785/tcp	0.000228
sometimes-rpc25	32786/tcp	0.000075	# Sometimes an RPC port (mountd)
sometimes-rpc26	32786/udp	0.001191	# Sometimes an RPC port
sometimes-rpc27	32787/tcp	0.000075	# Sometimes an RPC port dmispd (DMI Service Provider)
sometimes-rpc28	32787/udp	0.000956	# Sometimes an RPC port
unknown	32788/tcp	0.000076
unknown	32789/tcp	0.000076
unknown	32789/udp	0.000518
unknown	32790/tcp	0.000076
unknown	32790/udp	0.000518
unknown	32791/tcp	0.000152
unknown	32792/tcp	0.000152
unknown	32792/udp	0.000518
unknown	32793/udp	0.000518
unknown	32796/udp	0.000518
unknown	32797/tcp	0.000076
unknown	32798/tcp	0.000076
unknown	32798/udp	0.001554
unknown	32799/tcp	0.000076
unknown	32800/udp	0.000518
mlsn	32801/tcp	0.000000	# Multiple Listing Service Network
mlsn	32801/udp	0.000000	# Multiple Listing Service Network
unknown	32803/tcp	0.000152
unknown	32803/udp	0.000518
unknown	32804/udp	0.000518
unknown	32807/tcp	0.000076
unknown	32808/udp	0.000518
unknown	32809/udp	0.000518
retp	32811/tcp	0.000000	# Real Estate Transport Protocol
unknown	32811/udp	0.000518
unknown	32812/udp	0.001036
unknown	32813/udp	0.000518
unknown	32814/tcp	0.000076
unknown	32814/udp	0.000518
unknown	32815/tcp	0.000076
unknown	32815/udp	0.009322
unknown	32816/tcp	0.000152
unknown	32817/udp	0.000518
unknown	32818/udp	0.002071
unknown	32820/tcp	0.000076
unknown	32820/udp	0.001036
unknown	32821/udp	0.000518
unknown	32822/tcp	0.000152
unknown	32824/udp	0.000518
unknown	32835/tcp	0.000152
unknown	32837/tcp	0.000076
unknown	32841/udp	0.000518
unknown	32842/tcp	0.000076
unknown	32843/udp	0.001036
unknown	32847/udp	0.001036
unknown	32850/udp	0.000518
unknown	32854/udp	0.000518
unknown	32858/tcp	0.000076
unknown	32863/udp	0.000518
unknown	32868/tcp	0.000076
unknown	32869/tcp	0.000076
unknown	32871/tcp	0.000076
unknown	32871/udp	0.000518
unknown	32875/udp	0.000518
unknown	32878/udp	0.000518
unknown	32880/udp	0.000518
unknown	32886/udp	0.000518
unknown	32888/tcp	0.000076
unknown	32890/udp	0.000518
idmgratm	32896/tcp	0.000000	# Attachmate ID Manager
idmgratm	32896/udp	0.000518	# Attachmate ID Manager
unknown	32897/tcp	0.000076
unknown	32897/udp	0.001036
unknown	32898/tcp	0.000076
unknown	32899/udp	0.000518
unknown	32904/tcp	0.000076
unknown	32905/tcp	0.000076
unknown	32905/udp	0.000518
unknown	32908/tcp	0.000076
unknown	32908/udp	0.000518
unknown	32910/tcp	0.000076
unknown	32910/udp	0.000518
unknown	32911/tcp	0.000076
unknown	32915/udp	0.000518
unknown	32923/udp	0.000518
unknown	32931/udp	0.002071
unknown	32932/tcp	0.000076
unknown	32942/udp	0.000518
unknown	32944/tcp	0.000076
unknown	32951/udp	0.000518
unknown	32955/udp	0.001036
unknown	32956/udp	0.000518
unknown	32958/udp	0.000518
unknown	32960/tcp	0.000076
unknown	32961/tcp	0.000076
unknown	32964/udp	0.000518
unknown	32975/udp	0.000518
unknown	32976/tcp	0.000076
unknown	32976/udp	0.000518
unknown	32978/udp	0.000518
unknown	32993/udp	0.000518
unknown	32996/udp	0.000518
wg-endpt-comms	33000/tcp	0.000076	# WatchGuard Endpoint Communications
unknown	33008/udp	0.000518
unknown	33009/udp	0.000518
unknown	33011/tcp	0.000076
unknown	33011/udp	0.000518
unknown	33017/tcp	0.000076
unknown	33023/udp	0.000518
unknown	33024/udp	0.000518
unknown	33025/udp	0.000518
unknown	33027/udp	0.000518
unknown	33028/udp	0.001036
unknown	33029/udp	0.000518
unknown	33030/udp	0.001554
unknown	33035/udp	0.000518
unknown	33043/udp	0.001036
unknown	33046/udp	0.000518
unknown	33051/udp	0.000518
mysqlx	33060/tcp	0.000000	# MySQL Database Extended Interface
unknown	33065/udp	0.000518
unknown	33070/tcp	0.000076
unknown	33070/udp	0.000518
unknown	33073/udp	0.000518
unknown	33076/udp	0.000518
unknown	33080/udp	0.001036
unknown	33087/tcp	0.000076
unknown	33090/udp	0.000518
unknown	33104/udp	0.000518
unknown	33107/udp	0.000518
unknown	33116/udp	0.000518
unknown	33122/udp	0.000518
aurora-balaena	33123/tcp	0.000000	# Aurora (Balaena Ltd)
aurora-balaena	33123/udp	0.000000	# Aurora (Balaena Ltd)
unknown	33124/tcp	0.000076
unknown	33126/udp	0.000518
unknown	33144/udp	0.001036
unknown	33145/udp	0.000518
unknown	33147/udp	0.000518
unknown	33149/udp	0.001036
unknown	33156/udp	0.001036
unknown	33162/udp	0.001036
unknown	33175/tcp	0.000076
unknown	33183/udp	0.000518
unknown	33187/udp	0.000518
unknown	33188/udp	0.000518
unknown	33192/tcp	0.000076
unknown	33192/udp	0.000518
unknown	33200/tcp	0.000076
unknown	33201/udp	0.000518
unknown	33203/tcp	0.000076
unknown	33203/udp	0.000518
unknown	33206/udp	0.000518
unknown	33207/udp	0.001036
unknown	33208/udp	0.001036
unknown	33214/udp	0.000518
unknown	33216/udp	0.000518
unknown	33217/udp	0.000518
unknown	33221/udp	0.000518
unknown	33223/udp	0.000518
unknown	33228/udp	0.000518
unknown	33230/udp	0.000518
unknown	33231/udp	0.000518
unknown	33238/udp	0.000518
unknown	33240/udp	0.000518
unknown	33241/udp	0.000518
unknown	33248/udp	0.000518
unknown	33249/udp	0.001554
unknown	33264/udp	0.001036
unknown	33270/udp	0.000518
unknown	33272/udp	0.000518
unknown	33274/udp	0.000518
unknown	33277/tcp	0.000076
unknown	33279/udp	0.000518
unknown	33281/udp	0.008286
unknown	33283/udp	0.000518
unknown	33285/udp	0.001036
unknown	33287/udp	0.000518
unknown	33290/udp	0.001036
unknown	33298/udp	0.000518
unknown	33299/udp	0.000518
unknown	33302/udp	0.001036
unknown	33308/udp	0.000518
unknown	33311/udp	0.000518
unknown	33319/udp	0.000518
unknown	33320/udp	0.000518
unknown	33327/tcp	0.000076
unknown	33329/udp	0.000518
diamondport	33331/tcp	0.000000	# DiamondCentral Interface
diamondport	33331/udp	0.000000	# DiamondCentral Interface
dgi-serv	33333/tcp	0.000000	# Digital Gaslight Service
unknown	33333/udp	0.000518
speedtrace	33334/tcp	0.000000	# speedtrace-disc | SpeedTrace TraceAgent | SpeedTrace TraceAgent Discovery
unknown	33334/udp	0.000518
unknown	33335/tcp	0.000076
unknown	33336/udp	0.000518
unknown	33337/tcp	0.000076
unknown	33345/udp	0.000518
unknown	33348/udp	0.000518
unknown	33353/udp	0.000518
unknown	33354/tcp	0.000760
unknown	33354/udp	0.005179
unknown	33355/udp	0.002589
unknown	33356/udp	0.000518
unknown	33357/udp	0.000518
unknown	33364/udp	0.000518
unknown	33367/tcp	0.000076
unknown	33377/udp	0.001036
unknown	33379/udp	0.000518
unknown	33381/udp	0.000518
unknown	33386/udp	0.000518
unknown	33389/udp	0.000518
unknown	33394/udp	0.001036
unknown	33395/tcp	0.000076
unknown	33395/udp	0.000518
unknown	33397/udp	0.000518
unknown	33402/udp	0.000518
unknown	33407/udp	0.000518
unknown	33414/udp	0.001036
unknown	33418/udp	0.000518
unknown	33419/udp	0.000518
unknown	33422/udp	0.001036
unknown	33427/udp	0.000518
unknown	33429/udp	0.000518
unknown	33430/udp	0.000518
traceroute	33434/tcp	0.000000	# traceroute use
traceroute	33434/udp	0.000000	# traceroute use
mtrace	33435/tcp	0.000000	# IP Multicast Traceroute
unknown	33435/udp	0.000518
unknown	33443/udp	0.000518
unknown	33444/tcp	0.000076
unknown	33448/udp	0.001036
unknown	33453/tcp	0.000152
unknown	33456/udp	0.000518
unknown	33459/udp	0.001554
unknown	33460/udp	0.000518
unknown	33464/udp	0.000518
unknown	33465/udp	0.001036
unknown	33468/udp	0.000518
unknown	33472/udp	0.000518
unknown	33481/udp	0.000518
unknown	33483/udp	0.000518
unknown	33485/udp	0.000518
unknown	33497/udp	0.000518
unknown	33510/udp	0.000518
unknown	33513/udp	0.000518
unknown	33514/udp	0.000518
unknown	33517/udp	0.000518
unknown	33521/udp	0.000518
unknown	33522/tcp	0.000076
unknown	33523/tcp	0.000076
unknown	33528/udp	0.000518
unknown	33532/udp	0.000518
unknown	33534/udp	0.000518
unknown	33535/udp	0.000518
unknown	33540/udp	0.000518
unknown	33546/udp	0.000518
unknown	33550/tcp	0.000076
unknown	33550/udp	0.000518
unknown	33554/tcp	0.000152
unknown	33556/udp	0.001036
unknown	33558/udp	0.000518
unknown	33559/udp	0.000518
unknown	33562/udp	0.000518
unknown	33564/udp	0.000518
unknown	33575/udp	0.001036
unknown	33578/udp	0.000518
unknown	33581/udp	0.000518
unknown	33584/udp	0.001036
unknown	33586/udp	0.000518
unknown	33591/udp	0.001036
unknown	33593/udp	0.000518
unknown	33598/udp	0.000518
unknown	33599/udp	0.000518
unknown	33604/tcp	0.000076
unknown	33605/tcp	0.000076
unknown	33606/udp	0.000518
unknown	33635/udp	0.000518
unknown	33636/udp	0.000518
unknown	33641/udp	0.000518
unknown	33651/udp	0.000518
unknown	33652/udp	0.001036
unknown	33653/udp	0.000518
snip	33656/tcp	0.000000	# snip-slave | SNIP Slave
snip	33656/udp	0.000000
unknown	33671/udp	0.000518
unknown	33687/udp	0.001036
unknown	33691/udp	0.000518
unknown	33693/udp	0.001036
unknown	33699/udp	0.000518
unknown	33700/udp	0.001036
unknown	33702/udp	0.000518
unknown	33709/udp	0.000518
unknown	33710/udp	0.001036
unknown	33717/udp	0.001554
unknown	33722/udp	0.000518
unknown	33724/udp	0.001036
unknown	33726/udp	0.000518
unknown	33734/udp	0.000518
unknown	33744/udp	0.002071
unknown	33745/udp	0.000518
unknown	33753/udp	0.000518
unknown	33755/udp	0.000518
unknown	33761/udp	0.000518
unknown	33773/udp	0.000518
unknown	33774/udp	0.000518
unknown	33775/udp	0.000518
unknown	33776/udp	0.000518
unknown	33781/udp	0.000518
unknown	33782/udp	0.000518
unknown	33790/udp	0.000518
unknown	33795/udp	0.001036
unknown	33804/udp	0.000518
unknown	33813/udp	0.000518
unknown	33814/udp	0.000518
unknown	33821/udp	0.000518
unknown	33826/udp	0.001036
unknown	33832/udp	0.000518
unknown	33836/udp	0.000518
unknown	33837/udp	0.000518
unknown	33838/udp	0.000518
unknown	33841/tcp	0.000076
unknown	33843/udp	0.000518
unknown	33844/udp	0.000518
unknown	33845/udp	0.000518
unknown	33848/udp	0.000518
unknown	33849/udp	0.001036
unknown	33852/udp	0.000518
unknown	33858/udp	0.001036
unknown	33866/udp	0.001554
unknown	33871/udp	0.000518
unknown	33872/udp	0.001554
unknown	33873/udp	0.001036
unknown	33878/udp	0.001036
unknown	33879/tcp	0.000076
unknown	33879/udp	0.000518
unknown	33882/tcp	0.000076
unknown	33882/udp	0.001036
unknown	33889/tcp	0.000076
digilent-adept	33890/tcp	0.000000	# Adept IP protocol
unknown	33891/udp	0.000518
unknown	33892/udp	0.000518
unknown	33895/tcp	0.000076
unknown	33897/udp	0.000518
unknown	33898/udp	0.000518
unknown	33899/tcp	0.000380
unknown	33900/udp	0.000518
unknown	33902/udp	0.000518
unknown	33905/udp	0.000518
unknown	33906/udp	0.000518
unknown	33907/udp	0.000518
unknown	33908/udp	0.000518
unknown	33915/udp	0.000518
unknown	33916/udp	0.000518
unknown	33924/udp	0.000518
unknown	33933/udp	0.000518
unknown	33935/udp	0.000518
unknown	33962/udp	0.000518
unknown	33967/udp	0.000518
unknown	33968/udp	0.000518
unknown	33972/udp	0.000518
unknown	33973/udp	0.000518
unknown	33975/udp	0.001036
unknown	33979/udp	0.000518
unknown	33986/udp	0.001036
unknown	33987/udp	0.000518
unknown	33991/udp	0.000518
unknown	34012/udp	0.000518
unknown	34016/udp	0.000518
unknown	34021/tcp	0.000076
unknown	34021/udp	0.000518
unknown	34025/udp	0.000518
unknown	34031/udp	0.000518
unknown	34035/udp	0.000518
unknown	34036/tcp	0.000076
unknown	34038/udp	0.001554
unknown	34041/udp	0.000518
unknown	34044/udp	0.000518
unknown	34045/udp	0.000518
unknown	34047/udp	0.000518
unknown	34050/udp	0.000518
unknown	34052/udp	0.000518
unknown	34053/udp	0.000518
unknown	34060/udp	0.000518
unknown	34066/udp	0.000518
unknown	34069/udp	0.000518
unknown	34075/udp	0.001036
unknown	34079/udp	0.001554
unknown	34082/udp	0.001036
unknown	34084/udp	0.000518
unknown	34085/udp	0.000518
unknown	34090/udp	0.000518
unknown	34096/tcp	0.000076
unknown	34108/udp	0.000518
unknown	34111/udp	0.000518
unknown	34119/udp	0.001036
unknown	34125/udp	0.002071
unknown	34133/udp	0.001036
unknown	34136/udp	0.000518
unknown	34140/udp	0.000518
unknown	34153/udp	0.001036
unknown	34154/udp	0.000518
unknown	34156/udp	0.000518
unknown	34157/udp	0.001036
unknown	34167/udp	0.000518
unknown	34168/udp	0.000518
unknown	34172/udp	0.000518
unknown	34174/udp	0.000518
unknown	34178/udp	0.000518
unknown	34181/udp	0.000518
unknown	34182/udp	0.000518
unknown	34189/tcp	0.000076
unknown	34189/udp	0.000518
unknown	34197/udp	0.000518
unknown	34198/udp	0.000518
unknown	34204/udp	0.000518
unknown	34206/udp	0.000518
unknown	34209/udp	0.000518
unknown	34210/udp	0.000518
unknown	34214/udp	0.001036
unknown	34225/udp	0.000518
unknown	34227/udp	0.001036
unknown	34231/udp	0.001036
unknown	34235/udp	0.000518
unknown	34236/udp	0.000518
unknown	34242/udp	0.000518
unknown	34243/udp	0.001036
unknown	34245/udp	0.000518
turbonote-2	34249/tcp	0.000000	# TurboNote Relay Server Default Port
turbonote-2	34249/udp	0.000000	# TurboNote Relay Server Default Port
unknown	34250/udp	0.001036
unknown	34251/udp	0.000518
unknown	34253/udp	0.001036
unknown	34266/udp	0.000518
unknown	34268/udp	0.000518
unknown	34278/udp	0.000518
unknown	34279/udp	0.000518
unknown	34280/udp	0.000518
unknown	34282/udp	0.000518
unknown	34283/udp	0.000518
unknown	34284/udp	0.000518
unknown	34290/udp	0.000518
unknown	34295/udp	0.000518
unknown	34299/udp	0.000518
unknown	34306/udp	0.000518
unknown	34311/udp	0.000518
unknown	34315/udp	0.000518
unknown	34317/tcp	0.000076
unknown	34318/udp	0.000518
unknown	34319/udp	0.000518
unknown	34325/udp	0.000518
unknown	34326/udp	0.000518
unknown	34327/udp	0.000518
unknown	34335/udp	0.000518
unknown	34337/udp	0.000518
unknown	34338/udp	0.000518
unknown	34341/tcp	0.000076
unknown	34345/udp	0.000518
unknown	34349/udp	0.000518
unknown	34353/udp	0.000518
unknown	34358/udp	0.001554
unknown	34363/udp	0.000518
unknown	34366/udp	0.000518
unknown	34374/udp	0.001036
unknown	34375/udp	0.000518
unknown	34377/udp	0.000518
p-net-local	34378/tcp	0.000000	# P-Net on IP local
p-net-local	34378/udp	0.000000	# P-Net on IP local
p-net-remote	34379/tcp	0.000000	# P-Net on IP remote
p-net-remote	34379/udp	0.000000	# P-Net on IP remote
unknown	34381/tcp	0.000076
unknown	34381/udp	0.000518
unknown	34384/udp	0.000518
unknown	34394/udp	0.000518
unknown	34397/udp	0.000518
unknown	34400/udp	0.000518
unknown	34401/tcp	0.000076
unknown	34417/udp	0.001036
unknown	34419/udp	0.000518
unknown	34421/udp	0.001036
unknown	34422/udp	0.001554
unknown	34423/udp	0.000518
unknown	34425/udp	0.001036
unknown	34427/udp	0.000518
unknown	34433/udp	0.001554
unknown	34444/udp	0.000518
unknown	34449/udp	0.000518
unknown	34454/udp	0.000518
unknown	34455/udp	0.000518
unknown	34456/udp	0.000518
unknown	34460/udp	0.000518
unknown	34462/udp	0.000518
unknown	34464/udp	0.000518
unknown	34471/udp	0.000518
unknown	34472/udp	0.000518
unknown	34479/udp	0.000518
unknown	34484/udp	0.000518
unknown	34485/udp	0.000518
unknown	34487/udp	0.000518
unknown	34492/udp	0.000518
unknown	34496/udp	0.000518
unknown	34499/udp	0.000518
unknown	34503/udp	0.000518
unknown	34507/tcp	0.000076
unknown	34509/udp	0.000518
unknown	34510/tcp	0.000076
unknown	34511/udp	0.000518
unknown	34515/udp	0.000518
unknown	34516/udp	0.000518
unknown	34520/udp	0.000518
unknown	34522/udp	0.000518
unknown	34530/udp	0.000518
unknown	34539/udp	0.000518
unknown	34542/udp	0.000518
unknown	34547/udp	0.000518
unknown	34553/udp	0.000518
unknown	34555/udp	0.006732
unknown	34557/udp	0.000518
unknown	34560/udp	0.000518
unknown	34561/udp	0.000518
dhanalakshmi	34567/tcp	0.000000	# edi_service | dhanalakshmi.org EDI Service
unknown	34570/udp	0.001554
unknown	34571/tcp	0.000380
unknown	34571/udp	0.000518
unknown	34572/tcp	0.000380
unknown	34572/udp	0.000518
unknown	34573/tcp	0.000380
unknown	34574/udp	0.000518
unknown	34577/udp	0.001554
unknown	34578/udp	0.001554
unknown	34579/udp	0.001554
unknown	34580/udp	0.001554
unknown	34584/udp	0.000518
unknown	34586/udp	0.001036
unknown	34592/udp	0.000518
unknown	34611/udp	0.000518
unknown	34616/udp	0.000518
unknown	34623/udp	0.000518
unknown	34631/udp	0.000518
unknown	34632/udp	0.000518
unknown	34641/udp	0.000518
unknown	34642/udp	0.000518
unknown	34645/udp	0.000518
unknown	34652/udp	0.000518
unknown	34653/udp	0.001036
unknown	34657/udp	0.000518
unknown	34683/tcp	0.000076
unknown	34686/udp	0.000518
unknown	34688/udp	0.000518
unknown	34692/udp	0.001036
unknown	34701/udp	0.000518
unknown	34705/udp	0.001036
unknown	34717/udp	0.000518
unknown	34720/udp	0.000518
unknown	34722/udp	0.000518
unknown	34728/tcp	0.000076
unknown	34730/udp	0.000518
unknown	34732/udp	0.000518
unknown	34735/udp	0.000518
unknown	34747/udp	0.000518
unknown	34752/udp	0.000518
unknown	34757/udp	0.001036
unknown	34758/udp	0.001554
unknown	34763/udp	0.000518
unknown	34765/tcp	0.000076
unknown	34770/udp	0.001036
unknown	34771/udp	0.001036
unknown	34779/udp	0.000518
unknown	34780/udp	0.001036
unknown	34781/udp	0.000518
unknown	34782/udp	0.000518
unknown	34783/tcp	0.000076
unknown	34786/udp	0.000518
unknown	34788/udp	0.000518
unknown	34796/udp	0.001554
unknown	34797/udp	0.000518
unknown	34805/udp	0.000518
unknown	34811/udp	0.000518
unknown	34817/udp	0.000518
unknown	34821/udp	0.000518
unknown	34822/udp	0.001036
unknown	34826/udp	0.000518
unknown	34833/tcp	0.000076
unknown	34838/udp	0.000518
unknown	34841/udp	0.000518
unknown	34844/udp	0.000518
unknown	34847/udp	0.001036
unknown	34855/udp	0.001554
unknown	34856/udp	0.000518
unknown	34857/udp	0.000518
unknown	34861/udp	0.006732
unknown	34862/udp	0.006214
unknown	34867/udp	0.000518
unknown	34870/udp	0.000518
unknown	34872/udp	0.000518
unknown	34875/tcp	0.000076
unknown	34882/udp	0.000518
unknown	34886/udp	0.000518
unknown	34887/udp	0.000518
unknown	34892/udp	0.002071
unknown	34893/udp	0.001036
unknown	34896/udp	0.000518
unknown	34905/udp	0.000518
unknown	34913/udp	0.000518
unknown	34915/udp	0.000518
unknown	34931/udp	0.000518
unknown	34945/udp	0.000518
unknown	34946/udp	0.000518
unknown	34948/udp	0.000518
unknown	34950/udp	0.000518
profinet-rt	34962/tcp	0.000000	# PROFInet RT Unicast
profinet-rt	34962/udp	0.000000	# PROFInet RT Unicast
profinet-rtm	34963/tcp	0.000000	# PROFInet RT Multicast
profinet-rtm	34963/udp	0.000000	# PROFInet RT Multicast
profinet-cm	34964/tcp	0.000000	# PROFInet Context Manager
profinet-cm	34964/udp	0.000000	# PROFInet Context Manager
unknown	34976/udp	0.000518
unknown	34979/udp	0.001036
ethercat	34980/tcp	0.000000	# EtherCAT Port | EhterCAT Port
ethercat	34980/udp	0.000000	# EhterCAT Port
unknown	34984/udp	0.000518
unknown	34993/udp	0.000518
unknown	34994/udp	0.000518
unknown	34997/udp	0.000518
unknown	34999/udp	0.000518
heathview	35000/tcp	0.000000
rt-viewer	35001/tcp	0.000000	# ReadyTech Viewer
rt-sound	35002/tcp	0.000000	# ReadyTech Sound Server
rt-devicemapper	35003/tcp	0.000000	# ReadyTech DeviceMapper Server
rt-classmanager	35004/tcp	0.000000	# ReadyTech ClassManager
rt-labtracker	35005/tcp	0.000000	# ReadyTech LabTracker
rt-helper	35006/tcp	0.000000	# ReadyTech Helper Service
unknown	35015/udp	0.000518
unknown	35026/udp	0.001036
unknown	35027/udp	0.000518
unknown	35030/udp	0.000518
unknown	35033/tcp	0.000076
unknown	35038/udp	0.000518
unknown	35040/udp	0.000518
unknown	35044/udp	0.001036
unknown	35050/tcp	0.000076
unknown	35051/udp	0.001036
unknown	35060/udp	0.000518
unknown	35063/udp	0.000518
unknown	35067/udp	0.000518
unknown	35088/udp	0.000518
unknown	35099/udp	0.000518
axio-disc	35100/tcp	0.000000	# Axiomatic discovery protocol
unknown	35108/udp	0.001036
unknown	35116/tcp	0.000076
unknown	35120/udp	0.000518
unknown	35126/udp	0.000518
unknown	35130/udp	0.000518
unknown	35131/tcp	0.000076
unknown	35135/udp	0.000518
unknown	35136/udp	0.000518
unknown	35140/udp	0.000518
unknown	35147/udp	0.000518
unknown	35150/udp	0.000518
unknown	35159/udp	0.000518
unknown	35169/udp	0.000518
unknown	35171/udp	0.000518
unknown	35176/udp	0.001036
unknown	35178/udp	0.000518
unknown	35179/udp	0.000518
unknown	35180/udp	0.000518
unknown	35182/udp	0.000518
unknown	35183/udp	0.000518
unknown	35187/udp	0.000518
unknown	35188/udp	0.001036
unknown	35189/udp	0.000518
unknown	35193/udp	0.000518
unknown	35198/udp	0.000518
unknown	35209/udp	0.000518
unknown	35217/tcp	0.000076
unknown	35217/udp	0.000518
unknown	35218/udp	0.000518
unknown	35222/udp	0.001036
unknown	35228/udp	0.000518
unknown	35230/udp	0.000518
unknown	35233/udp	0.000518
unknown	35235/udp	0.000518
unknown	35236/udp	0.000518
unknown	35238/udp	0.000518
unknown	35240/udp	0.001036
unknown	35245/udp	0.000518
unknown	35247/udp	0.000518
unknown	35251/udp	0.000518
unknown	35272/tcp	0.000076
unknown	35274/udp	0.000518
unknown	35280/udp	0.001036
unknown	35281/udp	0.000518
unknown	35282/udp	0.000518
unknown	35283/udp	0.001036
unknown	35288/udp	0.000518
unknown	35294/udp	0.000518
unknown	35301/udp	0.000518
unknown	35303/udp	0.000518
unknown	35312/udp	0.000518
unknown	35323/udp	0.000518
unknown	35325/udp	0.000518
unknown	35341/udp	0.000518
unknown	35344/udp	0.000518
unknown	35349/tcp	0.000076
unknown	35350/udp	0.000518
kitim	35354/tcp	0.000000	# KIT Messenger
altova-lm	35355/tcp	0.000000	# altova-lm-disc | Altova License Management | Altova License Management Discovery
guttersnex	35356/tcp	0.000000	# Gutters Note Exchange
openstack-id	35357/tcp	0.000000	# OpenStack ID Service
unknown	35363/udp	0.000518
unknown	35373/udp	0.000518
unknown	35388/udp	0.000518
unknown	35389/udp	0.000518
unknown	35390/udp	0.001036
unknown	35392/tcp	0.000076
unknown	35393/tcp	0.000076
unknown	35394/udp	0.000518
unknown	35401/tcp	0.000076
unknown	35406/udp	0.000518
unknown	35411/udp	0.000518
unknown	35419/udp	0.000518
unknown	35425/udp	0.000518
unknown	35426/udp	0.000518
unknown	35432/udp	0.000518
unknown	35433/udp	0.000518
unknown	35437/udp	0.000518
unknown	35438/udp	0.002071
unknown	35442/udp	0.000518
unknown	35448/udp	0.000518
unknown	35456/udp	0.000518
unknown	35474/udp	0.001036
unknown	35482/udp	0.000518
unknown	35490/udp	0.001036
unknown	35493/udp	0.001036
unknown	35500/tcp	0.000760
unknown	35502/udp	0.000518
unknown	35506/tcp	0.000076
unknown	35507/udp	0.000518
unknown	35511/udp	0.000518
unknown	35513/tcp	0.000152
unknown	35515/udp	0.000518
unknown	35516/udp	0.001036
unknown	35522/udp	0.000518
unknown	35529/udp	0.000518
unknown	35530/udp	0.000518
unknown	35533/udp	0.000518
unknown	35534/udp	0.000518
unknown	35536/udp	0.000518
unknown	35541/udp	0.000518
unknown	35551/udp	0.000518
unknown	35553/tcp	0.000076
unknown	35555/udp	0.000518
unknown	35557/udp	0.000518
unknown	35558/udp	0.000518
unknown	35561/udp	0.000518
unknown	35571/udp	0.000518
unknown	35574/udp	0.000518
unknown	35575/udp	0.000518
unknown	35579/udp	0.000518
unknown	35585/udp	0.000518
unknown	35587/udp	0.000518
unknown	35593/tcp	0.000076
unknown	35596/udp	0.000518
unknown	35598/udp	0.000518
unknown	35604/udp	0.000518
unknown	35607/udp	0.000518
unknown	35618/udp	0.000518
unknown	35621/udp	0.000518
unknown	35624/udp	0.000518
unknown	35636/udp	0.001036
unknown	35638/udp	0.000518
unknown	35643/udp	0.000518
unknown	35650/udp	0.000518
unknown	35651/udp	0.000518
unknown	35656/udp	0.001036
unknown	35658/udp	0.000518
unknown	35673/udp	0.000518
unknown	35685/udp	0.000518
unknown	35686/udp	0.000518
unknown	35688/udp	0.000518
unknown	35691/udp	0.000518
unknown	35695/udp	0.000518
unknown	35699/udp	0.000518
unknown	35702/udp	0.001554
unknown	35711/udp	0.000518
unknown	35715/udp	0.000518
unknown	35717/udp	0.000518
unknown	35720/udp	0.000518
unknown	35721/udp	0.000518
unknown	35727/udp	0.000518
unknown	35731/tcp	0.000076
unknown	35736/udp	0.000518
unknown	35746/udp	0.001036
unknown	35760/udp	0.000518
unknown	35767/udp	0.000518
unknown	35772/udp	0.000518
unknown	35773/udp	0.001036
unknown	35774/udp	0.000518
unknown	35775/udp	0.001036
unknown	35776/udp	0.001036
unknown	35777/udp	0.003107
unknown	35787/udp	0.000518
unknown	35792/udp	0.000518
unknown	35794/udp	0.001554
unknown	35800/udp	0.000518
unknown	35807/udp	0.000518
unknown	35810/udp	0.001036
unknown	35811/udp	0.000518
unknown	35812/udp	0.000518
unknown	35826/udp	0.000518
unknown	35835/udp	0.000518
unknown	35836/udp	0.000518
unknown	35837/udp	0.000518
unknown	35855/udp	0.000518
unknown	35863/udp	0.000518
unknown	35866/udp	0.000518
unknown	35870/udp	0.000518
unknown	35875/udp	0.000518
unknown	35876/udp	0.000518
unknown	35877/udp	0.000518
unknown	35879/tcp	0.000076
unknown	35882/udp	0.000518
unknown	35887/udp	0.000518
unknown	35896/udp	0.001036
unknown	35900/tcp	0.000076
unknown	35901/tcp	0.000076
unknown	35904/udp	0.001036
unknown	35906/tcp	0.000076
unknown	35906/udp	0.000518
unknown	35918/udp	0.000518
unknown	35925/udp	0.000518
unknown	35928/udp	0.000518
unknown	35929/tcp	0.000076
unknown	35929/udp	0.000518
unknown	35935/udp	0.000518
unknown	35940/udp	0.001036
unknown	35945/udp	0.000518
unknown	35948/udp	0.001036
unknown	35962/udp	0.000518
unknown	35965/udp	0.000518
unknown	35973/udp	0.000518
unknown	35980/udp	0.000518
unknown	35983/udp	0.000518
unknown	35985/udp	0.001036
unknown	35986/tcp	0.000076
unknown	35989/udp	0.000518
unknown	35991/udp	0.001036
unknown	35992/udp	0.000518
unknown	35994/udp	0.000518
allpeers	36001/tcp	0.000000	# AllPeers Network
allpeers	36001/udp	0.000000	# AllPeers Network
unknown	36005/udp	0.000518
unknown	36012/udp	0.000518
unknown	36014/udp	0.000518
unknown	36019/udp	0.001036
unknown	36025/udp	0.000518
unknown	36027/udp	0.000518
unknown	36035/udp	0.000518
unknown	36039/udp	0.000518
unknown	36041/udp	0.001036
unknown	36042/udp	0.000518
unknown	36046/tcp	0.000076
unknown	36046/udp	0.000518
unknown	36052/udp	0.000518
unknown	36065/udp	0.001036
unknown	36069/udp	0.000518
unknown	36072/udp	0.000518
unknown	36073/udp	0.000518
unknown	36080/udp	0.000518
unknown	36083/udp	0.000518
unknown	36093/udp	0.000518
unknown	36096/udp	0.001036
unknown	36099/udp	0.001036
unknown	36102/udp	0.000518
unknown	36104/tcp	0.000076
unknown	36105/tcp	0.000076
unknown	36108/udp	0.001554
unknown	36112/udp	0.000518
unknown	36114/udp	0.000518
unknown	36115/udp	0.000518
unknown	36126/udp	0.001036
unknown	36128/udp	0.000518
unknown	36136/udp	0.001036
unknown	36140/udp	0.000518
unknown	36149/udp	0.000518
unknown	36161/udp	0.000518
unknown	36175/udp	0.000518
unknown	36177/udp	0.000518
unknown	36178/udp	0.001036
unknown	36190/udp	0.000518
unknown	36193/udp	0.000518
unknown	36196/udp	0.000518
unknown	36197/udp	0.000518
unknown	36199/udp	0.000518
unknown	36201/udp	0.000518
unknown	36206/udp	0.002071
unknown	36207/udp	0.000518
unknown	36209/udp	0.000518
unknown	36212/udp	0.000518
unknown	36213/udp	0.000518
unknown	36214/udp	0.001036
unknown	36216/udp	0.000518
unknown	36223/udp	0.000518
unknown	36227/udp	0.000518
unknown	36228/udp	0.000518
unknown	36230/udp	0.000518
unknown	36237/udp	0.001036
unknown	36239/udp	0.000518
unknown	36244/udp	0.000518
unknown	36249/udp	0.000518
unknown	36252/udp	0.000518
unknown	36256/tcp	0.000076
unknown	36267/udp	0.000518
unknown	36269/udp	0.000518
unknown	36270/udp	0.000518
unknown	36275/tcp	0.000076
unknown	36276/udp	0.000518
unknown	36277/udp	0.000518
unknown	36279/udp	0.000518
unknown	36291/udp	0.000518
unknown	36293/udp	0.001036
unknown	36297/udp	0.000518
unknown	36303/udp	0.000518
unknown	36306/udp	0.000518
unknown	36307/udp	0.000518
unknown	36309/udp	0.000518
unknown	36312/udp	0.000518
unknown	36321/udp	0.000518
unknown	36336/udp	0.000518
unknown	36338/udp	0.000518
unknown	36342/udp	0.000518
unknown	36344/udp	0.000518
unknown	36350/udp	0.000518
unknown	36368/tcp	0.000076
unknown	36373/udp	0.000518
unknown	36376/udp	0.000518
unknown	36380/udp	0.001036
unknown	36381/udp	0.000518
unknown	36382/udp	0.000518
unknown	36384/udp	0.001554
unknown	36391/udp	0.000518
unknown	36404/udp	0.000518
unknown	36405/udp	0.000518
wlcp	36411/tcp	0.000000	# Wireless LAN Control plane Protocol (WLCP)
s1-control	36412/sctp	0.000000	# S1-Control Plane (3GPP)
unknown	36412/udp	0.000518
x2-control	36422/sctp	0.000000	# X2-Control Plane (3GPP)
slmap	36423/tcp	0.000000	# SLm Interface Application Protocol
unknown	36423/udp	0.000518
nq-ap	36424/tcp	0.000000	# Nq and Nq' Application Protocol
unknown	36431/udp	0.000518
unknown	36434/udp	0.000518
unknown	36436/tcp	0.000076
m2ap	36443/tcp	0.000000	# M2 Application Part
m3ap	36444/tcp	0.000000	# M3 Application Part
unknown	36445/udp	0.000518
unknown	36455/udp	0.000518
unknown	36456/udp	0.000518
unknown	36458/udp	0.001554
unknown	36460/udp	0.000518
xw-control	36462/tcp	0.000000	# Xw-Control Plane (3GPP)
unknown	36462/udp	0.001036
unknown	36464/udp	0.000518
unknown	36465/udp	0.000518
unknown	36469/udp	0.000518
unknown	36471/udp	0.001036
unknown	36474/udp	0.000518
unknown	36475/udp	0.000518
unknown	36480/udp	0.000518
unknown	36482/udp	0.000518
unknown	36483/udp	0.000518
unknown	36485/udp	0.000518
unknown	36486/udp	0.000518
unknown	36489/udp	0.001554
unknown	36491/udp	0.000518
unknown	36500/udp	0.001036
unknown	36508/tcp	0.000076
unknown	36508/udp	0.000518
unknown	36513/udp	0.000518
unknown	36517/udp	0.000518
unknown	36519/udp	0.001036
unknown	36522/udp	0.001036
febooti-aw	36524/tcp	0.000000	# Febooti Automation Workshop
unknown	36525/udp	0.000518
unknown	36526/udp	0.000518
unknown	36529/udp	0.000518
unknown	36530/tcp	0.000076
unknown	36532/udp	0.000518
unknown	36535/udp	0.000518
unknown	36540/udp	0.000518
unknown	36543/udp	0.000518
unknown	36545/udp	0.000518
unknown	36546/udp	0.000518
unknown	36550/udp	0.000518
unknown	36552/tcp	0.000076
unknown	36556/udp	0.000518
unknown	36561/udp	0.000518
unknown	36562/udp	0.000518
unknown	36571/udp	0.000518
unknown	36576/udp	0.001036
unknown	36578/udp	0.000518
unknown	36590/udp	0.000518
unknown	36596/udp	0.000518
unknown	36600/udp	0.000518
unknown	36601/udp	0.000518
observium-agent	36602/tcp	0.000000	# Observium statistics collection agent
unknown	36612/udp	0.000518
unknown	36616/udp	0.000518
unknown	36618/udp	0.000518
unknown	36622/udp	0.000518
unknown	36624/udp	0.000518
unknown	36633/udp	0.000518
unknown	36640/udp	0.000518
unknown	36641/udp	0.001036
unknown	36645/udp	0.000518
unknown	36647/udp	0.000518
unknown	36655/udp	0.000518
unknown	36659/tcp	0.000076
unknown	36664/udp	0.000518
unknown	36666/udp	0.001036
unknown	36669/udp	0.001554
unknown	36671/udp	0.000518
unknown	36675/udp	0.000518
unknown	36677/tcp	0.000076
unknown	36677/udp	0.000518
unknown	36681/udp	0.000518
unknown	36682/udp	0.000518
unknown	36689/udp	0.000518
unknown	36694/tcp	0.000076
unknown	36694/udp	0.001036
unknown	36695/udp	0.001036
unknown	36696/udp	0.000518
unknown	36699/udp	0.000518
mapx	36700/tcp	0.000000	# MapX communication
unknown	36702/udp	0.000518
unknown	36705/udp	0.000518
unknown	36710/tcp	0.000076
unknown	36719/udp	0.001036
unknown	36721/udp	0.000518
unknown	36725/udp	0.000518
unknown	36728/udp	0.000518
unknown	36741/udp	0.000518
unknown	36743/udp	0.000518
unknown	36748/tcp	0.000076
unknown	36748/udp	0.000518
unknown	36754/udp	0.000518
unknown	36756/udp	0.000518
unknown	36757/udp	0.000518
unknown	36760/udp	0.000518
unknown	36776/udp	0.000518
unknown	36778/udp	0.001554
unknown	36788/udp	0.000518
unknown	36793/udp	0.000518
unknown	36802/udp	0.000518
unknown	36807/udp	0.000518
unknown	36810/udp	0.000518
unknown	36813/udp	0.000518
unknown	36816/udp	0.000518
unknown	36817/udp	0.001036
unknown	36823/tcp	0.000076
unknown	36824/tcp	0.000076
unknown	36832/udp	0.000518
unknown	36835/udp	0.000518
unknown	36837/udp	0.000518
unknown	36843/udp	0.000518
unknown	36845/udp	0.000518
unknown	36848/udp	0.000518
unknown	36849/udp	0.000518
unknown	36851/udp	0.000518
unknown	36854/udp	0.001036
unknown	36855/udp	0.000518
unknown	36861/udp	0.000518
unknown	36862/udp	0.001036
kastenxpipe	36865/tcp	0.000000	# KastenX Pipe
kastenxpipe	36865/udp	0.000000	# KastenX Pipe
unknown	36871/udp	0.000518
unknown	36882/udp	0.000518
unknown	36883/udp	0.000518
unknown	36887/udp	0.001036
unknown	36893/udp	0.001554
unknown	36905/udp	0.000518
unknown	36907/udp	0.000518
unknown	36909/udp	0.000518
unknown	36910/udp	0.001036
unknown	36911/udp	0.000518
unknown	36912/udp	0.000518
unknown	36914/tcp	0.000076
unknown	36923/udp	0.000518
unknown	36925/udp	0.000518
unknown	36930/udp	0.000518
unknown	36931/udp	0.001036
unknown	36934/udp	0.000518
unknown	36941/udp	0.000518
unknown	36945/udp	0.001554
unknown	36950/tcp	0.000076
unknown	36955/udp	0.000518
unknown	36962/tcp	0.000076
unknown	36970/udp	0.000518
unknown	36979/udp	0.000518
unknown	36980/udp	0.000518
unknown	36981/udp	0.000518
unknown	36983/tcp	0.000076
unknown	36986/udp	0.000518
unknown	36987/udp	0.000518
unknown	36990/udp	0.001036
unknown	36997/udp	0.000518
unknown	37004/udp	0.000518
unknown	37010/udp	0.000518
unknown	37012/udp	0.000518
unknown	37018/udp	0.001036
unknown	37019/udp	0.000518
unknown	37021/udp	0.000518
unknown	37024/udp	0.000518
unknown	37025/udp	0.001036
unknown	37034/udp	0.000518
unknown	37046/udp	0.001036
unknown	37053/udp	0.000518
unknown	37067/udp	0.000518
unknown	37085/udp	0.000518
unknown	37087/udp	0.000518
unknown	37093/udp	0.001036
unknown	37095/udp	0.000518
unknown	37097/udp	0.000518
unknown	37100/udp	0.000518
unknown	37103/udp	0.000518
unknown	37105/udp	0.000518
unknown	37106/udp	0.000518
unknown	37119/udp	0.000518
unknown	37120/udp	0.000518
unknown	37121/tcp	0.000076
unknown	37122/udp	0.000518
unknown	37126/udp	0.000518
unknown	37130/udp	0.000518
unknown	37136/udp	0.001036
unknown	37138/udp	0.000518
unknown	37139/udp	0.001036
unknown	37144/udp	0.001554
unknown	37148/udp	0.000518
unknown	37149/udp	0.000518
unknown	37151/tcp	0.000076
unknown	37151/udp	0.000518
unknown	37152/udp	0.001036
unknown	37154/udp	0.000518
unknown	37156/udp	0.001036
unknown	37158/udp	0.000518
unknown	37163/udp	0.001036
unknown	37168/udp	0.000518
unknown	37174/tcp	0.000076
unknown	37176/udp	0.000518
unknown	37179/udp	0.000518
unknown	37182/udp	0.001036
unknown	37184/udp	0.000518
unknown	37185/tcp	0.000076
unknown	37198/udp	0.001036
unknown	37203/udp	0.000518
unknown	37208/udp	0.000518
unknown	37210/udp	0.000518
unknown	37212/udp	0.001554
unknown	37214/udp	0.000518
unknown	37215/udp	0.000518
unknown	37216/udp	0.001036
unknown	37218/tcp	0.000076
unknown	37219/udp	0.000518
unknown	37221/udp	0.001036
unknown	37225/udp	0.000518
unknown	37228/udp	0.000518
unknown	37230/udp	0.000518
unknown	37253/udp	0.000518
unknown	37255/udp	0.001036
unknown	37256/udp	0.000518
unknown	37268/udp	0.000518
unknown	37279/udp	0.000518
unknown	37288/udp	0.000518
unknown	37292/udp	0.000518
unknown	37298/udp	0.000518
unknown	37299/udp	0.000518
unknown	37310/udp	0.000518
unknown	37313/udp	0.000518
unknown	37316/udp	0.001036
unknown	37318/udp	0.000518
unknown	37324/udp	0.000518
unknown	37327/udp	0.001036
unknown	37332/udp	0.000518
unknown	37338/udp	0.000518
unknown	37342/udp	0.000518
unknown	37343/udp	0.001036
unknown	37348/udp	0.001036
unknown	37351/udp	0.000518
unknown	37356/udp	0.000518
unknown	37357/udp	0.000518
unknown	37358/udp	0.000518
unknown	37376/udp	0.000518
unknown	37377/udp	0.001036
unknown	37385/udp	0.001036
unknown	37393/tcp	0.000076
unknown	37393/udp	0.001554
unknown	37396/udp	0.000518
unknown	37400/udp	0.001036
unknown	37401/udp	0.001036
unknown	37407/udp	0.000518
unknown	37411/udp	0.000518
unknown	37415/udp	0.000518
unknown	37420/udp	0.000518
unknown	37423/udp	0.001036
unknown	37425/udp	0.000518
unknown	37431/udp	0.000518
unknown	37438/udp	0.000518
unknown	37441/udp	0.001036
unknown	37443/udp	0.000518
unknown	37444/udp	0.006732
unknown	37450/udp	0.000518
unknown	37454/udp	0.000518
unknown	37456/udp	0.001036
unknown	37458/udp	0.000518
unknown	37463/udp	0.000518
unknown	37464/udp	0.001036
unknown	37467/udp	0.000518
3gpp-w1ap	37472/tcp	0.000000	# W1 signalling transport
unknown	37474/udp	0.000518
neckar	37475/tcp	0.000000	# science + computing's Venus Administration Port
neckar	37475/udp	0.000000	# science + computing's Venus Administration Port
unknown	37477/udp	0.000518
unknown	37478/udp	0.001036
gdrive-sync	37483/tcp	0.000000	# Google Drive Sync
unknown	37487/udp	0.000518
unknown	37488/udp	0.000518
unknown	37493/udp	0.000518
unknown	37494/udp	0.000518
unknown	37501/udp	0.000518
unknown	37506/udp	0.000518
unknown	37518/udp	0.000518
unknown	37522/tcp	0.000076
unknown	37522/udp	0.000518
unknown	37524/udp	0.000518
unknown	37525/udp	0.000518
unknown	37531/udp	0.000518
unknown	37541/udp	0.000518
unknown	37543/udp	0.000518
unknown	37546/udp	0.000518
unknown	37560/udp	0.000518
unknown	37561/udp	0.001036
unknown	37563/udp	0.001036
unknown	37567/udp	0.000518
unknown	37568/udp	0.000518
unknown	37572/udp	0.000518
unknown	37574/udp	0.001036
unknown	37587/udp	0.000518
unknown	37588/udp	0.000518
unknown	37589/udp	0.001036
unknown	37592/udp	0.001036
eftp	37601/tcp	0.000000	# Epipole File Transfer Protocol
unknown	37602/udp	0.001554
unknown	37607/tcp	0.000076
unknown	37611/udp	0.000518
unknown	37614/tcp	0.000076
unknown	37614/udp	0.000518
unknown	37617/udp	0.000518
unknown	37621/udp	0.000518
unknown	37624/udp	0.000518
unknown	37635/udp	0.000518
unknown	37636/udp	0.000518
unknown	37638/udp	0.000518
unknown	37641/udp	0.000518
unknown	37647/tcp	0.000076
unisys-eportal	37654/tcp	0.000000	# Unisys ClearPath ePortal
unisys-eportal	37654/udp	0.001036	# Unisys ClearPath ePortal
unknown	37657/udp	0.000518
unknown	37663/udp	0.001036
unknown	37664/udp	0.001036
unknown	37668/udp	0.000518
unknown	37670/udp	0.001036
unknown	37674/tcp	0.000076
unknown	37682/udp	0.001036
unknown	37686/udp	0.001036
unknown	37688/udp	0.000518
unknown	37690/udp	0.000518
unknown	37695/udp	0.000518
unknown	37698/udp	0.000518
unknown	37701/udp	0.000518
unknown	37710/udp	0.000518
unknown	37719/udp	0.000518
unknown	37720/udp	0.000518
unknown	37721/udp	0.000518
unknown	37728/udp	0.000518
unknown	37730/udp	0.000518
unknown	37731/udp	0.000518
unknown	37738/udp	0.000518
unknown	37749/udp	0.000518
unknown	37761/udp	0.001554
unknown	37764/udp	0.000518
unknown	37766/udp	0.000518
unknown	37767/udp	0.000518
unknown	37769/udp	0.000518
unknown	37770/udp	0.000518
unknown	37771/udp	0.000518
unknown	37777/tcp	0.000076
unknown	37778/udp	0.000518
unknown	37781/udp	0.000518
unknown	37783/udp	0.001554
unknown	37789/tcp	0.000076
unknown	37792/udp	0.000518
unknown	37795/udp	0.000518
unknown	37808/udp	0.000518
unknown	37813/udp	0.001554
unknown	37816/udp	0.000518
unknown	37817/udp	0.000518
unknown	37819/udp	0.000518
unknown	37820/udp	0.000518
unknown	37823/udp	0.001036
unknown	37829/udp	0.000518
unknown	37834/udp	0.000518
unknown	37839/tcp	0.000152
unknown	37839/udp	0.000518
unknown	37843/udp	0.001554
unknown	37844/udp	0.000518
unknown	37847/udp	0.000518
unknown	37853/udp	0.000518
unknown	37855/tcp	0.000076
unknown	37862/udp	0.000518
unknown	37863/udp	0.000518
unknown	37864/udp	0.000518
unknown	37866/udp	0.000518
unknown	37873/udp	0.000518
unknown	37874/udp	0.000518
unknown	37886/udp	0.000518
unknown	37888/udp	0.000518
unknown	37891/udp	0.000518
unknown	37893/udp	0.000518
unknown	37898/udp	0.000518
unknown	37900/udp	0.000518
unknown	37906/udp	0.000518
unknown	37907/udp	0.000518
unknown	37917/udp	0.000518
unknown	37920/udp	0.000518
unknown	37922/udp	0.001036
unknown	37923/udp	0.000518
unknown	37933/udp	0.001036
unknown	37942/udp	0.000518
unknown	37949/udp	0.000518
unknown	37952/udp	0.000518
unknown	37959/udp	0.000518
unknown	37964/udp	0.001036
unknown	37967/udp	0.000518
unknown	37968/udp	0.000518
unknown	37969/udp	0.000518
unknown	37974/udp	0.000518
unknown	37978/udp	0.000518
unknown	37985/udp	0.000518
unknown	37995/udp	0.000518
unknown	37997/udp	0.000518
ivs-database	38000/tcp	0.000000	# InfoVista Server Database
ivs-insertion	38001/tcp	0.000000	# InfoVista Server Insertion
cresco-control	38002/tcp	0.000000	# crescoctrl-disc | Cresco Controller | Cresco Controller Discovery
unknown	38007/udp	0.000518
unknown	38008/udp	0.000518
unknown	38013/udp	0.000518
unknown	38014/udp	0.001036
unknown	38016/udp	0.000518
unknown	38021/udp	0.000518
unknown	38025/udp	0.000518
unknown	38029/tcp	0.000076
unknown	38036/udp	0.000518
landesk-cba	38037/tcp	0.000088
landesk-cba	38037/udp	0.002869
unknown	38040/udp	0.000518
unknown	38041/udp	0.001036
unknown	38042/udp	0.000518
unknown	38050/udp	0.000518
unknown	38053/udp	0.001036
unknown	38058/udp	0.000518
unknown	38063/udp	0.001554
unknown	38064/udp	0.001036
unknown	38065/udp	0.000518
unknown	38069/udp	0.000518
unknown	38070/udp	0.000518
unknown	38073/udp	0.000518
unknown	38074/udp	0.000518
unknown	38082/udp	0.000518
unknown	38088/udp	0.000518
unknown	38089/udp	0.000518
unknown	38103/udp	0.000518
unknown	38104/udp	0.000518
unknown	38106/udp	0.000518
unknown	38111/udp	0.000518
unknown	38113/udp	0.000518
unknown	38125/udp	0.001036
unknown	38130/udp	0.000518
unknown	38136/udp	0.000518
unknown	38137/udp	0.000518
unknown	38138/udp	0.000518
unknown	38139/udp	0.000518
unknown	38142/udp	0.001036
unknown	38147/udp	0.000518
unknown	38152/udp	0.000518
unknown	38153/udp	0.001036
unknown	38155/udp	0.000518
unknown	38157/udp	0.000518
unknown	38159/udp	0.000518
unknown	38166/udp	0.000518
unknown	38168/udp	0.000518
unknown	38172/udp	0.001036
unknown	38175/udp	0.000518
unknown	38179/udp	0.000518
unknown	38181/udp	0.000518
unknown	38182/udp	0.000518
unknown	38183/udp	0.001036
unknown	38185/tcp	0.000152
unknown	38188/tcp	0.000152
unknown	38189/udp	0.000518
unknown	38190/udp	0.001036
unknown	38194/tcp	0.000076
unknown	38197/udp	0.000518
galaxy7-data	38201/tcp	0.000000	# Galaxy7 Data Tunnel
galaxy7-data	38201/udp	0.000000	# Galaxy7 Data Tunnel
fairview	38202/tcp	0.000000	# Fairview Message Service
fairview	38202/udp	0.000518	# Fairview Message Service
agpolicy	38203/tcp	0.000000	# AppGate Policy Server
agpolicy	38203/udp	0.000000	# AppGate Policy Server
unknown	38205/tcp	0.000076
unknown	38215/udp	0.000518
unknown	38218/udp	0.001036
unknown	38224/tcp	0.000076
unknown	38225/udp	0.000518
unknown	38233/udp	0.000518
unknown	38258/udp	0.000518
unknown	38259/udp	0.000518
unknown	38262/udp	0.000518
unknown	38266/udp	0.000518
unknown	38270/tcp	0.000076
unknown	38274/udp	0.001036
unknown	38280/udp	0.000518
unknown	38283/udp	0.000518
unknown	38288/udp	0.000518
unknown	38290/udp	0.000518
unknown	38291/udp	0.000518
landesk-cba	38292/tcp	0.000276
landesk-cba	38293/udp	0.002970
unknown	38294/udp	0.001036
unknown	38297/udp	0.000518
unknown	38300/udp	0.000518
unknown	38304/udp	0.001036
unknown	38312/udp	0.001036
unknown	38313/tcp	0.000076
unknown	38321/udp	0.000518
unknown	38325/udp	0.001036
unknown	38331/tcp	0.000076
unknown	38334/udp	0.000518
unknown	38341/udp	0.000518
unknown	38343/udp	0.000518
unknown	38345/udp	0.000518
unknown	38350/udp	0.000518
unknown	38354/udp	0.000518
unknown	38355/udp	0.000518
unknown	38356/udp	0.000518
unknown	38358/tcp	0.000076
unknown	38360/udp	0.000518
unknown	38370/udp	0.001036
unknown	38372/udp	0.000518
unknown	38379/udp	0.000518
unknown	38389/udp	0.000518
unknown	38391/udp	0.000518
unknown	38395/udp	0.000518
unknown	38396/udp	0.000518
unknown	38397/udp	0.000518
unknown	38402/udp	0.000518
unknown	38403/udp	0.000518
ng-control	38412/tcp	0.000000	# NG Control Plane (3GPP)
unknown	38412/udp	0.001554
xn-control	38422/tcp	0.000000	# Xn Control Plane (3GPP)
unknown	38428/udp	0.000518
unknown	38431/udp	0.000518
unknown	38432/udp	0.000518
unknown	38434/udp	0.000518
unknown	38435/udp	0.000518
unknown	38437/udp	0.000518
unknown	38438/udp	0.000518
unknown	38442/udp	0.000518
unknown	38446/tcp	0.000076
unknown	38450/udp	0.000518
unknown	38452/udp	0.000518
e1-interface	38462/tcp	0.000000	# E1 signalling transport (3GPP)
unknown	38465/udp	0.000518
unknown	38466/udp	0.000518
f1-control	38472/tcp	0.000000	# F1 Control Plane (3GPP)
unknown	38472/udp	0.000518
unknown	38475/udp	0.000518
unknown	38478/udp	0.000518
unknown	38480/udp	0.000518
unknown	38481/tcp	0.000076
unknown	38490/udp	0.000518
unknown	38494/udp	0.000518
unknown	38497/udp	0.000518
unknown	38498/udp	0.001554
unknown	38499/udp	0.001036
unknown	38500/udp	0.000518
unknown	38505/udp	0.000518
unknown	38510/udp	0.001036
unknown	38512/udp	0.000518
unknown	38519/udp	0.000518
unknown	38520/udp	0.000518
unknown	38526/udp	0.001036
unknown	38530/udp	0.000518
unknown	38544/udp	0.000518
unknown	38545/udp	0.000518
unknown	38546/tcp	0.000076
unknown	38547/udp	0.000518
unknown	38548/udp	0.000518
unknown	38555/udp	0.000518
unknown	38557/udp	0.000518
unknown	38561/tcp	0.000076
unknown	38567/udp	0.000518
unknown	38570/tcp	0.000076
unknown	38571/udp	0.001036
unknown	38579/udp	0.000518
unknown	38581/udp	0.000518
unknown	38582/udp	0.000518
unknown	38598/udp	0.000518
unknown	38599/udp	0.000518
unknown	38608/udp	0.001036
unknown	38609/udp	0.001036
unknown	38610/udp	0.000518
unknown	38615/udp	0.001554
unknown	38618/udp	0.000518
unknown	38620/udp	0.000518
unknown	38627/udp	0.000518
unknown	38630/udp	0.000518
unknown	38631/udp	0.000518
unknown	38634/udp	0.000518
psqlmws	38638/tcp	0.000000	# Premier SQL Middleware Server
unknown	38638/udp	0.000518
unknown	38639/udp	0.000518
unknown	38644/udp	0.001036
unknown	38647/udp	0.000518
unknown	38648/udp	0.001036
unknown	38662/udp	0.000518
unknown	38666/udp	0.000518
unknown	38667/udp	0.000518
unknown	38671/udp	0.000518
unknown	38672/udp	0.000518
unknown	38675/udp	0.000518
unknown	38677/udp	0.000518
unknown	38680/udp	0.000518
unknown	38681/udp	0.000518
unknown	38684/udp	0.000518
unknown	38686/udp	0.000518
unknown	38694/udp	0.000518
unknown	38697/udp	0.000518
unknown	38707/udp	0.000518
unknown	38710/udp	0.000518
unknown	38712/udp	0.000518
unknown	38714/udp	0.001036
unknown	38716/udp	0.000518
unknown	38720/udp	0.000518
unknown	38721/udp	0.000518
unknown	38723/udp	0.000518
unknown	38724/udp	0.000518
unknown	38727/udp	0.001036
unknown	38729/udp	0.000518
unknown	38732/udp	0.001036
unknown	38734/udp	0.001036
unknown	38739/udp	0.000518
unknown	38742/udp	0.001036
unknown	38744/udp	0.000518
unknown	38745/udp	0.000518
unknown	38750/udp	0.000518
unknown	38759/udp	0.000518
unknown	38761/tcp	0.000076
unknown	38764/tcp	0.000076
unknown	38777/udp	0.000518
unknown	38780/tcp	0.000076
unknown	38780/udp	0.000518
unknown	38784/udp	0.000518
unknown	38788/udp	0.000518
unknown	38794/udp	0.000518
unknown	38799/udp	0.000518
sruth	38800/tcp	0.000000	# Sruth is a service for the distribution of routinely- generated but arbitrary files based on a publish/subscribe distribution model and implemented using a peer-to-peer transport mechanism
unknown	38805/tcp	0.000076
unknown	38812/udp	0.001036
unknown	38817/udp	0.000518
unknown	38826/udp	0.000518
unknown	38836/udp	0.000518
unknown	38837/udp	0.000518
unknown	38840/udp	0.000518
unknown	38842/udp	0.000518
unknown	38844/udp	0.000518
unknown	38845/udp	0.000518
unknown	38850/udp	0.000518
unknown	38851/udp	0.000518
unknown	38857/udp	0.000518
unknown	38862/udp	0.000518
unknown	38864/udp	0.001036
secrmmsafecopya	38865/tcp	0.000000	# Security approval process for use of the secRMM SafeCopy program
unknown	38869/udp	0.000518
unknown	38875/udp	0.000518
unknown	38889/udp	0.000518
unknown	38898/udp	0.000518
unknown	38901/udp	0.000518
unknown	38902/udp	0.000518
unknown	38907/udp	0.000518
unknown	38909/udp	0.000518
unknown	38911/udp	0.000518
unknown	38912/udp	0.000518
unknown	38922/udp	0.000518
unknown	38927/udp	0.000518
unknown	38936/tcp	0.000076
unknown	38938/udp	0.000518
unknown	38946/udp	0.000518
unknown	38949/udp	0.000518
unknown	38956/udp	0.000518
unknown	38964/udp	0.000518
unknown	38966/udp	0.000518
unknown	38972/udp	0.001036
unknown	38973/udp	0.000518
unknown	38974/udp	0.000518
unknown	38978/udp	0.000518
unknown	38989/udp	0.000518
unknown	39006/udp	0.000518
unknown	39009/udp	0.000518
unknown	39013/udp	0.000518
unknown	39018/udp	0.000518
unknown	39022/udp	0.000518
unknown	39023/udp	0.000518
unknown	39024/udp	0.000518
unknown	39027/udp	0.000518
unknown	39028/udp	0.001036
unknown	39030/udp	0.000518
unknown	39033/udp	0.000518
unknown	39035/udp	0.001036
unknown	39037/udp	0.000518
unknown	39041/udp	0.000518
unknown	39042/udp	0.001036
unknown	39045/udp	0.000518
unknown	39054/udp	0.000518
unknown	39056/udp	0.001036
unknown	39057/udp	0.000518
vroa	39063/tcp	0.000000	# Children's hearing test/Telemedicine
unknown	39067/tcp	0.000076
unknown	39068/udp	0.000518
unknown	39074/udp	0.000518
unknown	39076/udp	0.000518
unknown	39083/udp	0.000518
unknown	39084/udp	0.000518
unknown	39085/udp	0.000518
unknown	39086/udp	0.001036
unknown	39087/udp	0.000518
unknown	39091/udp	0.000518
unknown	39095/udp	0.000518
unknown	39104/udp	0.000518
unknown	39107/udp	0.000518
unknown	39109/udp	0.000518
unknown	39114/udp	0.000518
unknown	39115/udp	0.000518
unknown	39116/udp	0.001036
unknown	39117/tcp	0.000076
unknown	39118/udp	0.000518
unknown	39120/udp	0.000518
unknown	39124/udp	0.000518
unknown	39126/udp	0.000518
unknown	39132/udp	0.000518
unknown	39133/udp	0.000518
unknown	39135/udp	0.001036
unknown	39136/tcp	0.000152
unknown	39137/udp	0.000518
unknown	39143/udp	0.000518
unknown	39146/udp	0.001036
unknown	39156/udp	0.000518
unknown	39157/udp	0.000518
unknown	39163/udp	0.001036
unknown	39167/udp	0.000518
unknown	39170/udp	0.000518
unknown	39179/udp	0.000518
unknown	39184/udp	0.000518
unknown	39185/udp	0.000518
unknown	39187/udp	0.000518
unknown	39190/udp	0.000518
unknown	39199/udp	0.000518
unknown	39201/udp	0.000518
sygatefw	39213/udp	0.004446	# Sygate Firewall management port version 3.0 build 521 and above
unknown	39214/udp	0.000518
unknown	39217/udp	0.001554
unknown	39218/udp	0.000518
unknown	39220/udp	0.001036
unknown	39227/udp	0.000518
unknown	39231/udp	0.000518
unknown	39232/udp	0.000518
unknown	39235/udp	0.000518
unknown	39239/udp	0.000518
unknown	39243/udp	0.001036
unknown	39259/udp	0.000518
unknown	39261/udp	0.000518
unknown	39265/tcp	0.000076
unknown	39265/udp	0.000518
unknown	39269/udp	0.000518
unknown	39275/udp	0.000518
unknown	39289/udp	0.000518
unknown	39290/udp	0.000518
unknown	39293/tcp	0.000076
unknown	39294/udp	0.000518
unknown	39297/udp	0.001036
unknown	39301/udp	0.000518
unknown	39303/udp	0.000518
unknown	39307/udp	0.000518
unknown	39313/udp	0.001036
unknown	39315/udp	0.000518
unknown	39318/udp	0.000518
unknown	39324/udp	0.000518
unknown	39330/udp	0.000518
unknown	39332/udp	0.001036
unknown	39344/udp	0.000518
unknown	39350/udp	0.000518
unknown	39375/udp	0.000518
unknown	39376/tcp	0.000152
unknown	39377/udp	0.001036
unknown	39380/tcp	0.000076
unknown	39383/udp	0.001036
unknown	39386/udp	0.000518
unknown	39388/udp	0.000518
unknown	39392/udp	0.000518
unknown	39397/udp	0.000518
unknown	39398/udp	0.000518
unknown	39401/udp	0.001036
unknown	39404/udp	0.000518
unknown	39407/udp	0.000518
unknown	39415/udp	0.000518
unknown	39417/udp	0.000518
unknown	39424/udp	0.000518
unknown	39426/udp	0.000518
unknown	39430/udp	0.001036
unknown	39433/tcp	0.000076
unknown	39439/udp	0.000518
unknown	39440/udp	0.001036
unknown	39444/udp	0.000518
unknown	39445/udp	0.000518
unknown	39452/udp	0.000518
unknown	39453/udp	0.001036
unknown	39457/udp	0.001036
unknown	39463/udp	0.000518
unknown	39466/udp	0.000518
unknown	39472/udp	0.000518
unknown	39477/udp	0.000518
unknown	39480/udp	0.000518
unknown	39482/tcp	0.000076
unknown	39483/udp	0.000518
unknown	39487/udp	0.000518
unknown	39489/tcp	0.000076
unknown	39492/udp	0.000518
unknown	39499/udp	0.000518
unknown	39505/udp	0.000518
unknown	39507/udp	0.001036
unknown	39518/udp	0.000518
unknown	39524/udp	0.000518
unknown	39526/udp	0.000518
unknown	39528/udp	0.000518
unknown	39529/udp	0.000518
unknown	39541/udp	0.000518
unknown	39542/udp	0.000518
unknown	39544/udp	0.000518
unknown	39548/udp	0.001036
unknown	39552/udp	0.000518
unknown	39560/udp	0.000518
unknown	39565/udp	0.000518
unknown	39566/udp	0.000518
unknown	39570/udp	0.000518
unknown	39574/udp	0.000518
unknown	39586/udp	0.000518
unknown	39590/udp	0.001036
unknown	39591/udp	0.000518
unknown	39596/udp	0.001036
unknown	39600/udp	0.001036
unknown	39605/udp	0.000518
unknown	39610/udp	0.000518
unknown	39611/udp	0.000518
unknown	39616/udp	0.000518
unknown	39617/udp	0.000518
unknown	39630/tcp	0.000076
unknown	39630/udp	0.001036
unknown	39632/udp	0.001554
unknown	39638/udp	0.000518
unknown	39641/udp	0.001036
unknown	39649/udp	0.001036
unknown	39659/tcp	0.000152
unknown	39659/udp	0.001036
unknown	39664/udp	0.000518
unknown	39666/udp	0.000518
unknown	39668/udp	0.000518
unknown	39674/udp	0.000518
unknown	39679/udp	0.000518
turbonote-1	39681/tcp	0.000000	# TurboNote Default Port
turbonote-1	39681/udp	0.000000	# TurboNote Default Port
unknown	39683/udp	0.001554
unknown	39685/udp	0.000518
unknown	39687/udp	0.000518
unknown	39697/udp	0.001036
unknown	39701/udp	0.000518
unknown	39702/udp	0.000518
unknown	39703/udp	0.000518
unknown	39707/udp	0.000518
unknown	39709/udp	0.001036
unknown	39713/udp	0.000518
unknown	39714/udp	0.001554
unknown	39715/udp	0.000518
unknown	39716/udp	0.000518
unknown	39720/udp	0.000518
unknown	39723/udp	0.001554
unknown	39726/udp	0.000518
unknown	39727/udp	0.000518
unknown	39731/udp	0.000518
unknown	39732/tcp	0.000076
unknown	39733/udp	0.001036
unknown	39739/udp	0.000518
unknown	39740/udp	0.000518
unknown	39743/udp	0.001036
unknown	39745/udp	0.001036
unknown	39750/udp	0.000518
unknown	39753/udp	0.001036
unknown	39754/udp	0.000518
unknown	39763/tcp	0.000076
unknown	39763/udp	0.000518
unknown	39765/udp	0.000518
unknown	39773/udp	0.000518
unknown	39774/tcp	0.000076
unknown	39783/udp	0.000518
unknown	39786/udp	0.000518
unknown	39791/udp	0.000518
unknown	39792/udp	0.000518
unknown	39795/tcp	0.000076
unknown	39795/udp	0.000518
unknown	39796/udp	0.000518
unknown	39799/udp	0.000518
unknown	39800/udp	0.000518
unknown	39801/udp	0.000518
unknown	39802/udp	0.000518
unknown	39805/udp	0.000518
unknown	39811/udp	0.001036
unknown	39812/udp	0.001036
unknown	39816/udp	0.000518
unknown	39827/udp	0.000518
unknown	39829/udp	0.000518
unknown	39832/udp	0.000518
unknown	39835/udp	0.000518
unknown	39839/udp	0.000518
unknown	39845/udp	0.000518
unknown	39846/udp	0.000518
unknown	39848/udp	0.000518
unknown	39849/udp	0.000518
unknown	39856/udp	0.000518
unknown	39858/udp	0.000518
unknown	39863/udp	0.001036
unknown	39867/udp	0.000518
unknown	39869/tcp	0.000076
unknown	39871/udp	0.000518
unknown	39873/udp	0.000518
unknown	39878/udp	0.000518
unknown	39883/tcp	0.000076
unknown	39883/udp	0.000518
unknown	39888/udp	0.002071
unknown	39895/tcp	0.000076
unknown	39897/udp	0.000518
unknown	39898/udp	0.000518
unknown	39911/udp	0.000518
unknown	39917/tcp	0.000076
unknown	39919/udp	0.001036
unknown	39930/udp	0.000518
unknown	39938/udp	0.000518
unknown	39940/udp	0.000518
unknown	39948/udp	0.000518
unknown	39951/udp	0.000518
unknown	39959/udp	0.000518
unknown	39967/udp	0.000518
unknown	39973/udp	0.000518
unknown	39978/udp	0.000518
unknown	39980/udp	0.000518
unknown	39982/udp	0.001036
unknown	39990/udp	0.000518
unknown	39991/udp	0.000518
unknown	39997/udp	0.000518
safetynetp	40000/tcp	0.000152	# SafetyNET p
safetynetp	40000/udp	0.000000	# SafetyNET p
unknown	40001/tcp	0.000076
unknown	40002/tcp	0.000076
unknown	40003/tcp	0.000076
unknown	40005/tcp	0.000076
unknown	40008/udp	0.000518
unknown	40009/udp	0.000518
unknown	40010/udp	0.000518
unknown	40011/tcp	0.000076
unknown	40019/udp	0.001554
unknown	40022/udp	0.000518
k-patentssensor	40023/tcp	0.000000	# K-PatentsSensorInformation
unknown	40028/udp	0.000518
unknown	40031/udp	0.000518
unknown	40036/udp	0.000518
unknown	40041/udp	0.000518
unknown	40043/udp	0.001036
unknown	40045/udp	0.000518
unknown	40049/udp	0.000518
unknown	40054/udp	0.000518
unknown	40055/udp	0.000518
unknown	40060/udp	0.000518
unknown	40061/udp	0.000518
unknown	40063/udp	0.000518
unknown	40071/udp	0.001036
unknown	40074/udp	0.001036
unknown	40076/udp	0.000518
unknown	40089/udp	0.000518
unknown	40090/udp	0.000518
unknown	40093/udp	0.000518
unknown	40101/udp	0.001036
unknown	40102/udp	0.001036
unknown	40111/udp	0.001036
unknown	40113/udp	0.000518
unknown	40116/udp	0.002071
unknown	40123/udp	0.000518
unknown	40127/udp	0.000518
unknown	40136/udp	0.000518
unknown	40138/udp	0.000518
unknown	40141/udp	0.000518
unknown	40142/udp	0.000518
unknown	40143/udp	0.000518
unknown	40144/udp	0.000518
unknown	40147/udp	0.000518
unknown	40148/udp	0.000518
unknown	40159/udp	0.000518
unknown	40176/udp	0.000518
unknown	40181/udp	0.000518
unknown	40183/udp	0.000518
unknown	40186/udp	0.000518
unknown	40187/udp	0.000518
unknown	40188/udp	0.000518
unknown	40191/udp	0.000518
unknown	40192/udp	0.000518
unknown	40193/tcp	0.000380
unknown	40198/udp	0.000518
unknown	40207/udp	0.000518
unknown	40211/udp	0.000518
unknown	40216/udp	0.000518
unknown	40218/udp	0.000518
unknown	40224/udp	0.000518
unknown	40249/udp	0.000518
unknown	40250/udp	0.000518
unknown	40251/udp	0.000518
unknown	40266/udp	0.001036
unknown	40268/udp	0.000518
unknown	40270/udp	0.000518
unknown	40287/udp	0.000518
unknown	40291/udp	0.000518
unknown	40293/udp	0.000518
unknown	40299/udp	0.000518
unknown	40301/udp	0.000518
unknown	40303/udp	0.001036
unknown	40306/tcp	0.000076
unknown	40308/udp	0.000518
unknown	40310/udp	0.000518
unknown	40315/udp	0.000518
unknown	40319/udp	0.000518
unknown	40320/udp	0.000518
unknown	40322/udp	0.001036
unknown	40328/udp	0.000518
unknown	40329/udp	0.000518
unknown	40335/udp	0.000518
unknown	40337/udp	0.000518
unknown	40346/udp	0.000518
unknown	40348/udp	0.000518
unknown	40349/udp	0.000518
unknown	40351/udp	0.001036
unknown	40355/udp	0.000518
unknown	40360/udp	0.000518
unknown	40361/udp	0.000518
unknown	40364/udp	0.000518
unknown	40369/udp	0.000518
unknown	40377/udp	0.000518
unknown	40387/udp	0.000518
unknown	40393/tcp	0.000076
unknown	40396/udp	0.000518
unknown	40398/udp	0.000518
unknown	40399/udp	0.001036
unknown	40400/tcp	0.000076
unknown	40400/udp	0.000518
unknown	40402/udp	0.000518
sptx	40404/tcp	0.000000	# Simplify Printing TX
unknown	40411/udp	0.000518
unknown	40415/udp	0.000518
unknown	40418/udp	0.000518
unknown	40423/udp	0.001036
unknown	40433/udp	0.000518
unknown	40436/udp	0.001036
unknown	40441/udp	0.002071
unknown	40448/udp	0.000518
unknown	40450/udp	0.000518
unknown	40451/udp	0.000518
unknown	40452/udp	0.000518
unknown	40453/udp	0.001036
unknown	40456/udp	0.000518
unknown	40457/tcp	0.000076
unknown	40460/udp	0.000518
unknown	40462/udp	0.000518
unknown	40464/udp	0.000518
unknown	40480/udp	0.001036
unknown	40486/udp	0.000518
unknown	40487/udp	0.001036
unknown	40489/tcp	0.000076
unknown	40489/udp	0.000518
unknown	40491/udp	0.001036
unknown	40492/udp	0.000518
unknown	40499/udp	0.000518
unknown	40512/udp	0.001036
unknown	40513/tcp	0.000076
unknown	40515/udp	0.000518
unknown	40517/udp	0.000518
unknown	40522/udp	0.000518
unknown	40530/udp	0.000518
unknown	40538/udp	0.000518
unknown	40539/udp	0.001554
unknown	40542/udp	0.000518
unknown	40543/udp	0.000518
unknown	40551/udp	0.001036
unknown	40554/udp	0.000518
unknown	40564/udp	0.000518
unknown	40566/udp	0.000518
unknown	40571/udp	0.000518
unknown	40574/udp	0.000518
unknown	40580/udp	0.001036
unknown	40581/udp	0.000518
unknown	40584/udp	0.000518
unknown	40586/udp	0.000518
unknown	40591/udp	0.001036
unknown	40594/udp	0.000518
unknown	40606/udp	0.000518
unknown	40607/udp	0.000518
unknown	40611/udp	0.000518
unknown	40613/udp	0.000518
unknown	40614/tcp	0.000076
unknown	40622/udp	0.001554
unknown	40625/udp	0.001036
unknown	40628/tcp	0.000076
unknown	40639/udp	0.000518
unknown	40642/udp	0.001036
unknown	40643/udp	0.000518
unknown	40649/udp	0.000518
unknown	40653/udp	0.001036
unknown	40656/udp	0.000518
unknown	40657/udp	0.000518
unknown	40667/udp	0.001036
unknown	40669/udp	0.000518
unknown	40670/udp	0.000518
unknown	40672/udp	0.000518
unknown	40674/udp	0.000518
unknown	40676/udp	0.000518
unknown	40683/udp	0.000518
unknown	40687/udp	0.000518
unknown	40693/udp	0.000518
unknown	40694/udp	0.000518
unknown	40696/udp	0.000518
unknown	40697/udp	0.000518
unknown	40698/udp	0.000518
unknown	40700/udp	0.000518
unknown	40706/udp	0.000518
unknown	40707/udp	0.000518
unknown	40708/udp	0.002071
unknown	40711/udp	0.001554
unknown	40712/tcp	0.000076
unknown	40713/udp	0.000518
unknown	40719/udp	0.000518
unknown	40721/udp	0.000518
unknown	40722/udp	0.001036
unknown	40724/udp	0.001554
unknown	40726/udp	0.000518
unknown	40732/tcp	0.000076
unknown	40732/udp	0.002071
unknown	40734/udp	0.000518
unknown	40735/udp	0.000518
unknown	40736/udp	0.001036
unknown	40750/udp	0.000518
unknown	40751/udp	0.000518
unknown	40754/tcp	0.000076
unknown	40755/udp	0.000518
unknown	40757/udp	0.000518
unknown	40758/udp	0.000518
unknown	40764/udp	0.000518
unknown	40766/udp	0.000518
unknown	40773/udp	0.000518
unknown	40774/udp	0.000518
unknown	40787/udp	0.000518
unknown	40792/udp	0.000518
unknown	40793/udp	0.000518
unknown	40794/udp	0.000518
unknown	40803/udp	0.000518
unknown	40805/udp	0.001554
unknown	40811/tcp	0.000152
unknown	40812/tcp	0.000076
unknown	40817/udp	0.000518
unknown	40826/udp	0.000518
unknown	40830/udp	0.001036
unknown	40834/tcp	0.000076
cscp	40841/tcp	0.000000
cscp	40841/udp	0.000518
csccredir	40842/tcp	0.000000
csccredir	40842/udp	0.000000
csccfirewall	40843/tcp	0.000000
csccfirewall	40843/udp	0.000000
unknown	40844/udp	0.000518
unknown	40847/udp	0.001554
unknown	40849/udp	0.000518
unknown	40851/udp	0.000518
ortec-disc	40853/tcp	0.000000	# ORTEC Service Discovery
ortec-disc	40853/udp	0.000000	# ORTEC Service Discovery
unknown	40864/udp	0.000518
unknown	40866/udp	0.001554
unknown	40871/udp	0.000518
unknown	40877/udp	0.001036
unknown	40881/udp	0.000518
unknown	40882/udp	0.001036
unknown	40888/udp	0.000518
unknown	40893/udp	0.001036
unknown	40894/udp	0.000518
unknown	40897/udp	0.000518
unknown	40898/udp	0.000518
unknown	40904/udp	0.001036
unknown	40905/udp	0.000518
unknown	40909/udp	0.000518
unknown	40911/tcp	0.000228
unknown	40914/udp	0.001036
unknown	40915/udp	0.002071
unknown	40923/udp	0.000518
unknown	40938/udp	0.000518
unknown	40940/udp	0.001036
unknown	40946/udp	0.000518
unknown	40951/tcp	0.000076
unknown	40954/udp	0.000518
unknown	40958/udp	0.001036
unknown	40962/udp	0.000518
unknown	40963/udp	0.000518
unknown	40970/udp	0.000518
unknown	40972/udp	0.001036
unknown	40982/udp	0.001036
unknown	40991/udp	0.000518
unknown	40993/udp	0.001036
unknown	41011/udp	0.001036
unknown	41014/udp	0.001036
unknown	41015/udp	0.000518
unknown	41018/udp	0.000518
unknown	41020/udp	0.000518
unknown	41033/udp	0.000518
unknown	41036/udp	0.000518
unknown	41039/udp	0.000518
unknown	41042/udp	0.000518
unknown	41049/udp	0.000518
unknown	41053/udp	0.000518
unknown	41057/udp	0.000518
unknown	41058/udp	0.003107
unknown	41064/tcp	0.000152
unknown	41065/udp	0.000518
unknown	41070/udp	0.000518
unknown	41073/udp	0.001036
unknown	41075/udp	0.000518
unknown	41078/udp	0.000518
unknown	41081/udp	0.002071
unknown	41082/udp	0.000518
unknown	41086/udp	0.000518
fs-qos	41111/tcp	0.000000	# Foursticks QoS Protocol
fs-qos	41111/udp	0.000000	# Foursticks QoS Protocol
unknown	41113/udp	0.000518
tentacle	41121/tcp	0.000000	# Tentacle Server
unknown	41121/udp	0.000518
unknown	41123/tcp	0.000076
unknown	41123/udp	0.000518
unknown	41130/udp	0.000518
unknown	41135/udp	0.000518
unknown	41139/udp	0.001036
unknown	41141/udp	0.000518
unknown	41142/tcp	0.000076
unknown	41148/udp	0.001036
unknown	41149/udp	0.001036
unknown	41150/udp	0.000518
unknown	41151/udp	0.000518
unknown	41154/udp	0.000518
unknown	41156/udp	0.001036
unknown	41161/udp	0.001036
unknown	41169/udp	0.000518
unknown	41170/udp	0.000518
unknown	41171/udp	0.000518
unknown	41172/udp	0.000518
unknown	41203/udp	0.000518
unknown	41207/udp	0.000518
unknown	41226/udp	0.000518
z-wave-s	41230/tcp	0.000000	# Z-Wave Protocol over SSL/TLS | Z-Wave Protocol over DTLS
unknown	41232/udp	0.000518
unknown	41233/udp	0.000518
unknown	41237/udp	0.000518
unknown	41245/udp	0.000518
unknown	41250/tcp	0.000076
unknown	41251/udp	0.000518
unknown	41252/udp	0.000518
unknown	41254/udp	0.000518
unknown	41262/udp	0.000518
unknown	41264/udp	0.000518
unknown	41265/udp	0.001036
unknown	41274/udp	0.000518
unknown	41278/udp	0.000518
unknown	41281/tcp	0.000076
unknown	41283/udp	0.000518
unknown	41289/udp	0.000518
unknown	41295/udp	0.000518
unknown	41308/udp	0.001554
unknown	41309/udp	0.000518
unknown	41318/tcp	0.000076
unknown	41319/udp	0.000518
unknown	41320/udp	0.000518
unknown	41327/udp	0.001036
unknown	41330/udp	0.000518
unknown	41332/udp	0.000518
unknown	41334/udp	0.001036
unknown	41335/udp	0.001036
unknown	41337/udp	0.000518
unknown	41342/tcp	0.000076
unknown	41343/udp	0.001036
unknown	41345/tcp	0.000076
unknown	41348/tcp	0.000076
unknown	41348/udp	0.001036
unknown	41351/udp	0.000518
unknown	41353/udp	0.000518
unknown	41356/udp	0.000518
unknown	41359/udp	0.000518
unknown	41360/udp	0.001036
unknown	41369/udp	0.000518
unknown	41370/udp	0.002071
unknown	41376/udp	0.000518
unknown	41379/udp	0.000518
unknown	41380/udp	0.001036
unknown	41381/udp	0.000518
unknown	41384/udp	0.000518
unknown	41387/udp	0.000518
unknown	41393/udp	0.000518
unknown	41398/tcp	0.000076
unknown	41401/udp	0.000518
unknown	41406/udp	0.001036
unknown	41407/udp	0.000518
unknown	41408/udp	0.000518
unknown	41410/udp	0.000518
unknown	41414/udp	0.000518
unknown	41415/udp	0.000518
unknown	41416/udp	0.000518
unknown	41425/udp	0.000518
unknown	41430/udp	0.000518
unknown	41435/udp	0.000518
unknown	41436/udp	0.000518
unknown	41439/udp	0.000518
unknown	41441/udp	0.000518
unknown	41442/tcp	0.000076
unknown	41446/udp	0.001554
unknown	41448/udp	0.000518
unknown	41450/udp	0.000518
unknown	41458/udp	0.000518
unknown	41463/udp	0.000518
unknown	41464/udp	0.000518
unknown	41470/udp	0.000518
unknown	41474/udp	0.000518
unknown	41475/udp	0.000518
unknown	41479/udp	0.000518
unknown	41484/udp	0.000518
unknown	41485/udp	0.000518
unknown	41494/udp	0.000518
unknown	41496/udp	0.001036
unknown	41497/udp	0.000518
unknown	41498/udp	0.000518
unknown	41499/udp	0.001036
unknown	41504/udp	0.000518
unknown	41507/udp	0.000518
unknown	41511/tcp	0.000228
unknown	41514/udp	0.000518
unknown	41515/udp	0.000518
unknown	41518/udp	0.000518
unknown	41523/tcp	0.000152
unknown	41524/udp	0.005697
unknown	41543/udp	0.000518
unknown	41544/udp	0.000518
unknown	41545/udp	0.000518
unknown	41546/udp	0.000518
unknown	41549/udp	0.000518
unknown	41551/tcp	0.000076
unknown	41551/udp	0.000518
unknown	41554/udp	0.000518
unknown	41562/udp	0.000518
unknown	41564/udp	0.000518
unknown	41565/udp	0.000518
unknown	41568/udp	0.000518
unknown	41570/udp	0.000518
unknown	41571/udp	0.000518
unknown	41574/udp	0.000518
unknown	41584/udp	0.000518
unknown	41589/udp	0.000518
unknown	41596/udp	0.000518
unknown	41602/udp	0.000518
unknown	41606/udp	0.000518
unknown	41610/udp	0.000518
unknown	41616/udp	0.000518
unknown	41617/udp	0.000518
unknown	41619/udp	0.001036
unknown	41620/udp	0.000518
unknown	41631/udp	0.000518
unknown	41632/tcp	0.000076
unknown	41632/udp	0.000518
unknown	41633/udp	0.000518
unknown	41635/udp	0.000518
unknown	41636/udp	0.000518
unknown	41637/udp	0.000518
unknown	41638/udp	0.001554
unknown	41641/udp	0.000518
unknown	41645/udp	0.000518
unknown	41656/udp	0.000518
unknown	41659/udp	0.000518
unknown	41667/udp	0.000518
unknown	41672/udp	0.000518
unknown	41674/udp	0.000518
unknown	41675/udp	0.000518
unknown	41676/udp	0.000518
unknown	41680/udp	0.000518
unknown	41684/udp	0.000518
unknown	41702/udp	0.001554
unknown	41709/udp	0.000518
unknown	41710/udp	0.000518
unknown	41711/udp	0.000518
unknown	41717/udp	0.001036
unknown	41718/udp	0.000518
unknown	41721/udp	0.000518
unknown	41730/udp	0.000518
unknown	41731/udp	0.001036
unknown	41742/udp	0.000518
unknown	41761/udp	0.000518
unknown	41763/udp	0.000518
unknown	41771/udp	0.001036
unknown	41773/tcp	0.000076
unknown	41773/udp	0.000518
unknown	41774/udp	0.001554
unknown	41778/udp	0.000518
unknown	41779/udp	0.001036
unknown	41780/udp	0.000518
unknown	41781/udp	0.000518
unknown	41785/udp	0.000518
crestron-cip	41794/tcp	0.000076	# Crestron Control Port
crestron-cip	41794/udp	0.000000	# Crestron Control Port
crestron-ctp	41795/tcp	0.000076	# Crestron Terminal Port
crestron-ctp	41795/udp	0.000000	# Crestron Terminal Port
crestron-cips	41796/tcp	0.000000	# Crestron Secure Control Port
crestron-ctps	41797/tcp	0.000000	# Crestron Secure Terminal Port
unknown	41799/udp	0.000518
unknown	41800/udp	0.000518
unknown	41801/udp	0.000518
unknown	41806/udp	0.000518
unknown	41807/udp	0.000518
unknown	41808/tcp	0.000076
unknown	41810/udp	0.000518
unknown	41815/udp	0.000518
unknown	41816/udp	0.001036
unknown	41829/udp	0.000518
unknown	41837/udp	0.001036
unknown	41846/udp	0.000518
unknown	41849/udp	0.000518
unknown	41850/udp	0.000518
unknown	41851/udp	0.001036
unknown	41860/udp	0.000518
unknown	41865/udp	0.000518
unknown	41867/udp	0.000518
unknown	41868/udp	0.000518
unknown	41875/udp	0.001036
unknown	41876/udp	0.000518
unknown	41886/udp	0.000518
unknown	41896/udp	0.001554
unknown	41901/udp	0.000518
unknown	41914/udp	0.000518
unknown	41916/udp	0.000518
unknown	41927/udp	0.000518
unknown	41930/udp	0.000518
unknown	41933/udp	0.000518
unknown	41937/udp	0.000518
unknown	41947/udp	0.000518
unknown	41950/udp	0.000518
unknown	41954/udp	0.000518
unknown	41955/udp	0.000518
unknown	41964/udp	0.000518
unknown	41967/udp	0.001554
unknown	41968/udp	0.000518
unknown	41971/udp	0.001554
unknown	41972/udp	0.000518
unknown	41975/udp	0.000518
unknown	41978/udp	0.000518
unknown	41982/udp	0.000518
unknown	41987/udp	0.000518
unknown	41990/udp	0.000518
unknown	41999/udp	0.000518
unknown	42001/tcp	0.000076
unknown	42005/udp	0.001036
unknown	42006/udp	0.000518
unknown	42021/udp	0.000518
unknown	42022/udp	0.000518
unknown	42029/udp	0.000518
unknown	42031/udp	0.000518
unknown	42032/udp	0.000518
unknown	42034/udp	0.000518
unknown	42035/tcp	0.000076
unknown	42046/udp	0.000518
unknown	42048/udp	0.000518
unknown	42051/udp	0.001036
unknown	42054/udp	0.000518
unknown	42056/udp	0.001554
unknown	42067/udp	0.000518
unknown	42072/udp	0.000518
unknown	42081/udp	0.000518
unknown	42085/udp	0.000518
unknown	42088/udp	0.000518
unknown	42093/udp	0.000518
unknown	42096/udp	0.000518
unknown	42100/udp	0.000518
unknown	42101/udp	0.000518
unknown	42112/udp	0.000518
unknown	42123/udp	0.000518
unknown	42126/udp	0.000518
unknown	42127/tcp	0.000076
unknown	42133/udp	0.000518
unknown	42135/udp	0.000518
unknown	42139/udp	0.001036
unknown	42141/udp	0.000518
unknown	42148/udp	0.001036
unknown	42155/udp	0.000518
unknown	42158/tcp	0.000076
unknown	42158/udp	0.000518
unknown	42159/udp	0.000518
unknown	42162/udp	0.000518
unknown	42163/udp	0.000518
unknown	42168/udp	0.000518
unknown	42172/udp	0.002589
unknown	42173/udp	0.000518
unknown	42179/udp	0.000518
unknown	42190/udp	0.000518
unknown	42197/udp	0.000518
unknown	42198/udp	0.000518
unknown	42199/udp	0.000518
unknown	42215/udp	0.001036
unknown	42220/udp	0.001036
unknown	42224/udp	0.000518
unknown	42235/udp	0.000518
unknown	42251/tcp	0.000076
unknown	42251/udp	0.001036
unknown	42262/udp	0.000518
unknown	42276/tcp	0.000076
unknown	42279/udp	0.001036
unknown	42280/udp	0.000518
unknown	42281/udp	0.000518
unknown	42283/udp	0.000518
unknown	42284/udp	0.001036
unknown	42285/udp	0.001036
unknown	42294/udp	0.001036
unknown	42298/udp	0.000518
unknown	42302/udp	0.000518
unknown	42312/udp	0.000518
unknown	42313/udp	0.001554
unknown	42318/udp	0.000518
unknown	42322/tcp	0.000076
unknown	42325/udp	0.000518
unknown	42328/udp	0.000518
unknown	42332/udp	0.000518
unknown	42338/udp	0.000518
unknown	42340/udp	0.001036
unknown	42341/udp	0.001036
unknown	42343/udp	0.000518
unknown	42350/udp	0.000518
unknown	42368/udp	0.000518
unknown	42373/udp	0.001036
unknown	42379/udp	0.000518
unknown	42380/udp	0.000518
unknown	42383/udp	0.000518
unknown	42393/udp	0.000518
unknown	42394/udp	0.000518
unknown	42409/udp	0.000518
unknown	42411/udp	0.000518
unknown	42417/udp	0.000518
unknown	42422/udp	0.000518
unknown	42423/udp	0.000518
unknown	42425/udp	0.000518
unknown	42426/udp	0.000518
unknown	42428/udp	0.000518
unknown	42429/udp	0.000518
unknown	42431/udp	0.001554
unknown	42434/udp	0.001554
unknown	42445/udp	0.000518
unknown	42449/tcp	0.000076
unknown	42452/tcp	0.000076
unknown	42456/udp	0.000518
unknown	42459/udp	0.000518
unknown	42463/udp	0.000518
unknown	42465/udp	0.000518
unknown	42471/udp	0.000518
unknown	42478/udp	0.000518
unknown	42482/udp	0.000518
unknown	42484/udp	0.000518
unknown	42498/udp	0.001036
unknown	42504/udp	0.000518
unknown	42506/udp	0.000518
candp	42508/tcp	0.000000	# Computer Associates network discovery protocol
candp	42508/udp	0.002071	# Computer Associates network discovery protocol
candrp	42509/tcp	0.000000	# CA discovery response
candrp	42509/udp	0.000000	# CA discovery response
caerpc	42510/tcp	0.000988	# CA eTrust RPC
caerpc	42510/udp	0.000000	# CA eTrust RPC
unknown	42512/udp	0.000518
unknown	42522/udp	0.000518
unknown	42533/udp	0.001036
unknown	42534/udp	0.000518
unknown	42535/udp	0.000518
unknown	42545/udp	0.000518
unknown	42546/udp	0.000518
unknown	42551/udp	0.000518
unknown	42557/udp	0.001554
unknown	42558/udp	0.001036
unknown	42559/tcp	0.000076
unknown	42560/tcp	0.000076
unknown	42562/udp	0.000518
unknown	42571/udp	0.000518
unknown	42575/tcp	0.000076
unknown	42577/udp	0.001554
unknown	42584/udp	0.000518
unknown	42585/udp	0.001036
unknown	42590/tcp	0.000076
unknown	42591/udp	0.000518
unknown	42606/udp	0.000518
unknown	42608/udp	0.000518
unknown	42610/udp	0.000518
unknown	42612/udp	0.001036
unknown	42618/udp	0.000518
unknown	42621/udp	0.000518
unknown	42622/udp	0.000518
unknown	42624/udp	0.000518
unknown	42625/udp	0.000518
unknown	42627/udp	0.001554
unknown	42632/tcp	0.000076
unknown	42632/udp	0.000518
unknown	42633/udp	0.000518
unknown	42634/udp	0.000518
unknown	42638/udp	0.001036
unknown	42639/udp	0.001554
unknown	42644/udp	0.000518
unknown	42648/udp	0.001036
unknown	42651/udp	0.000518
unknown	42652/udp	0.000518
unknown	42664/udp	0.000518
unknown	42666/udp	0.000518
unknown	42668/udp	0.000518
unknown	42671/udp	0.000518
unknown	42672/udp	0.000518
unknown	42674/udp	0.000518
unknown	42675/tcp	0.000076
unknown	42677/udp	0.000518
unknown	42679/tcp	0.000076
unknown	42681/udp	0.000518
unknown	42684/udp	0.000518
unknown	42685/tcp	0.000076
unknown	42687/udp	0.000518
unknown	42695/udp	0.000518
unknown	42699/udp	0.000518
unknown	42702/udp	0.001036
unknown	42706/udp	0.000518
unknown	42708/udp	0.001036
unknown	42716/udp	0.001036
unknown	42717/udp	0.000518
unknown	42721/udp	0.000518
unknown	42734/udp	0.000518
unknown	42735/tcp	0.000076
unknown	42741/udp	0.000518
unknown	42747/udp	0.000518
unknown	42762/udp	0.000518
unknown	42763/udp	0.000518
unknown	42773/udp	0.001036
unknown	42776/udp	0.000518
unknown	42784/udp	0.000518
unknown	42791/udp	0.000518
unknown	42796/udp	0.000518
unknown	42799/udp	0.000518
unknown	42800/udp	0.000518
unknown	42803/udp	0.001036
unknown	42804/udp	0.000518
unknown	42807/udp	0.001036
unknown	42811/udp	0.000518
unknown	42812/udp	0.001036
unknown	42815/udp	0.000518
unknown	42816/udp	0.000518
unknown	42819/udp	0.000518
unknown	42822/udp	0.000518
unknown	42823/udp	0.000518
unknown	42825/udp	0.001036
unknown	42827/udp	0.001036
unknown	42828/udp	0.000518
unknown	42831/udp	0.000518
unknown	42832/udp	0.000518
unknown	42837/udp	0.000518
unknown	42843/udp	0.000518
unknown	42849/udp	0.000518
unknown	42857/udp	0.001036
unknown	42859/udp	0.000518
unknown	42863/udp	0.000518
unknown	42864/udp	0.000518
unknown	42868/udp	0.001036
unknown	42869/udp	0.000518
unknown	42870/udp	0.000518
unknown	42874/udp	0.000518
unknown	42875/udp	0.000518
unknown	42877/udp	0.000518
unknown	42880/udp	0.000518
unknown	42882/udp	0.001036
unknown	42886/udp	0.000518
unknown	42887/udp	0.000518
unknown	42893/udp	0.000518
unknown	42902/udp	0.000518
unknown	42903/udp	0.000518
unknown	42904/udp	0.000518
unknown	42906/tcp	0.000076
unknown	42906/udp	0.000518
unknown	42910/udp	0.000518
unknown	42916/udp	0.001036
unknown	42923/udp	0.000518
unknown	42940/udp	0.000518
unknown	42941/udp	0.001036
unknown	42945/udp	0.000518
unknown	42946/udp	0.000518
unknown	42947/udp	0.000518
unknown	42949/udp	0.000518
unknown	42950/udp	0.000518
unknown	42951/udp	0.000518
unknown	42955/udp	0.000518
unknown	42960/udp	0.000518
unknown	42961/udp	0.000518
unknown	42965/udp	0.000518
unknown	42974/udp	0.000518
unknown	42975/udp	0.000518
unknown	42986/udp	0.000518
unknown	42990/tcp	0.000076
curiosity	42999/tcp	0.000000	# API endpoint for search application
recvr-rc	43000/tcp	0.000076	# recvr-rc-disc | Receiver Remote Control | Receiver Remote Control Discovery
unknown	43002/tcp	0.000076
unknown	43002/udp	0.000518
unknown	43005/udp	0.000518
unknown	43009/udp	0.000518
unknown	43011/udp	0.000518
unknown	43014/udp	0.000518
unknown	43018/tcp	0.000076
unknown	43024/udp	0.000518
unknown	43027/tcp	0.000076
unknown	43032/udp	0.000518
unknown	43036/udp	0.000518
unknown	43039/udp	0.001036
unknown	43054/udp	0.000518
unknown	43057/udp	0.000518
unknown	43064/udp	0.000518
unknown	43069/udp	0.000518
unknown	43070/udp	0.000518
unknown	43072/udp	0.001036
unknown	43074/udp	0.000518
unknown	43080/udp	0.001036
unknown	43085/udp	0.000518
unknown	43086/udp	0.000518
unknown	43091/udp	0.000518
unknown	43092/udp	0.001036
unknown	43094/udp	0.001554
unknown	43103/tcp	0.000076
unknown	43106/udp	0.000518
unknown	43108/udp	0.000518
unknown	43121/udp	0.000518
unknown	43122/udp	0.000518
unknown	43126/udp	0.000518
unknown	43128/udp	0.000518
unknown	43129/udp	0.000518
unknown	43131/udp	0.000518
unknown	43139/tcp	0.000076
unknown	43139/udp	0.000518
unknown	43141/udp	0.000518
unknown	43143/tcp	0.000076
unknown	43145/udp	0.000518
unknown	43146/udp	0.000518
unknown	43147/udp	0.000518
unknown	43150/udp	0.000518
unknown	43157/udp	0.000518
unknown	43170/udp	0.001036
unknown	43171/udp	0.000518
unknown	43173/udp	0.001036
unknown	43175/udp	0.001036
unknown	43185/udp	0.000518
reachout	43188/tcp	0.000013
reachout	43188/udp	0.000000
ndm-agent-port	43189/tcp	0.000000
ndm-agent-port	43189/udp	0.000000
ip-provision	43190/tcp	0.000000
ip-provision	43190/udp	0.000000
noit-transport	43191/tcp	0.000000	# Reconnoiter Agent Data Transport
unknown	43195/udp	0.001554
shaperai	43210/tcp	0.000000	# shaperai-disc | Shaper Automation Server Management | Shaper Automation Server Management Discovery
unknown	43212/tcp	0.000076
unknown	43216/udp	0.000518
unknown	43225/udp	0.000518
unknown	43231/tcp	0.000076
unknown	43237/udp	0.000518
unknown	43242/tcp	0.000076
unknown	43248/udp	0.001036
unknown	43249/udp	0.000518
unknown	43254/udp	0.000518
unknown	43256/udp	0.000518
unknown	43257/udp	0.000518
unknown	43260/udp	0.001036
unknown	43268/udp	0.001036
unknown	43279/udp	0.000518
unknown	43280/udp	0.000518
unknown	43283/udp	0.000518
unknown	43284/udp	0.001036
unknown	43285/udp	0.000518
unknown	43288/udp	0.001036
unknown	43289/udp	0.000518
unknown	43295/udp	0.000518
unknown	43304/udp	0.000518
unknown	43306/udp	0.000518
unknown	43316/udp	0.000518
unknown	43317/udp	0.000518
unknown	43320/udp	0.000518
unknown	43322/udp	0.000518
unknown	43323/udp	0.000518
unknown	43326/udp	0.000518
unknown	43327/udp	0.000518
unknown	43334/udp	0.001036
unknown	43336/udp	0.001036
unknown	43355/udp	0.000518
unknown	43359/udp	0.000518
unknown	43360/udp	0.000518
unknown	43361/udp	0.001036
unknown	43370/udp	0.001554
unknown	43372/udp	0.000518
unknown	43376/udp	0.000518
unknown	43382/udp	0.000518
unknown	43403/udp	0.000518
unknown	43414/udp	0.000518
unknown	43418/udp	0.000518
unknown	43420/udp	0.000518
unknown	43422/udp	0.000518
unknown	43423/udp	0.001036
unknown	43425/tcp	0.000076
unknown	43432/udp	0.000518
hmip-routing	43438/tcp	0.000000	# HmIP LAN Routing
eq3-update	43439/tcp	0.000000	# eq3-config | EQ3 firmware update | EQ3 discovery and configuration
ew-mgmt	43440/tcp	0.000000	# ew-disc-cmd | Cisco EnergyWise Management | Cisco EnergyWise Discovery and Command Flooding
ew-disc-cmd	43440/udp	0.000000	# Cisco EnergyWise Discovery and Command Flooding
ciscocsdb	43441/tcp	0.000000	# Cisco NetMgmt DB Ports
ciscocsdb	43441/udp	0.000000	# Cisco NetMgmt DB Ports
unknown	43446/udp	0.000518
unknown	43455/udp	0.001036
unknown	43464/udp	0.000518
unknown	43472/udp	0.000518
unknown	43474/udp	0.000518
unknown	43477/udp	0.000518
unknown	43485/udp	0.000518
unknown	43491/udp	0.000518
unknown	43503/udp	0.000518
unknown	43505/udp	0.000518
unknown	43506/udp	0.000518
unknown	43510/udp	0.001036
unknown	43511/udp	0.000518
unknown	43514/udp	0.001554
unknown	43523/udp	0.000518
unknown	43525/udp	0.001036
unknown	43527/udp	0.000518
unknown	43544/udp	0.000518
unknown	43547/udp	0.000518
unknown	43550/udp	0.000518
unknown	43552/udp	0.000518
unknown	43553/udp	0.000518
unknown	43558/udp	0.000518
unknown	43589/udp	0.000518
unknown	43590/udp	0.000518
unknown	43594/udp	0.000518
unknown	43600/udp	0.000518
unknown	43601/udp	0.000518
unknown	43608/udp	0.000518
unknown	43610/udp	0.000518
unknown	43613/udp	0.000518
unknown	43617/udp	0.000518
unknown	43632/udp	0.000518
unknown	43640/udp	0.001036
unknown	43653/udp	0.000518
unknown	43654/tcp	0.000076
unknown	43670/udp	0.000518
unknown	43679/udp	0.000518
unknown	43684/udp	0.000518
unknown	43686/udp	0.001554
unknown	43690/tcp	0.000076
unknown	43697/udp	0.000518
unknown	43707/udp	0.000518
unknown	43709/udp	0.000518
unknown	43710/udp	0.000518
unknown	43713/udp	0.000518
unknown	43715/udp	0.001036
unknown	43719/udp	0.000518
unknown	43723/udp	0.000518
unknown	43724/udp	0.000518
unknown	43725/udp	0.000518
unknown	43734/tcp	0.000076
unknown	43735/udp	0.000518
unknown	43739/udp	0.000518
unknown	43740/udp	0.001036
unknown	43756/udp	0.000518
unknown	43774/udp	0.000518
unknown	43781/udp	0.000518
unknown	43785/udp	0.000518
unknown	43786/udp	0.000518
unknown	43788/udp	0.000518
unknown	43791/udp	0.000518
unknown	43794/udp	0.000518
unknown	43798/udp	0.000518
unknown	43799/udp	0.000518
unknown	43802/udp	0.001036
unknown	43803/udp	0.000518
unknown	43805/udp	0.000518
unknown	43811/udp	0.000518
unknown	43812/udp	0.000518
unknown	43814/udp	0.000518
unknown	43816/udp	0.000518
unknown	43823/tcp	0.000076
unknown	43823/udp	0.000518
unknown	43824/udp	0.001554
unknown	43835/udp	0.000518
unknown	43836/udp	0.000518
unknown	43837/udp	0.000518
unknown	43841/udp	0.000518
unknown	43842/udp	0.001036
unknown	43843/udp	0.000518
unknown	43844/udp	0.000518
unknown	43845/udp	0.000518
unknown	43847/udp	0.000518
unknown	43850/udp	0.000518
unknown	43854/udp	0.000518
unknown	43859/udp	0.000518
unknown	43861/udp	0.000518
unknown	43868/tcp	0.000076
unknown	43870/udp	0.000518
unknown	43881/udp	0.000518
unknown	43891/udp	0.000518
unknown	43901/udp	0.000518
unknown	43905/udp	0.000518
unknown	43910/udp	0.000518
unknown	43913/udp	0.000518
unknown	43923/udp	0.000518
unknown	43928/udp	0.000518
unknown	43941/udp	0.001036
unknown	43942/udp	0.001036
unknown	43954/udp	0.000518
unknown	43956/udp	0.000518
unknown	43961/udp	0.000518
unknown	43967/udp	0.001554
unknown	43973/udp	0.000518
unknown	43977/udp	0.000518
unknown	43983/udp	0.001036
unknown	43986/udp	0.000518
unknown	43991/udp	0.000518
unknown	43994/udp	0.000518
unknown	44004/tcp	0.000076
unknown	44009/udp	0.001036
unknown	44010/udp	0.000518
unknown	44013/udp	0.000518
unknown	44021/udp	0.000518
unknown	44024/udp	0.000518
unknown	44026/udp	0.001036
unknown	44032/udp	0.000518
unknown	44034/udp	0.001036
unknown	44035/udp	0.000518
unknown	44037/udp	0.001036
unknown	44040/udp	0.000518
unknown	44042/udp	0.000518
unknown	44048/udp	0.000518
unknown	44054/udp	0.001036
unknown	44056/udp	0.000518
unknown	44058/udp	0.000518
unknown	44059/udp	0.000518
unknown	44061/udp	0.000518
unknown	44075/udp	0.000518
unknown	44076/udp	0.000518
unknown	44079/udp	0.001036
unknown	44080/udp	0.000518
unknown	44087/udp	0.000518
unknown	44090/udp	0.000518
unknown	44093/udp	0.001036
unknown	44094/udp	0.000518
unknown	44098/udp	0.000518
unknown	44099/udp	0.001036
unknown	44100/udp	0.001036
unknown	44101/tcp	0.000076
unknown	44101/udp	0.001554
unknown	44107/udp	0.000518
unknown	44109/udp	0.000518
unknown	44115/udp	0.000518
unknown	44116/udp	0.001036
unknown	44117/udp	0.001036
unknown	44119/tcp	0.000076
unknown	44119/udp	0.000518
z-wave-tunnel	44123/tcp	0.000000	# Z-Wave Secure Tunnel
unknown	44126/udp	0.000518
unknown	44129/udp	0.000518
unknown	44135/udp	0.001036
unknown	44139/udp	0.000518
unknown	44160/udp	0.001554
unknown	44164/udp	0.000518
unknown	44166/udp	0.000518
unknown	44176/tcp	0.000228
unknown	44176/udp	0.000518
unknown	44177/udp	0.000518
unknown	44179/udp	0.001554
unknown	44180/udp	0.000518
unknown	44185/udp	0.001554
unknown	44190/udp	0.001554
unknown	44194/udp	0.000518
unknown	44195/udp	0.000518
unknown	44200/tcp	0.000076
unknown	44200/udp	0.000518
unknown	44215/udp	0.000518
unknown	44226/udp	0.000518
unknown	44227/udp	0.000518
unknown	44234/udp	0.000518
unknown	44236/udp	0.000518
unknown	44242/udp	0.000518
unknown	44245/udp	0.000518
unknown	44253/udp	0.001554
unknown	44257/udp	0.000518
unknown	44260/udp	0.000518
unknown	44266/udp	0.000518
unknown	44268/udp	0.000518
unknown	44275/udp	0.001036
unknown	44277/udp	0.000518
unknown	44282/udp	0.000518
unknown	44293/udp	0.000518
unknown	44299/udp	0.000518
unknown	44310/udp	0.001036
unknown	44312/udp	0.001036
unknown	44313/udp	0.000518
pmcd	44321/tcp	0.000000	# PCP server (pmcd)
pmcd	44321/udp	0.000000	# PCP server (pmcd)
pmcdproxy	44322/tcp	0.000000	# PCP server (pmcd) proxy
pmcdproxy	44322/udp	0.000000	# PCP server (pmcd) proxy
pmwebapi	44323/tcp	0.000000	# HTTP binding for Performance Co-Pilot client API
unknown	44324/udp	0.000518
unknown	44327/udp	0.000518
unknown	44328/udp	0.000518
unknown	44332/udp	0.000518
tinyfw	44334/tcp	0.000088	# tiny personal firewall admin port
unknown	44334/udp	0.001554
unknown	44336/udp	0.000518
unknown	44339/udp	0.000518
unknown	44342/udp	0.000518
unknown	44349/udp	0.000518
unknown	44357/udp	0.000518
unknown	44364/udp	0.001036
unknown	44367/udp	0.000518
unknown	44371/udp	0.001036
unknown	44373/udp	0.000518
unknown	44376/udp	0.000518
unknown	44380/tcp	0.000076
unknown	44390/udp	0.000518
unknown	44395/udp	0.000518
unknown	44396/udp	0.000518
unknown	44402/udp	0.000518
unknown	44403/udp	0.000518
unknown	44408/udp	0.001036
unknown	44409/udp	0.000518
unknown	44410/tcp	0.000076
unknown	44411/udp	0.000518
unknown	44415/udp	0.000518
unknown	44420/udp	0.001036
unknown	44423/udp	0.000518
unknown	44431/tcp	0.000076
unknown	44434/udp	0.000518
unknown	44439/udp	0.000518
coldfusion-auth	44442/tcp	0.000163	# ColdFusion Advanced Security/Siteminder Authentication Port (by Allaire/Netegrity)
coldfusion-auth	44443/tcp	0.000201	# ColdFusion Advanced Security/Siteminder Authentication Port (by Allaire/Netegrity)
unknown	44443/udp	0.000518
cognex-dataman	44444/tcp	0.000000	# Cognex DataMan Management Protocol
unknown	44444/udp	0.000518
acronis-backup	44445/tcp	0.000000	# Acronis Backup Gateway service port
unknown	44445/udp	0.000518
unknown	44448/udp	0.000518
unknown	44450/udp	0.000518
unknown	44452/udp	0.000518
unknown	44453/udp	0.000518
unknown	44454/udp	0.001036
unknown	44460/udp	0.000518
unknown	44466/udp	0.000518
unknown	44469/udp	0.000518
unknown	44476/udp	0.000518
unknown	44479/tcp	0.000076
unknown	44479/udp	0.000518
unknown	44483/udp	0.000518
unknown	44501/tcp	0.000228
unknown	44503/udp	0.001036
unknown	44504/udp	0.000518
unknown	44505/tcp	0.000076
unknown	44508/udp	0.001554
unknown	44509/udp	0.000518
unknown	44518/udp	0.001036
unknown	44522/udp	0.000518
unknown	44533/udp	0.000518
unknown	44534/udp	0.000518
unknown	44539/udp	0.001036
unknown	44541/tcp	0.000076
unknown	44541/udp	0.000518
unknown	44542/udp	0.000518
domiq	44544/tcp	0.000000	# DOMIQ Building Automation
rbr-debug	44553/tcp	0.000000	# REALbasic Remote Debug
rbr-debug	44553/udp	0.000000	# REALbasic Remote Debug
unknown	44557/udp	0.000518
unknown	44558/udp	0.000518
unknown	44559/udp	0.000518
unknown	44561/udp	0.000518
unknown	44577/udp	0.001036
unknown	44586/udp	0.000518
unknown	44595/udp	0.000518
unknown	44597/udp	0.000518
unknown	44598/udp	0.001036
asihpi	44600/tcp	0.000000	# AudioScience HPI
unknown	44609/udp	0.000518
unknown	44611/udp	0.001036
unknown	44612/udp	0.000518
unknown	44614/udp	0.000518
unknown	44616/tcp	0.000076
unknown	44622/udp	0.000518
unknown	44624/udp	0.000518
unknown	44628/tcp	0.000076
unknown	44630/udp	0.000518
unknown	44632/udp	0.000518
unknown	44637/udp	0.000518
unknown	44640/udp	0.000518
unknown	44652/udp	0.000518
unknown	44654/udp	0.000518
unknown	44660/udp	0.000518
unknown	44661/udp	0.001036
unknown	44667/udp	0.000518
unknown	44671/udp	0.000518
unknown	44673/udp	0.000518
unknown	44684/udp	0.000518
unknown	44693/udp	0.000518
unknown	44702/udp	0.000518
unknown	44704/tcp	0.000076
unknown	44709/tcp	0.000152
unknown	44710/udp	0.000518
unknown	44711/tcp	0.000076
unknown	44711/udp	0.000518
unknown	44713/udp	0.000518
unknown	44714/udp	0.000518
unknown	44721/udp	0.000518
unknown	44726/udp	0.000518
unknown	44727/udp	0.000518
unknown	44730/udp	0.000518
unknown	44732/udp	0.000518
unknown	44733/udp	0.001036
unknown	44736/udp	0.000518
unknown	44738/udp	0.000518
unknown	44745/udp	0.000518
unknown	44746/udp	0.000518
unknown	44748/udp	0.001036
unknown	44752/udp	0.000518
unknown	44757/udp	0.000518
unknown	44767/udp	0.000518
unknown	44774/udp	0.000518
unknown	44775/udp	0.000518
unknown	44780/udp	0.000518
unknown	44794/udp	0.000518
unknown	44800/udp	0.000518
unknown	44815/udp	0.000518
unknown	44817/udp	0.000518
EtherNetIP-2	44818/tcp	0.000000	# EtherNet/IP-2 | EtherNet-IP-2 | EtherNet/IP messaging
EtherNetIP-2	44818/udp	0.000518	# EtherNet/IP messaging
unknown	44819/udp	0.001036
unknown	44823/udp	0.000518
unknown	44831/udp	0.000518
unknown	44837/udp	0.000518
unknown	44845/udp	0.000518
unknown	44850/udp	0.000518
unknown	44851/udp	0.000518
unknown	44856/udp	0.001036
unknown	44866/udp	0.000518
unknown	44869/udp	0.000518
unknown	44871/udp	0.000518
unknown	44873/udp	0.000518
unknown	44876/udp	0.000518
unknown	44880/udp	0.000518
unknown	44885/udp	0.000518
m3da	44900/tcp	0.000000	# m3da-disc | M3DA is used for efficient machine-to-machine communications | M3DA Discovery is used for efficient machine-to-machine communications
unknown	44901/udp	0.000518
unknown	44912/udp	0.000518
unknown	44915/udp	0.000518
unknown	44917/udp	0.001036
unknown	44919/udp	0.000518
unknown	44923/udp	0.001554
unknown	44924/udp	0.000518
unknown	44927/udp	0.000518
unknown	44935/udp	0.000518
unknown	44937/udp	0.000518
unknown	44941/udp	0.000518
unknown	44943/udp	0.001036
unknown	44946/udp	0.001554
unknown	44955/udp	0.000518
unknown	44956/udp	0.000518
unknown	44958/udp	0.000518
unknown	44965/tcp	0.000076
unknown	44968/udp	0.004143
unknown	44969/udp	0.000518
unknown	44972/udp	0.000518
unknown	44973/udp	0.000518
unknown	44977/udp	0.000518
unknown	44981/tcp	0.000076
unknown	44983/udp	0.000518
unknown	44994/udp	0.000518
unknown	44999/udp	0.000518
asmp	45000/tcp	0.000000	# asmp-mon | Nuance AutoStore Status Monitoring Protocol (data transfer) | Nuance AutoStore Status Monitoring Protocol (device monitoring)
ciscopop	45000/udp	0.000839	# Cisco Postoffice Protocol for Cisco Secure IDS
asmps	45001/tcp	0.000000	# Nuance AutoStore Status Monitoring Protocol (secure data transfer)
unknown	45001/udp	0.000518
rs-status	45002/tcp	0.000000	# Redspeed Status Monitor
unknown	45006/udp	0.001036
unknown	45014/udp	0.000518
unknown	45020/udp	0.000518
unknown	45021/udp	0.000518
unknown	45032/udp	0.000518
unknown	45037/udp	0.001036
unknown	45038/tcp	0.000076
synctest	45045/tcp	0.000000	# Remote application control protocol
unknown	45046/udp	0.000518
unknown	45050/tcp	0.000076
invision-ag	45054/tcp	0.000000	# InVision AG
invision-ag	45054/udp	0.000000	# InVision AG
unknown	45061/udp	0.001036
unknown	45063/udp	0.000518
unknown	45079/udp	0.000518
unknown	45082/udp	0.000518
unknown	45087/udp	0.000518
unknown	45092/udp	0.000518
unknown	45093/udp	0.000518
unknown	45095/udp	0.000518
unknown	45099/udp	0.000518
unknown	45100/tcp	0.000684
unknown	45103/udp	0.000518
unknown	45106/udp	0.000518
unknown	45114/udp	0.000518
unknown	45118/udp	0.000518
unknown	45120/udp	0.000518
unknown	45121/udp	0.000518
unknown	45124/udp	0.000518
unknown	45125/udp	0.000518
unknown	45133/udp	0.000518
unknown	45135/udp	0.000518
unknown	45136/tcp	0.000076
unknown	45148/udp	0.001036
unknown	45149/udp	0.000518
unknown	45154/udp	0.000518
unknown	45156/udp	0.000518
unknown	45162/udp	0.000518
unknown	45164/tcp	0.000076
unknown	45175/udp	0.000518
unknown	45179/udp	0.000518
unknown	45185/udp	0.000518
unknown	45189/udp	0.000518
unknown	45190/udp	0.000518
unknown	45193/udp	0.001036
unknown	45198/udp	0.000518
unknown	45208/udp	0.000518
unknown	45210/udp	0.000518
unknown	45215/udp	0.000518
unknown	45220/tcp	0.000076
unknown	45220/udp	0.000518
unknown	45223/udp	0.000518
unknown	45225/udp	0.000518
unknown	45226/tcp	0.000076
unknown	45231/udp	0.000518
unknown	45235/udp	0.000518
unknown	45240/udp	0.000518
unknown	45247/udp	0.001554
unknown	45251/udp	0.000518
unknown	45259/udp	0.000518
unknown	45261/udp	0.000518
unknown	45262/udp	0.000518
unknown	45271/udp	0.000518
unknown	45275/udp	0.000518
unknown	45279/udp	0.000518
unknown	45281/udp	0.000518
unknown	45284/udp	0.000518
unknown	45290/udp	0.000518
unknown	45291/udp	0.000518
unknown	45298/udp	0.000518
unknown	45304/udp	0.000518
unknown	45305/udp	0.000518
unknown	45308/udp	0.000518
unknown	45309/udp	0.000518
unknown	45327/udp	0.000518
unknown	45337/udp	0.000518
unknown	45338/udp	0.001036
unknown	45339/udp	0.000518
unknown	45345/udp	0.001036
unknown	45353/udp	0.000518
unknown	45370/udp	0.000518
unknown	45371/udp	0.000518
unknown	45374/udp	0.000518
unknown	45380/udp	0.001554
unknown	45390/udp	0.000518
unknown	45392/udp	0.000518
unknown	45394/udp	0.000518
unknown	45400/udp	0.000518
unknown	45413/tcp	0.000076
unknown	45415/udp	0.000518
unknown	45418/udp	0.000518
unknown	45419/udp	0.000518
unknown	45425/udp	0.000518
unknown	45431/udp	0.000518
unknown	45438/tcp	0.000076
unknown	45441/udp	0.002071
unknown	45442/udp	0.000518
unknown	45449/udp	0.001036
unknown	45452/udp	0.000518
unknown	45454/udp	0.000518
unknown	45463/tcp	0.000076
unknown	45467/udp	0.000518
unknown	45472/udp	0.000518
unknown	45475/udp	0.000518
unknown	45488/udp	0.000518
unknown	45491/udp	0.000518
unknown	45495/udp	0.000518
unknown	45497/udp	0.000518
unknown	45503/udp	0.001036
cloudcheck	45514/tcp	0.000000	# cloudcheck-ping | ASSIA CloudCheck WiFi Management System | ASSIA CloudCheck WiFi Management keepalive
unknown	45515/udp	0.000518
unknown	45516/udp	0.000518
unknown	45517/udp	0.000518
unknown	45519/udp	0.000518
unknown	45524/udp	0.000518
unknown	45525/udp	0.000518
unknown	45533/udp	0.000518
unknown	45537/udp	0.000518
unknown	45538/udp	0.001036
unknown	45541/udp	0.000518
unknown	45542/udp	0.000518
unknown	45548/udp	0.000518
unknown	45554/udp	0.000518
unknown	45556/udp	0.000518
unknown	45563/udp	0.000518
unknown	45568/udp	0.000518
unknown	45573/udp	0.000518
unknown	45577/udp	0.000518
unknown	45579/udp	0.000518
unknown	45588/udp	0.000518
unknown	45596/udp	0.001036
unknown	45602/tcp	0.000076
unknown	45602/udp	0.000518
unknown	45615/udp	0.000518
unknown	45616/udp	0.000518
unknown	45622/udp	0.000518
unknown	45624/tcp	0.000076
unknown	45624/udp	0.000518
unknown	45628/udp	0.000518
unknown	45645/udp	0.000518
unknown	45651/udp	0.000518
unknown	45657/udp	0.000518
unknown	45658/udp	0.000518
unknown	45665/udp	0.000518
unknown	45672/udp	0.000518
unknown	45673/udp	0.000518
unknown	45675/udp	0.000518
unknown	45676/udp	0.000518
eba	45678/tcp	0.000000	# EBA PRISE
eba	45678/udp	0.000000	# EBA PRISE
unknown	45679/udp	0.000518
unknown	45683/udp	0.000518
unknown	45685/udp	0.001554
unknown	45686/udp	0.000518
unknown	45689/udp	0.000518
unknown	45691/udp	0.000518
unknown	45697/tcp	0.000076
unknown	45703/udp	0.000518
unknown	45710/udp	0.000518
unknown	45717/udp	0.000518
unknown	45719/udp	0.001036
unknown	45722/udp	0.001554
unknown	45723/udp	0.000518
unknown	45725/udp	0.000518
unknown	45730/udp	0.000518
unknown	45742/udp	0.000518
unknown	45749/udp	0.000518
unknown	45751/udp	0.000518
unknown	45754/udp	0.000518
unknown	45758/udp	0.000518
unknown	45759/udp	0.000518
unknown	45765/udp	0.000518
unknown	45769/udp	0.001036
unknown	45773/udp	0.000518
unknown	45776/udp	0.000518
unknown	45777/tcp	0.000076
unknown	45781/udp	0.000518
unknown	45786/udp	0.000518
unknown	45788/udp	0.000518
unknown	45792/udp	0.000518
unknown	45801/udp	0.000518
unknown	45804/udp	0.000518
unknown	45810/udp	0.000518
unknown	45814/udp	0.000518
unknown	45815/udp	0.000518
unknown	45816/udp	0.000518
unknown	45818/udp	0.001554
dai-shell	45824/tcp	0.000000	# Server for the DAI family of client-server products
qdb2service	45825/tcp	0.000000	# Qpuncture Data Access Service
qdb2service	45825/udp	0.000000	# Qpuncture Data Access Service
unknown	45830/udp	0.000518
unknown	45832/udp	0.000518
unknown	45834/udp	0.000518
unknown	45837/udp	0.000518
unknown	45845/udp	0.000518
unknown	45849/udp	0.000518
unknown	45856/udp	0.000518
unknown	45859/udp	0.000518
unknown	45864/tcp	0.000076
unknown	45865/udp	0.000518
unknown	45871/udp	0.000518
unknown	45875/udp	0.000518
unknown	45877/udp	0.000518
unknown	45883/udp	0.001036
unknown	45889/udp	0.000518
unknown	45891/udp	0.001036
unknown	45895/udp	0.000518
unknown	45900/udp	0.000518
unknown	45906/udp	0.001036
unknown	45910/udp	0.000518
unknown	45913/udp	0.000518
unknown	45917/udp	0.000518
unknown	45920/udp	0.000518
unknown	45925/udp	0.000518
unknown	45928/udp	0.001554
unknown	45943/udp	0.000518
unknown	45947/udp	0.000518
unknown	45948/udp	0.000518
unknown	45954/udp	0.000518
unknown	45960/tcp	0.000076
unknown	45963/udp	0.000518
ssr-servermgr	45966/tcp	0.000000	# SSRServerMgr
ssr-servermgr	45966/udp	0.000000	# SSRServerMgr
unknown	45971/udp	0.001036
unknown	45986/udp	0.000518
unknown	45991/udp	0.000518
unknown	46005/udp	0.000518
unknown	46015/udp	0.000518
unknown	46016/udp	0.000518
unknown	46020/udp	0.000518
unknown	46025/udp	0.000518
unknown	46032/udp	0.000518
unknown	46034/tcp	0.000076
unknown	46034/udp	0.000518
unknown	46040/udp	0.001036
unknown	46051/udp	0.000518
unknown	46055/udp	0.001036
unknown	46062/udp	0.000518
unknown	46065/udp	0.000518
unknown	46066/udp	0.001036
unknown	46069/tcp	0.000076
unknown	46069/udp	0.000518
unknown	46070/udp	0.000518
unknown	46071/udp	0.000518
unknown	46072/udp	0.000518
unknown	46081/udp	0.000518
unknown	46082/udp	0.000518
unknown	46087/udp	0.000518
unknown	46093/udp	0.001554
unknown	46108/udp	0.000518
unknown	46109/udp	0.000518
unknown	46110/udp	0.000518
unknown	46112/udp	0.000518
unknown	46114/udp	0.001036
unknown	46115/tcp	0.000076
unknown	46126/udp	0.000518
unknown	46128/udp	0.000518
unknown	46137/udp	0.000518
unknown	46140/udp	0.000518
unknown	46148/udp	0.000518
unknown	46156/udp	0.000518
unknown	46158/udp	0.000518
unknown	46171/tcp	0.000076
unknown	46174/udp	0.000518
unknown	46176/udp	0.000518
unknown	46182/tcp	0.000076
unknown	46187/udp	0.000518
unknown	46195/udp	0.001036
unknown	46200/tcp	0.000152
unknown	46200/udp	0.000518
unknown	46201/udp	0.001036
unknown	46207/udp	0.001036
unknown	46214/udp	0.000518
unknown	46217/udp	0.000518
unknown	46223/udp	0.000518
unknown	46228/udp	0.000518
unknown	46230/udp	0.000518
unknown	46231/udp	0.000518
unknown	46234/udp	0.000518
unknown	46235/udp	0.000518
unknown	46249/udp	0.001036
unknown	46257/udp	0.000518
unknown	46265/udp	0.001036
unknown	46267/udp	0.000518
unknown	46269/udp	0.000518
unknown	46270/udp	0.001036
unknown	46283/udp	0.000518
unknown	46284/udp	0.000518
unknown	46287/udp	0.000518
unknown	46294/udp	0.001036
unknown	46297/udp	0.000518
unknown	46306/udp	0.000518
unknown	46310/tcp	0.000076
unknown	46311/udp	0.000518
unknown	46319/udp	0.000518
unknown	46321/udp	0.000518
unknown	46334/udp	0.000518
inedo	46336/tcp	0.000000	# Listen port used for Inedo agent communication
unknown	46341/udp	0.000518
unknown	46342/udp	0.000518
unknown	46350/udp	0.000518
unknown	46352/udp	0.000518
unknown	46363/udp	0.000518
unknown	46369/udp	0.000518
unknown	46370/udp	0.000518
unknown	46372/tcp	0.000076
unknown	46373/udp	0.000518
unknown	46374/udp	0.000518
unknown	46383/udp	0.000518
unknown	46387/udp	0.001036
unknown	46391/udp	0.000518
unknown	46395/udp	0.000518
unknown	46414/udp	0.000518
unknown	46418/tcp	0.000076
unknown	46419/udp	0.000518
unknown	46420/udp	0.000518
unknown	46421/udp	0.000518
unknown	46432/udp	0.000518
unknown	46434/udp	0.000518
unknown	46436/tcp	0.000076
unknown	46440/udp	0.001036
unknown	46442/udp	0.000518
unknown	46453/udp	0.000518
unknown	46455/udp	0.000518
unknown	46457/udp	0.001036
unknown	46459/udp	0.000518
unknown	46462/udp	0.001036
unknown	46464/udp	0.001036
unknown	46472/udp	0.000518
unknown	46474/udp	0.000518
unknown	46478/udp	0.000518
unknown	46483/udp	0.001036
unknown	46486/udp	0.000518
unknown	46491/udp	0.000518
unknown	46502/udp	0.000518
unknown	46504/udp	0.000518
unknown	46514/udp	0.000518
unknown	46515/udp	0.000518
unknown	46517/udp	0.000518
unknown	46529/udp	0.000518
unknown	46532/udp	0.001554
unknown	46534/udp	0.000518
unknown	46535/udp	0.000518
unknown	46537/udp	0.000518
unknown	46542/udp	0.000518
unknown	46546/udp	0.000518
unknown	46548/udp	0.000518
unknown	46555/udp	0.000518
unknown	46556/udp	0.000518
unknown	46557/udp	0.000518
unknown	46559/udp	0.000518
unknown	46574/udp	0.000518
unknown	46576/udp	0.000518
unknown	46580/udp	0.000518
unknown	46581/udp	0.000518
unknown	46582/udp	0.000518
unknown	46584/udp	0.001036
unknown	46587/udp	0.000518
unknown	46593/tcp	0.000076
unknown	46594/udp	0.001036
unknown	46599/udp	0.000518
unknown	46602/udp	0.000518
unknown	46603/udp	0.001036
unknown	46606/udp	0.000518
unknown	46625/udp	0.000518
unknown	46630/udp	0.001036
unknown	46640/udp	0.000518
unknown	46641/udp	0.001036
unknown	46643/udp	0.001036
unknown	46644/udp	0.000518
unknown	46652/udp	0.001036
unknown	46653/udp	0.000518
unknown	46654/udp	0.000518
unknown	46656/udp	0.000518
unknown	46657/udp	0.000518
unknown	46658/udp	0.000518
unknown	46662/udp	0.000518
unknown	46666/udp	0.000518
unknown	46668/udp	0.000518
unknown	46688/udp	0.000518
unknown	46689/udp	0.000518
unknown	46692/udp	0.000518
unknown	46693/udp	0.000518
unknown	46694/udp	0.000518
unknown	46698/udp	0.001036
unknown	46699/udp	0.000518
unknown	46717/udp	0.000518
unknown	46741/udp	0.000518
unknown	46745/udp	0.000518
unknown	46746/udp	0.000518
unknown	46749/udp	0.000518
unknown	46757/udp	0.000518
unknown	46758/udp	0.001036
unknown	46764/udp	0.000518
unknown	46765/udp	0.000518
unknown	46779/udp	0.000518
unknown	46780/udp	0.000518
unknown	46785/udp	0.000518
unknown	46788/udp	0.000518
unknown	46793/udp	0.001036
unknown	46799/udp	0.000518
unknown	46803/udp	0.000518
unknown	46804/udp	0.000518
unknown	46805/udp	0.000518
unknown	46808/udp	0.001036
unknown	46813/tcp	0.000076
unknown	46813/udp	0.000518
unknown	46823/udp	0.000518
unknown	46825/udp	0.000518
unknown	46830/udp	0.000518
unknown	46831/udp	0.000518
unknown	46836/udp	0.001554
unknown	46837/udp	0.001036
unknown	46850/udp	0.000518
unknown	46851/udp	0.000518
unknown	46865/udp	0.000518
unknown	46869/udp	0.000518
unknown	46871/udp	0.000518
unknown	46872/udp	0.000518
unknown	46882/udp	0.000518
unknown	46887/udp	0.000518
unknown	46893/udp	0.000518
unknown	46894/udp	0.000518
unknown	46895/udp	0.000518
unknown	46899/udp	0.000518
unknown	46909/udp	0.000518
unknown	46911/udp	0.000518
unknown	46919/udp	0.000518
unknown	46930/udp	0.000518
unknown	46932/udp	0.000518
unknown	46934/udp	0.000518
unknown	46942/udp	0.000518
unknown	46944/udp	0.000518
unknown	46946/udp	0.000518
unknown	46949/udp	0.000518
unknown	46955/udp	0.000518
unknown	46959/udp	0.000518
unknown	46968/udp	0.000518
unknown	46972/udp	0.000518
unknown	46975/udp	0.000518
unknown	46981/udp	0.000518
unknown	46989/udp	0.000518
unknown	46990/udp	0.000518
unknown	46992/tcp	0.000076
unknown	46996/tcp	0.000152
spremotetablet	46998/tcp	0.000000	# Connection between a desktop computer or server and a signature tablet to capture handwritten signatures
mediabox	46999/tcp	0.000000	# MediaBox Server
mediabox	46999/udp	0.000518	# MediaBox Server
mbus	47000/tcp	0.000000	# Message Bus
mbus	47000/udp	0.000000	# Message Bus
winrm	47001/tcp	0.000000	# Windows Remote Management Service
unknown	47005/udp	0.000518
unknown	47009/udp	0.000518
unknown	47012/tcp	0.000076
unknown	47012/udp	0.000518
unknown	47014/udp	0.000518
unknown	47021/udp	0.000518
unknown	47026/udp	0.000518
unknown	47029/tcp	0.000076
unknown	47030/udp	0.001036
unknown	47037/udp	0.000518
unknown	47042/udp	0.000518
unknown	47043/udp	0.000518
unknown	47045/udp	0.000518
unknown	47057/udp	0.000518
unknown	47058/udp	0.000518
unknown	47060/udp	0.000518
unknown	47065/udp	0.000518
unknown	47069/udp	0.000518
unknown	47073/udp	0.000518
unknown	47074/udp	0.000518
unknown	47079/udp	0.000518
unknown	47080/udp	0.000518
unknown	47083/udp	0.001036
unknown	47086/udp	0.000518
unknown	47087/udp	0.000518
unknown	47090/udp	0.000518
unknown	47091/udp	0.000518
jvl-mactalk	47100/tcp	0.000000	# Configuration of motors connected to Industrial Ethernet
unknown	47100/udp	0.000518
unknown	47102/udp	0.000518
unknown	47103/udp	0.000518
unknown	47119/tcp	0.000076
unknown	47120/udp	0.000518
unknown	47128/udp	0.000518
unknown	47130/udp	0.000518
unknown	47131/udp	0.000518
unknown	47132/udp	0.001036
unknown	47134/udp	0.001036
unknown	47139/udp	0.000518
unknown	47142/udp	0.000518
unknown	47143/udp	0.000518
unknown	47144/udp	0.000518
unknown	47154/udp	0.000518
unknown	47155/udp	0.000518
unknown	47157/udp	0.000518
unknown	47159/udp	0.000518
unknown	47160/udp	0.001036
unknown	47161/udp	0.000518
unknown	47162/udp	0.000518
unknown	47169/udp	0.001036
unknown	47176/udp	0.000518
unknown	47183/udp	0.000518
unknown	47184/udp	0.000518
unknown	47185/udp	0.001036
unknown	47190/udp	0.000518
unknown	47197/tcp	0.000076
unknown	47197/udp	0.000518
unknown	47198/udp	0.001036
unknown	47213/udp	0.000518
unknown	47217/udp	0.000518
unknown	47220/udp	0.000518
unknown	47224/udp	0.000518
unknown	47229/udp	0.000518
unknown	47231/udp	0.000518
unknown	47234/udp	0.000518
unknown	47242/udp	0.000518
unknown	47247/udp	0.000518
unknown	47259/udp	0.000518
unknown	47260/udp	0.000518
unknown	47262/udp	0.000518
unknown	47265/udp	0.000518
unknown	47267/tcp	0.000076
unknown	47267/udp	0.000518
unknown	47270/udp	0.001036
unknown	47279/udp	0.001036
unknown	47281/udp	0.000518
unknown	47289/udp	0.000518
unknown	47290/udp	0.000518
unknown	47291/udp	0.000518
unknown	47298/udp	0.000518
unknown	47300/udp	0.000518
unknown	47306/udp	0.000518
unknown	47307/udp	0.000518
unknown	47310/udp	0.000518
unknown	47315/udp	0.000518
unknown	47335/udp	0.000518
unknown	47336/udp	0.000518
unknown	47337/udp	0.001036
unknown	47346/udp	0.000518
unknown	47348/tcp	0.000076
unknown	47352/udp	0.000518
unknown	47357/udp	0.000518
unknown	47359/udp	0.000518
unknown	47364/udp	0.000518
unknown	47370/udp	0.000518
unknown	47371/udp	0.001036
unknown	47372/tcp	0.000076
unknown	47386/udp	0.000518
unknown	47391/udp	0.000518
unknown	47400/udp	0.000518
unknown	47405/udp	0.000518
unknown	47406/udp	0.001036
unknown	47409/udp	0.000518
unknown	47413/udp	0.000518
unknown	47415/udp	0.000518
unknown	47421/udp	0.000518
unknown	47432/udp	0.001036
unknown	47437/udp	0.000518
unknown	47442/udp	0.000518
unknown	47445/udp	0.000518
unknown	47446/udp	0.000518
unknown	47448/tcp	0.000076
unknown	47456/udp	0.000518
unknown	47457/udp	0.001036
unknown	47470/udp	0.000518
unknown	47474/udp	0.000518
unknown	47475/udp	0.000518
unknown	47477/udp	0.000518
unknown	47481/udp	0.000518
unknown	47490/udp	0.000518
unknown	47494/udp	0.000518
unknown	47496/udp	0.000518
unknown	47513/udp	0.000518
unknown	47526/udp	0.000518
unknown	47531/udp	0.000518
unknown	47535/udp	0.000518
unknown	47544/tcp	0.000152
unknown	47544/udp	0.000518
unknown	47552/udp	0.000518
unknown	47554/udp	0.000518
unknown	47555/udp	0.000518
dbbrowse	47557/tcp	0.000038	# Databeam Corporation
dbbrowse	47557/udp	0.001158	# Databeam Corporation
unknown	47560/udp	0.000518
unknown	47567/tcp	0.000076
unknown	47572/udp	0.001036
unknown	47575/udp	0.000518
unknown	47577/udp	0.001036
unknown	47581/tcp	0.000076
unknown	47582/udp	0.000518
unknown	47584/udp	0.000518
unknown	47586/udp	0.001036
unknown	47594/udp	0.000518
unknown	47595/tcp	0.000076
unknown	47595/udp	0.000518
unknown	47598/udp	0.000518
unknown	47600/udp	0.000518
unknown	47609/udp	0.000518
unknown	47610/udp	0.000518
unknown	47616/udp	0.000518
unknown	47618/udp	0.000518
directplaysrvr	47624/tcp	0.000076	# Direct Play Server
directplaysrvr	47624/udp	0.002071	# Direct Play Server
unknown	47626/udp	0.000518
unknown	47628/udp	0.000518
unknown	47631/udp	0.000518
unknown	47632/udp	0.000518
unknown	47634/tcp	0.000076
unknown	47634/udp	0.000518
unknown	47636/udp	0.000518
unknown	47637/udp	0.000518
unknown	47640/udp	0.000518
unknown	47648/udp	0.000518
unknown	47652/udp	0.000518
unknown	47653/udp	0.000518
unknown	47656/udp	0.001036
unknown	47658/udp	0.000518
unknown	47663/udp	0.000518
unknown	47667/udp	0.000518
unknown	47669/udp	0.000518
unknown	47671/udp	0.000518
unknown	47672/udp	0.000518
unknown	47674/udp	0.000518
unknown	47678/udp	0.000518
unknown	47695/udp	0.000518
unknown	47697/udp	0.000518
unknown	47700/tcp	0.000076
unknown	47701/udp	0.000518
unknown	47702/udp	0.000518
unknown	47706/udp	0.001036
unknown	47708/udp	0.000518
unknown	47717/udp	0.000518
unknown	47718/udp	0.000518
unknown	47751/udp	0.001036
unknown	47756/udp	0.000518
unknown	47762/udp	0.000518
unknown	47765/udp	0.001554
unknown	47768/udp	0.000518
unknown	47771/udp	0.000518
unknown	47772/udp	0.001554
unknown	47775/udp	0.000518
unknown	47777/tcp	0.000076
unknown	47780/udp	0.000518
unknown	47783/udp	0.000518
unknown	47785/udp	0.000518
unknown	47788/udp	0.000518
unknown	47790/udp	0.000518
unknown	47792/udp	0.000518
unknown	47798/udp	0.000518
unknown	47802/udp	0.001036
unknown	47805/udp	0.000518
ap	47806/tcp	0.000076	# ALC Protocol
ap	47806/udp	0.000518	# ALC Protocol
bacnet	47808/tcp	0.000000	# Building Automation and Control Networks
bacnet	47808/udp	0.001554	# Building Automation and Control Networks
presonus-ucnet	47809/tcp	0.000000	# PreSonus Universal Control Network Protocol
unknown	47817/udp	0.001036
unknown	47821/udp	0.001036
unknown	47839/udp	0.000518
unknown	47841/udp	0.000518
unknown	47842/udp	0.001036
unknown	47845/udp	0.000518
unknown	47847/udp	0.001036
unknown	47850/tcp	0.000076
unknown	47851/udp	0.001036
unknown	47852/udp	0.000518
unknown	47858/tcp	0.000076
unknown	47858/udp	0.000518
unknown	47860/tcp	0.000076
unknown	47869/udp	0.000518
unknown	47875/udp	0.000518
unknown	47876/udp	0.000518
unknown	47877/udp	0.000518
unknown	47882/udp	0.000518
unknown	47884/udp	0.000518
unknown	47885/udp	0.000518
unknown	47889/udp	0.000518
unknown	47892/udp	0.000518
unknown	47896/udp	0.000518
unknown	47902/udp	0.000518
unknown	47908/udp	0.000518
unknown	47915/udp	0.001554
unknown	47917/udp	0.001036
unknown	47926/udp	0.001036
unknown	47931/udp	0.000518
unknown	47936/udp	0.001036
unknown	47946/udp	0.000518
unknown	47952/udp	0.000518
unknown	47955/udp	0.000518
unknown	47966/tcp	0.000076
unknown	47968/udp	0.000518
unknown	47969/tcp	0.000076
unknown	47971/udp	0.001036
unknown	47973/udp	0.000518
unknown	47981/udp	0.001554
unknown	47985/udp	0.000518
unknown	47989/udp	0.000518
unknown	47993/udp	0.000518
nimcontroller	48000/tcp	0.000000	# Nimbus Controller
nimcontroller	48000/udp	0.000000	# Nimbus Controller
nimspooler	48001/tcp	0.000000	# Nimbus Spooler
nimspooler	48001/udp	0.000000	# Nimbus Spooler
nimhub	48002/tcp	0.000000	# Nimbus Hub
nimhub	48002/udp	0.000518	# Nimbus Hub
nimgtw	48003/tcp	0.000000	# Nimbus Gateway
nimgtw	48003/udp	0.000000	# Nimbus Gateway
nimbusdb	48004/tcp	0.000000	# NimbusDB Connector
unknown	48004/udp	0.000518
nimbusdbctrl	48005/tcp	0.000000	# NimbusDB Control
unknown	48005/udp	0.000518
unknown	48009/tcp	0.000076
unknown	48024/udp	0.000518
unknown	48029/udp	0.000518
unknown	48031/udp	0.000518
unknown	48036/udp	0.000518
unknown	48041/udp	0.000518
unknown	48045/udp	0.000518
juka	48048/tcp	0.000000	# Juliar Programming Language Protocol
3gpp-cbsp	48049/tcp	0.000000	# 3GPP Cell Broadcast Service Protocol
unknown	48049/udp	0.000518
weandsf	48050/tcp	0.000000	# WeFi Access Network Discovery and Selection Function
unknown	48051/udp	0.000518
unknown	48053/udp	0.000518
unknown	48057/udp	0.000518
unknown	48067/tcp	0.000076
unknown	48068/udp	0.000518
unknown	48078/udp	0.001554
unknown	48080/tcp	0.000380
unknown	48080/udp	0.000518
unknown	48083/tcp	0.000076
unknown	48086/udp	0.000518
unknown	48091/udp	0.000518
unknown	48097/udp	0.000518
unknown	48103/udp	0.000518
unknown	48105/udp	0.001036
unknown	48113/udp	0.000518
unknown	48116/udp	0.000518
unknown	48117/udp	0.000518
unknown	48126/udp	0.001036
unknown	48127/tcp	0.000076
isnetserv	48128/tcp	0.000000	# Image Systems Network Services
isnetserv	48128/udp	0.000518	# Image Systems Network Services
blp5	48129/tcp	0.000000	# Bloomberg locator
blp5	48129/udp	0.000000	# Bloomberg locator
unknown	48130/udp	0.000518
unknown	48132/udp	0.000518
unknown	48133/udp	0.000518
unknown	48137/udp	0.000518
unknown	48152/udp	0.000518
unknown	48153/tcp	0.000076
unknown	48153/udp	0.000518
unknown	48155/udp	0.000518
unknown	48156/udp	0.001036
unknown	48161/udp	0.000518
unknown	48167/tcp	0.000076
unknown	48174/udp	0.000518
unknown	48175/udp	0.000518
unknown	48184/udp	0.000518
unknown	48185/udp	0.000518
unknown	48189/udp	0.001554
unknown	48194/udp	0.000518
unknown	48195/udp	0.000518
unknown	48205/udp	0.000518
unknown	48215/udp	0.000518
unknown	48221/udp	0.000518
unknown	48222/udp	0.001036
unknown	48226/udp	0.000518
unknown	48229/udp	0.000518
unknown	48232/udp	0.000518
unknown	48234/udp	0.000518
unknown	48244/udp	0.000518
unknown	48250/udp	0.000518
unknown	48251/udp	0.000518
unknown	48255/udp	0.001554
unknown	48256/udp	0.000518
unknown	48263/udp	0.001036
unknown	48270/udp	0.000518
unknown	48280/udp	0.000518
unknown	48282/udp	0.001036
unknown	48288/udp	0.000518
unknown	48291/udp	0.000518
unknown	48309/udp	0.000518
unknown	48314/udp	0.001036
unknown	48315/udp	0.001036
unknown	48319/udp	0.000518
unknown	48321/udp	0.001036
unknown	48324/udp	0.001036
unknown	48326/udp	0.000518
unknown	48329/udp	0.001036
unknown	48337/udp	0.000518
unknown	48342/udp	0.001036
unknown	48348/udp	0.000518
unknown	48356/tcp	0.000076
unknown	48357/udp	0.000518
unknown	48365/udp	0.000518
unknown	48366/udp	0.000518
unknown	48369/udp	0.000518
unknown	48370/udp	0.000518
unknown	48372/udp	0.000518
unknown	48374/udp	0.000518
unknown	48376/udp	0.000518
unknown	48378/udp	0.000518
unknown	48386/udp	0.000518
unknown	48387/udp	0.000518
unknown	48390/udp	0.000518
unknown	48395/udp	0.000518
unknown	48406/udp	0.000518
unknown	48409/udp	0.000518
unknown	48411/udp	0.001036
unknown	48424/udp	0.000518
unknown	48427/udp	0.000518
unknown	48434/tcp	0.000076
unknown	48454/udp	0.000518
unknown	48455/udp	0.001554
unknown	48459/udp	0.000518
unknown	48464/udp	0.000518
unknown	48474/udp	0.000518
unknown	48476/udp	0.000518
unknown	48478/udp	0.000518
unknown	48481/udp	0.000518
unknown	48487/udp	0.000518
unknown	48489/udp	0.001554
unknown	48490/udp	0.000518
unknown	48491/udp	0.000518
unknown	48494/udp	0.000518
unknown	48496/udp	0.001036
unknown	48497/udp	0.000518
unknown	48501/udp	0.000518
unknown	48512/udp	0.000518
unknown	48514/udp	0.000518
unknown	48523/udp	0.000518
unknown	48540/udp	0.000518
unknown	48546/udp	0.000518
unknown	48548/udp	0.001036
unknown	48551/udp	0.000518
unknown	48554/udp	0.000518
unknown	48555/udp	0.001036
com-bardac-dw	48556/tcp	0.000000
com-bardac-dw	48556/udp	0.001036
unknown	48558/udp	0.001036
unknown	48564/udp	0.000518
unknown	48566/udp	0.000518
unknown	48571/udp	0.000518
unknown	48572/udp	0.000518
unknown	48573/udp	0.000518
unknown	48574/udp	0.000518
unknown	48577/udp	0.000518
unknown	48588/udp	0.000518
unknown	48598/udp	0.000518
unknown	48601/udp	0.000518
unknown	48602/udp	0.000518
unknown	48605/udp	0.001036
unknown	48606/udp	0.000518
unknown	48611/udp	0.000518
unknown	48613/udp	0.000518
iqobject	48619/tcp	0.000076
iqobject	48619/udp	0.000000
unknown	48620/udp	0.000518
unknown	48626/udp	0.001036
unknown	48629/udp	0.000518
unknown	48631/tcp	0.000076
unknown	48631/udp	0.001036
unknown	48648/tcp	0.000076
unknown	48648/udp	0.000518
robotraconteur	48653/tcp	0.000000	# Robot Raconteur transport
unknown	48663/udp	0.000518
unknown	48672/udp	0.000518
unknown	48674/udp	0.000518
unknown	48682/tcp	0.000076
unknown	48686/udp	0.000518
unknown	48698/udp	0.000518
unknown	48701/udp	0.000518
unknown	48705/udp	0.000518
unknown	48706/udp	0.000518
unknown	48707/udp	0.000518
unknown	48712/udp	0.001036
unknown	48717/udp	0.000518
unknown	48721/udp	0.000518
unknown	48725/udp	0.000518
unknown	48726/udp	0.000518
unknown	48729/udp	0.000518
unknown	48733/udp	0.001036
unknown	48740/udp	0.000518
unknown	48741/udp	0.000518
unknown	48753/udp	0.000518
unknown	48755/udp	0.000518
unknown	48757/udp	0.000518
unknown	48758/udp	0.000518
unknown	48761/udp	0.001554
unknown	48762/udp	0.000518
unknown	48764/udp	0.000518
unknown	48780/udp	0.001036
unknown	48783/tcp	0.000076
unknown	48786/udp	0.000518
unknown	48790/udp	0.001036
unknown	48793/udp	0.000518
unknown	48794/udp	0.000518
unknown	48800/udp	0.000518
unknown	48803/udp	0.000518
unknown	48813/tcp	0.000076
unknown	48824/udp	0.000518
unknown	48825/udp	0.000518
unknown	48829/udp	0.000518
unknown	48830/udp	0.000518
unknown	48847/udp	0.000518
unknown	48853/udp	0.000518
unknown	48854/udp	0.001036
unknown	48860/udp	0.001036
unknown	48862/udp	0.000518
unknown	48864/udp	0.000518
unknown	48869/udp	0.000518
unknown	48883/udp	0.000518
unknown	48887/udp	0.001036
unknown	48890/udp	0.000518
unknown	48898/udp	0.001036
tc_ads_discovery	48899/udp	0.000518
unknown	48901/udp	0.001036
unknown	48903/udp	0.000518
unknown	48906/udp	0.001036
unknown	48913/udp	0.000518
unknown	48918/udp	0.000518
unknown	48921/udp	0.000518
unknown	48923/udp	0.000518
unknown	48925/tcp	0.000076
unknown	48925/udp	0.000518
unknown	48933/udp	0.000518
unknown	48935/udp	0.000518
unknown	48954/udp	0.001036
unknown	48956/udp	0.000518
unknown	48966/tcp	0.000076
unknown	48967/tcp	0.000076
unknown	48972/udp	0.000518
unknown	48973/tcp	0.000076
unknown	48980/udp	0.000518
unknown	48986/udp	0.000518
unknown	48991/udp	0.000518
unknown	48998/udp	0.000518
matahari	49000/tcp	0.000000	# Matahari Broker
nusrp	49001/tcp	0.000000	# nusdp-disc | Nuance Unity Service Request Protocol | Nuance Unity Service Discovery Protocol
unknown	49001/udp	0.000518
unknown	49002/tcp	0.000076
unknown	49005/udp	0.000518
unknown	49011/udp	0.000518
unknown	49015/udp	0.000518
unknown	49017/udp	0.000518
unknown	49020/udp	0.000518
unknown	49022/udp	0.000518
unknown	49028/udp	0.000518
unknown	49032/udp	0.000518
unknown	49034/udp	0.000518
unknown	49036/udp	0.000518
unknown	49040/udp	0.000518
unknown	49042/udp	0.001036
unknown	49048/tcp	0.000076
unknown	49048/udp	0.000518
unknown	49052/udp	0.001036
unknown	49057/udp	0.000518
unknown	49062/udp	0.000518
unknown	49066/udp	0.000518
unknown	49076/udp	0.000518
unknown	49080/udp	0.000518
unknown	49082/udp	0.000518
unknown	49085/udp	0.000518
unknown	49087/udp	0.000518
unknown	49100/udp	0.000518
unknown	49104/udp	0.000518
unknown	49108/udp	0.000518
unknown	49114/udp	0.001036
unknown	49122/udp	0.000518
unknown	49123/udp	0.000518
unknown	49127/udp	0.001036
unknown	49128/udp	0.000518
unknown	49131/udp	0.000518
unknown	49132/tcp	0.000076
unknown	49133/udp	0.000518
unknown	49134/udp	0.000518
unknown	49136/udp	0.001036
unknown	49138/udp	0.000518
unknown	49142/udp	0.000518
unknown	49146/udp	0.000518
inspider	49150/tcp	0.000000	# InSpider System
unknown	49152/tcp	0.007907
unknown	49152/udp	0.116002
unknown	49153/tcp	0.006158
unknown	49153/udp	0.060743
unknown	49154/tcp	0.006767
unknown	49154/udp	0.092369
unknown	49155/tcp	0.005702
unknown	49155/udp	0.001506
unknown	49156/tcp	0.005322
unknown	49156/udp	0.007530
unknown	49157/tcp	0.003573
unknown	49157/udp	0.002008
unknown	49158/tcp	0.000380
unknown	49158/udp	0.006526
unknown	49159/tcp	0.000380
unknown	49159/udp	0.004016
unknown	49160/tcp	0.000380
unknown	49160/udp	0.003012
unknown	49161/tcp	0.000228
unknown	49161/udp	0.002008
unknown	49162/udp	0.006024
unknown	49163/tcp	0.000304
unknown	49163/udp	0.003514
unknown	49164/tcp	0.000152
unknown	49164/udp	0.001004
unknown	49165/tcp	0.000304
unknown	49165/udp	0.003514
unknown	49166/tcp	0.000076
unknown	49166/udp	0.004016
unknown	49167/tcp	0.000228
unknown	49167/udp	0.002510
unknown	49168/tcp	0.000152
unknown	49168/udp	0.003514
unknown	49169/tcp	0.000076
unknown	49169/udp	0.003012
unknown	49170/tcp	0.000076
unknown	49170/udp	0.002008
unknown	49171/tcp	0.000152
unknown	49171/udp	0.004518
unknown	49172/tcp	0.000076
unknown	49172/udp	0.003514
unknown	49173/tcp	0.000076
unknown	49173/udp	0.002008
unknown	49174/udp	0.003012
unknown	49175/tcp	0.000304
unknown	49175/udp	0.002510
unknown	49176/tcp	0.000228
unknown	49176/udp	0.002008
unknown	49177/udp	0.001506
unknown	49178/udp	0.001506
unknown	49179/tcp	0.000076
unknown	49179/udp	0.004518
unknown	49180/udp	0.005020
unknown	49181/udp	0.010542
unknown	49182/udp	0.007530
unknown	49183/udp	0.001004
unknown	49184/udp	0.004518
unknown	49185/udp	0.007028
unknown	49186/tcp	0.000152
unknown	49186/udp	0.012550
unknown	49187/udp	0.006024
unknown	49188/udp	0.007028
unknown	49189/tcp	0.000076
unknown	49189/udp	0.006024
unknown	49190/tcp	0.000076
unknown	49190/udp	0.007028
unknown	49191/tcp	0.000076
unknown	49191/udp	0.007530
unknown	49192/udp	0.011044
unknown	49193/udp	0.015562
unknown	49194/udp	0.007530
unknown	49195/tcp	0.000152
unknown	49195/udp	0.006024
unknown	49196/tcp	0.000076
unknown	49196/udp	0.006526
unknown	49197/tcp	0.000076
unknown	49197/udp	0.002008
unknown	49198/udp	0.002510
unknown	49199/udp	0.005020
unknown	49200/udp	0.010040
unknown	49201/tcp	0.000076
unknown	49201/udp	0.011044
unknown	49202/tcp	0.000076
unknown	49202/udp	0.004518
unknown	49203/tcp	0.000076
unknown	49203/udp	0.001004
unknown	49204/tcp	0.000076
unknown	49204/udp	0.002510
unknown	49205/udp	0.004518
unknown	49206/udp	0.001004
unknown	49207/udp	0.002008
unknown	49208/udp	0.004518
unknown	49209/udp	0.004518
unknown	49210/udp	0.004518
unknown	49211/tcp	0.000076
unknown	49211/udp	0.007028
unknown	49212/udp	0.002510
unknown	49213/tcp	0.000076
unknown	49213/udp	0.002510
unknown	49214/udp	0.001506
unknown	49215/udp	0.002510
unknown	49216/tcp	0.000076
unknown	49216/udp	0.001506
unknown	49217/udp	0.001004
unknown	49218/udp	0.001004
unknown	49219/udp	0.001004
unknown	49220/udp	0.001506
unknown	49221/udp	0.000502
unknown	49222/udp	0.001506
unknown	49223/udp	0.001004
unknown	49225/udp	0.000502
unknown	49226/udp	0.001506
unknown	49227/udp	0.001004
unknown	49228/tcp	0.000076
unknown	49228/udp	0.000502
unknown	49230/udp	0.000502
unknown	49231/udp	0.001004
unknown	49232/tcp	0.000076
unknown	49233/udp	0.000502
unknown	49235/tcp	0.000076
unknown	49235/udp	0.000502
unknown	49236/tcp	0.000152
unknown	49236/udp	0.001004
unknown	49237/udp	0.001004
unknown	49238/udp	0.000502
unknown	49241/tcp	0.000076
unknown	49241/udp	0.000502
unknown	49244/udp	0.000502
unknown	49245/udp	0.000502
unknown	49248/udp	0.000502
unknown	49249/udp	0.001004
unknown	49250/udp	0.000502
unknown	49251/udp	0.000502
unknown	49252/udp	0.001004
unknown	49255/udp	0.001004
unknown	49258/udp	0.000502
unknown	49259/udp	0.001506
unknown	49260/udp	0.000502
unknown	49261/udp	0.000502
unknown	49262/udp	0.001506
unknown	49263/udp	0.000502
unknown	49264/udp	0.001004
unknown	49265/udp	0.000502
unknown	49266/udp	0.001004
unknown	49268/udp	0.001004
unknown	49269/udp	0.000502
unknown	49270/udp	0.000502
unknown	49273/udp	0.001004
unknown	49275/tcp	0.000076
unknown	49277/udp	0.000502
unknown	49279/udp	0.000502
unknown	49288/udp	0.000502
unknown	49290/udp	0.000502
unknown	49295/udp	0.001004
unknown	49297/udp	0.000502
unknown	49299/udp	0.000502
unknown	49302/tcp	0.000076
unknown	49305/udp	0.000502
unknown	49306/udp	0.001506
unknown	49309/udp	0.000502
unknown	49312/udp	0.000502
unknown	49313/udp	0.000502
unknown	49315/udp	0.000502
unknown	49317/udp	0.001004
unknown	49319/udp	0.001004
unknown	49321/udp	0.000502
unknown	49322/udp	0.000502
unknown	49324/udp	0.001004
unknown	49328/udp	0.000502
unknown	49329/udp	0.000502
unknown	49331/udp	0.000502
unknown	49332/udp	0.000502
unknown	49333/udp	0.000502
unknown	49334/udp	0.001004
unknown	49335/udp	0.000502
unknown	49337/udp	0.001004
unknown	49338/udp	0.000502
unknown	49339/udp	0.000502
unknown	49342/udp	0.000502
unknown	49343/udp	0.000502
unknown	49345/udp	0.000502
unknown	49346/udp	0.000502
unknown	49347/udp	0.000502
unknown	49348/udp	0.001004
unknown	49350/udp	0.001506
unknown	49351/udp	0.000502
unknown	49352/tcp	0.000076
unknown	49358/udp	0.000502
unknown	49360/udp	0.001506
unknown	49361/udp	0.000502
unknown	49362/udp	0.000502
unknown	49367/udp	0.000502
unknown	49372/tcp	0.000076
unknown	49374/udp	0.000502
unknown	49375/udp	0.001004
unknown	49379/udp	0.000502
unknown	49384/udp	0.001004
unknown	49389/udp	0.000502
unknown	49393/udp	0.001506
unknown	49395/udp	0.000502
unknown	49396/udp	0.001506
unknown	49398/tcp	0.000076
unknown	49398/udp	0.000502
compaqdiag	49400/tcp	0.000276	# Compaq Web-based management
unknown	49401/tcp	0.000152
unknown	49401/udp	0.000502
unknown	49408/udp	0.000502
unknown	49411/udp	0.000502
unknown	49412/udp	0.000502
unknown	49413/udp	0.000502
unknown	49421/udp	0.000502
unknown	49424/udp	0.000502
unknown	49430/udp	0.000502
unknown	49436/udp	0.000502
unknown	49440/udp	0.001004
unknown	49441/udp	0.000502
unknown	49442/udp	0.000502
unknown	49443/udp	0.001004
unknown	49448/udp	0.000502
unknown	49450/udp	0.000502
unknown	49451/udp	0.000502
unknown	49452/tcp	0.000076
unknown	49452/udp	0.000502
unknown	49453/udp	0.000502
unknown	49454/udp	0.000502
unknown	49459/udp	0.000502
unknown	49460/udp	0.000502
unknown	49464/udp	0.000502
unknown	49465/udp	0.000502
unknown	49467/udp	0.000502
unknown	49468/udp	0.000502
unknown	49470/udp	0.000502
unknown	49473/udp	0.000502
unknown	49474/udp	0.000502
unknown	49478/udp	0.001004
unknown	49479/udp	0.000502
unknown	49480/udp	0.000502
unknown	49481/udp	0.000502
unknown	49484/udp	0.000502
unknown	49488/udp	0.000502
unknown	49489/udp	0.000502
unknown	49490/udp	0.000502
unknown	49494/udp	0.000502
unknown	49498/tcp	0.000076
unknown	49498/udp	0.000502
unknown	49499/udp	0.000502
unknown	49500/tcp	0.000076
unknown	49502/udp	0.000502
unknown	49503/udp	0.002008
unknown	49505/udp	0.000502
unknown	49506/udp	0.001004
unknown	49509/udp	0.000502
unknown	49511/udp	0.000502
unknown	49513/udp	0.001004
unknown	49514/udp	0.000502
unknown	49517/udp	0.000502
unknown	49519/tcp	0.000076
unknown	49519/udp	0.000502
unknown	49520/tcp	0.000076
unknown	49520/udp	0.000502
unknown	49521/tcp	0.000076
unknown	49522/tcp	0.000076
unknown	49525/udp	0.001004
unknown	49530/udp	0.000502
unknown	49535/udp	0.000502
unknown	49544/udp	0.000502
unknown	49546/udp	0.000502
unknown	49550/udp	0.000502
unknown	49557/udp	0.001004
unknown	49560/udp	0.000502
unknown	49562/udp	0.001004
unknown	49567/udp	0.000502
unknown	49569/udp	0.000502
unknown	49579/udp	0.001004
unknown	49582/udp	0.000502
unknown	49586/udp	0.000502
unknown	49589/udp	0.001004
unknown	49590/udp	0.000502
unknown	49596/udp	0.000502
unknown	49597/tcp	0.000076
unknown	49597/udp	0.000502
unknown	49600/udp	0.001004
unknown	49603/tcp	0.000076
unknown	49603/udp	0.000502
unknown	49605/udp	0.000502
unknown	49608/udp	0.000502
unknown	49615/udp	0.000502
unknown	49618/udp	0.000502
unknown	49619/udp	0.000502
unknown	49620/udp	0.001004
unknown	49622/udp	0.000502
unknown	49631/udp	0.000502
unknown	49633/udp	0.000502
unknown	49635/udp	0.000502
unknown	49639/udp	0.001004
unknown	49640/udp	0.001506
unknown	49642/udp	0.000502
unknown	49644/udp	0.000502
unknown	49651/udp	0.000502
unknown	49653/udp	0.000502
unknown	49654/udp	0.000502
unknown	49656/udp	0.000502
unknown	49668/udp	0.000502
unknown	49669/udp	0.001004
unknown	49678/tcp	0.000076
unknown	49685/udp	0.000502
unknown	49692/udp	0.000502
unknown	49698/udp	0.000502
unknown	49705/udp	0.000502
unknown	49708/udp	0.000502
unknown	49709/udp	0.000502
unknown	49717/udp	0.000502
unknown	49718/udp	0.000502
unknown	49720/udp	0.000502
unknown	49721/udp	0.000502
unknown	49735/udp	0.000502
unknown	49737/udp	0.000502
unknown	49741/udp	0.000502
unknown	49746/udp	0.001004
unknown	49748/udp	0.000502
unknown	49750/udp	0.000502
unknown	49751/tcp	0.000076
unknown	49754/udp	0.001004
unknown	49757/udp	0.000502
unknown	49760/udp	0.000502
unknown	49761/udp	0.000502
unknown	49762/tcp	0.000076
unknown	49764/udp	0.000502
unknown	49765/tcp	0.000076
unknown	49772/udp	0.000502
unknown	49773/udp	0.000502
unknown	49775/udp	0.000502
unknown	49776/udp	0.000502
unknown	49780/udp	0.000502
unknown	49781/udp	0.000502
unknown	49783/udp	0.000502
unknown	49785/udp	0.000502
unknown	49793/udp	0.000502
unknown	49801/udp	0.001004
unknown	49802/udp	0.000502
unknown	49803/tcp	0.000076
unknown	49809/udp	0.000502
unknown	49818/udp	0.000502
unknown	49824/udp	0.000502
unknown	49825/udp	0.000502
unknown	49837/udp	0.000502
unknown	49839/udp	0.001004
unknown	49847/udp	0.000502
unknown	49848/udp	0.000502
unknown	49852/udp	0.000502
unknown	49855/udp	0.000502
unknown	49865/udp	0.000502
unknown	49871/udp	0.000502
unknown	49873/udp	0.000502
unknown	49874/udp	0.000502
unknown	49875/udp	0.000502
unknown	49887/udp	0.000502
unknown	49890/udp	0.000502
unknown	49893/udp	0.000502
unknown	49894/udp	0.000502
unknown	49895/udp	0.000502
unknown	49906/udp	0.000502
unknown	49907/udp	0.000502
unknown	49912/udp	0.000502
unknown	49919/udp	0.000502
unknown	49926/udp	0.001004
unknown	49927/tcp	0.000076
unknown	49930/udp	0.000502
unknown	49935/udp	0.000502
unknown	49939/udp	0.001004
unknown	49942/udp	0.000502
unknown	49945/udp	0.001004
unknown	49955/udp	0.000502
unknown	49957/udp	0.000502
unknown	49960/udp	0.000502
unknown	49962/udp	0.000502
unknown	49964/udp	0.000502
unknown	49965/udp	0.000502
unknown	49968/udp	0.001506
unknown	49969/udp	0.000502
unknown	49978/udp	0.000502
unknown	49984/udp	0.001004
unknown	49986/udp	0.001004
unknown	49990/udp	0.001004
unknown	49996/udp	0.000502
unknown	49998/udp	0.001004
unknown	49999/tcp	0.000684
ibm-db2	50000/tcp	0.001317	# (also Internet/Intranet Input Method Server Framework?)
unknown	50001/tcp	0.000836
iiimsf	50002/tcp	0.000351	# Internet/Intranet Input Method Server Framework
unknown	50003/tcp	0.000380
unknown	50006/tcp	0.000380
unknown	50009/udp	0.001004
unknown	50015/udp	0.000502
unknown	50016/tcp	0.000076
unknown	50019/tcp	0.000076
unknown	50020/udp	0.000502
unknown	50024/udp	0.001004
unknown	50029/udp	0.000502
unknown	50033/udp	0.000502
unknown	50040/tcp	0.000076
unknown	50041/udp	0.001004
unknown	50044/udp	0.000502
unknown	50049/udp	0.001004
unknown	50050/tcp	0.000152
unknown	50058/udp	0.000502
unknown	50060/udp	0.000502
unknown	50065/udp	0.000502
unknown	50067/udp	0.000502
unknown	50075/udp	0.000502
unknown	50085/udp	0.001004
unknown	50093/udp	0.000502
unknown	50096/udp	0.000502
unknown	50099/udp	0.001506
unknown	50100/udp	0.000502
unknown	50101/tcp	0.000076
unknown	50103/udp	0.000502
unknown	50105/udp	0.000502
unknown	50106/udp	0.000502
unknown	50114/udp	0.000502
unknown	50119/udp	0.000502
unknown	50121/udp	0.000502
unknown	50122/udp	0.001004
unknown	50127/udp	0.001004
unknown	50131/udp	0.000502
unknown	50133/udp	0.000502
unknown	50134/udp	0.000502
unknown	50136/udp	0.000502
unknown	50143/udp	0.001004
unknown	50146/udp	0.000502
unknown	50149/udp	0.001004
unknown	50154/udp	0.000502
unknown	50155/udp	0.000502
unknown	50157/udp	0.000502
unknown	50162/udp	0.000502
unknown	50163/udp	0.001004
unknown	50164/udp	0.001506
unknown	50173/udp	0.000502
unknown	50175/udp	0.000502
unknown	50177/udp	0.000502
unknown	50183/udp	0.000502
unknown	50187/udp	0.000502
unknown	50189/tcp	0.000076
unknown	50189/udp	0.000502
unknown	50190/udp	0.000502
unknown	50191/udp	0.000502
unknown	50192/udp	0.000502
unknown	50197/udp	0.000502
unknown	50198/tcp	0.000076
unknown	50202/tcp	0.000076
unknown	50205/tcp	0.000076
unknown	50209/udp	0.000502
unknown	50212/udp	0.000502
unknown	50213/udp	0.000502
unknown	50218/udp	0.000502
unknown	50222/udp	0.000502
unknown	50224/tcp	0.000076
unknown	50234/udp	0.000502
unknown	50239/udp	0.001004
unknown	50246/tcp	0.000076
unknown	50246/udp	0.000502
unknown	50249/udp	0.000502
unknown	50251/udp	0.000502
unknown	50255/udp	0.000502
unknown	50258/tcp	0.000076
unknown	50264/udp	0.000502
unknown	50266/udp	0.000502
unknown	50273/udp	0.001004
unknown	50276/udp	0.000502
unknown	50277/tcp	0.000076
unknown	50282/udp	0.000502
unknown	50287/udp	0.000502
unknown	50288/udp	0.000502
unknown	50289/udp	0.000502
unknown	50295/udp	0.000502
unknown	50296/udp	0.001004
unknown	50300/tcp	0.000228
unknown	50300/udp	0.001004
unknown	50304/udp	0.000502
unknown	50305/udp	0.000502
unknown	50308/udp	0.000502
unknown	50315/udp	0.000502
unknown	50326/udp	0.000502
unknown	50328/udp	0.000502
unknown	50329/udp	0.000502
unknown	50338/udp	0.000502
unknown	50345/udp	0.001004
unknown	50349/udp	0.001004
unknown	50351/udp	0.000502
unknown	50352/udp	0.000502
unknown	50356/tcp	0.000076
unknown	50361/udp	0.000502
unknown	50364/udp	0.000502
unknown	50374/udp	0.000502
unknown	50376/udp	0.001004
unknown	50378/udp	0.000502
unknown	50382/udp	0.000502
unknown	50385/udp	0.000502
unknown	50387/udp	0.000502
unknown	50388/udp	0.000502
unknown	50389/tcp	0.000304
unknown	50404/udp	0.000502
unknown	50409/udp	0.001004
unknown	50411/udp	0.000502
unknown	50413/udp	0.000502
unknown	50420/udp	0.001004
unknown	50427/udp	0.001004
unknown	50430/udp	0.000502
unknown	50434/udp	0.000502
unknown	50439/udp	0.000502
unknown	50443/udp	0.000502
unknown	50444/udp	0.000502
unknown	50446/udp	0.000502
unknown	50447/udp	0.001004
unknown	50448/udp	0.000502
unknown	50453/udp	0.000502
unknown	50461/udp	0.000502
unknown	50470/udp	0.000502
unknown	50474/udp	0.001004
unknown	50475/udp	0.000502
unknown	50476/udp	0.000502
unknown	50484/udp	0.000502
unknown	50492/udp	0.000502
unknown	50493/udp	0.000502
unknown	50494/udp	0.000502
unknown	50497/udp	0.001506
unknown	50500/tcp	0.000228
unknown	50503/udp	0.000502
unknown	50506/udp	0.000502
unknown	50507/udp	0.000502
unknown	50511/udp	0.000502
unknown	50513/tcp	0.000076
unknown	50515/udp	0.000502
unknown	50520/udp	0.000502
unknown	50523/udp	0.001004
unknown	50529/tcp	0.000076
unknown	50533/udp	0.000502
unknown	50536/udp	0.000502
unknown	50545/tcp	0.000076
unknown	50546/udp	0.000502
unknown	50551/udp	0.000502
unknown	50556/udp	0.000502
unknown	50559/udp	0.000502
unknown	50573/udp	0.001004
unknown	50574/udp	0.001004
unknown	50575/udp	0.000502
unknown	50576/tcp	0.000076
unknown	50576/udp	0.000502
unknown	50577/tcp	0.000076
unknown	50577/udp	0.000502
unknown	50579/udp	0.001004
unknown	50585/tcp	0.000076
unknown	50587/udp	0.000502
unknown	50595/udp	0.000502
unknown	50598/udp	0.000502
unknown	50604/udp	0.000502
unknown	50610/udp	0.000502
unknown	50612/udp	0.002008
unknown	50614/udp	0.000502
unknown	50615/udp	0.000502
unknown	50618/udp	0.000502
unknown	50620/udp	0.001004
unknown	50622/udp	0.001004
unknown	50624/udp	0.000502
unknown	50626/udp	0.000502
unknown	50627/udp	0.000502
unknown	50629/udp	0.000502
unknown	50635/udp	0.000502
unknown	50636/tcp	0.000304
unknown	50649/udp	0.001004
unknown	50653/udp	0.000502
unknown	50655/udp	0.000502
unknown	50672/udp	0.000502
unknown	50678/udp	0.000502
unknown	50679/udp	0.000502
unknown	50680/udp	0.000502
unknown	50690/udp	0.000502
unknown	50692/tcp	0.000076
unknown	50703/udp	0.000502
unknown	50707/udp	0.000502
unknown	50708/udp	0.001506
unknown	50711/udp	0.000502
unknown	50712/udp	0.000502
unknown	50714/udp	0.000502
unknown	50722/udp	0.001004
unknown	50729/udp	0.000502
unknown	50733/tcp	0.000076
unknown	50734/udp	0.000502
unknown	50735/udp	0.000502
unknown	50749/udp	0.000502
unknown	50750/udp	0.000502
unknown	50756/udp	0.001004
unknown	50766/udp	0.000502
unknown	50768/udp	0.000502
unknown	50777/udp	0.000502
unknown	50786/udp	0.000502
unknown	50787/tcp	0.000076
unknown	50789/udp	0.000502
unknown	50790/udp	0.000502
unknown	50797/udp	0.000502
unknown	50800/tcp	0.000380
unknown	50802/udp	0.000502
unknown	50807/udp	0.000502
unknown	50809/tcp	0.000076
unknown	50811/udp	0.000502
unknown	50814/udp	0.000502
unknown	50815/tcp	0.000076
unknown	50831/tcp	0.000076
unknown	50833/tcp	0.000076
unknown	50834/tcp	0.000076
unknown	50834/udp	0.000502
unknown	50835/tcp	0.000076
unknown	50835/udp	0.000502
unknown	50836/tcp	0.000076
unknown	50848/udp	0.000502
unknown	50849/tcp	0.000076
unknown	50851/udp	0.000502
unknown	50854/tcp	0.000076
unknown	50860/udp	0.000502
unknown	50862/udp	0.000502
unknown	50868/udp	0.000502
unknown	50870/udp	0.000502
unknown	50873/udp	0.000502
unknown	50881/udp	0.000502
unknown	50883/udp	0.000502
unknown	50886/udp	0.000502
unknown	50887/tcp	0.000076
unknown	50891/udp	0.000502
unknown	50895/udp	0.000502
unknown	50896/udp	0.001004
unknown	50900/udp	0.001004
unknown	50903/tcp	0.000076
unknown	50904/udp	0.001004
unknown	50913/udp	0.001004
unknown	50919/udp	0.001506
unknown	50921/udp	0.000502
unknown	50925/udp	0.000502
unknown	50937/udp	0.000502
unknown	50939/udp	0.000502
unknown	50941/udp	0.000502
unknown	50942/udp	0.000502
unknown	50945/tcp	0.000076
unknown	50954/udp	0.000502
unknown	50959/udp	0.000502
unknown	50960/udp	0.000502
unknown	50974/udp	0.000502
unknown	50977/udp	0.000502
unknown	50981/udp	0.000502
unknown	50982/udp	0.000502
unknown	50985/udp	0.000502
unknown	50987/udp	0.000502
unknown	50990/udp	0.001004
unknown	50994/udp	0.000502
unknown	50995/udp	0.000502
unknown	50997/tcp	0.000076
unknown	50998/udp	0.000502
unknown	51000/udp	0.000502
unknown	51004/udp	0.000502
unknown	51011/tcp	0.000076
unknown	51013/udp	0.001004
unknown	51014/udp	0.001004
unknown	51016/udp	0.000502
unknown	51020/tcp	0.000076
unknown	51020/udp	0.001004
unknown	51021/udp	0.000502
unknown	51023/udp	0.000502
unknown	51025/udp	0.000502
unknown	51027/udp	0.000502
unknown	51037/tcp	0.000076
unknown	51042/udp	0.000502
unknown	51045/udp	0.000502
unknown	51047/udp	0.000502
unknown	51067/tcp	0.000076
unknown	51074/udp	0.000502
unknown	51080/udp	0.000502
unknown	51083/udp	0.000502
unknown	51086/udp	0.000502
unknown	51087/udp	0.000502
unknown	51092/udp	0.000502
unknown	51093/udp	0.000502
unknown	51098/udp	0.000502
unknown	51101/udp	0.000502
unknown	51103/tcp	0.000684
unknown	51111/udp	0.000502
unknown	51112/udp	0.000502
unknown	51118/tcp	0.000076
unknown	51118/udp	0.000502
unknown	51120/udp	0.001004
unknown	51124/udp	0.000502
unknown	51127/udp	0.000502
unknown	51137/udp	0.000502
unknown	51138/udp	0.000502
unknown	51139/tcp	0.000076
unknown	51142/udp	0.000502
unknown	51143/udp	0.001004
unknown	51156/udp	0.000502
unknown	51165/udp	0.000502
unknown	51167/udp	0.001004
unknown	51169/udp	0.000502
unknown	51172/udp	0.001004
unknown	51180/udp	0.000502
unknown	51185/udp	0.000502
unknown	51191/tcp	0.000152
unknown	51193/udp	0.001004
unknown	51195/udp	0.000502
unknown	51199/udp	0.000502
unknown	51211/udp	0.001004
unknown	51212/udp	0.000502
unknown	51221/udp	0.000502
unknown	51225/udp	0.001004
unknown	51233/tcp	0.000076
unknown	51233/udp	0.000502
unknown	51234/tcp	0.000076
unknown	51235/tcp	0.000076
unknown	51240/tcp	0.000076
unknown	51244/udp	0.000502
unknown	51250/udp	0.000502
unknown	51251/udp	0.000502
unknown	51255/udp	0.001506
unknown	51264/udp	0.000502
unknown	51265/udp	0.000502
unknown	51267/udp	0.001004
unknown	51273/udp	0.000502
unknown	51274/udp	0.000502
unknown	51275/udp	0.000502
unknown	51279/udp	0.000502
unknown	51280/udp	0.001004
unknown	51281/udp	0.000502
unknown	51286/udp	0.000502
unknown	51294/udp	0.000502
unknown	51295/udp	0.000502
unknown	51300/tcp	0.000076
unknown	51304/udp	0.000502
unknown	51309/udp	0.000502
unknown	51322/udp	0.000502
unknown	51323/udp	0.001004
unknown	51327/udp	0.000502
unknown	51343/tcp	0.000076
unknown	51351/tcp	0.000076
unknown	51351/udp	0.000502
unknown	51364/udp	0.000502
unknown	51365/udp	0.000502
unknown	51366/tcp	0.000076
unknown	51366/udp	0.000502
unknown	51375/udp	0.000502
unknown	51378/udp	0.000502
unknown	51382/udp	0.000502
unknown	51383/udp	0.001004
unknown	51386/udp	0.000502
unknown	51387/udp	0.000502
unknown	51393/udp	0.000502
unknown	51398/udp	0.000502
unknown	51400/udp	0.001004
unknown	51402/udp	0.000502
unknown	51405/udp	0.000502
unknown	51407/udp	0.001004
unknown	51413/tcp	0.000152
unknown	51418/udp	0.000502
unknown	51423/tcp	0.000076
unknown	51426/udp	0.000502
unknown	51427/udp	0.001004
unknown	51429/udp	0.000502
unknown	51432/udp	0.000502
unknown	51438/udp	0.000502
unknown	51450/udp	0.000502
unknown	51456/udp	0.001506
unknown	51460/tcp	0.000076
unknown	51462/udp	0.000502
unknown	51465/udp	0.000502
unknown	51466/udp	0.000502
unknown	51471/udp	0.001004
unknown	51474/udp	0.000502
unknown	51477/udp	0.001004
unknown	51484/tcp	0.000076
unknown	51485/tcp	0.000076
unknown	51485/udp	0.000502
unknown	51486/udp	0.000502
unknown	51487/udp	0.000502
unknown	51488/tcp	0.000076
unknown	51493/tcp	0.000304
unknown	51500/udp	0.000502
unknown	51503/udp	0.000502
unknown	51506/udp	0.000502
unknown	51509/udp	0.000502
unknown	51515/tcp	0.000076
unknown	51515/udp	0.000502
unknown	51516/udp	0.000502
unknown	51517/udp	0.000502
unknown	51520/udp	0.000502
unknown	51524/udp	0.000502
unknown	51534/udp	0.000502
unknown	51535/udp	0.000502
unknown	51544/udp	0.001004
unknown	51551/udp	0.000502
unknown	51554/udp	0.001506
unknown	51556/udp	0.000502
unknown	51559/udp	0.000502
unknown	51562/udp	0.000502
unknown	51580/udp	0.000502
unknown	51581/udp	0.001004
unknown	51582/tcp	0.000076
unknown	51582/udp	0.000502
unknown	51583/udp	0.000502
unknown	51584/udp	0.000502
unknown	51585/udp	0.000502
unknown	51586/udp	0.001506
unknown	51587/udp	0.000502
unknown	51588/udp	0.000502
unknown	51589/udp	0.001004
unknown	51590/udp	0.000502
unknown	51591/udp	0.000502
unknown	51592/udp	0.000502
unknown	51596/udp	0.000502
unknown	51602/udp	0.000502
unknown	51603/udp	0.000502
unknown	51606/udp	0.000502
unknown	51614/udp	0.000502
unknown	51621/udp	0.000502
unknown	51628/udp	0.000502
unknown	51634/udp	0.000502
unknown	51638/udp	0.000502
unknown	51644/udp	0.000502
unknown	51646/udp	0.000502
unknown	51649/udp	0.001004
unknown	51651/udp	0.000502
unknown	51656/udp	0.000502
unknown	51657/udp	0.000502
unknown	51658/tcp	0.000076
unknown	51662/udp	0.000502
unknown	51668/udp	0.000502
unknown	51670/udp	0.000502
unknown	51677/udp	0.000502
unknown	51683/udp	0.000502
unknown	51684/udp	0.000502
unknown	51690/udp	0.001506
unknown	51705/udp	0.000502
unknown	51710/udp	0.001004
unknown	51712/udp	0.000502
unknown	51714/udp	0.000502
unknown	51717/udp	0.002008
unknown	51718/udp	0.000502
unknown	51724/udp	0.000502
unknown	51738/udp	0.000502
unknown	51749/udp	0.000502
unknown	51751/udp	0.000502
unknown	51753/udp	0.000502
unknown	51760/udp	0.000502
unknown	51763/udp	0.000502
unknown	51765/udp	0.000502
unknown	51768/udp	0.000502
unknown	51771/tcp	0.000076
unknown	51772/tcp	0.000076
unknown	51781/udp	0.001004
unknown	51788/udp	0.000502
unknown	51800/tcp	0.000076
unknown	51804/udp	0.000502
unknown	51805/udp	0.000502
unknown	51807/udp	0.000502
unknown	51809/tcp	0.000076
unknown	51809/udp	0.000502
unknown	51820/udp	0.000502
unknown	51823/udp	0.000502
unknown	51825/udp	0.000502
unknown	51828/udp	0.000502
unknown	51837/udp	0.000502
unknown	51843/udp	0.001004
unknown	51845/udp	0.000502
unknown	51846/udp	0.000502
unknown	51847/udp	0.001004
unknown	51848/udp	0.000502
unknown	51855/udp	0.000502
unknown	51857/udp	0.000502
unknown	51859/udp	0.000502
unknown	51860/udp	0.000502
unknown	51861/udp	0.000502
unknown	51864/udp	0.000502
unknown	51865/udp	0.000502
unknown	51869/udp	0.000502
unknown	51871/udp	0.000502
unknown	51882/udp	0.000502
unknown	51894/udp	0.001004
unknown	51903/udp	0.001004
unknown	51905/udp	0.001506
unknown	51906/tcp	0.000076
unknown	51908/udp	0.000502
unknown	51909/tcp	0.000076
unknown	51918/udp	0.000502
unknown	51921/udp	0.000502
unknown	51927/udp	0.000502
unknown	51936/udp	0.000502
unknown	51949/udp	0.000502
unknown	51950/udp	0.000502
unknown	51952/udp	0.000502
unknown	51960/udp	0.000502
unknown	51961/tcp	0.000076
unknown	51961/udp	0.000502
unknown	51965/tcp	0.000076
unknown	51965/udp	0.000502
unknown	51966/udp	0.000502
unknown	51969/udp	0.000502
unknown	51972/udp	0.001506
unknown	51976/udp	0.000502
unknown	51991/udp	0.000502
unknown	52000/tcp	0.000076
unknown	52001/tcp	0.000076
unknown	52002/tcp	0.000076
unknown	52003/tcp	0.000076
unknown	52003/udp	0.000502
unknown	52004/udp	0.000502
unknown	52005/udp	0.000502
unknown	52006/udp	0.001004
unknown	52012/udp	0.000502
unknown	52016/udp	0.000502
unknown	52019/udp	0.000502
unknown	52025/tcp	0.000076
unknown	52025/udp	0.000502
unknown	52027/udp	0.000502
unknown	52038/udp	0.000502
unknown	52046/tcp	0.000076
unknown	52046/udp	0.000502
unknown	52049/udp	0.000502
unknown	52052/udp	0.000502
unknown	52057/udp	0.000502
unknown	52059/udp	0.000502
unknown	52064/udp	0.000502
unknown	52071/tcp	0.000076
unknown	52072/udp	0.000502
unknown	52081/udp	0.000502
unknown	52088/udp	0.000502
unknown	52089/udp	0.001004
unknown	52092/udp	0.000502
unknown	52099/udp	0.000502
unknown	52100/udp	0.000502
unknown	52103/udp	0.000502
unknown	52106/udp	0.000502
unknown	52107/udp	0.000502
unknown	52109/udp	0.000502
unknown	52114/udp	0.000502
unknown	52121/udp	0.000502
unknown	52127/udp	0.000502
unknown	52130/udp	0.001004
unknown	52133/udp	0.000502
unknown	52138/udp	0.001004
unknown	52141/udp	0.000502
unknown	52144/udp	0.001506
unknown	52148/udp	0.000502
unknown	52151/udp	0.000502
unknown	52152/udp	0.000502
unknown	52154/udp	0.000502
unknown	52155/udp	0.001004
unknown	52158/udp	0.000502
unknown	52167/udp	0.000502
unknown	52173/tcp	0.000076
unknown	52178/udp	0.000502
unknown	52182/udp	0.000502
unknown	52194/udp	0.000502
unknown	52195/udp	0.000502
unknown	52197/udp	0.000502
unknown	52201/udp	0.000502
unknown	52203/udp	0.000502
unknown	52211/udp	0.000502
unknown	52212/udp	0.000502
unknown	52220/udp	0.001004
unknown	52222/udp	0.000502
unknown	52224/udp	0.001004
unknown	52225/tcp	0.000076
unknown	52225/udp	0.003012
unknown	52226/tcp	0.000076
unknown	52227/udp	0.001004
unknown	52228/udp	0.000502
unknown	52230/tcp	0.000076
unknown	52237/tcp	0.000076
unknown	52237/udp	0.000502
unknown	52248/udp	0.000502
unknown	52253/udp	0.000502
unknown	52254/udp	0.001004
unknown	52255/udp	0.000502
unknown	52258/udp	0.000502
unknown	52260/udp	0.000502
unknown	52262/tcp	0.000076
unknown	52268/udp	0.000502
unknown	52276/udp	0.000502
unknown	52277/udp	0.000502
unknown	52278/udp	0.000502
unknown	52279/udp	0.000502
unknown	52287/udp	0.000502
unknown	52294/udp	0.000502
unknown	52298/udp	0.000502
unknown	52302/udp	0.000502
unknown	52306/udp	0.000502
unknown	52315/udp	0.000502
unknown	52316/udp	0.000502
unknown	52317/udp	0.000502
unknown	52321/udp	0.000502
unknown	52330/udp	0.000502
unknown	52331/udp	0.000502
unknown	52332/udp	0.000502
unknown	52333/udp	0.001004
unknown	52335/udp	0.000502
unknown	52336/udp	0.000502
unknown	52344/udp	0.000502
unknown	52350/udp	0.000502
unknown	52356/udp	0.000502
unknown	52361/udp	0.000502
unknown	52364/udp	0.001004
unknown	52368/udp	0.000502
unknown	52375/udp	0.000502
unknown	52391/tcp	0.000076
unknown	52394/udp	0.000502
unknown	52395/udp	0.000502
unknown	52402/udp	0.000502
unknown	52408/udp	0.000502
unknown	52412/udp	0.001004
unknown	52419/udp	0.000502
unknown	52420/udp	0.000502
unknown	52424/udp	0.000502
unknown	52425/udp	0.000502
unknown	52428/udp	0.000502
unknown	52443/udp	0.000502
unknown	52451/udp	0.000502
unknown	52460/udp	0.000502
unknown	52467/udp	0.000502
unknown	52477/tcp	0.000076
unknown	52478/udp	0.000502
unknown	52480/udp	0.000502
unknown	52492/udp	0.000502
unknown	52494/udp	0.000502
unknown	52496/udp	0.000502
unknown	52499/udp	0.000502
unknown	52503/udp	0.002510
unknown	52506/tcp	0.000076
unknown	52509/udp	0.000502
unknown	52515/udp	0.000502
unknown	52516/udp	0.001004
unknown	52519/udp	0.000502
unknown	52524/udp	0.000502
unknown	52533/udp	0.000502
unknown	52540/udp	0.000502
unknown	52552/udp	0.000502
unknown	52571/udp	0.001004
unknown	52573/tcp	0.000076
unknown	52580/udp	0.000502
unknown	52582/udp	0.001004
unknown	52585/udp	0.000502
unknown	52592/udp	0.000502
unknown	52596/udp	0.000502
unknown	52610/udp	0.000502
unknown	52616/udp	0.000502
unknown	52620/udp	0.000502
unknown	52623/udp	0.000502
unknown	52628/udp	0.000502
unknown	52649/udp	0.001004
unknown	52651/udp	0.000502
unknown	52660/tcp	0.000152
unknown	52663/udp	0.000502
unknown	52665/tcp	0.000076
unknown	52667/udp	0.000502
unknown	52669/udp	0.000502
unknown	52671/udp	0.000502
unknown	52673/tcp	0.000228
unknown	52674/udp	0.001004
unknown	52675/tcp	0.000076
unknown	52677/udp	0.000502
unknown	52679/udp	0.000502
unknown	52685/udp	0.000502
unknown	52692/udp	0.000502
unknown	52696/udp	0.000502
unknown	52700/udp	0.000502
unknown	52706/udp	0.001004
unknown	52710/tcp	0.000152
unknown	52713/udp	0.001004
unknown	52716/udp	0.000502
unknown	52724/udp	0.000502
unknown	52726/udp	0.000502
unknown	52727/udp	0.000502
unknown	52734/udp	0.000502
unknown	52735/tcp	0.000152
unknown	52740/udp	0.000502
unknown	52755/udp	0.000502
unknown	52761/udp	0.000502
unknown	52762/udp	0.001004
unknown	52766/udp	0.000502
unknown	52772/udp	0.001004
unknown	52775/udp	0.000502
unknown	52780/udp	0.000502
unknown	52781/udp	0.000502
unknown	52791/udp	0.000502
unknown	52792/udp	0.001004
unknown	52806/udp	0.000502
unknown	52807/udp	0.000502
unknown	52813/udp	0.001004
unknown	52815/udp	0.000502
unknown	52817/udp	0.000502
unknown	52820/udp	0.000502
unknown	52821/udp	0.000502
unknown	52822/tcp	0.000456
unknown	52825/udp	0.000502
unknown	52830/udp	0.000502
unknown	52833/udp	0.000502
unknown	52844/udp	0.000502
unknown	52845/udp	0.000502
unknown	52847/tcp	0.000152
unknown	52847/udp	0.000502
unknown	52848/tcp	0.000228
unknown	52848/udp	0.000502
unknown	52849/tcp	0.000152
unknown	52849/udp	0.000502
unknown	52850/tcp	0.000152
unknown	52851/tcp	0.000152
unknown	52853/tcp	0.000152
unknown	52861/udp	0.001004
unknown	52864/udp	0.000502
unknown	52865/udp	0.000502
unknown	52869/tcp	0.000760
unknown	52872/udp	0.000502
unknown	52886/udp	0.000502
unknown	52887/udp	0.000502
unknown	52889/udp	0.000502
unknown	52891/udp	0.000502
unknown	52893/tcp	0.000076
unknown	52894/udp	0.000502
unknown	52899/udp	0.000502
unknown	52908/udp	0.000502
unknown	52909/udp	0.000502
unknown	52915/udp	0.000502
unknown	52916/udp	0.000502
unknown	52920/udp	0.000502
unknown	52931/udp	0.000502
unknown	52934/udp	0.000502
unknown	52938/udp	0.000502
unknown	52944/udp	0.000502
unknown	52945/udp	0.001004
unknown	52946/udp	0.000502
unknown	52947/udp	0.000502
unknown	52948/tcp	0.000076
unknown	52950/udp	0.000502
unknown	52956/udp	0.000502
unknown	52959/udp	0.000502
unknown	52965/udp	0.000502
unknown	52966/udp	0.000502
unknown	52967/udp	0.000502
unknown	52969/udp	0.000502
unknown	52981/udp	0.000502
unknown	52992/udp	0.000502
unknown	52994/udp	0.000502
unknown	53000/udp	0.000502
unknown	53006/udp	0.001506
unknown	53008/udp	0.000502
unknown	53011/udp	0.000502
unknown	53014/udp	0.000502
unknown	53015/udp	0.000502
unknown	53019/udp	0.000502
unknown	53020/udp	0.000502
unknown	53023/udp	0.001004
unknown	53024/udp	0.000502
unknown	53029/udp	0.000502
unknown	53033/udp	0.000502
unknown	53034/udp	0.000502
unknown	53036/udp	0.000502
unknown	53037/udp	0.001506
unknown	53044/udp	0.000502
unknown	53050/udp	0.000502
unknown	53059/udp	0.000502
unknown	53069/udp	0.000502
unknown	53070/udp	0.000502
unknown	53071/udp	0.000502
unknown	53073/udp	0.000502
unknown	53079/udp	0.000502
unknown	53080/udp	0.000502
unknown	53084/udp	0.001004
unknown	53085/tcp	0.000076
unknown	53085/udp	0.000502
unknown	53094/udp	0.000502
unknown	53098/udp	0.000502
unknown	53101/udp	0.000502
unknown	53112/udp	0.000502
unknown	53126/udp	0.001004
unknown	53128/udp	0.000502
unknown	53135/udp	0.000502
unknown	53142/udp	0.000502
unknown	53153/udp	0.000502
unknown	53157/udp	0.000502
unknown	53160/udp	0.000502
unknown	53161/udp	0.001004
unknown	53164/udp	0.000502
unknown	53176/udp	0.000502
unknown	53178/tcp	0.000076
unknown	53179/udp	0.000502
unknown	53182/udp	0.001004
unknown	53189/tcp	0.000076
unknown	53191/udp	0.000502
unknown	53198/udp	0.000502
unknown	53199/udp	0.000502
unknown	53200/udp	0.000502
unknown	53202/udp	0.000502
unknown	53208/udp	0.000502
unknown	53211/tcp	0.000152
unknown	53212/tcp	0.000076
unknown	53212/udp	0.001004
unknown	53218/udp	0.000502
unknown	53222/udp	0.000502
unknown	53228/udp	0.001004
unknown	53240/tcp	0.000076
unknown	53242/udp	0.000502
unknown	53245/udp	0.000502
unknown	53246/udp	0.000502
unknown	53249/udp	0.001004
unknown	53250/udp	0.000502
unknown	53252/udp	0.000502
unknown	53258/udp	0.000502
unknown	53260/udp	0.000502
unknown	53265/udp	0.000502
unknown	53266/udp	0.000502
unknown	53271/udp	0.000502
unknown	53273/udp	0.000502
unknown	53276/udp	0.000502
unknown	53279/udp	0.001004
unknown	53284/udp	0.000502
unknown	53285/udp	0.000502
unknown	53286/udp	0.001004
unknown	53292/udp	0.000502
unknown	53301/udp	0.000502
unknown	53305/udp	0.000502
unknown	53308/udp	0.000502
unknown	53311/udp	0.000502
unknown	53313/tcp	0.000152
unknown	53313/udp	0.000502
unknown	53314/tcp	0.000152
unknown	53318/udp	0.000502
unknown	53319/tcp	0.000076
unknown	53321/udp	0.000502
unknown	53322/udp	0.000502
unknown	53326/udp	0.000502
unknown	53331/udp	0.000502
unknown	53332/udp	0.000502
unknown	53336/udp	0.000502
unknown	53339/udp	0.000502
unknown	53340/udp	0.000502
unknown	53341/udp	0.000502
unknown	53347/udp	0.000502
unknown	53361/tcp	0.000076
unknown	53362/udp	0.000502
unknown	53366/udp	0.000502
unknown	53367/udp	0.001004
unknown	53370/tcp	0.000076
unknown	53373/udp	0.000502
unknown	53375/udp	0.000502
unknown	53385/udp	0.000502
unknown	53389/udp	0.000502
unknown	53390/udp	0.000502
unknown	53392/udp	0.000502
unknown	53393/udp	0.000502
unknown	53396/udp	0.001004
unknown	53399/udp	0.000502
unknown	53401/udp	0.000502
unknown	53403/udp	0.001004
unknown	53410/udp	0.000502
unknown	53412/udp	0.000502
unknown	53420/udp	0.000502
unknown	53421/udp	0.000502
unknown	53433/udp	0.001004
unknown	53434/udp	0.000502
unknown	53442/udp	0.000502
unknown	53455/udp	0.000502
unknown	53458/udp	0.000502
unknown	53460/tcp	0.000076
unknown	53460/udp	0.001004
unknown	53468/udp	0.000502
unknown	53469/tcp	0.000076
unknown	53470/udp	0.000502
unknown	53491/tcp	0.000076
unknown	53491/udp	0.000502
unknown	53500/udp	0.000502
unknown	53503/udp	0.000502
unknown	53505/udp	0.000502
unknown	53507/udp	0.000502
unknown	53513/udp	0.000502
unknown	53514/udp	0.000502
unknown	53516/udp	0.000502
unknown	53517/udp	0.000502
unknown	53520/udp	0.000502
unknown	53526/udp	0.000502
unknown	53528/udp	0.000502
unknown	53535/tcp	0.000152
unknown	53535/udp	0.000502
unknown	53536/udp	0.000502
unknown	53537/udp	0.000502
unknown	53539/udp	0.000502
unknown	53545/udp	0.000502
unknown	53549/udp	0.000502
unknown	53551/udp	0.000502
unknown	53554/udp	0.001004
unknown	53555/udp	0.000502
unknown	53560/udp	0.000502
unknown	53562/udp	0.000502
unknown	53564/udp	0.000502
unknown	53571/udp	0.002510
unknown	53574/udp	0.000502
unknown	53586/udp	0.000502
unknown	53589/udp	0.001506
unknown	53620/udp	0.000502
unknown	53633/tcp	0.000076
unknown	53633/udp	0.000502
unknown	53635/udp	0.000502
unknown	53639/tcp	0.000076
unknown	53643/udp	0.000502
unknown	53645/udp	0.000502
unknown	53647/udp	0.000502
unknown	53649/udp	0.000502
unknown	53651/udp	0.001004
unknown	53656/tcp	0.000076
unknown	53660/udp	0.000502
unknown	53670/udp	0.000502
unknown	53674/udp	0.000502
unknown	53677/udp	0.000502
unknown	53678/udp	0.000502
unknown	53684/udp	0.000502
unknown	53685/udp	0.000502
unknown	53688/udp	0.000502
unknown	53690/tcp	0.000076
unknown	53695/udp	0.000502
unknown	53702/udp	0.000502
unknown	53708/udp	0.000502
unknown	53723/udp	0.000502
unknown	53724/udp	0.000502
unknown	53730/udp	0.000502
unknown	53731/udp	0.000502
unknown	53732/udp	0.000502
unknown	53733/udp	0.000502
unknown	53735/udp	0.000502
unknown	53740/udp	0.000502
unknown	53742/tcp	0.000076
unknown	53750/udp	0.000502
unknown	53751/udp	0.000502
unknown	53753/udp	0.000502
unknown	53758/udp	0.000502
unknown	53761/udp	0.000502
unknown	53766/udp	0.000502
unknown	53768/udp	0.000502
unknown	53769/udp	0.000502
unknown	53780/udp	0.000502
unknown	53782/tcp	0.000076
unknown	53787/udp	0.000502
unknown	53797/udp	0.000502
unknown	53808/udp	0.000502
unknown	53813/udp	0.000502
unknown	53826/udp	0.000502
unknown	53827/tcp	0.000076
unknown	53829/udp	0.000502
unknown	53830/udp	0.001004
unknown	53835/udp	0.000502
unknown	53836/udp	0.000502
unknown	53838/udp	0.001506
unknown	53847/udp	0.000502
unknown	53852/tcp	0.000076
unknown	53857/udp	0.000502
unknown	53860/udp	0.000502
unknown	53867/udp	0.000502
unknown	53880/udp	0.001004
unknown	53882/udp	0.000502
unknown	53887/udp	0.000502
unknown	53888/udp	0.000502
unknown	53894/udp	0.000502
unknown	53901/udp	0.000502
unknown	53904/udp	0.000502
unknown	53910/tcp	0.000076
unknown	53912/udp	0.000502
unknown	53919/udp	0.000502
unknown	53921/udp	0.000502
unknown	53924/udp	0.000502
unknown	53925/udp	0.000502
unknown	53926/udp	0.000502
unknown	53934/udp	0.000502
unknown	53935/udp	0.000502
unknown	53940/udp	0.001004
unknown	53941/udp	0.000502
unknown	53951/udp	0.000502
unknown	53954/udp	0.000502
unknown	53958/tcp	0.000076
unknown	53960/udp	0.000502
unknown	53987/udp	0.001004
unknown	53988/udp	0.000502
unknown	53993/udp	0.000502
unknown	53996/udp	0.001004
unknown	53997/udp	0.000502
unknown	54001/udp	0.000502
unknown	54002/udp	0.000502
unknown	54007/udp	0.000502
unknown	54011/udp	0.000502
unknown	54016/udp	0.000502
unknown	54018/udp	0.000502
unknown	54020/udp	0.000502
unknown	54021/udp	0.000502
unknown	54023/udp	0.001004
unknown	54024/udp	0.000502
unknown	54027/udp	0.001004
unknown	54032/udp	0.000502
unknown	54033/udp	0.000502
unknown	54034/udp	0.000502
unknown	54040/udp	0.001004
unknown	54045/tcp	0.000228
unknown	54045/udp	0.001004
unknown	54048/udp	0.000502
unknown	54049/udp	0.000502
unknown	54054/udp	0.000502
unknown	54055/udp	0.001004
unknown	54068/udp	0.000502
unknown	54075/tcp	0.000076
unknown	54077/udp	0.000502
unknown	54081/udp	0.000502
unknown	54089/udp	0.000502
unknown	54090/udp	0.000502
unknown	54092/udp	0.000502
unknown	54094/udp	0.001506
unknown	54096/udp	0.000502
unknown	54100/udp	0.000502
unknown	54101/tcp	0.000076
unknown	54103/udp	0.000502
unknown	54111/udp	0.000502
unknown	54114/udp	0.001506
unknown	54115/udp	0.000502
unknown	54125/udp	0.000502
unknown	54126/udp	0.001004
unknown	54127/tcp	0.000076
unknown	54131/udp	0.000502
unknown	54152/udp	0.000502
unknown	54159/udp	0.000502
unknown	54165/udp	0.000502
unknown	54171/udp	0.000502
unknown	54178/udp	0.000502
unknown	54183/udp	0.000502
unknown	54190/udp	0.000502
unknown	54193/udp	0.000502
unknown	54198/udp	0.000502
unknown	54203/udp	0.000502
unknown	54212/udp	0.000502
unknown	54219/udp	0.000502
unknown	54233/udp	0.000502
unknown	54235/tcp	0.000076
unknown	54235/udp	0.000502
unknown	54253/udp	0.000502
unknown	54258/udp	0.000502
unknown	54259/udp	0.001004
unknown	54261/udp	0.000502
unknown	54263/tcp	0.000076
unknown	54264/udp	0.001004
unknown	54266/udp	0.000502
unknown	54267/udp	0.001004
unknown	54268/udp	0.000502
unknown	54276/tcp	0.000076
unknown	54277/udp	0.000502
unknown	54279/udp	0.000502
unknown	54280/udp	0.000502
unknown	54281/udp	0.002008
unknown	54282/udp	0.000502
unknown	54284/udp	0.000502
unknown	54289/udp	0.000502
unknown	54296/udp	0.001004
unknown	54298/udp	0.001004
unknown	54301/udp	0.000502
unknown	54302/udp	0.000502
unknown	54311/udp	0.000502
bo2k	54320/tcp	0.000075	# Back Orifice 2K Default Port
unknown	54321/tcp	0.000076
bo2k	54321/udp	0.002246	# Back Orifice 2K Default Port
unknown	54323/tcp	0.000076
unknown	54324/udp	0.001004
unknown	54326/udp	0.000502
unknown	54328/tcp	0.000228
unknown	54331/udp	0.000502
unknown	54335/udp	0.000502
unknown	54341/udp	0.000502
unknown	54348/udp	0.000502
unknown	54349/udp	0.001004
unknown	54356/udp	0.000502
unknown	54370/udp	0.000502
unknown	54375/udp	0.001004
unknown	54377/udp	0.000502
unknown	54382/udp	0.000502
unknown	54383/udp	0.000502
unknown	54389/udp	0.000502
unknown	54398/udp	0.001004
unknown	54412/udp	0.000502
unknown	54414/udp	0.000502
unknown	54417/udp	0.000502
unknown	54418/udp	0.000502
unknown	54425/udp	0.000502
unknown	54434/udp	0.000502
unknown	54435/udp	0.000502
unknown	54436/udp	0.000502
unknown	54446/udp	0.000502
unknown	54448/udp	0.000502
unknown	54451/udp	0.000502
unknown	54475/udp	0.000502
unknown	54480/udp	0.000502
unknown	54482/udp	0.000502
unknown	54490/udp	0.000502
unknown	54495/udp	0.000502
unknown	54496/udp	0.000502
unknown	54499/udp	0.000502
unknown	54513/udp	0.001004
unknown	54514/tcp	0.000076
unknown	54517/udp	0.000502
unknown	54521/udp	0.001004
unknown	54526/udp	0.000502
unknown	54531/udp	0.001004
unknown	54535/udp	0.000502
unknown	54536/udp	0.000502
unknown	54537/udp	0.000502
unknown	54540/udp	0.000502
unknown	54541/udp	0.000502
unknown	54545/udp	0.000502
unknown	54547/udp	0.000502
unknown	54551/tcp	0.000076
unknown	54553/udp	0.000502
unknown	54561/udp	0.000502
unknown	54573/udp	0.000502
unknown	54578/udp	0.000502
unknown	54579/udp	0.000502
unknown	54587/udp	0.000502
unknown	54588/udp	0.000502
unknown	54593/udp	0.000502
unknown	54603/udp	0.000502
unknown	54604/udp	0.000502
unknown	54605/tcp	0.000076
unknown	54606/udp	0.000502
unknown	54607/udp	0.001004
unknown	54608/udp	0.000502
unknown	54612/udp	0.000502
unknown	54615/udp	0.000502
unknown	54627/udp	0.001004
unknown	54628/udp	0.000502
unknown	54629/udp	0.000502
unknown	54631/udp	0.000502
unknown	54632/udp	0.000502
unknown	54633/udp	0.000502
unknown	54638/udp	0.000502
unknown	54639/udp	0.000502
unknown	54642/udp	0.000502
unknown	54644/udp	0.000502
unknown	54653/udp	0.001004
unknown	54658/tcp	0.000076
unknown	54665/udp	0.000502
unknown	54668/udp	0.000502
unknown	54669/udp	0.000502
unknown	54670/udp	0.000502
unknown	54674/udp	0.000502
unknown	54675/udp	0.000502
unknown	54676/udp	0.001004
unknown	54688/tcp	0.000076
unknown	54696/udp	0.000502
unknown	54711/udp	0.001506
unknown	54722/tcp	0.000076
unknown	54722/udp	0.001004
unknown	54741/tcp	0.000076
unknown	54747/udp	0.001004
unknown	54748/udp	0.000502
unknown	54751/udp	0.000502
unknown	54755/udp	0.000502
unknown	54757/udp	0.000502
unknown	54758/udp	0.001004
unknown	54763/udp	0.000502
unknown	54783/udp	0.000502
unknown	54788/udp	0.000502
unknown	54790/udp	0.000502
unknown	54792/udp	0.000502
unknown	54793/udp	0.000502
unknown	54801/udp	0.000502
unknown	54805/udp	0.000502
unknown	54806/udp	0.000502
unknown	54807/udp	0.001506
unknown	54811/udp	0.000502
unknown	54812/udp	0.001004
unknown	54820/udp	0.000502
unknown	54833/udp	0.000502
unknown	54835/udp	0.000502
unknown	54838/udp	0.000502
unknown	54843/udp	0.000502
unknown	54847/udp	0.000502
unknown	54848/udp	0.001004
unknown	54849/udp	0.000502
unknown	54853/udp	0.000502
unknown	54854/udp	0.000502
unknown	54862/udp	0.000502
unknown	54863/udp	0.000502
unknown	54873/tcp	0.000076
unknown	54875/udp	0.000502
unknown	54878/udp	0.000502
unknown	54884/udp	0.000502
unknown	54887/udp	0.000502
unknown	54890/udp	0.000502
unknown	54902/udp	0.000502
unknown	54906/udp	0.000502
unknown	54907/tcp	0.000076
unknown	54907/udp	0.000502
unknown	54911/udp	0.000502
unknown	54920/udp	0.000502
unknown	54922/udp	0.000502
unknown	54923/udp	0.000502
unknown	54924/udp	0.000502
unknown	54925/udp	0.001506
unknown	54927/udp	0.000502
unknown	54933/udp	0.000502
unknown	54937/udp	0.000502
unknown	54938/udp	0.000502
unknown	54939/udp	0.001004
unknown	54942/udp	0.000502
unknown	54946/udp	0.001004
unknown	54948/udp	0.000502
unknown	54952/udp	0.001004
unknown	54957/udp	0.000502
unknown	54959/udp	0.000502
unknown	54965/udp	0.000502
unknown	54970/udp	0.000502
unknown	54971/udp	0.000502
unknown	54978/udp	0.000502
unknown	54981/udp	0.000502
unknown	54982/udp	0.000502
unknown	54987/tcp	0.000076
unknown	54991/tcp	0.000076
unknown	54993/udp	0.001004
unknown	54995/udp	0.000502
unknown	54999/udp	0.000502
unknown	55000/tcp	0.000076
unknown	55020/tcp	0.000152
unknown	55020/udp	0.000502
unknown	55034/udp	0.001004
unknown	55038/udp	0.000502
unknown	55043/udp	0.001506
unknown	55051/udp	0.000502
unknown	55055/tcp	0.000304
unknown	55056/tcp	0.000228
unknown	55095/udp	0.000502
unknown	55100/udp	0.000502
unknown	55101/udp	0.000502
unknown	55102/udp	0.000502
unknown	55105/udp	0.000502
unknown	55108/udp	0.000502
unknown	55109/udp	0.000502
unknown	55120/udp	0.000502
unknown	55121/udp	0.000502
unknown	55124/udp	0.001004
unknown	55125/udp	0.000502
unknown	55129/udp	0.000502
unknown	55133/udp	0.000502
unknown	55142/udp	0.000502
unknown	55145/udp	0.000502
unknown	55147/udp	0.000502
unknown	55155/udp	0.000502
unknown	55156/udp	0.001004
unknown	55157/udp	0.000502
unknown	55165/udp	0.000502
unknown	55168/udp	0.000502
unknown	55174/udp	0.000502
unknown	55176/udp	0.000502
unknown	55179/udp	0.000502
unknown	55183/tcp	0.000076
unknown	55185/udp	0.000502
unknown	55187/tcp	0.000076
unknown	55194/udp	0.000502
unknown	55198/udp	0.000502
unknown	55200/udp	0.000502
unknown	55201/udp	0.000502
unknown	55203/udp	0.000502
unknown	55204/udp	0.000502
unknown	55205/udp	0.001004
unknown	55206/udp	0.000502
unknown	55212/udp	0.000502
unknown	55214/udp	0.000502
unknown	55215/udp	0.000502
unknown	55227/tcp	0.000076
unknown	55228/udp	0.000502
unknown	55229/udp	0.000502
unknown	55230/udp	0.000502
unknown	55233/udp	0.000502
unknown	55234/udp	0.000502
unknown	55243/udp	0.000502
unknown	55247/udp	0.000502
unknown	55249/udp	0.000502
unknown	55250/udp	0.000502
unknown	55251/udp	0.000502
unknown	55264/udp	0.000502
unknown	55266/udp	0.000502
unknown	55267/udp	0.001004
unknown	55271/udp	0.000502
unknown	55272/udp	0.000502
unknown	55292/udp	0.000502
unknown	55296/udp	0.000502
unknown	55303/udp	0.000502
unknown	55311/udp	0.000502
unknown	55312/tcp	0.000076
unknown	55316/udp	0.001004
unknown	55321/udp	0.000502
unknown	55323/udp	0.000502
unknown	55330/udp	0.000502
unknown	55334/udp	0.000502
unknown	55341/udp	0.000502
unknown	55344/udp	0.000502
unknown	55345/udp	0.000502
unknown	55350/tcp	0.000076
unknown	55352/udp	0.001004
unknown	55353/udp	0.000502
unknown	55365/udp	0.000502
unknown	55367/udp	0.000502
unknown	55373/udp	0.000502
unknown	55382/tcp	0.000076
unknown	55384/udp	0.000502
unknown	55395/udp	0.000502
unknown	55400/tcp	0.000076
unknown	55403/udp	0.000502
unknown	55411/udp	0.000502
unknown	55412/udp	0.000502
unknown	55414/udp	0.000502
unknown	55415/udp	0.000502
unknown	55416/udp	0.000502
unknown	55423/udp	0.000502
unknown	55425/udp	0.000502
unknown	55426/tcp	0.000076
unknown	55436/udp	0.000502
unknown	55437/udp	0.000502
unknown	55438/udp	0.000502
unknown	55443/udp	0.000502
unknown	55451/udp	0.000502
unknown	55456/udp	0.000502
unknown	55457/udp	0.000502
unknown	55469/udp	0.000502
unknown	55471/udp	0.000502
unknown	55472/udp	0.000502
unknown	55479/tcp	0.000076
unknown	55485/udp	0.000502
unknown	55488/udp	0.001004
unknown	55504/udp	0.000502
unknown	55527/tcp	0.000076
unknown	55527/udp	0.000502
unknown	55529/udp	0.000502
unknown	55534/udp	0.000502
unknown	55537/udp	0.000502
unknown	55539/udp	0.000502
unknown	55540/udp	0.000502
unknown	55541/udp	0.001004
unknown	55543/udp	0.000502
unknown	55544/udp	0.001506
unknown	55553/udp	0.001004
unknown	55555/tcp	0.000760
unknown	55556/tcp	0.000076
unknown	55566/udp	0.000502
unknown	55568/tcp	0.000076
unknown	55569/tcp	0.000076
unknown	55575/udp	0.000502
unknown	55576/tcp	0.000152
unknown	55576/udp	0.000502
unknown	55577/udp	0.000502
unknown	55578/udp	0.000502
unknown	55579/tcp	0.000076
unknown	55579/udp	0.001004
unknown	55581/udp	0.001004
unknown	55582/udp	0.000502
unknown	55587/udp	0.001506
unknown	55593/udp	0.001004
unknown	55595/udp	0.000502
unknown	55596/udp	0.000502
unknown	55597/udp	0.000502
unknown	55600/tcp	0.000760
unknown	55600/udp	0.000502
unknown	55603/udp	0.000502
unknown	55605/udp	0.000502
unknown	55609/udp	0.000502
unknown	55614/udp	0.000502
unknown	55617/udp	0.000502
unknown	55618/udp	0.001004
unknown	55619/udp	0.000502
unknown	55622/udp	0.000502
unknown	55623/udp	0.000502
unknown	55624/udp	0.000502
unknown	55628/udp	0.000502
unknown	55630/udp	0.000502
unknown	55632/udp	0.000502
unknown	55633/udp	0.000502
unknown	55635/tcp	0.000076
unknown	55642/udp	0.000502
unknown	55643/udp	0.000502
unknown	55650/udp	0.001004
unknown	55652/tcp	0.000076
unknown	55659/udp	0.000502
unknown	55665/udp	0.000502
unknown	55672/udp	0.000502
unknown	55676/udp	0.000502
unknown	55679/udp	0.000502
unknown	55684/tcp	0.000076
unknown	55695/udp	0.000502
unknown	55697/udp	0.000502
unknown	55698/udp	0.000502
unknown	55701/udp	0.000502
unknown	55703/udp	0.000502
unknown	55712/udp	0.000502
unknown	55718/udp	0.000502
unknown	55719/udp	0.000502
unknown	55721/tcp	0.000076
unknown	55728/udp	0.000502
unknown	55729/udp	0.000502
unknown	55736/udp	0.000502
unknown	55745/udp	0.001004
unknown	55746/udp	0.000502
unknown	55752/udp	0.000502
unknown	55758/tcp	0.000076
unknown	55760/udp	0.000502
unknown	55763/udp	0.000502
unknown	55766/udp	0.001004
unknown	55767/udp	0.000502
unknown	55769/udp	0.000502
unknown	55773/tcp	0.000076
unknown	55781/tcp	0.000076
unknown	55784/udp	0.001004
unknown	55789/udp	0.000502
unknown	55795/udp	0.001004
unknown	55797/udp	0.000502
unknown	55803/udp	0.000502
unknown	55805/udp	0.000502
unknown	55808/udp	0.000502
unknown	55818/udp	0.000502
unknown	55828/udp	0.000502
unknown	55830/udp	0.000502
unknown	55832/udp	0.000502
unknown	55843/udp	0.000502
unknown	55846/udp	0.000502
unknown	55847/udp	0.000502
unknown	55864/udp	0.000502
unknown	55870/udp	0.001004
unknown	55876/udp	0.000502
unknown	55877/udp	0.000502
unknown	55880/udp	0.000502
unknown	55888/udp	0.000502
unknown	55899/udp	0.000502
unknown	55901/tcp	0.000076
unknown	55905/udp	0.000502
unknown	55906/udp	0.000502
unknown	55907/tcp	0.000076
unknown	55909/udp	0.000502
unknown	55910/tcp	0.000076
unknown	55918/udp	0.000502
unknown	55921/udp	0.000502
unknown	55922/udp	0.000502
unknown	55924/udp	0.000502
unknown	55929/udp	0.000502
unknown	55937/udp	0.000502
unknown	55939/udp	0.000502
unknown	55941/udp	0.001004
unknown	55944/udp	0.000502
unknown	55948/tcp	0.000076
unknown	55949/udp	0.000502
unknown	55954/udp	0.001004
unknown	55957/udp	0.000502
unknown	55960/udp	0.000502
unknown	55961/udp	0.000502
unknown	55969/udp	0.000502
unknown	55978/udp	0.000502
unknown	55979/udp	0.000502
unknown	55990/udp	0.000502
unknown	55993/udp	0.000502
unknown	55994/udp	0.000502
unknown	55998/udp	0.000502
unknown	56005/udp	0.000502
unknown	56006/udp	0.000502
unknown	56011/udp	0.000502
unknown	56012/udp	0.000502
unknown	56013/udp	0.000502
unknown	56015/udp	0.000502
unknown	56016/tcp	0.000076
unknown	56018/udp	0.000502
unknown	56028/udp	0.000502
unknown	56029/udp	0.000502
unknown	56037/udp	0.000502
unknown	56054/udp	0.000502
unknown	56055/tcp	0.000076
unknown	56057/udp	0.000502
unknown	56059/udp	0.000502
unknown	56068/udp	0.000502
unknown	56073/udp	0.000502
unknown	56074/udp	0.000502
unknown	56092/udp	0.000502
unknown	56096/udp	0.000502
unknown	56099/udp	0.000502
unknown	56103/udp	0.001004
unknown	56105/udp	0.001004
unknown	56107/udp	0.000502
unknown	56109/udp	0.000502
unknown	56110/udp	0.000502
unknown	56111/udp	0.000502
unknown	56116/udp	0.000502
unknown	56119/udp	0.000502
unknown	56120/udp	0.000502
unknown	56122/udp	0.000502
unknown	56127/udp	0.000502
unknown	56129/udp	0.000502
unknown	56130/udp	0.000502
unknown	56137/udp	0.000502
unknown	56141/udp	0.002008
unknown	56147/udp	0.000502
unknown	56152/udp	0.000502
unknown	56153/udp	0.001004
unknown	56163/udp	0.000502
unknown	56168/udp	0.001004
unknown	56171/udp	0.000502
unknown	56192/udp	0.000502
unknown	56202/udp	0.000502
unknown	56203/udp	0.000502
unknown	56209/udp	0.001004
unknown	56213/udp	0.000502
unknown	56214/udp	0.000502
unknown	56221/udp	0.000502
unknown	56225/udp	0.001004
unknown	56228/udp	0.000502
unknown	56235/udp	0.000502
unknown	56241/udp	0.000502
unknown	56246/udp	0.000502
unknown	56259/tcp	0.000076
unknown	56259/udp	0.000502
unknown	56262/udp	0.000502
unknown	56267/udp	0.000502
unknown	56273/udp	0.001004
unknown	56274/udp	0.000502
unknown	56278/udp	0.000502
unknown	56284/udp	0.001004
unknown	56288/udp	0.001004
unknown	56289/udp	0.000502
unknown	56293/tcp	0.000076
unknown	56293/udp	0.000502
unknown	56308/udp	0.000502
unknown	56321/udp	0.000502
unknown	56324/udp	0.000502
unknown	56326/udp	0.001004
unknown	56332/udp	0.000502
unknown	56333/udp	0.000502
unknown	56337/udp	0.001004
unknown	56358/udp	0.000502
unknown	56359/udp	0.001004
unknown	56360/udp	0.000502
unknown	56366/udp	0.001004
unknown	56369/udp	0.000502
unknown	56371/udp	0.000502
unknown	56377/udp	0.000502
unknown	56380/udp	0.000502
unknown	56384/udp	0.000502
unknown	56393/udp	0.000502
unknown	56396/udp	0.000502
unknown	56404/udp	0.000502
unknown	56411/udp	0.000502
unknown	56418/udp	0.000502
unknown	56427/udp	0.000502
unknown	56433/udp	0.000502
unknown	56435/udp	0.000502
unknown	56438/udp	0.000502
unknown	56442/udp	0.000502
unknown	56457/udp	0.000502
unknown	56460/udp	0.000502
unknown	56462/udp	0.000502
unknown	56463/udp	0.000502
unknown	56466/udp	0.000502
unknown	56468/udp	0.001004
unknown	56469/udp	0.000502
unknown	56478/udp	0.000502
unknown	56485/udp	0.000502
unknown	56487/udp	0.000502
unknown	56491/udp	0.001004
unknown	56494/udp	0.000502
unknown	56497/udp	0.000502
unknown	56507/tcp	0.000076
unknown	56515/udp	0.000502
unknown	56525/udp	0.000502
unknown	56531/udp	0.000502
unknown	56533/udp	0.000502
unknown	56535/tcp	0.000076
unknown	56542/udp	0.000502
unknown	56548/udp	0.000502
unknown	56554/udp	0.001004
unknown	56555/udp	0.001004
unknown	56560/udp	0.000502
unknown	56591/tcp	0.000076
unknown	56592/udp	0.000502
unknown	56594/udp	0.000502
unknown	56597/udp	0.000502
unknown	56603/udp	0.000502
unknown	56615/udp	0.000502
unknown	56620/udp	0.000502
unknown	56621/udp	0.000502
unknown	56622/udp	0.001004
unknown	56627/udp	0.000502
unknown	56632/udp	0.000502
unknown	56637/udp	0.001004
unknown	56639/udp	0.000502
unknown	56643/udp	0.000502
unknown	56645/udp	0.000502
unknown	56653/udp	0.000502
unknown	56654/udp	0.000502
unknown	56657/udp	0.000502
unknown	56659/udp	0.000502
unknown	56666/udp	0.000502
unknown	56668/tcp	0.000076
unknown	56668/udp	0.001004
unknown	56679/udp	0.000502
unknown	56681/tcp	0.000076
unknown	56690/udp	0.000502
unknown	56691/udp	0.000502
unknown	56696/udp	0.000502
unknown	56704/udp	0.000502
unknown	56708/udp	0.000502
unknown	56710/udp	0.000502
unknown	56723/tcp	0.000076
unknown	56725/tcp	0.000076
unknown	56728/udp	0.000502
unknown	56732/udp	0.000502
unknown	56733/udp	0.000502
unknown	56736/udp	0.000502
unknown	56737/tcp	0.000228
unknown	56738/tcp	0.000304
unknown	56744/udp	0.000502
unknown	56750/udp	0.000502
unknown	56751/udp	0.000502
unknown	56753/udp	0.000502
unknown	56761/udp	0.000502
unknown	56765/udp	0.001004
unknown	56766/udp	0.000502
unknown	56782/udp	0.000502
unknown	56789/udp	0.000502
unknown	56798/udp	0.000502
unknown	56799/udp	0.000502
unknown	56800/udp	0.000502
unknown	56801/udp	0.000502
unknown	56802/udp	0.000502
unknown	56803/udp	0.000502
unknown	56804/udp	0.000502
unknown	56806/udp	0.000502
unknown	56810/tcp	0.000076
unknown	56816/udp	0.000502
unknown	56822/tcp	0.000076
unknown	56823/udp	0.000502
unknown	56825/udp	0.001004
unknown	56826/udp	0.000502
unknown	56827/tcp	0.000076
unknown	56838/udp	0.000502
unknown	56848/udp	0.001004
unknown	56851/udp	0.000502
unknown	56856/udp	0.000502
unknown	56863/udp	0.000502
unknown	56867/udp	0.000502
unknown	56869/udp	0.001004
unknown	56870/udp	0.000502
unknown	56876/udp	0.001004
unknown	56878/udp	0.000502
unknown	56880/udp	0.000502
unknown	56888/udp	0.000502
unknown	56891/udp	0.000502
unknown	56892/udp	0.001004
unknown	56895/udp	0.001004
unknown	56897/udp	0.001004
unknown	56904/udp	0.000502
unknown	56909/udp	0.000502
unknown	56913/udp	0.000502
unknown	56916/udp	0.000502
unknown	56921/udp	0.000502
unknown	56929/udp	0.001004
unknown	56933/udp	0.000502
unknown	56939/udp	0.000502
unknown	56943/udp	0.000502
unknown	56949/udp	0.000502
unknown	56950/udp	0.000502
unknown	56954/udp	0.001004
unknown	56960/udp	0.000502
unknown	56970/udp	0.000502
unknown	56973/tcp	0.000076
unknown	56975/tcp	0.000076
unknown	56980/udp	0.001004
unknown	56984/udp	0.000502
unknown	57000/udp	0.000502
unknown	57005/udp	0.001004
unknown	57010/udp	0.000502
unknown	57018/udp	0.000502
unknown	57020/tcp	0.000076
unknown	57020/udp	0.000502
unknown	57028/udp	0.000502
unknown	57050/udp	0.000502
unknown	57053/udp	0.000502
unknown	57060/udp	0.000502
unknown	57063/udp	0.001004
unknown	57068/udp	0.000502
unknown	57082/udp	0.000502
unknown	57086/udp	0.000502
unknown	57096/udp	0.000502
unknown	57099/udp	0.000502
unknown	57103/tcp	0.000076
unknown	57104/udp	0.000502
unknown	57110/udp	0.000502
unknown	57114/udp	0.001004
unknown	57121/udp	0.000502
unknown	57122/udp	0.000502
unknown	57123/tcp	0.000076
unknown	57128/udp	0.000502
unknown	57133/udp	0.001004
unknown	57134/udp	0.000502
unknown	57135/udp	0.000502
unknown	57154/udp	0.000502
unknown	57156/udp	0.001004
unknown	57167/udp	0.000502
unknown	57172/udp	0.001506
unknown	57176/udp	0.000502
unknown	57180/udp	0.000502
unknown	57182/udp	0.000502
unknown	57194/udp	0.000502
unknown	57202/udp	0.000502
unknown	57204/udp	0.000502
unknown	57208/udp	0.000502
unknown	57213/udp	0.000502
unknown	57217/udp	0.000502
unknown	57221/udp	0.000502
unknown	57234/udp	0.000502
unknown	57237/udp	0.000502
unknown	57244/udp	0.000502
unknown	57245/udp	0.000502
unknown	57247/udp	0.000502
unknown	57250/udp	0.000502
unknown	57252/udp	0.000502
unknown	57254/udp	0.000502
unknown	57255/udp	0.000502
unknown	57279/udp	0.000502
unknown	57283/udp	0.000502
unknown	57286/udp	0.000502
unknown	57294/tcp	0.000380
unknown	57304/udp	0.000502
unknown	57320/udp	0.000502
unknown	57322/udp	0.000502
unknown	57325/tcp	0.000076
unknown	57328/udp	0.000502
unknown	57335/tcp	0.000076
unknown	57336/udp	0.000502
unknown	57337/udp	0.000502
unknown	57344/udp	0.000502
unknown	57347/tcp	0.000076
unknown	57348/udp	0.000502
unknown	57350/tcp	0.000076
unknown	57352/tcp	0.000076
unknown	57357/udp	0.000502
unknown	57358/udp	0.000502
unknown	57361/udp	0.000502
unknown	57369/udp	0.000502
unknown	57373/udp	0.000502
unknown	57375/udp	0.000502
unknown	57379/udp	0.000502
unknown	57381/udp	0.000502
unknown	57382/udp	0.000502
unknown	57383/udp	0.000502
unknown	57386/udp	0.001004
unknown	57387/tcp	0.000076
unknown	57388/udp	0.000502
unknown	57391/udp	0.000502
unknown	57392/udp	0.000502
unknown	57395/udp	0.000502
unknown	57398/tcp	0.000076
unknown	57399/udp	0.000502
unknown	57402/udp	0.000502
unknown	57407/udp	0.000502
unknown	57409/udp	0.001506
unknown	57410/udp	0.001506
unknown	57416/udp	0.000502
unknown	57421/udp	0.001004
unknown	57425/udp	0.000502
unknown	57426/udp	0.000502
unknown	57456/udp	0.000502
unknown	57461/udp	0.001004
unknown	57471/udp	0.000502
unknown	57473/udp	0.000502
unknown	57474/udp	0.000502
unknown	57479/tcp	0.000076
unknown	57479/udp	0.000502
unknown	57483/udp	0.000502
unknown	57486/udp	0.000502
unknown	57491/udp	0.000502
unknown	57503/udp	0.000502
unknown	57504/udp	0.000502
unknown	57505/udp	0.000502
unknown	57510/udp	0.000502
unknown	57515/udp	0.000502
unknown	57516/udp	0.000502
unknown	57522/udp	0.000502
unknown	57527/udp	0.000502
unknown	57530/udp	0.000502
unknown	57552/udp	0.000502
unknown	57559/udp	0.000502
unknown	57576/tcp	0.000076
unknown	57577/udp	0.000502
unknown	57580/udp	0.000502
unknown	57587/udp	0.000502
unknown	57594/udp	0.000502
unknown	57614/udp	0.000502
unknown	57616/udp	0.000502
unknown	57619/udp	0.000502
unknown	57620/udp	0.000502
unknown	57622/udp	0.000502
unknown	57624/udp	0.000502
unknown	57629/udp	0.001004
unknown	57632/udp	0.000502
unknown	57633/udp	0.000502
unknown	57637/udp	0.000502
unknown	57638/udp	0.000502
unknown	57644/udp	0.000502
unknown	57646/udp	0.000502
unknown	57651/udp	0.000502
unknown	57655/udp	0.000502
unknown	57662/udp	0.001004
unknown	57665/tcp	0.000152
unknown	57671/udp	0.000502
unknown	57675/udp	0.000502
unknown	57676/udp	0.000502
unknown	57677/udp	0.000502
unknown	57678/tcp	0.000076
unknown	57679/udp	0.001004
unknown	57681/tcp	0.000076
unknown	57692/udp	0.000502
unknown	57696/udp	0.000502
unknown	57700/udp	0.000502
unknown	57702/tcp	0.000076
unknown	57711/udp	0.000502
unknown	57714/udp	0.000502
unknown	57719/udp	0.000502
unknown	57720/udp	0.000502
unknown	57728/udp	0.000502
unknown	57729/udp	0.000502
unknown	57730/tcp	0.000076
unknown	57733/tcp	0.000076
unknown	57733/udp	0.000502
unknown	57734/udp	0.000502
unknown	57739/udp	0.000502
unknown	57747/udp	0.000502
unknown	57756/udp	0.001004
unknown	57757/udp	0.000502
unknown	57758/udp	0.000502
unknown	57761/udp	0.000502
unknown	57767/udp	0.000502
unknown	57774/udp	0.000502
unknown	57784/udp	0.000502
unknown	57787/udp	0.000502
unknown	57797/tcp	0.000228
unknown	57800/udp	0.000502
unknown	57802/udp	0.000502
unknown	57812/udp	0.000502
unknown	57813/udp	0.001506
unknown	57814/udp	0.000502
unknown	57816/udp	0.000502
unknown	57821/udp	0.000502
unknown	57827/udp	0.001004
unknown	57836/udp	0.001004
unknown	57839/udp	0.000502
unknown	57843/udp	0.001506
unknown	57848/udp	0.001004
unknown	57850/udp	0.000502
unknown	57852/udp	0.000502
unknown	57858/udp	0.001004
unknown	57862/udp	0.000502
unknown	57864/udp	0.000502
unknown	57868/udp	0.001004
unknown	57871/udp	0.000502
unknown	57884/udp	0.000502
unknown	57891/tcp	0.000076
unknown	57893/udp	0.000502
unknown	57896/tcp	0.000076
unknown	57896/udp	0.000502
unknown	57899/udp	0.000502
unknown	57904/udp	0.000502
unknown	57916/udp	0.000502
unknown	57917/udp	0.000502
unknown	57920/udp	0.000502
unknown	57921/udp	0.000502
unknown	57923/tcp	0.000076
unknown	57928/tcp	0.000076
unknown	57933/udp	0.000502
unknown	57942/udp	0.001004
unknown	57946/udp	0.001004
unknown	57956/udp	0.000502
unknown	57958/udp	0.001506
unknown	57960/udp	0.000502
unknown	57963/udp	0.000502
unknown	57965/udp	0.000502
unknown	57972/udp	0.000502
unknown	57975/udp	0.000502
unknown	57976/udp	0.000502
unknown	57977/udp	0.001506
unknown	57988/tcp	0.000076
unknown	57990/udp	0.000502
unknown	57999/tcp	0.000076
unknown	57999/udp	0.000502
unknown	58000/udp	0.000502
unknown	58001/tcp	0.000152
unknown	58002/tcp	0.000152
unknown	58002/udp	0.003514
unknown	58003/udp	0.000502
unknown	58004/udp	0.000502
unknown	58007/udp	0.000502
unknown	58008/udp	0.000502
unknown	58009/udp	0.000502
unknown	58010/udp	0.000502
unknown	58011/udp	0.000502
unknown	58012/udp	0.000502
unknown	58014/udp	0.000502
unknown	58016/udp	0.000502
unknown	58020/udp	0.000502
unknown	58023/udp	0.000502
unknown	58026/udp	0.001004
unknown	58027/udp	0.000502
unknown	58033/udp	0.000502
unknown	58042/udp	0.000502
unknown	58049/udp	0.000502
unknown	58050/udp	0.000502
unknown	58070/udp	0.000502
unknown	58072/tcp	0.000076
unknown	58075/udp	0.001506
unknown	58076/udp	0.000502
unknown	58077/udp	0.000502
unknown	58080/tcp	0.000380
unknown	58085/udp	0.000502
unknown	58088/udp	0.000502
unknown	58089/udp	0.001004
unknown	58091/udp	0.001004
unknown	58101/udp	0.000502
unknown	58102/udp	0.001004
unknown	58105/udp	0.000502
unknown	58107/tcp	0.000076
unknown	58109/tcp	0.000076
unknown	58111/udp	0.000502
unknown	58114/udp	0.001004
unknown	58117/udp	0.000502
unknown	58123/udp	0.000502
unknown	58127/udp	0.000502
unknown	58141/udp	0.001004
unknown	58154/udp	0.000502
unknown	58162/udp	0.000502
unknown	58164/tcp	0.000076
unknown	58167/udp	0.000502
unknown	58176/udp	0.000502
unknown	58178/udp	0.001506
unknown	58179/udp	0.000502
unknown	58182/udp	0.000502
unknown	58183/udp	0.000502
unknown	58184/udp	0.000502
unknown	58185/udp	0.000502
unknown	58187/udp	0.000502
unknown	58189/udp	0.000502
unknown	58201/udp	0.000502
unknown	58205/udp	0.001004
unknown	58219/udp	0.000502
unknown	58224/udp	0.000502
unknown	58228/udp	0.000502
unknown	58229/udp	0.000502
unknown	58235/udp	0.000502
unknown	58236/udp	0.000502
unknown	58241/udp	0.000502
unknown	58244/udp	0.000502
unknown	58248/udp	0.000502
unknown	58252/tcp	0.000076
unknown	58252/udp	0.000502
unknown	58254/udp	0.000502
unknown	58261/udp	0.000502
unknown	58262/udp	0.000502
unknown	58266/udp	0.000502
unknown	58279/udp	0.000502
unknown	58293/udp	0.000502
unknown	58302/udp	0.000502
unknown	58305/tcp	0.000076
unknown	58306/udp	0.000502
unknown	58308/udp	0.001004
unknown	58310/tcp	0.000076
unknown	58314/udp	0.000502
unknown	58315/udp	0.000502
unknown	58318/udp	0.000502
unknown	58327/udp	0.000502
unknown	58328/udp	0.000502
unknown	58334/udp	0.000502
unknown	58347/udp	0.000502
unknown	58348/udp	0.000502
unknown	58349/udp	0.000502
unknown	58350/udp	0.000502
unknown	58352/udp	0.000502
unknown	58353/udp	0.000502
unknown	58358/udp	0.000502
unknown	58363/udp	0.000502
unknown	58364/udp	0.000502
unknown	58369/udp	0.001004
unknown	58371/udp	0.000502
unknown	58374/tcp	0.000076
unknown	58390/udp	0.000502
unknown	58391/udp	0.000502
unknown	58395/udp	0.000502
unknown	58401/udp	0.000502
unknown	58402/udp	0.000502
unknown	58408/udp	0.000502
unknown	58416/udp	0.000502
unknown	58419/udp	0.001506
unknown	58427/udp	0.000502
unknown	58430/tcp	0.000076
unknown	58432/udp	0.001004
unknown	58441/udp	0.000502
unknown	58442/udp	0.000502
unknown	58446/tcp	0.000076
unknown	58446/udp	0.000502
unknown	58455/udp	0.001004
unknown	58456/tcp	0.000076
unknown	58463/udp	0.000502
unknown	58465/udp	0.000502
unknown	58468/tcp	0.000076
unknown	58478/udp	0.000502
unknown	58479/udp	0.000502
unknown	58486/udp	0.000502
unknown	58498/tcp	0.000076
unknown	58504/udp	0.000502
unknown	58525/udp	0.000502
unknown	58526/udp	0.000502
unknown	58528/udp	0.000502
unknown	58537/udp	0.000502
unknown	58546/udp	0.000502
unknown	58549/udp	0.000502
unknown	58558/udp	0.000502
unknown	58561/udp	0.000502
unknown	58562/tcp	0.000076
unknown	58570/tcp	0.000076
unknown	58571/udp	0.000502
unknown	58572/udp	0.000502
unknown	58576/udp	0.000502
unknown	58577/udp	0.000502
unknown	58580/udp	0.000502
unknown	58584/udp	0.000502
unknown	58589/udp	0.000502
unknown	58590/udp	0.000502
unknown	58596/udp	0.000502
unknown	58606/udp	0.000502
unknown	58609/udp	0.000502
unknown	58610/tcp	0.000076
unknown	58614/udp	0.000502
unknown	58618/udp	0.000502
unknown	58620/udp	0.000502
unknown	58622/tcp	0.000076
unknown	58627/udp	0.000502
unknown	58629/udp	0.000502
unknown	58630/tcp	0.000152
unknown	58630/udp	0.000502
unknown	58631/udp	0.002008
unknown	58632/tcp	0.000152
unknown	58632/udp	0.000502
unknown	58634/tcp	0.000076
unknown	58640/udp	0.002008
unknown	58646/udp	0.001004
unknown	58648/udp	0.000502
unknown	58649/udp	0.000502
unknown	58654/udp	0.000502
unknown	58655/udp	0.000502
unknown	58657/udp	0.000502
unknown	58658/udp	0.000502
unknown	58667/udp	0.000502
unknown	58670/udp	0.000502
unknown	58672/udp	0.000502
unknown	58674/udp	0.001004
unknown	58686/udp	0.000502
unknown	58690/udp	0.000502
unknown	58691/udp	0.000502
unknown	58697/udp	0.000502
unknown	58698/udp	0.000502
unknown	58699/tcp	0.000076
unknown	58700/udp	0.001004
unknown	58703/udp	0.000502
unknown	58705/udp	0.001004
unknown	58710/udp	0.000502
unknown	58713/udp	0.000502
unknown	58715/udp	0.000502
unknown	58721/tcp	0.000076
unknown	58722/udp	0.000502
unknown	58728/udp	0.000502
unknown	58731/udp	0.000502
unknown	58733/udp	0.000502
unknown	58742/udp	0.000502
unknown	58744/udp	0.000502
unknown	58747/udp	0.001004
unknown	58761/udp	0.000502
unknown	58768/udp	0.000502
unknown	58772/udp	0.000502
unknown	58776/udp	0.000502
unknown	58777/udp	0.001004
unknown	58782/udp	0.001004
unknown	58786/udp	0.000502
unknown	58793/udp	0.000502
unknown	58795/udp	0.000502
unknown	58797/udp	0.001506
unknown	58803/udp	0.000502
unknown	58814/udp	0.000502
unknown	58817/udp	0.001004
unknown	58828/udp	0.000502
unknown	58831/udp	0.000502
unknown	58838/tcp	0.000152
unknown	58838/udp	0.000502
unknown	58839/udp	0.000502
unknown	58845/udp	0.000502
unknown	58847/udp	0.000502
unknown	58848/udp	0.000502
unknown	58866/udp	0.000502
unknown	58871/udp	0.000502
unknown	58876/udp	0.000502
unknown	58880/udp	0.000502
unknown	58891/udp	0.000502
unknown	58892/udp	0.000502
unknown	58893/udp	0.001004
unknown	58899/udp	0.000502
unknown	58903/udp	0.000502
unknown	58908/tcp	0.000076
unknown	58911/udp	0.000502
unknown	58914/udp	0.001004
unknown	58925/udp	0.000502
unknown	58926/udp	0.000502
unknown	58929/udp	0.001004
unknown	58931/udp	0.000502
unknown	58933/udp	0.000502
unknown	58937/udp	0.000502
unknown	58938/udp	0.001004
unknown	58943/udp	0.000502
unknown	58944/udp	0.000502
unknown	58952/udp	0.000502
unknown	58954/udp	0.000502
unknown	58960/udp	0.000502
unknown	58964/udp	0.000502
unknown	58966/udp	0.000502
unknown	58970/tcp	0.000076
unknown	58970/udp	0.000502
unknown	58972/udp	0.000502
unknown	58975/udp	0.001004
unknown	58988/udp	0.000502
unknown	58991/tcp	0.000076
unknown	59002/udp	0.001004
unknown	59014/udp	0.000502
unknown	59016/udp	0.000502
unknown	59023/udp	0.000502
unknown	59035/udp	0.001004
unknown	59037/udp	0.001004
unknown	59039/udp	0.000502
unknown	59045/udp	0.000502
unknown	59047/udp	0.000502
unknown	59055/udp	0.000502
unknown	59079/udp	0.000502
unknown	59083/udp	0.000502
unknown	59087/tcp	0.000076
unknown	59090/udp	0.000502
unknown	59093/udp	0.001004
unknown	59097/udp	0.000502
unknown	59101/udp	0.000502
unknown	59107/tcp	0.000076
unknown	59110/tcp	0.000152
unknown	59116/udp	0.000502
unknown	59122/tcp	0.000076
unknown	59128/udp	0.000502
unknown	59130/udp	0.000502
unknown	59131/udp	0.000502
unknown	59132/udp	0.001004
unknown	59134/udp	0.000502
unknown	59138/udp	0.000502
unknown	59140/udp	0.000502
unknown	59141/udp	0.000502
unknown	59149/tcp	0.000076
unknown	59158/udp	0.000502
unknown	59159/udp	0.000502
unknown	59160/tcp	0.000076
unknown	59166/udp	0.000502
unknown	59179/udp	0.000502
unknown	59184/udp	0.000502
unknown	59186/udp	0.001004
unknown	59189/udp	0.001004
unknown	59191/tcp	0.000076
unknown	59193/udp	0.001506
unknown	59196/udp	0.000502
unknown	59200/tcp	0.000152
unknown	59201/tcp	0.000152
unknown	59202/tcp	0.000152
unknown	59205/udp	0.000502
unknown	59207/udp	0.001506
unknown	59209/udp	0.000502
unknown	59212/udp	0.000502
unknown	59214/udp	0.001004
unknown	59215/udp	0.000502
unknown	59216/udp	0.001004
unknown	59223/udp	0.000502
unknown	59231/udp	0.000502
unknown	59239/tcp	0.000076
unknown	59239/udp	0.000502
unknown	59253/udp	0.000502
unknown	59254/udp	0.001004
unknown	59256/udp	0.000502
unknown	59258/udp	0.000502
unknown	59260/udp	0.000502
unknown	59265/udp	0.000502
unknown	59267/udp	0.000502
unknown	59272/udp	0.000502
unknown	59279/udp	0.000502
unknown	59282/udp	0.000502
unknown	59295/udp	0.000502
unknown	59296/udp	0.001004
unknown	59301/udp	0.001004
unknown	59303/udp	0.000502
unknown	59324/udp	0.000502
unknown	59327/udp	0.001004
unknown	59328/udp	0.000502
unknown	59335/udp	0.000502
unknown	59340/tcp	0.000076
unknown	59351/udp	0.000502
unknown	59356/udp	0.000502
unknown	59357/udp	0.000502
unknown	59360/udp	0.000502
unknown	59361/udp	0.000502
unknown	59364/udp	0.000502
unknown	59369/udp	0.000502
unknown	59371/udp	0.000502
unknown	59372/udp	0.000502
unknown	59380/udp	0.000502
unknown	59388/udp	0.001004
unknown	59390/udp	0.000502
unknown	59392/udp	0.000502
unknown	59398/udp	0.000502
unknown	59401/udp	0.000502
unknown	59415/udp	0.001004
unknown	59434/udp	0.001004
unknown	59435/udp	0.000502
unknown	59439/udp	0.000502
unknown	59447/udp	0.000502
unknown	59449/udp	0.000502
unknown	59450/udp	0.000502
unknown	59452/udp	0.000502
unknown	59453/udp	0.000502
unknown	59454/udp	0.000502
unknown	59461/udp	0.000502
unknown	59465/udp	0.000502
unknown	59468/udp	0.000502
unknown	59473/udp	0.000502
unknown	59482/udp	0.000502
unknown	59483/udp	0.001004
unknown	59484/udp	0.000502
unknown	59486/udp	0.000502
unknown	59487/udp	0.000502
unknown	59488/udp	0.000502
unknown	59490/udp	0.000502
unknown	59495/udp	0.000502
unknown	59497/udp	0.000502
unknown	59499/tcp	0.000076
unknown	59500/udp	0.000502
unknown	59504/tcp	0.000076
unknown	59506/udp	0.001004
unknown	59509/tcp	0.000076
unknown	59510/tcp	0.000076
unknown	59516/udp	0.000502
unknown	59525/tcp	0.000076
unknown	59554/udp	0.000502
unknown	59555/udp	0.001004
unknown	59563/udp	0.000502
unknown	59564/udp	0.000502
unknown	59565/tcp	0.000076
unknown	59573/udp	0.000502
unknown	59574/udp	0.000502
unknown	59576/udp	0.000502
unknown	59577/udp	0.001004
unknown	59580/udp	0.000502
unknown	59581/udp	0.001004
unknown	59586/udp	0.000502
unknown	59589/udp	0.000502
unknown	59593/udp	0.001004
unknown	59595/udp	0.000502
unknown	59598/udp	0.000502
unknown	59603/udp	0.001004
unknown	59607/udp	0.000502
unknown	59608/udp	0.000502
unknown	59609/udp	0.000502
unknown	59620/udp	0.000502
unknown	59625/udp	0.000502
unknown	59632/udp	0.001004
unknown	59637/udp	0.000502
unknown	59640/udp	0.000502
unknown	59646/udp	0.000502
unknown	59659/udp	0.000502
unknown	59669/udp	0.001004
unknown	59672/udp	0.000502
unknown	59683/udp	0.000502
unknown	59684/tcp	0.000076
unknown	59684/udp	0.000502
unknown	59688/udp	0.000502
unknown	59689/udp	0.000502
unknown	59691/udp	0.000502
unknown	59701/udp	0.000502
unknown	59709/udp	0.000502
unknown	59710/udp	0.000502
unknown	59715/udp	0.000502
unknown	59727/udp	0.000502
unknown	59734/udp	0.000502
unknown	59743/udp	0.000502
unknown	59747/udp	0.000502
unknown	59757/udp	0.000502
unknown	59758/udp	0.001004
unknown	59762/udp	0.000502
unknown	59763/udp	0.000502
unknown	59764/udp	0.000502
unknown	59765/udp	0.001506
unknown	59766/udp	0.000502
unknown	59767/udp	0.000502
unknown	59768/udp	0.000502
unknown	59769/udp	0.000502
unknown	59778/tcp	0.000076
unknown	59781/udp	0.000502
unknown	59790/udp	0.000502
unknown	59791/udp	0.001004
unknown	59794/udp	0.000502
unknown	59797/udp	0.000502
unknown	59798/udp	0.000502
unknown	59805/udp	0.001004
unknown	59809/udp	0.000502
unknown	59810/tcp	0.000076
unknown	59829/tcp	0.000076
unknown	59834/udp	0.000502
unknown	59835/udp	0.000502
unknown	59836/udp	0.000502
unknown	59841/tcp	0.000076
unknown	59846/udp	0.001506
unknown	59847/udp	0.000502
unknown	59853/udp	0.000502
unknown	59860/udp	0.001004
unknown	59874/udp	0.000502
unknown	59883/udp	0.000502
unknown	59884/udp	0.000502
unknown	59885/udp	0.000502
unknown	59888/udp	0.000502
unknown	59891/udp	0.000502
unknown	59897/udp	0.000502
unknown	59902/udp	0.000502
unknown	59919/udp	0.000502
unknown	59925/udp	0.000502
unknown	59928/udp	0.000502
unknown	59933/udp	0.000502
unknown	59934/udp	0.000502
unknown	59935/udp	0.000502
unknown	59943/udp	0.001004
unknown	59948/udp	0.000502
unknown	59949/udp	0.000502
unknown	59951/udp	0.000502
unknown	59952/udp	0.000502
unknown	59960/udp	0.000502
unknown	59966/udp	0.000502
unknown	59969/udp	0.000502
unknown	59971/udp	0.001004
unknown	59984/udp	0.000502
unknown	59987/tcp	0.000076
unknown	59987/udp	0.000502
unknown	59992/udp	0.000502
unknown	59995/udp	0.000502
unknown	59998/udp	0.001004
unknown	60000/tcp	0.000076
unknown	60001/udp	0.000502
unknown	60002/tcp	0.000076
unknown	60003/tcp	0.000076
unknown	60004/udp	0.000502
unknown	60020/tcp	0.000380
unknown	60025/udp	0.000502
unknown	60028/udp	0.001004
unknown	60032/udp	0.000502
unknown	60035/udp	0.001004
unknown	60037/udp	0.000502
unknown	60041/udp	0.000502
unknown	60043/udp	0.000502
unknown	60048/udp	0.000502
unknown	60052/udp	0.000502
unknown	60055/tcp	0.000076
unknown	60055/udp	0.000502
unknown	60062/udp	0.000502
unknown	60067/udp	0.000502
unknown	60069/udp	0.001004
unknown	60071/udp	0.000502
unknown	60075/udp	0.000502
unknown	60076/udp	0.000502
unknown	60086/tcp	0.000076
unknown	60095/udp	0.000502
unknown	60097/udp	0.001004
unknown	60105/udp	0.000502
unknown	60111/tcp	0.000076
unknown	60119/udp	0.000502
unknown	60123/tcp	0.000152
unknown	60126/udp	0.000502
unknown	60129/udp	0.000502
unknown	60130/udp	0.000502
unknown	60134/udp	0.000502
unknown	60138/udp	0.000502
unknown	60140/udp	0.000502
unknown	60142/udp	0.000502
unknown	60145/udp	0.001004
unknown	60146/tcp	0.000152
unknown	60147/udp	0.000502
unknown	60148/udp	0.000502
unknown	60150/udp	0.000502
unknown	60152/udp	0.000502
unknown	60154/udp	0.000502
unknown	60160/udp	0.000502
unknown	60164/udp	0.000502
unknown	60170/udp	0.000502
unknown	60171/udp	0.000502
unknown	60172/udp	0.001506
unknown	60177/tcp	0.000076
unknown	60191/udp	0.000502
unknown	60203/udp	0.000502
unknown	60214/udp	0.000502
unknown	60216/udp	0.000502
unknown	60227/tcp	0.000076
unknown	60227/udp	0.001004
unknown	60236/udp	0.000502
unknown	60240/udp	0.000502
unknown	60243/tcp	0.000076
unknown	60243/udp	0.000502
unknown	60244/udp	0.000502
unknown	60246/udp	0.000502
unknown	60247/udp	0.000502
unknown	60250/udp	0.000502
unknown	60255/udp	0.001004
unknown	60256/udp	0.000502
unknown	60268/udp	0.000502
unknown	60279/tcp	0.000076
unknown	60288/udp	0.000502
unknown	60291/udp	0.000502
unknown	60292/udp	0.000502
unknown	60299/udp	0.000502
unknown	60316/udp	0.000502
unknown	60322/udp	0.000502
unknown	60326/udp	0.000502
unknown	60331/udp	0.000502
unknown	60341/udp	0.001004
unknown	60347/udp	0.001004
unknown	60354/udp	0.000502
unknown	60356/udp	0.000502
unknown	60360/udp	0.000502
unknown	60363/udp	0.001004
unknown	60365/udp	0.000502
unknown	60369/udp	0.000502
unknown	60370/udp	0.000502
unknown	60376/udp	0.000502
unknown	60377/tcp	0.000076
unknown	60381/udp	0.001506
unknown	60383/udp	0.000502
unknown	60384/udp	0.001004
unknown	60401/tcp	0.000076
unknown	60401/udp	0.000502
unknown	60403/tcp	0.000076
unknown	60404/udp	0.000502
unknown	60406/udp	0.000502
unknown	60423/udp	0.001506
unknown	60430/udp	0.001004
unknown	60431/udp	0.001004
unknown	60433/udp	0.000502
unknown	60435/udp	0.001004
unknown	60436/udp	0.000502
unknown	60438/udp	0.001004
unknown	60443/tcp	0.000228
unknown	60449/udp	0.000502
unknown	60454/udp	0.000502
unknown	60455/udp	0.000502
unknown	60462/udp	0.000502
unknown	60472/udp	0.000502
unknown	60485/tcp	0.000076
unknown	60491/udp	0.000502
unknown	60492/tcp	0.000076
unknown	60493/udp	0.000502
unknown	60504/tcp	0.000076
unknown	60517/udp	0.000502
unknown	60522/udp	0.000502
unknown	60528/udp	0.000502
unknown	60544/tcp	0.000076
unknown	60546/udp	0.000502
unknown	60548/udp	0.000502
unknown	60550/udp	0.000502
unknown	60557/udp	0.000502
unknown	60575/udp	0.000502
unknown	60578/udp	0.000502
unknown	60579/tcp	0.000076
unknown	60579/udp	0.000502
unknown	60587/udp	0.000502
unknown	60594/udp	0.000502
unknown	60598/udp	0.000502
unknown	60606/udp	0.000502
unknown	60612/tcp	0.000076
unknown	60613/udp	0.000502
unknown	60618/udp	0.000502
unknown	60621/tcp	0.000076
unknown	60628/tcp	0.000076
unknown	60629/udp	0.000502
unknown	60630/udp	0.000502
unknown	60631/udp	0.000502
unknown	60640/udp	0.000502
unknown	60642/tcp	0.000152
unknown	60650/udp	0.001004
unknown	60655/udp	0.000502
unknown	60662/udp	0.000502
unknown	60665/udp	0.000502
unknown	60675/udp	0.000502
unknown	60677/udp	0.000502
unknown	60678/udp	0.000502
unknown	60679/udp	0.001004
unknown	60683/udp	0.000502
unknown	60696/udp	0.000502
unknown	60700/udp	0.000502
unknown	60701/udp	0.001004
unknown	60704/udp	0.000502
unknown	60705/udp	0.001004
unknown	60707/udp	0.001004
unknown	60712/udp	0.000502
unknown	60713/tcp	0.000076
unknown	60715/udp	0.000502
unknown	60716/udp	0.000502
unknown	60727/udp	0.000502
unknown	60728/tcp	0.000076
unknown	60731/udp	0.000502
unknown	60735/udp	0.000502
unknown	60743/tcp	0.000076
unknown	60748/udp	0.000502
unknown	60753/tcp	0.000076
unknown	60754/udp	0.000502
unknown	60768/udp	0.000502
unknown	60774/udp	0.000502
unknown	60775/udp	0.000502
unknown	60778/udp	0.000502
unknown	60781/udp	0.000502
unknown	60782/tcp	0.000076
unknown	60783/tcp	0.000076
unknown	60789/tcp	0.000076
unknown	60791/udp	0.000502
unknown	60792/udp	0.000502
unknown	60794/tcp	0.000076
unknown	60799/udp	0.000502
unknown	60803/udp	0.000502
unknown	60822/udp	0.000502
unknown	60824/udp	0.000502
unknown	60831/udp	0.000502
unknown	60833/udp	0.000502
unknown	60842/udp	0.000502
unknown	60846/udp	0.000502
unknown	60848/udp	0.000502
unknown	60856/udp	0.000502
unknown	60861/udp	0.000502
unknown	60863/udp	0.000502
unknown	60872/udp	0.000502
unknown	60873/udp	0.000502
unknown	60878/udp	0.000502
unknown	60880/udp	0.000502
unknown	60883/udp	0.000502
unknown	60885/udp	0.000502
unknown	60889/udp	0.000502
unknown	60890/udp	0.000502
unknown	60899/udp	0.000502
unknown	60912/udp	0.000502
unknown	60922/udp	0.000502
unknown	60925/udp	0.000502
unknown	60936/udp	0.000502
unknown	60937/udp	0.000502
unknown	60941/udp	0.000502
unknown	60948/udp	0.000502
unknown	60950/udp	0.001004
unknown	60963/udp	0.000502
unknown	60966/udp	0.001004
unknown	60973/udp	0.000502
unknown	60988/udp	0.001004
unknown	60989/tcp	0.000076
unknown	60990/udp	0.000502
unknown	60996/udp	0.000502
unknown	60998/udp	0.000502
unknown	61000/udp	0.000502
unknown	61001/udp	0.000502
unknown	61003/udp	0.000502
unknown	61005/udp	0.000502
unknown	61006/udp	0.000502
unknown	61016/udp	0.000502
unknown	61020/udp	0.000502
unknown	61024/udp	0.001506
unknown	61027/udp	0.001004
unknown	61032/udp	0.000502
unknown	61038/udp	0.000502
unknown	61042/udp	0.000502
unknown	61046/udp	0.001004
unknown	61047/udp	0.001004
unknown	61048/udp	0.000502
unknown	61050/udp	0.001004
unknown	61054/udp	0.000502
unknown	61055/udp	0.001004
unknown	61081/udp	0.001004
unknown	61086/udp	0.000502
unknown	61095/udp	0.001004
unknown	61100/udp	0.000502
unknown	61107/udp	0.000502
unknown	61125/udp	0.000502
unknown	61127/udp	0.001004
unknown	61128/udp	0.000502
unknown	61130/udp	0.000502
unknown	61137/udp	0.000502
unknown	61142/udp	0.001506
unknown	61149/udp	0.000502
unknown	61151/udp	0.000502
unknown	61159/tcp	0.000076
unknown	61163/udp	0.000502
unknown	61167/udp	0.001004
unknown	61169/tcp	0.000076
unknown	61170/tcp	0.000076
unknown	61171/udp	0.000502
unknown	61188/udp	0.000502
unknown	61192/udp	0.001004
unknown	61193/udp	0.001004
unknown	61198/udp	0.000502
unknown	61202/udp	0.000502
unknown	61207/udp	0.000502
unknown	61210/udp	0.000502
unknown	61213/udp	0.000502
unknown	61219/udp	0.000502
unknown	61226/udp	0.001004
unknown	61233/udp	0.000502
unknown	61244/udp	0.000502
unknown	61260/udp	0.000502
unknown	61265/udp	0.000502
unknown	61269/udp	0.000502
unknown	61270/udp	0.000502
unknown	61277/udp	0.000502
unknown	61278/udp	0.000502
unknown	61284/udp	0.000502
unknown	61294/udp	0.000502
unknown	61301/udp	0.000502
unknown	61309/udp	0.000502
unknown	61315/udp	0.000502
unknown	61318/udp	0.000502
unknown	61319/udp	0.001506
unknown	61321/udp	0.000502
unknown	61322/udp	0.001506
unknown	61338/udp	0.000502
unknown	61348/udp	0.000502
unknown	61349/udp	0.000502
unknown	61364/udp	0.000502
unknown	61370/udp	0.002008
unknown	61371/udp	0.000502
unknown	61373/udp	0.000502
unknown	61374/udp	0.000502
unknown	61381/udp	0.001004
unknown	61389/udp	0.000502
unknown	61393/udp	0.000502
unknown	61395/udp	0.001004
unknown	61397/udp	0.000502
unknown	61400/udp	0.001004
unknown	61401/udp	0.000502
unknown	61402/tcp	0.000076
unknown	61405/udp	0.000502
unknown	61408/udp	0.000502
unknown	61411/udp	0.000502
unknown	61412/udp	0.001506
unknown	61414/udp	0.000502
unknown	61418/udp	0.000502
unknown	61420/udp	0.000502
unknown	61422/udp	0.001004
unknown	61427/udp	0.000502
unknown	61431/udp	0.001004
unknown	61435/udp	0.000502
unknown	61438/udp	0.001004
netprowler-manager	61439/tcp	0.000000
netprowler-manager2	61440/tcp	0.000000
netprowler-sensor	61441/tcp	0.000000
unknown	61448/udp	0.000502
unknown	61452/udp	0.000502
unknown	61455/udp	0.000502
unknown	61456/udp	0.000502
unknown	61458/udp	0.000502
unknown	61463/udp	0.000502
unknown	61466/udp	0.000502
unknown	61473/tcp	0.000076
unknown	61480/udp	0.001004
unknown	61481/udp	0.001506
unknown	61483/udp	0.000502
unknown	61484/udp	0.000502
unknown	61485/udp	0.001004
unknown	61492/udp	0.000502
unknown	61493/udp	0.000502
unknown	61494/udp	0.000502
unknown	61497/udp	0.000502
unknown	61500/udp	0.000502
unknown	61501/udp	0.000502
unknown	61508/udp	0.000502
unknown	61512/udp	0.001004
unknown	61516/tcp	0.000076
unknown	61518/udp	0.000502
unknown	61523/udp	0.001004
unknown	61524/udp	0.000502
unknown	61527/udp	0.000502
unknown	61529/udp	0.000502
unknown	61532/tcp	0.000304
unknown	61532/udp	0.001004
unknown	61539/udp	0.001004
unknown	61542/udp	0.000502
unknown	61550/udp	0.001506
unknown	61551/udp	0.000502
unknown	61553/udp	0.000502
unknown	61554/udp	0.000502
unknown	61556/udp	0.000502
unknown	61574/udp	0.000502
unknown	61579/udp	0.000502
unknown	61586/udp	0.000502
unknown	61587/udp	0.001004
unknown	61590/udp	0.000502
unknown	61601/udp	0.000502
unknown	61613/tcp	0.000152
unknown	61616/tcp	0.000076
unknown	61617/tcp	0.000076
unknown	61623/udp	0.000502
unknown	61635/udp	0.000502
unknown	61638/udp	0.000502
unknown	61652/udp	0.000502
unknown	61653/udp	0.001004
unknown	61654/udp	0.000502
unknown	61667/udp	0.000502
unknown	61669/tcp	0.000076
unknown	61678/udp	0.001004
unknown	61681/udp	0.000502
unknown	61685/udp	0.001506
unknown	61687/udp	0.000502
unknown	61688/udp	0.000502
unknown	61695/udp	0.000502
unknown	61703/udp	0.000502
unknown	61707/udp	0.000502
unknown	61709/udp	0.001004
unknown	61716/udp	0.000502
unknown	61722/tcp	0.000076
unknown	61734/tcp	0.000076
unknown	61748/udp	0.000502
unknown	61753/udp	0.000502
unknown	61756/udp	0.000502
unknown	61762/udp	0.000502
unknown	61764/udp	0.000502
unknown	61774/udp	0.000502
unknown	61781/udp	0.001004
unknown	61783/udp	0.000502
unknown	61784/udp	0.000502
unknown	61786/udp	0.000502
unknown	61790/udp	0.000502
unknown	61794/udp	0.000502
unknown	61795/udp	0.000502
unknown	61802/udp	0.000502
unknown	61804/udp	0.000502
unknown	61815/udp	0.000502
unknown	61818/udp	0.000502
unknown	61821/udp	0.000502
unknown	61825/udp	0.000502
unknown	61827/tcp	0.000076
unknown	61828/udp	0.001004
unknown	61834/udp	0.000502
unknown	61838/udp	0.000502
unknown	61848/udp	0.000502
unknown	61851/tcp	0.000076
unknown	61862/udp	0.000502
unknown	61867/udp	0.001004
unknown	61876/udp	0.000502
unknown	61886/udp	0.000502
unknown	61893/udp	0.000502
unknown	61894/udp	0.000502
unknown	61900/tcp	0.000304
unknown	61902/udp	0.001004
unknown	61906/udp	0.000502
unknown	61921/udp	0.001004
unknown	61936/udp	0.000502
unknown	61937/udp	0.001004
unknown	61942/tcp	0.000076
unknown	61943/udp	0.000502
unknown	61951/udp	0.000502
unknown	61956/udp	0.000502
unknown	61957/udp	0.000502
unknown	61960/udp	0.000502
unknown	61961/udp	0.001506
unknown	61965/udp	0.000502
unknown	61967/udp	0.001004
unknown	61973/udp	0.001004
unknown	61980/udp	0.000502
unknown	61983/udp	0.001004
unknown	61987/udp	0.000502
unknown	61989/udp	0.000502
unknown	61995/udp	0.000502
unknown	61997/udp	0.000502
unknown	62000/udp	0.000502
unknown	62005/udp	0.000502
unknown	62006/tcp	0.000076
unknown	62009/udp	0.000502
unknown	62011/udp	0.000502
unknown	62017/udp	0.000502
unknown	62023/udp	0.000502
unknown	62026/udp	0.000502
unknown	62038/udp	0.001004
unknown	62039/udp	0.000502
unknown	62042/tcp	0.000076
unknown	62046/udp	0.000502
unknown	62053/udp	0.000502
unknown	62056/udp	0.000502
unknown	62064/udp	0.000502
unknown	62070/udp	0.000502
unknown	62071/udp	0.000502
unknown	62072/udp	0.000502
unknown	62074/udp	0.000502
iphone-sync	62078/tcp	0.000304	# Apparently used by iPhone while syncing - http://code.google.com/p/iphone-elite/source/browse/wiki/Port_62078.wiki
unknown	62080/tcp	0.000076
unknown	62083/udp	0.000502
unknown	62086/udp	0.000502
unknown	62089/udp	0.000502
unknown	62090/udp	0.000502
unknown	62092/udp	0.000502
unknown	62100/udp	0.001004
unknown	62101/udp	0.001004
unknown	62111/udp	0.000502
unknown	62114/udp	0.001004
unknown	62116/udp	0.000502
unknown	62132/udp	0.000502
unknown	62133/udp	0.001004
unknown	62143/udp	0.000502
unknown	62146/udp	0.000502
unknown	62152/udp	0.000502
unknown	62154/udp	0.001506
unknown	62164/udp	0.001004
unknown	62165/udp	0.000502
unknown	62166/udp	0.000502
unknown	62170/udp	0.000502
unknown	62178/udp	0.000502
unknown	62181/udp	0.000502
unknown	62187/udp	0.000502
unknown	62188/tcp	0.000076
unknown	62188/udp	0.001004
unknown	62200/udp	0.000502
unknown	62201/udp	0.000502
unknown	62203/udp	0.000502
unknown	62211/udp	0.000502
unknown	62214/udp	0.000502
unknown	62215/udp	0.000502
unknown	62216/udp	0.001004
unknown	62218/udp	0.000502
unknown	62232/udp	0.000502
unknown	62233/udp	0.000502
unknown	62243/udp	0.000502
unknown	62245/udp	0.000502
unknown	62246/udp	0.000502
unknown	62250/udp	0.000502
unknown	62251/udp	0.000502
unknown	62256/udp	0.000502
unknown	62267/udp	0.000502
unknown	62270/udp	0.000502
unknown	62274/udp	0.000502
unknown	62281/udp	0.001004
unknown	62285/udp	0.000502
unknown	62287/udp	0.002008
unknown	62295/udp	0.000502
unknown	62302/udp	0.000502
unknown	62305/udp	0.000502
unknown	62312/tcp	0.000076
unknown	62312/udp	0.000502
unknown	62320/udp	0.000502
unknown	62321/udp	0.000502
unknown	62325/udp	0.001004
unknown	62345/udp	0.000502
unknown	62346/udp	0.000502
unknown	62362/udp	0.000502
unknown	62370/udp	0.000502
unknown	62377/udp	0.000502
unknown	62383/udp	0.000502
unknown	62385/udp	0.000502
unknown	62386/udp	0.000502
unknown	62392/udp	0.000502
unknown	62398/udp	0.000502
unknown	62404/udp	0.001004
unknown	62408/udp	0.000502
unknown	62412/udp	0.001004
unknown	62413/udp	0.000502
unknown	62418/udp	0.000502
unknown	62420/udp	0.001004
unknown	62424/udp	0.000502
unknown	62431/udp	0.000502
unknown	62435/udp	0.000502
unknown	62436/udp	0.001004
unknown	62440/udp	0.000502
unknown	62442/udp	0.000502
unknown	62449/udp	0.001004
unknown	62454/udp	0.000502
unknown	62458/udp	0.001004
unknown	62461/udp	0.000502
unknown	62466/udp	0.000502
unknown	62469/udp	0.000502
unknown	62477/udp	0.000502
unknown	62479/udp	0.000502
unknown	62484/udp	0.000502
unknown	62485/udp	0.000502
unknown	62493/udp	0.001004
unknown	62496/udp	0.000502
unknown	62511/udp	0.000502
unknown	62516/udp	0.000502
unknown	62518/udp	0.000502
unknown	62519/tcp	0.000076
unknown	62522/udp	0.001004
unknown	62526/udp	0.000502
unknown	62533/udp	0.000502
unknown	62534/udp	0.000502
unknown	62540/udp	0.000502
unknown	62544/udp	0.000502
unknown	62556/udp	0.000502
unknown	62562/udp	0.001004
unknown	62563/udp	0.000502
unknown	62566/udp	0.000502
unknown	62570/tcp	0.000076
unknown	62574/udp	0.000502
unknown	62575/udp	0.001506
unknown	62578/udp	0.000502
unknown	62581/udp	0.000502
unknown	62590/udp	0.000502
unknown	62599/udp	0.000502
unknown	62600/udp	0.000502
unknown	62604/udp	0.000502
unknown	62606/udp	0.000502
unknown	62612/udp	0.000502
unknown	62617/udp	0.000502
unknown	62621/udp	0.000502
unknown	62629/udp	0.000502
unknown	62630/udp	0.000502
unknown	62631/udp	0.000502
unknown	62635/udp	0.000502
unknown	62637/udp	0.000502
unknown	62647/udp	0.000502
unknown	62652/udp	0.000502
unknown	62658/udp	0.000502
unknown	62662/udp	0.000502
unknown	62671/udp	0.000502
unknown	62674/tcp	0.000076
unknown	62677/udp	0.001506
unknown	62678/udp	0.000502
unknown	62679/udp	0.000502
unknown	62680/udp	0.000502
unknown	62682/udp	0.000502
unknown	62689/udp	0.000502
unknown	62690/udp	0.001004
unknown	62697/udp	0.001004
unknown	62699/udp	0.001506
unknown	62701/udp	0.001004
unknown	62707/udp	0.000502
unknown	62708/udp	0.000502
unknown	62711/udp	0.000502
unknown	62725/udp	0.000502
unknown	62738/udp	0.000502
unknown	62760/udp	0.000502
unknown	62761/udp	0.000502
unknown	62764/udp	0.000502
unknown	62766/udp	0.000502
unknown	62778/udp	0.001004
unknown	62779/udp	0.000502
unknown	62783/udp	0.000502
unknown	62785/udp	0.000502
unknown	62788/udp	0.000502
unknown	62791/udp	0.000502
unknown	62820/udp	0.000502
unknown	62821/udp	0.000502
unknown	62822/udp	0.000502
unknown	62825/udp	0.000502
unknown	62827/udp	0.001004
unknown	62834/udp	0.000502
unknown	62841/udp	0.000502
unknown	62843/udp	0.000502
unknown	62845/udp	0.001004
unknown	62846/udp	0.000502
unknown	62856/udp	0.000502
unknown	62858/udp	0.000502
unknown	62866/tcp	0.000076
unknown	62866/udp	0.001004
unknown	62874/udp	0.000502
unknown	62878/udp	0.000502
unknown	62880/udp	0.001004
unknown	62884/udp	0.000502
unknown	62887/udp	0.000502
unknown	62888/udp	0.000502
unknown	62892/udp	0.000502
unknown	62902/udp	0.000502
unknown	62906/udp	0.000502
unknown	62909/udp	0.000502
unknown	62923/udp	0.000502
unknown	62933/udp	0.000502
unknown	62934/udp	0.000502
unknown	62935/udp	0.000502
unknown	62936/udp	0.000502
unknown	62937/udp	0.000502
unknown	62955/udp	0.001004
unknown	62957/udp	0.000502
unknown	62958/udp	0.001506
unknown	62962/udp	0.000502
unknown	62964/udp	0.000502
unknown	62965/udp	0.000502
unknown	62972/udp	0.000502
unknown	62973/udp	0.000502
unknown	62975/udp	0.001004
unknown	62982/udp	0.000502
unknown	62985/udp	0.000502
unknown	62993/udp	0.000502
unknown	62998/udp	0.000502
unknown	63000/udp	0.000502
unknown	63006/udp	0.001004
unknown	63014/udp	0.000502
unknown	63017/udp	0.000502
unknown	63021/udp	0.000502
unknown	63033/udp	0.000502
unknown	63036/udp	0.000502
unknown	63039/udp	0.000502
unknown	63049/udp	0.000502
unknown	63062/udp	0.000502
unknown	63067/udp	0.000502
unknown	63071/udp	0.000502
unknown	63073/udp	0.000502
unknown	63079/udp	0.001004
unknown	63086/udp	0.000502
unknown	63088/udp	0.000502
unknown	63089/udp	0.000502
unknown	63091/udp	0.000502
unknown	63092/udp	0.000502
unknown	63101/udp	0.001004
unknown	63105/tcp	0.000076
unknown	63106/udp	0.001004
unknown	63109/udp	0.000502
unknown	63112/udp	0.000502
unknown	63120/udp	0.000502
unknown	63129/udp	0.001004
unknown	63135/udp	0.000502
unknown	63136/udp	0.001004
unknown	63139/udp	0.000502
unknown	63143/udp	0.000502
unknown	63145/udp	0.000502
unknown	63146/udp	0.001004
unknown	63147/udp	0.000502
unknown	63149/udp	0.000502
unknown	63151/udp	0.000502
unknown	63156/tcp	0.000076
unknown	63160/udp	0.000502
unknown	63162/udp	0.000502
unknown	63172/udp	0.000502
unknown	63173/udp	0.001004
unknown	63176/udp	0.000502
unknown	63179/udp	0.000502
unknown	63186/udp	0.000502
unknown	63197/udp	0.000502
unknown	63203/udp	0.000502
unknown	63210/udp	0.000502
unknown	63211/udp	0.000502
unknown	63213/udp	0.000502
unknown	63217/udp	0.000502
unknown	63220/udp	0.000502
unknown	63231/udp	0.000502
unknown	63232/udp	0.000502
unknown	63237/udp	0.000502
unknown	63238/udp	0.000502
unknown	63246/udp	0.000502
unknown	63247/udp	0.001004
unknown	63251/udp	0.000502
unknown	63266/udp	0.000502
unknown	63270/udp	0.000502
unknown	63273/udp	0.000502
unknown	63278/udp	0.000502
unknown	63281/udp	0.001004
unknown	63289/udp	0.000502
unknown	63315/udp	0.000502
unknown	63318/udp	0.000502
unknown	63322/udp	0.000502
unknown	63325/udp	0.000502
unknown	63330/udp	0.000502
unknown	63331/tcp	0.000380
unknown	63331/udp	0.001004
unknown	63335/udp	0.000502
unknown	63336/udp	0.000502
unknown	63337/udp	0.001004
unknown	63343/udp	0.000502
unknown	63344/udp	0.001004
unknown	63346/udp	0.001004
unknown	63351/udp	0.000502
unknown	63356/udp	0.000502
unknown	63363/udp	0.000502
unknown	63366/udp	0.000502
unknown	63373/udp	0.000502
unknown	63385/udp	0.000502
unknown	63397/udp	0.000502
unknown	63398/udp	0.000502
unknown	63407/udp	0.000502
unknown	63409/udp	0.000502
unknown	63410/udp	0.000502
unknown	63411/udp	0.000502
unknown	63420/udp	0.001506
unknown	63423/tcp	0.000076
unknown	63423/udp	0.000502
unknown	63427/udp	0.000502
unknown	63446/udp	0.000502
unknown	63447/udp	0.001004
unknown	63449/udp	0.000502
unknown	63451/udp	0.000502
unknown	63461/udp	0.000502
unknown	63464/udp	0.000502
unknown	63466/udp	0.000502
unknown	63477/udp	0.000502
unknown	63481/udp	0.000502
unknown	63495/udp	0.000502
unknown	63499/udp	0.001004
unknown	63508/udp	0.001004
unknown	63514/udp	0.000502
unknown	63515/udp	0.000502
unknown	63517/udp	0.000502
unknown	63524/udp	0.000502
unknown	63532/udp	0.000502
unknown	63533/udp	0.000502
unknown	63534/udp	0.001004
unknown	63535/udp	0.000502
unknown	63543/udp	0.000502
unknown	63546/udp	0.000502
unknown	63555/udp	0.002008
unknown	63564/udp	0.000502
unknown	63566/udp	0.000502
unknown	63567/udp	0.000502
unknown	63574/udp	0.000502
unknown	63587/udp	0.000502
unknown	63595/udp	0.000502
unknown	63613/udp	0.000502
unknown	63614/udp	0.000502
unknown	63619/udp	0.000502
unknown	63625/udp	0.000502
unknown	63626/udp	0.000502
unknown	63632/udp	0.000502
unknown	63636/udp	0.000502
unknown	63638/udp	0.000502
unknown	63640/udp	0.000502
unknown	63644/udp	0.000502
unknown	63647/udp	0.000502
unknown	63656/udp	0.000502
unknown	63657/udp	0.000502
unknown	63661/udp	0.000502
unknown	63663/udp	0.000502
unknown	63664/udp	0.000502
unknown	63671/udp	0.000502
unknown	63673/udp	0.001004
unknown	63675/tcp	0.000076
unknown	63677/udp	0.000502
unknown	63678/udp	0.000502
unknown	63681/udp	0.000502
unknown	63682/udp	0.000502
unknown	63683/udp	0.000502
unknown	63686/udp	0.000502
unknown	63698/udp	0.000502
unknown	63700/udp	0.001004
unknown	63707/udp	0.000502
unknown	63710/udp	0.001004
unknown	63714/udp	0.000502
unknown	63715/udp	0.000502
unknown	63720/udp	0.000502
unknown	63721/udp	0.000502
unknown	63740/udp	0.000502
unknown	63747/udp	0.000502
unknown	63753/udp	0.000502
unknown	63757/udp	0.000502
unknown	63774/udp	0.000502
unknown	63776/udp	0.000502
unknown	63777/udp	0.000502
unknown	63786/udp	0.001004
unknown	63791/udp	0.000502
unknown	63793/udp	0.000502
unknown	63803/tcp	0.000076
unknown	63803/udp	0.000502
unknown	63814/udp	0.000502
unknown	63820/udp	0.001004
unknown	63823/udp	0.000502
unknown	63826/udp	0.000502
unknown	63830/udp	0.000502
unknown	63833/udp	0.000502
unknown	63835/udp	0.000502
unknown	63853/udp	0.000502
unknown	63856/udp	0.000502
unknown	63864/udp	0.000502
unknown	63874/udp	0.000502
unknown	63875/udp	0.000502
unknown	63877/udp	0.000502
unknown	63878/udp	0.000502
unknown	63879/udp	0.000502
unknown	63892/udp	0.000502
unknown	63901/udp	0.000502
unknown	63904/udp	0.000502
unknown	63906/udp	0.000502
unknown	63907/udp	0.000502
unknown	63914/udp	0.000502
unknown	63917/udp	0.001004
unknown	63930/udp	0.000502
unknown	63931/udp	0.000502
unknown	63942/udp	0.000502
unknown	63943/udp	0.000502
unknown	63946/udp	0.000502
unknown	63948/udp	0.000502
unknown	63951/udp	0.000502
unknown	63962/udp	0.001004
unknown	63966/udp	0.000502
unknown	63967/udp	0.000502
unknown	63973/udp	0.000502
unknown	63975/udp	0.000502
unknown	63983/udp	0.000502
unknown	63995/udp	0.000502
unknown	64006/udp	0.000502
unknown	64007/udp	0.000502
unknown	64012/udp	0.000502
unknown	64015/udp	0.000502
unknown	64016/udp	0.000502
unknown	64035/udp	0.000502
unknown	64042/udp	0.000502
unknown	64047/udp	0.000502
unknown	64053/udp	0.000502
unknown	64058/udp	0.000502
unknown	64065/udp	0.000502
unknown	64072/udp	0.000502
unknown	64080/tcp	0.000076
unknown	64080/udp	0.001506
unknown	64081/udp	0.000502
unknown	64083/udp	0.000502
unknown	64090/udp	0.000502
unknown	64113/udp	0.000502
unknown	64114/udp	0.000502
unknown	64118/udp	0.000502
unknown	64120/udp	0.000502
unknown	64123/udp	0.000502
unknown	64127/tcp	0.000076
unknown	64127/udp	0.000502
unknown	64130/udp	0.000502
unknown	64135/udp	0.000502
unknown	64139/udp	0.000502
unknown	64140/udp	0.000502
unknown	64150/udp	0.000502
unknown	64151/udp	0.000502
unknown	64161/udp	0.000502
unknown	64163/udp	0.000502
unknown	64165/udp	0.000502
unknown	64175/udp	0.000502
unknown	64183/udp	0.000502
unknown	64184/udp	0.000502
unknown	64187/udp	0.000502
unknown	64188/udp	0.000502
unknown	64198/udp	0.000502
unknown	64202/udp	0.001004
unknown	64215/udp	0.000502
unknown	64222/udp	0.000502
unknown	64225/udp	0.000502
unknown	64240/udp	0.000502
unknown	64244/udp	0.000502
unknown	64247/udp	0.000502
unknown	64252/udp	0.000502
unknown	64257/udp	0.000502
unknown	64258/udp	0.001004
unknown	64259/udp	0.001004
unknown	64273/udp	0.000502
unknown	64277/udp	0.000502
unknown	64280/udp	0.000502
unknown	64284/udp	0.001004
unknown	64286/udp	0.000502
unknown	64296/udp	0.000502
unknown	64312/udp	0.001004
unknown	64313/udp	0.001004
unknown	64320/tcp	0.000076
unknown	64325/udp	0.000502
unknown	64335/udp	0.000502
unknown	64337/udp	0.000502
unknown	64340/udp	0.001004
unknown	64341/udp	0.000502
unknown	64345/udp	0.001004
unknown	64348/udp	0.000502
unknown	64360/udp	0.000502
unknown	64363/udp	0.000502
unknown	64365/udp	0.001004
unknown	64367/udp	0.000502
unknown	64370/udp	0.000502
unknown	64401/udp	0.000502
unknown	64406/udp	0.001004
unknown	64410/udp	0.000502
unknown	64428/udp	0.000502
unknown	64430/udp	0.000502
unknown	64438/tcp	0.000076
unknown	64441/udp	0.000502
unknown	64442/udp	0.000502
unknown	64446/udp	0.000502
unknown	64447/udp	0.000502
unknown	64450/udp	0.000502
unknown	64456/udp	0.001004
unknown	64460/udp	0.000502
unknown	64461/udp	0.000502
unknown	64466/udp	0.000502
unknown	64469/udp	0.001004
unknown	64474/udp	0.000502
unknown	64481/udp	0.001506
unknown	64492/udp	0.001004
unknown	64493/udp	0.000502
unknown	64494/udp	0.000502
unknown	64507/tcp	0.000076
unknown	64511/udp	0.000502
unknown	64512/udp	0.000502
unknown	64513/udp	0.002008
unknown	64530/udp	0.000502
unknown	64533/udp	0.000502
unknown	64534/udp	0.000502
unknown	64536/udp	0.000502
unknown	64540/udp	0.000502
unknown	64541/udp	0.000502
unknown	64544/udp	0.001004
unknown	64550/udp	0.000502
unknown	64551/tcp	0.000076
unknown	64555/udp	0.000502
unknown	64556/udp	0.000502
unknown	64558/udp	0.000502
unknown	64566/udp	0.001004
unknown	64574/udp	0.000502
unknown	64576/udp	0.000502
unknown	64585/udp	0.000502
unknown	64589/udp	0.001004
unknown	64590/udp	0.001506
unknown	64612/udp	0.000502
unknown	64615/udp	0.001004
unknown	64616/udp	0.001004
unknown	64621/udp	0.000502
unknown	64623/tcp	0.000760
unknown	64625/udp	0.000502
unknown	64630/udp	0.001004
unknown	64636/udp	0.000502
unknown	64640/udp	0.001004
unknown	64644/udp	0.000502
unknown	64646/udp	0.000502
unknown	64647/udp	0.000502
unknown	64649/udp	0.000502
unknown	64652/udp	0.000502
unknown	64654/udp	0.000502
unknown	64657/udp	0.000502
unknown	64658/udp	0.000502
unknown	64660/udp	0.000502
unknown	64676/udp	0.000502
unknown	64680/tcp	0.000760
unknown	64682/udp	0.001004
unknown	64685/udp	0.000502
unknown	64693/udp	0.001004
unknown	64696/udp	0.000502
unknown	64709/udp	0.000502
unknown	64721/udp	0.000502
unknown	64726/tcp	0.000076
unknown	64726/udp	0.000502
unknown	64727/tcp	0.000076
unknown	64727/udp	0.001506
unknown	64729/udp	0.000502
unknown	64731/udp	0.000502
unknown	64735/udp	0.000502
unknown	64737/udp	0.000502
murmur	64738/udp	0.000502	# Murmur is the server-side software for Mumble open source voice chat software
unknown	64740/udp	0.000502
unknown	64743/udp	0.000502
unknown	64746/udp	0.000502
unknown	64750/udp	0.000502
unknown	64751/udp	0.000502
unknown	64755/udp	0.000502
unknown	64767/udp	0.000502
unknown	64772/udp	0.001004
unknown	64774/udp	0.000502
unknown	64778/udp	0.000502
unknown	64779/udp	0.000502
unknown	64795/udp	0.001004
unknown	64798/udp	0.001004
unknown	64800/udp	0.000502
unknown	64802/udp	0.000502
unknown	64811/udp	0.000502
unknown	64813/udp	0.000502
unknown	64815/udp	0.000502
unknown	64816/udp	0.000502
unknown	64817/udp	0.000502
unknown	64820/udp	0.000502
unknown	64829/udp	0.001004
unknown	64836/udp	0.000502
unknown	64840/udp	0.000502
unknown	64843/udp	0.000502
unknown	64846/udp	0.000502
unknown	64874/udp	0.001004
unknown	64875/udp	0.000502
unknown	64876/udp	0.000502
unknown	64878/udp	0.000502
unknown	64884/udp	0.001004
unknown	64889/udp	0.000502
unknown	64890/tcp	0.000076
unknown	64890/udp	0.001004
unknown	64892/udp	0.000502
unknown	64894/udp	0.000502
unknown	64916/udp	0.000502
unknown	64918/udp	0.000502
unknown	64921/udp	0.000502
unknown	64926/udp	0.000502
unknown	64939/udp	0.000502
unknown	64944/udp	0.001004
unknown	64949/udp	0.000502
unknown	64982/udp	0.000502
unknown	64998/udp	0.000502
unknown	65000/tcp	0.000760
unknown	65001/udp	0.000502
unknown	65002/udp	0.000502
unknown	65003/udp	0.000502
unknown	65018/udp	0.000502
unknown	65019/udp	0.000502
unknown	65024/udp	0.016064
unknown	65025/udp	0.000502
unknown	65030/udp	0.000502
unknown	65031/udp	0.000502
unknown	65043/udp	0.000502
unknown	65048/tcp	0.000076
unknown	65052/udp	0.000502
unknown	65053/udp	0.000502
unknown	65062/udp	0.000502
unknown	65066/udp	0.000502
unknown	65068/udp	0.000502
unknown	65073/udp	0.000502
unknown	65077/udp	0.000502
unknown	65080/udp	0.000502
unknown	65082/udp	0.000502
unknown	65087/udp	0.000502
unknown	65098/udp	0.000502
unknown	65101/udp	0.000502
unknown	65105/udp	0.001004
unknown	65113/udp	0.000502
unknown	65116/udp	0.000502
unknown	65122/udp	0.000502
unknown	65123/udp	0.000502
unknown	65124/udp	0.000502
unknown	65129/tcp	0.000380
unknown	65129/udp	0.000502
unknown	65152/udp	0.000502
unknown	65155/udp	0.000502
unknown	65159/udp	0.000502
unknown	65174/udp	0.000502
unknown	65176/udp	0.000502
unknown	65178/udp	0.000502
unknown	65199/udp	0.000502
unknown	65200/udp	0.000502
unknown	65214/udp	0.000502
unknown	65220/udp	0.000502
unknown	65227/udp	0.000502
unknown	65230/udp	0.000502
unknown	65232/udp	0.001004
unknown	65239/udp	0.000502
unknown	65248/udp	0.000502
unknown	65266/udp	0.000502
unknown	65274/udp	0.000502
unknown	65275/udp	0.000502
unknown	65276/udp	0.000502
unknown	65282/udp	0.000502
unknown	65286/udp	0.001004
unknown	65292/udp	0.000502
pcanywhere	65301/tcp	0.000025
unknown	65305/udp	0.000502
unknown	65310/tcp	0.000152
unknown	65310/udp	0.000502
unknown	65311/tcp	0.000076
unknown	65311/udp	0.000502
unknown	65312/udp	0.000502
unknown	65320/udp	0.000502
unknown	65324/udp	0.000502
unknown	65338/udp	0.000502
unknown	65347/udp	0.001004
unknown	65361/udp	0.000502
unknown	65363/udp	0.000502
unknown	65373/udp	0.000502
unknown	65376/udp	0.000502
unknown	65377/udp	0.000502
unknown	65380/udp	0.001004
unknown	65386/udp	0.000502
unknown	65389/tcp	0.000760
unknown	65392/udp	0.000502
unknown	65396/udp	0.001004
unknown	65397/udp	0.000502
unknown	65407/udp	0.000502
unknown	65419/udp	0.000502
unknown	65420/udp	0.001004
unknown	65421/udp	0.000502
unknown	65429/udp	0.000502
unknown	65434/udp	0.000502
unknown	65444/udp	0.000502
unknown	65451/udp	0.000502
unknown	65460/udp	0.001004
unknown	65469/udp	0.000502
unknown	65476/udp	0.000502
unknown	65483/udp	0.000502
unknown	65487/udp	0.000502
unknown	65488/tcp	0.000076
unknown	65492/udp	0.000502
unknown	65493/udp	0.000502
unknown	65498/udp	0.000502
unknown	65499/udp	0.000502
unknown	65501/udp	0.000502
unknown	65506/udp	0.000502
unknown	65512/udp	0.000502
unknown	65514/tcp	0.000076
unknown	65517/udp	0.000502
unknown	65520/udp	0.001004
unknown	65526/udp	0.000502
unknown	65530/udp	0.000502
unknown	65531/udp	0.000502
unknown	65532/udp	0.000502
## service-names-port-numbers.xml
```