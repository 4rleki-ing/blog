---
icon: git
cover: ../.gitbook/assets/Portada (1).jpg
coverY: 27
layout:
  cover:
    visible: true
    size: full
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

# Git

**`Git`** se ha convertido en el estándar mundial para el control de versiones; es un _sistema de control de versiones distribuido_, lo que significa que un clon local del proyecto es un repositorio de control de versiones completo. Estos repositorios locales plenamente funcionales permiten trabajar sin conexión o de forma remota con facilidad. Los desarrolladores confirman su trabajo localmente y, a continuación, sincronizan la copia del repositorio con la del servidor. Este paradigma es distinto del _control de versiones centralizado_, donde los clientes deben sincronizar el código con un servidor antes de crear nuevas versiones.

La comunidad de usuarios de Git ha creado recursos para entrenar a los desarrolladores y la popularidad de Git facilita recibir ayuda cuando se necesita. Casi todos los entornos de desarrollo tienen compatibilidad con Git y las herramientas de línea de comandos de Git implementadas en todos los sistemas operativos principales.

### Aspectos básicos de Git <a href="#aspectos-basicos-de-git" id="aspectos-basicos-de-git"></a>

Cada vez que se guarda el trabajo, Git crea una _confirmación_. Una `confirmación` es una instantanéa de todos los archivos en un momento dado. Si un archivo no ha cambiado de una confirmación a la siguiente, Git usa el archivo almacenado anteriormente. Este diseño difiere de otros sistemas que almacenan una versión inicial de un archivo y mantienen un registro de las diferencias a lo largo del tiempo.

Las confirmaciones crean vínculos a otras confirmaciones, formando un gráfico del historial de desarrollo. Es posible revertir el código a una confirmación anterior, inspeccionar cómo cambian los archivos de una cofirmación a la siguiente y revisar información como dónde y cuándo se realizaron los cambios. Las confirmaciones se identifican en Git mediante un hash criptográfico único del contenido de la confirmación. Dado que todo tiene hash, es imposible realizar cambios, perder la información o dañar los archivos sin que Git lo detecte.

### Ramas <a href="#ramas" id="ramas"></a>

Cada desarrollador guarda los cambios en su propio repositorio de código local. Como resultado, puede haber diversos cambios diferentes basados en la misma confirmación. Git proporciona herramientas para aislar los cambios y volver a combinarlos posteriormente. Las ramas, que son punteros ligeros para el trabajo en curso, administran esta separación. Una vez finalizado el trabajo creado en una rama, se puede combinar de nuevo en la rama principal (o troncal) del equipo.

### Archivos y Confirmaciones <a href="#archivos-y-confirmaciones" id="archivos-y-confirmaciones"></a>

Los archivos de Git se encuentran en uno de los 3 estados:

1. Modificados
2. Almacenados
3. Confirmados

Cuando se modifica un archivo por primera vez, los cambios solo existen en el directorio de trabajo. Todavía no forman parte de una confirmación ni del historial de desarrollo. El desarrollador debe _almacenar provisionalmente_ los archivos modificados que se incluirán en la confirmación. El área de almacenamiento provisional contiene todos los cambios que se incluirán en la siguiente confirmación.

Una vez que el desarrollador esté satisfecho con los archivos almacenados provisionalmente, los archivos se empaquetan como una _confirmación_ con un mensaje que describe lo que ha cambiado. Esta confirmación pasa a formar parte del historial de desarrollo.

El almacenamiento provisional permite a los desarrolladores elegir qué cambios de archivo se guardarán en una confirmación para desglosar los cambios grandes en una serie de confirmaciones más pequeñas. Al reducir el ámbito de las confirmaciones, es más fácil revisar el historial de confirmaciones para buscar cambios de archivo específicos.

### Ventajas de Git <a href="#ventajas-de-git" id="ventajas-de-git"></a>

