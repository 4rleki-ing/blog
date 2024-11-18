---
icon: forklift
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

# Dorking



* <mark style="color:green;">**Google Dork - Server Errors**</mark>

```
inurl:"error" | intitle:"exception" | intitle:"failure" | intitle:"server at" | inurl:exception | "database error" | "SQL syntax" | "undefined index" | "unhandled exception" | "stack trace" site:example.com 
```











Google Dorks for Bug Bounty\
\
Extensión PHP con parámetros\
site:[http://example.com](http://example.com/) ext:php inurl:?\
\
Puntos de conexión de API\
site:example\[.]com inurl:api | site:\*/rest | site:\*/v1 | site:\*/v2 | site:\*/v3\
\
Extensiones jugosas\
site:"example\[.]com" ext:log | ext:txt | ext:conf | ext:cnf | ext:ini | ext:env | ext:sh | ext:bak | ext:backup | ext:swp | ext:old | ext:\~ | ext:git | ext:svn | ext:htpasswd | ext:htaccess | ext:json\
\
Palabras clave inurl de alto %\
inurl:conf | inurl:env | inurl:cgi | inurl:bin | inurl:etc | inurl:root | inurl:sql | inurl:backup | inurl:admin | inurl:php site:example\[.]com\
\
Errores del servidor\
inurl:"error" | intitle:"exception" | intitle:"failure" | intitle:"server at" | inurl:exception | "database error" | "SQL syntax" | "undefined index" | "unhandled exception" | "stack trace" site:example\[.]com\
\
Parámetros propensos a XSS\
inurl:q= | inurl:s= | inurl:search= | inurl:query= | inurl:keyword= | inurl:lang= inurl:& site:[http://example.com](http://example.com/)\
\
Parámetros propensos a redireccionar abiertos\
inurl:url= | inurl:return= | inurl:next= | inurl:redirect= | inurl:redir= | inurl:ret= | inurl:r2= | inurl:page= inurl:& inurl:http site:[http://example.com](http://example.com/)\
\
Parámetros propensos a SQLi\
inurl:id= | inurl:pid= | inurl:category= | inurl:cat= | inurl:action= | inurl:sid= | inurl:dir= inurl:& site:[http://example.com](http://example.com/)\
\
Parámetros propensos a la SSRF\
inurl:http | inurl:url= | inurl:path= | inurl:dest= | inurl:html= | inurl:data= | inurl:domain= | inurl:page= inurl:& site:[http://example.com](http://example.com/)\
\
Parámetros propensos a LFI\
inurl:include | inurl:dir | inurl:detail= | inurl:file= | inurl:folder= | inurl:inc= | inurl:locate= | inurl:doc= | inurl:conf= inurl:& site:[http://example.com](http://example.com/)\
\
Parámetros propensos a RCE\
inurl:cmd | inurl:exec= | inurl:query= | inurl:code= | inurl:do= | inurl:run= | inurl:read= | inurl:ping= inurl:& site:[http://example.com](http://example.com/)\
\
Puntos de conexión de carga de archivos\
site:[http://example.com](http://example.com/) ”choose file”\
\
Documentos de API\
inurl:apidocs | inurl:api-docs | inurl:swagger | inurl:api-explorer site:"[http://example.com](http://example.com/)"\
\
Páginas de inicio de sesión\
inurl:login | inurl:signin | intitle:login | intitle:signin | inurl:secure site:example\[.]com\
\
Entornos de prueba\
inurl:test | inurl:env | inurl:dev | inurl:staging | inurl:sandbox | inurl:debug | inurl:temp | inurl:internal | inurl:demo site:[http://example.com](http://example.com/)\
\
Documentos confidenciales\
site:[http://example.com](http://example.com/) ext:txt | ext:pdf | ext:xml | ext:xls | ext:xlsx | ext:ppt | ext:pptx | ext:doc | ext:docx intext:“confidential” | intext:“Not for Public Release” | intext:”internal use only” | intext:“do not distribute”\
\
Parámetros sensibles\
inurl:email= | inurl:phone= | inurl:password= | inurl:secret= inurl:& site:[http://example.com](http://example.com/)\
\
Adobe Experience Manager (AEM)\
inurl:/content/usergenerated | inurl:/content/dam | inurl:/jcr:content | inurl:/libs/granite | inurl:/etc/clientlibs | inurl:/content/geometrixx | inurl:/bin/wcm | inurl:/crx/de site:[http://example.com](http://example.com/)













