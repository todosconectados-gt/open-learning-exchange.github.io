# Creación de tu Página de Perfil en GitHub: Una Guía de Markdown y el Flujo de Trabajo de Forking

## 1. Objetivos

- Aprender sobre GitHub y Markdown
- Crear tu propia página de perfil en Markdown
- Entender el flujo de trabajo de Forking en GitHub (incluyendo forks, repositorios, commits y pull requests)

## 2. Preparación

Antes de profundizar en GitHub, Markdown y el flujo de trabajo de forking, es crucial entender las herramientas y recursos esenciales involucrados en este tutorial:

- [Markdown](https://es.wikipedia.org/wiki/Markdown) – un lenguaje de marcado ligero con sintaxis de formato de texto plano.
- [GitHub](https://docs.github.com/en) – una plataforma para alojar código, control de versiones y colaboración.
- [MDwiki](http://dynalon.github.io/mdwiki/#!quickstart.md) – un sistema de gestión de contenido que aprovecha Markdown. El sitio que estás leyendo está construido con MDwiki.
- [Flujo de Trabajo de Forking](https://www.atlassian.com/git/tutorials/comparing-workflows/forking-workflow) - Este es el flujo de trabajo que utilizarás durante la fase de Primeros Pasos, ya que aún no tendrás acceso directo a nuestros repositorios. Este tutorial se centrará exclusivamente en utilizar este flujo de trabajo en GitHub.com para mantener las cosas simples. Exploraremos el trabajo con Git en la línea de comandos con más profundidad más adelante.

**NOTA**: A lo largo de estos pasos, se utilizarán `<>` para marcar las áreas donde debes insertar tu propia información. No incluyas los corchetes en sí.

### 2.1 Introducción a Markdown

1. Revisa [Getting Started | Markdown Guide](https://www.markdownguide.org/getting-started/) para una visión general de Markdown, cómo funciona y qué puedes hacer con él.
2. Recorre [Basic Syntax | Markdown Guide](https://www.markdownguide.org/basic-syntax/) para aprender la sintaxis fundamental.
3. Completa [este tutorial interactivo de Markdown](https://tylingsoft.github.io/tutorial.md/#whats-markdown) para obtener experiencia práctica.

### 2.2 Introducción a GitHub

Asegúrate de estar conectado a GitHub con tus credenciales de cuenta. Si no estás familiarizado con la interfaz y funcionalidades de GitHub, visita [nuestro repositorio](https://github.com/todosconectados-gt/todosconectados-gt.github.io) para explorar.

**NOTA**: Confirma que tu dirección de correo electrónico para commits en GitHub está configurada correctamente. Para pasos detallados, consulta [Configuración de tu dirección de correo electrónico para commits en GitHub - GitHub Doc](https://docs.github.com/en/account-and-profile/setting-up-and-managing-your-personal-account-on-github/managing-email-preferences/setting-your-commit-email-address#setting-your-commit-email-address-on-github).

### 2.3 Introducción al Flujo de Trabajo de Forking

El [flujo de trabajo de forking](https://www.atlassian.com/git/tutorials/comparing-workflows/forking-workflow) es un enfoque colaborativo para el desarrollo de software, comúnmente utilizado en proyectos de código abierto. Permite a los desarrolladores contribuir a un proyecto sin requerir acceso directo al repositorio original. Así es como funciona:

- **Forking**: Aquí es donde creas una copia de un repositorio de proyecto existente en tu propia cuenta de GitHub. Es como duplicar un libro para poder hacer anotaciones sin alterar el original.
- **Cambios Independientes**: En tu repositorio forked, tienes la libertad de explorar, experimentar y hacer cambios. Puedes crear nuevas características, corregir errores o mejorar la documentación.
- **Pull Requests**: Una vez que estés satisfecho con tus cambios, puedes proponerlos al proyecto original creando un pull request. Esto es una solicitud para que los mantenedores del proyecto revisen y posiblemente fusionen tus cambios en su base de código.

## 3. Añade tu Propia Página de Perfil en Markdown con el Flujo de Trabajo de Forking en github.com

A continuación se muestra un resumen de los pasos que te guiaremos:

1. [Encuentra y haz fork del repositorio correcto](#3.1_Encuentra_y_haz_fork_del_repositorio_correcto)
2. [Ve a Configuración y renombra tu repositorio](#3.2_Ve_a_Configuración_y_renombra_tu_repositorio)
3. [Comprueba si tu sitio github.io funciona](#3.3_Comprueba_si_tu_sitio_github.io_funciona)
4. [Crea un nuevo archivo como tu página personal de MDwiki y realiza tus commits](#3.4_Crea_un_nuevo_archivo_como_tu_página_personal_de_MDwiki_y_realiza_tus_commits)
5. [Abre un pull request y elimina tu rama después de que se fusione](#3.5_Abre_un_pull_request_y_elimina_tu_rama_despues_de_que_se_fusione)

### 3.1 Encuentra y haz fork del repositorio correcto

Forking crea una copia personal de un repositorio en tu cuenta de GitHub, permitiéndote hacer cambios sin afectar el repositorio original.

Para hacer fork del repositorio correcto, sigue estos pasos:

1. Visita el [repositorio github.io de todosconectados-gt](https://github.com/todosconectados-gt/todosconectados-gt.github.io).
2. Haz clic en el botón "Fork" en la esquina superior derecha. Si no puedes encontrarlo, consulta [Forking un repositorio - GitHub Docs](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/working-with-forks/fork-a-repo#forking-a-repository).

**NOTA**: Hasta que te conviertas en un intern virtual oficial, siempre haz fork del repositorio antes de hacer cambios. Realiza tus commits en tu versión forked y envía pull requests para contribuir de vuelta al repositorio de OLE. El repositorio principal se actualizará una vez que se aprueben tus pull requests.

### 3.2 Ve a Configuración y renombra tu repositorio

Después de hacer fork del repositorio, serás redirigido a tu copia personal del repositorio: **&lt;TuNombreDeUsuario&gt;/todosconectados-gt.github.io**. Para renombrar este repositorio y crear tu sitio de GitHub Pages:

1. Haz clic en Configuración en la parte superior de la página del repositorio.
2. En el campo de nombre del repositorio, cámbialo a `<TuNombreDeUsuario>.github.io`.
3. Haz clic en **Renombrar** para confirmar el cambio.

**Nota:** Si ya tienes un sitio de GitHub Pages en uso en https://&lt;TuNombreDeUsuario&gt;.github.io, consulta [esta pregunta frecuente](#!pages/mi/mi-faq.md#Q17:_What_do_I_do_if_I_already_have_a_github.io_with_my_username?) para obtener orientación.

![Renombrar Repositorio](image/mi-rename-repository.png)

### 3.3 Comprueba si tu sitio github.io funciona

Después de renombrar tu repositorio, visita `https://<TuNombreDeUsuario>.github.io` para verificar si tu sitio está activo.

Si ves un error "404 Page Not Found", no te preocupes. Puede que tarde un tiempo en que tu sitio de GitHub Pages se construya y se vuelva accesible. Para asegurarte de que esté configurado correctamente, ve a **Configuración > Pages** del repositorio y confirma que la **Fuente** esté configurada en "Deploy from a branch" y `todos` `/(root)` estén seleccionados bajo **Branch**.

### 3.4 Crea un nuevo archivo como tu página personal de MDwiki y realiza tus commits

Antes de editar, asegúrate de que estás trabajando en tu propio repositorio de GitHub. Verifica que el nombre del repositorio incluya tu **nombre de usuario** de GitHub. Por ejemplo, debería verse como `<TuNombreDeUsuario>/<TuNombreDeUsuario>.github.io`.

#### 3.4.1 Crea una nueva rama

1. **Cambia a la Rama todos**: Haz clic en el selector de ramas en la esquina superior izquierda de tu repositorio. Si no dice "**todos**", cambia a la rama todos.
2. **Nombra la Nueva Rama**: Haz clic en el selector de ramas nuevamente, luego escribe un nombre descriptivo como `add-<TuNombreDeUsuario>-profile`. Para mejores prácticas en nombramiento de ramas, consulta esta [guía](https://github.com/agis/git-style-guide#branches).
3. **Confirma la Creación de la Nueva Rama**: Haz clic en "Crear rama **add-&lt;TuNombreDeUsuario&gt;-profile** desde **todos**." Ahora deberías ver "**add-&lt;TuNombreDeUsuario&gt;-profile**" como tu rama actual.

  ![Nueva Rama](image/mi-new-branch.png)

#### 3.4.2 Crea tu archivo de perfil en Markdown

Para crear tu archivo de perfil, sigue estos pasos:

1. Navega a la carpeta `pages/mi/profiles/` desde la página principal de tu repositorio forked.
2. Asegúrate de que aún estás en la rama que acabas de crear, busca "**add-&lt;TuNombreDeUsuario&gt;-profile**" en el menú del selector de ramas.
de ramas.
3. Arriba de la lista de archivos, selecciona el menú desplegable "Add file" y luego haz clic en "Create new file".
4. Nombra el archivo usando `<TuNombreDeUsuario>` con la extensión `.md` (por ejemplo, `JohnDoe.md`). Esto asegura que tu perfil sea fácil de encontrar.

En este nuevo archivo Markdown, incluye la siguiente información usando un mínimo de 5 elementos de Markdown:

- Tu nombre, ubicación/zona horaria y sistema operativo (con versión)
- Una breve descripción de ti mismo para que otros puedan conocerte.

Usa la pestaña "Preview" para ver preliminarmente cómo se verá tu Markdown. Trata de usar al menos cinco tipos diferentes de elementos de Markdown para la variedad. Evita el HTML, ya que el propósito de Markdown es mantener las cosas simples. Considera ejemplos creativos, como:

- [Perfil 1](profiles/Okuro3499.md) (usando tabla y listas)
- [Perfil 2](profiles/rlam20.md) (usando encabezados, emojis, tabla y lista)

Cuando estés listo, haz clic en el botón "Commit changes...". Si necesitas editar tu archivo de nuevo, haz clic en el icono del lápiz.

Para previsualizar tus cambios renderizados por MDwiki, usa el siguiente enlace, reemplazando `<TuNombreDeUsuario>` con tu **nombre de usuario** de GitHub y `<TuNombreDeRama>` con el nombre de tu rama:

`https://raw.githack.com/<TuNombreDeUsuario>/<TuNombreDeUsuario>.github.io/<TuNombreDeRama>/#!pages/mi/profiles/<TuNombreDeUsuario>.md`

Antes de proceder a la siguiente sección, por favor:

- asegúrate de que todo se vea como esperas y funcione correctamente con el enlace de raw.githack.
- verifica que usaste al menos **5 elementos diferentes** de Markdown en tu perfil
  - Para usar emojis en tu perfil, copia el emoji directamente (por ejemplo, '🐱' en lugar de ':emojicode:'). Puedes encontrar y copiar emojis de [emojipedia](https://emojipedia.org/).
  - Las listas de tareas son compatibles en GitHub pero no en MDwiki. Pueden verse correctas en GitHub pero no en MDwiki.

**NOTA**:
- Los nuevos cambios que empujes deberían reflejarse en minutos en raw.githack. Si los cambios aún no aparecen, limpia el caché de tu navegador o abre tu página en modo "incógnito" o "privado". También puedes forzar la actualización/recarga de la página usando `Ctrl+Shift+R` o `Ctrl+F5` (en Mac: `Cmd+Shift+R`).
- Recuerda que hay [diferentes sabores de Markdown](https://github.com/commonmark/CommonMark/wiki/Markdown-Flavors). Dado que el sitio MDwiki se usa para "producción", siempre verifica si tu contenido se renderiza correctamente en el enlace de raw.githack. Usa la pestaña de vista previa de GitHub como guía, pero confía en raw.githack para la precisión.

### 3.5 Abre un pull request y elimina tu rama después de que se fusione

Una vez que tengas tu perfil listo, es hora de crear un pull request. Sigue las instrucciones en [Tutorial de Crear un Pull Request y Eliminar una Rama](mi-github-pull-request.md).

Después de crear el pull request, publica el enlace a tu GitHub Pages y al pull request de tu perfil en el [canal de discord del intern móvil](https://discord.gg/mtgGD4EnYW):

> Estoy en el paso 1, por favor revisa `https://<TuNombreDeUsuario>.github.io` y revisa mi pull request de perfil `LinkToYourPullRequest`

Recuerda, puede tardar un tiempo en que `https://<TuNombreDeUsuario>.github.io` esté en funcionamiento, ¡así que no te preocupes si ves un **404** cuando accedas al enlace!

Después de recibir suficientes revisiones aprobatorias, fusionaremos tu perfil de Markdown en el repositorio principal.

Después de que el pull request se fusione, podrás ver tu página personal en `todosconectados-gt.github.io/#!pages/mi/profiles/<TuNombreDeUsuario>.md`. Avísanos en el [canal del intern móvil de discord](https://discord.gg/mtgGD4EnYW) después de completar este paso.

## 4. Enlaces Útiles

- [Sintaxis básica de escritura y formato - GitHub Docs](https://guides.github.com/features/mastering-markdown/)
- [MDWiki – Inicio Rápido](http://dynalon.github.io/mdwiki/#!quickstart.md) - La guía oficial de inicio rápido de MDwiki sobre la sintaxis de Markdown.
- [Hacer fork de un repositorio - GitHub Docs](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/working-with-forks/fork-a-repo) - Una explicación más detallada sobre cómo y por qué hacemos fork de repositorios.
- [Gestión de archivos - GitHub Docs](https://docs.github.com/en/repositories/working-with-files/managing-files)

[Otros enlaces y videos útiles](../vi/vi-faq.md#Helpful_Links)

#### Volver a [Primeros Pasos](mi-10-steps.md#Step_1_-_Markdown_&_Forking_Workflow)
