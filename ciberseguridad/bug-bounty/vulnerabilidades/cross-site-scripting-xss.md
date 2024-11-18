---
description: >-
  Cross-Site Scripting (XSS) es una vulnerabilidad de seguridad web frecuente
  que permite a los atacantes inyectar scripts maliciosos en las páginas web
  vistas por los usuarios.
icon: syringe
cover: ../../../.gitbook/assets/1731705666033.jpg
coverY: 36.596461668070766
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

# Cross-Site Scripting (XSS)

Los ataques XSS se producen cuando un atacante utiliza una aplicación web para enviar código malicioso, normalmente en forma de script del lado del navegador, a un usuario final diferente. Estos ataques explotan la confianza que un usuario tiene en un sitio web en particular, lo que permite al atacante robar información confidencial, secuestrar sesiones de usuario o desfigurar sitios web2.

## <mark style="color:blue;">Tipos de vulnerabilidades XSS</mark> <a href="#ember11601" id="ember11601"></a>

1. <mark style="color:green;">**XSS reflejado**</mark>: El script malicioso se refleja fuera del servidor web, como en un mensaje de error o en un resultado de búsqueda.
2. <mark style="color:green;">**XSS almacenado**</mark>: El script malicioso se almacena en el servidor y se ejecuta cuando los usuarios acceden a la página afectada.
3. <mark style="color:green;">**XSS basado en DOM**</mark>: La vulnerabilidad existe en el código del lado del cliente en lugar del código del lado del servidor.

#### Métodos de explotación <a href="#ember11603" id="ember11603"></a>

Los atacantes explotan las vulnerabilidades XSS inyectando código malicioso en aplicaciones web que no validan ni codifican correctamente las entradas del usuario. Esto se puede hacer a través de varios medios, tales como:

* **Campos de entrada**: Los atacantes introducen scripts maliciosos en los campos del formulario.
* **Parámetros de URL**: Los scripts maliciosos se anexan a las direcciones URL.
* **Encabezados HTTP**: Los scripts se inyectan en los encabezados enviados por el navegador.

#### Herramientas para detectar vulnerabilidades XSS <a href="#ember11606" id="ember11606"></a>

Varias herramientas pueden ayudar a identificar vulnerabilidades XSS en aplicaciones web:

* **Suite de eructos**: Pruebas exhaustivas de seguridad de aplicaciones web.
* **XSStrike**: Herramienta avanzada de fuzzing para la detección de vulnerabilidades XSS.
* **Alce**: Detección de vulnerabilidades en la línea de comandos de código abierto.
* **Detectar**: Escaneo automatizado de XSS y otras vulnerabilidades.
* **OWASP ZAP**: Herramienta integrada de pruebas de seguridad.

#### Escaneo y detección de vulnerabilidades XSS <a href="#ember11609" id="ember11609"></a>

Para detectar vulnerabilidades XSS, las aplicaciones web deben analizarse regularmente utilizando herramientas automatizadas y revisiones manuales del código. Los escáneres simulan ataques y detectan puntos de inyección explotables, lo que proporciona informes completos para la corrección4.

#### El ataque XSS más peligroso <a href="#ember11611" id="ember11611"></a>

Los ataques XSS almacenados se consideran los más peligrosos porque el script malicioso se almacena permanentemente en el servidor y se ejecuta cada vez que se accede a la página afectada. Esto puede llevar a un compromiso generalizado de los datos de los usuarios y a una exposición prolongada a los ataques.

#### Actualizaciones actuales y estrategias de prevención <a href="#ember11613" id="ember11613"></a>

Para mitigar las vulnerabilidades de XSS, los desarrolladores deben:

* **Validar y codificar entradas**: Asegúrese de que todas las entradas del usuario estén validadas y codificadas correctamente.
* **Usar bibliotecas de seguridad**: Implemente bibliotecas y marcos de seguridad que ofrezcan protección XSS integrada.
* **Auditorías periódicas**: Realizar auditorías de seguridad periódicas y revisiones de código para identificar y corregir vulnerabilidades.
* **Política de seguridad de contenido (CSP)**: Implemente CSP para restringir la ejecución de scripts de orígenes no autorizados.

#### Conclusión <a href="#ember11616" id="ember11616"></a>

Las vulnerabilidades XSS representan una amenaza significativa para la seguridad web, pero con las herramientas de detección adecuadas y las estrategias de prevención, se pueden mitigar de manera efectiva. Al mantenerse informados y proactivos, los desarrolladores pueden proteger sus aplicaciones y usuarios de los ataques XSS.

