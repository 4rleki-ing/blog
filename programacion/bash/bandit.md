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

# Bandit

El juego de guerra Bandit está dirigido a principiantes absolutos. Enseñará los conceptos básicos necesarios para poder jugar a otros juegos de guerra. Si notas que falta algo esencial o tienes ideas para nuevos niveles, ¡háznoslo saber!

### <mark style="color:purple;">Nota para principiantes</mark>

Este juego, como la mayoría de los demás, está organizado en niveles. Comienzas en el **`nivel 0`** e intentas "superarlo" o "terminarlo". Al finalizar un nivel, obtienes información sobre cómo comenzar el siguiente nivel. Las páginas de este sitio web para el "_**Nivel X**_ " contienen información sobre cómo comenzar el nivel X desde el nivel anterior.&#x20;

{% hint style="info" %}
Por ejemplo:&#x20;



La página del Nivel 1 tiene información sobre cómo acceder del Nivel 0 al Nivel 1.
{% endhint %}

Todos los niveles de este juego tienen una página en este sitio web y todos están vinculados desde el menú lateral a la izquierda de esta página.

Te encontrarás con muchas situaciones en las que no tendrás idea de lo que se supone que debes hacer. ¡No te asustes! ¡No te rindas! El objetivo de este juego es que aprendas los conceptos básicos. Parte de aprender los conceptos básicos es leer mucha información nueva. Si nunca ha usado la línea de comandos antes, una buena primera lectura es esta introducción a los comandos de usuario.

Hay varias cosas que puede intentar cuando no esté seguro de cómo continuar:

1. **`Primero`**, si conoce un comando, pero no sabe cómo usarlo, pruebe el manual (página man) ingresando <mark style="color:yellow;">**`man comando`**</mark>. Por ejemplo, <mark style="color:yellow;">**`man ls`**</mark> para aprender sobre el comando “**`ls`**”. El comando “**`man`**” también tiene un manual, ¡pruébelo! Cuando use man, presione <mark style="color:yellow;">**`q`**</mark> para salir (también puede usar <mark style="color:yellow;">`/`</mark> y <mark style="color:yellow;">**`n`**</mark> y <mark style="color:yellow;">**`N`**</mark> para buscar).
2. **`Segundo`**, si no hay una página **man**, el comando puede ser un comando incorporado del shell. En ese caso, use el comando “<mark style="color:yellow;">**`help`**</mark> ”. Por ejemplo, <mark style="color:yellow;">**`help cd`**</mark>&#x20;
3. Además, su motor de búsqueda favorito es su amigo. ¡Aprenda a usarlo! Recomiendo Google.
4. Por último, si aún no sabe cómo usarlo, puede unirse a nosotros a través del chat

¡Está listo para comenzar! Comience con el nivel 0, cuyo vínculo se encuentra a la izquierda de esta página. ¡Buena suerte!

<mark style="color:yellow;">**`Nota para las máquinas virtuales`**</mark>: es posible que no pueda conectarse a _**overthewire.org**_ a través de SSH con un “error de tubería rota” cuando el adaptador de red de la máquina virtual esté configurado para usar el modo NAT. Agregar la configuración de rendimiento IPQoS **`/etc/ssh/ssh_config`** debería resolver el problema. Si esto no resuelve el problema, la única opción es cambiar el adaptador al modo Bridged.