* <mark style="color:purple;">**`Desarrollo Simultáneo`**</mark>: Todos los usuarios tienen su propia copia local de código y pueden trabajar simultáneamente en sus propias ramas. Git funciona sin conexión, ya que casi todas las operaciones son locales.
* <mark style="color:purple;">**`Versiones de lanzamiento más rápidas`**</mark>: Las ramas permiten un desarrollo flexible y simultáneo. La rama principal contiene código estable y de alta calidad desde el que publica. Las ramas de características contienen trabajo en curso y se combinan con la rama principal tras la finalización. Al separar la rama de versión del desarrollo en curso, es más fácil administrar código estable y enviar actualizaciones más rápidamente.
* <mark style="color:purple;">**`Integración Incorporada`**</mark>: Debido a su popularidad, Git se integra en la mayoría de las herramientas y productos. Todos los IDE principales tienen compatibilidad integrada con Git y muchas herramientas admiten la integración y la implementación continuas, las pruebas automatizadas, el seguimiento de los elementos de trabajo, las métricas y la integración de características de informes con Git. Esta integración simplifica el flujo de trabajo diario.
* <mark style="color:purple;">**`Sólido soporte técnico de la comunidad`**</mark>: Git es de código abierto y se ha convertido en el estándar de facto para el control de versiones. No hay escasez de herramientas y recursos disponibles para que los equipos aprovechen. El volumen de soporte técnico de la comunidad para Git en comparación con otros sistemas de control de versiones facilita recibir ayuda cuando se necesita.
* <mark style="color:purple;">**`Git funciona con cualquier equipo`**</mark>: Utilizar Git con una herramienta de administración de código fuente aumenta la productividad de un equipo al fomentar la colaboración, aplicar directivas, automatizar procesos y mejorar la visibilidad y la rastreabilidad del trabajo. El equipo puede decidirse por herramientas individuales para el control de versiones, el seguimiento de los elementos de trabajo y la integración e implementación continuas. O bien, pueden elegir una solución como [GitHub](https://github.com/) o [Azure DevOps](https://azure.microsoft.com/en-us/products/devops/repos/) que admita todas estas tareas en un solo lugar.
* <mark style="color:purple;">**`Solicitudes de incorporación de cambios`**</mark>: Use [solicitudes de incorporación de cambios](https://learn.microsoft.com/es-es/devops/develop/git/git-pull-requests) para analizar los cambios de código con el equipo antes de combinarlos con la rama principal. Las discusiones en las solicitudes de incorporación de cambios son valiosas para garantizar la calidad del código y aumentar los conocimientos en todo el equipo. Las plataformas _Github_ y _Azure DevOps_ ofrecen una experiencia de solicitud de incorporación de cambios enriquecida en la que los desarrolladores pueden examinar los cambios de archivos, dejar comentarios, inspeccionar confirmaciones, ver compilaciones y votar para aprobar el código.
* <mark style="color:purple;">**`Directivas de rama`**</mark>: Los equipos pueden configurar _GitHub_ y _Azure DevOps_ para aplicar flujos de trabajo y procesos coherentes en todo el equipo. Pueden configurar [directivas de rama](https://learn.microsoft.com/es-es/azure/devops/repos/git/branch-policies?view=azure-devops\&tabs=browser) para asegurarse de que las solicitudes de incorporación de cambios cumplan los requisitos antes de la finalización. Las directivas de rama protegen las ramas importantes al prevenir las inserciones directas, requerir revisores y garantizar compilaciones limpias.

## Instalación y Configuración

Git aún no es una opción predeterminada en los equipos, por lo que debe instalarse y configurarse manualmente. Y, al igual que cualquier otro software, es importante mantenerlo actualizado. Las actualizaciones protegen frente a vulnerabilidades de seguridad, corrige errores y proporcionan acceso a nuevas características.

### Instalar en Windows <a href="#instalar-en-windows" id="instalar-en-windows"></a>

Descargue e instale Git para [Windows](https://git-scm.com/downloads/win). Una vez instalado, Git está disponible desde el _símbolo del sistema_ o _PowerShell_. Se recomienda seleccionar los **valores predeterminados** durante la instalación, a menos que haya una buena razón para cambiarlos.

Git para Windows **no se actualiza** automáticamente. Para actualizar Git en Windows, descargue la nueva versión del instalador, que actualiza Git para Windows en su lugar y conserva toda la configuración.

### Instalar en macOS <a href="#instalar-en-macos" id="instalar-en-macos"></a>

`macOS 10.9 (Mavericks)` y versiones posteriores instala Git la primera vez que intenta ejecutarlo desde la terminal. Aunque este método es una manera fácil de obtener git en un sistema, no permite el control sobre la frecuencia con la que se aplican las actualizaciones o las correcciones de seguridad.

En su lugar , se recomienda instalar Git a tarvés de [Homebrew](https://brew.sh/) y usar las herramientas de _Homebrew_ para mantener Git actualizado. `Homebrew` es una excelente manera de instalar y administrar herramientas de desarrollo de código abierto en un equipo Mac desde la línea de comandos.

Instale **Homebrew** y ejecute lo siguiente para instalar la versión más reciente de Git en un equipo Mac:

```
brew install git
```

Para actualizar la instalación de Git, utilice la opción de actualización de _Homebrew_:

```
brew upgrade git
```

También hay disponible un instalador gráfico para Git en macOS en el [sitio oficial](https://git-scm.com/downloads/mac) de Git.

### Instalar en Linux <a href="#instalar-en-linux" id="instalar-en-linux"></a>

Utilice el sistema de administración de paquetes nativo de la distribución de Linux para instalar y actualizar Git. Por ejemplo, en **Ubuntu**:

```
sudo apt-get install git
```

#### <mark style="color:green;">Configurar Git en Linux</mark> <a href="#configurar-git-en-linux" id="configurar-git-en-linux"></a>

Configure el nombre y la dirección de correo electrónico antes de empezar a trabajar con Git. Git adjunta esta información a los cambios y permite a otros usuarios identificar qué cambios pertenecen a qué autores. Ejecute los siguientes comandos desde la terminal después de instalar Git para configurar esta información:

```
git config --global user.name 4rleki-ing
```

```
git config --global user.email ceo@4rlekiing.net
```

```
git init
```

Visual Studio ofrece una excelente experiencia de Git integrada sin ninguna herramienta adicional. Obtenga más información en este [tutorial](https://learn.microsoft.com/es-es/azure/devops/repos/git/gitworkflow?view=azure-devops) de Git sobre Visual Studio.

### <mark style="color:purple;">Comandos empleados</mark> <a href="#comandos-empleados" id="comandos-empleados"></a>

Muestra la versión de Git instalada

```
git --version
```

Muestra las comandos disponibles

```
git help
```

Brinda ayuda sobre los comandos (manual)

```
git help <comando>
```

Muestra la configuración de Git

```
git config --list
```

Inicia un nuevo repositorio y crea la carpeta oculta .git

<pre><code><strong>git init
</strong></code></pre>

Lista el estado de los archivos

```
git status
```

Agrega todos los archivos pendientes de cambios

```
git add --all
```

```
git add .
```

Captura estado del código y lo almacena en el repositorio local (Posterior a git add \*)

```
git commit -m created file
```

Abre un editor de texto con los cambios del último commit y posibles modificaciones y realizar un commit reemplazando al último

```
git commit --amend
```

#### <mark style="color:green;">Tags</mark> <a href="#tags" id="tags"></a>

Crea un tag

```
git tag <name_tag> -m "Release x.y.z"
```

Lista tags

```
git tag
```

Borra un tag en específico

```
git tag -d <name_tag>
```

Hace un tag en un commit anterior

```
git tag -a <name_tag> <código> -m "Released x.y.z"
```

Mostrar información del tag

```
git show <name_tag>
```

Deshace la captura del estado del código

```
git reset
```

#### <mark style="color:green;">Commits</mark> <a href="#commits" id="commits"></a>

Cambiamos a un commit en específico perdiendo todos los cambios posterior a este

```
git reset --hard <código>
```

Muestra los commit realizados hasta el momento

```
git log --oneline
```

Lista todos los commits de todas las ramas de forma gráfica tomando como base la rama actual

```
git log --oneline --graph --all
```

Cambia a un commit en específico con todos sus cambios

```
git checkout <código>
```

Muestra los cambios de 2 commits

```
git diff <código> <código>
```

#### <mark style="color:green;">Ramas</mark> <a href="#ramas-1" id="ramas-1"></a>

Crea una nueva rama

```
git branch <name_rama>
```

Nos muestra en que rama estamos y lista las demás

```
git branch
```

Nos movemos de la rama actual a una específica

```
git checkout <name_rama>
```

Crea y nos movemos a la nueva rama

```
git checkout -b <name_rama>
```

Renombra la rama actual

```
git branch -m <nuevo_name>
```

Elimina una rama

```
git branch -d <name_rama>
```

Permite juntar 2 ramas. Trae los cambios de la rama especificada a la rama actual

```
git merge <name_rama>
```

Permite juntar 2 ramas, pero las mantiene. Genera un commit del merge en la rama actual

```
git merge --no-ff develop
```

Permite traer los commits de otra rama a la rama actual reorganizan los commits

```
git rebase main
```

#### <mark style="color:green;">Repositorio Remoto</mark> <a href="#repositorio-remoto" id="repositorio-remoto"></a>

&#x20;    Para subir nuestro proyecto debemos crear un repositorio remoto. Al crearlo nos mostrará una serie de comandos para subir el proyecto. Te pedirá un usuario y contraseña de tu cuenta de git si aún no lo registras.

* Vincular repositorio remoto con repositorio local

```
git remote add origin https://github.com/4rleki-ing/AprendizajeGit.git
```

* Cambiar URL del repositorio remoto

```
git remote set-url origin https://github.com/4rleki-ing/AprendizajeGit.git
```

* Nos muestra en que repositorio estamos enlazados remotamente

```
git remote -v
```

* Sube los cambios del repositorio local al remoto y especifica la rama principal

```
git push -u origin <name_rama>
```

* Eliminar una rama remota

```
git push origin --delete <name_rama>
```

* Sube todos los tags locales al remoto

```
git push --tags
```

* Elimina un tag remoto

```
git tag -d <name_tag>
git push origin :refs/tags/<name_tag>
```

* Descarga los cambios del repositorio remoto y actualiza el local en la rama por defecto

```
git pull
```

* Descarga los cambios del repositorio remoto actualiza el local en una rama específica

```
git pull origin <name_rama>
```

* Clona un repositorio remoto en la rama por defecto

```
git clone https://github.com/4rleki-ing/AprendizajeGit.git
```

* Clona un repositorio remoto en una rama específica

```
git clone --branch <name_rama> https://github.com/4rleki-ing/AprendizajeGit.git
```