## <mark style="color:blue;">XSS Reflejado</mark>

Este ataque se produce cuando el hacker inyecta código malicioso en la solicitud HTTP (como una URL o un formulario) y el resultado se devuelve directamente al usuario infectado sin almacenarlo en el servidor.

¡XSS reflejado en el formulario de registro!

```
"onmous%25%37%34eover=alerta(documento.cookie)>123
```

## <mark style="color:blue;">Stored Cross-Site Scripting (XSS)</mark>

Un ataque XSS almacenado se produce cuando el hacker inyecta permanentemente código malicioso en la base de datos o en el servidor. Significa que el código malicioso se almacena en un lugar específico, como comentarios del usuario o formulario de entrada de datos, y cuando el usuario ingresa a la página infectada, el código se descarga y se ejecuta en el navegador.

una carga útil que inyectaba una etiqueta de estilo para reemplazar el fondo de una página web con un GIF personalizado:

```
<𝘀𝘁𝘆𝗹𝗲>
div {
 imagen-de-fondo: url('Enter_Your_URL');
}
</𝘀𝘁𝘆𝗹𝗲>
```

## <mark style="color:blue;">XSS basado en DOM</mark>

Este tipo es diferente de otros tipos porque ocurre solo dentro del navegador, sin la intervención del servidor. El hacker explota los códigos JavaScript que se ocupan del DOM, como cuando se introducen datos en una página y los elementos se modifican en consecuencia.

### <mark style="color:yellow;">Ejemplo.</mark>

La interfaz de usuario de Swagger permite a los usuarios proporcionar una URL que apunte a una especificación de API (ya sea un archivo YAML o JSON) a través de parámetros de consulta como:

* ?url=https://your\_api\_spec/spec.yaml
* ?configUrl=https://your\_api\_spec/file.json

Un atacante puede alojar un archivo JSON malintencionado que contenga un enlace a otro archivo YAML con una carga XSS incrustada.

Cuando la URL se proporciona a la interfaz de usuario de Swagger a través de parámetros de consulta, carga el archivo YAML malintencionado.

Debido a la desinfección inadecuada en versiones obsoletas de la interfaz de usuario de Swagger, esta carga útil puede ejecutar JavaScript en el navegador de la víctima, lo que lleva a un posible ataque XSS.

## <mark style="color:red;">¿Cómo proteger tu proyecto de los ataques XSS?</mark>

1️⃣ Filtrar la entrada del usuario (Validación de entrada): Cualquier dato procedente del usuario debe filtrarse antes de que se pueda mostrar. En Angular, existe la esterilización automática, pero debes tener especial cuidado con innerHTML.

2️⃣ Política de seguridad de contenido (CSP): La directiva de CSP limita el contenido que la aplicación puede ver o reproducir. Esto reduce las posibilidades de que opere código malicioso.

3️⃣ Codificación de salida: Cuando los datos de usuario se muestren como HTML, asegúrese de que estén codificados para que el código se convierta en texto y no se implemente como código.

4️⃣ Uso de HttpOnly y Cookies Seguras: Las cookies con datos confidenciales, como tokens, son HttpOnly para que no lean JavaScript y Secure para que no realice un seguimiento sin una conexión segura.

5️⃣ Evite JavaScript en línea: Escriba códigos JavaScript en archivos separados para evitar la piratería.

6️⃣ Utilizar herramientas de seguridad en Angular: Como DomSanitizer para mostrar los datos del usuario de forma segura.

7️⃣ Encriptación de datos sensibles: Antes de almacenar datos confidenciales, como tokens o identificadores, en localStorage o sessionStorage, asegúrese de que estén cifrados para que estén seguros incluso si se accede a ellos. En cuanto a los ID o datos que se colocan en la URL, intente cifrarlos para que no se entiendan fácilmente.

8️⃣ Usar firewall de aplicaciones web (WAF): Este firewall escanea las solicitudes de la aplicación y protege contra intentos de ataque y actividades sospechosas.

9️⃣ Bibliotecas de revisión: Cualquier biblioteca externa que utilices se asegura de que sea segura y esté actualizada.

Proteger su aplicación de ataques XSS es esencial para garantizar la seguridad de los datos y la seguridad del usuario. Cada paso del seguro reduce significativamente el riesgo. 🛡️
