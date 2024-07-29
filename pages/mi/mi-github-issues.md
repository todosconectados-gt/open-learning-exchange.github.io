# Tutorial de Issues en GitHub

## 1. Objetivos

- Aprender sobre Issues, Commits y Pull Requests en GitHub
- Entender el flujo de trabajo colaborativo de git/GitHub utilizado durante la pasantía
- Crear un Issue sobre los Primeros Pasos para Internos Móviles, luego crear una rama para solucionarlo tras su aprobación
- Después de resolver el Issue, hacer un Pull Request al repositorio `open-learning-exchange/open-learning-exchange.github.io`
- Trabajar con nosotros para realizar los cambios necesarios, luego fusionar la rama en el repositorio principal
- Comentar en un Issue existente

## 2. Introducción

Los repositorios de GitHub tienen una sección para Issues, donde los problemas pueden ser categorizados, discutidos y solucionados. Los Issues suelen ser abiertos por los miembros de nuestro equipo para crear nuevas funciones o solucionar errores en nuestros proyectos. Este tutorial te guiará a través del proceso de creación de Issues, creación de ramas, realización de Pull Requests y colaboración con los miembros del equipo.

Te animamos a que presentes tantos issues como sea posible, ya sean grandes o pequeños. Si detectas un problema pero no sabes cómo solucionarlo, presenta un issue para que otros estén al tanto y puedan trabajar en una solución. Intenta agregar el mayor valor posible con tus issues, ya que esto ayuda a apoyar a la comunidad y mejora la calidad general de este sitio MDwiki.

NOTA: Los Issues no solo se tratan de agregar nuevo contenido o mejorar este MDwiki; también pueden implicar la eliminación de material redundante o innecesario. El objetivo es mantener la documentación clara y concisa. Si encuentras secciones que podrían simplificarse o reducirse, siéntete libre de crear un issue para ayudar a agilizar el proceso.

## 3. Crear un Issue

Si has notado un área que podría mejorarse en los Primeros Pasos para Pasantes Móviles, abordémoslo. Si no, por favor, revisa para encontrar un problema. Comienza por revisar [tanto los problemas abiertos como los cerrados existentes](https://github.com/todosconectados-gt/todosconectados-gt.github.io/issues?q=is%3Aissue), para asegurarte de que no se haya planteado o solucionado antes. Si no se ha planteado, vamos a crear un nuevo problema:

- Ve a la [pestaña de Issues del repositorio principal](https://github.com/todosconectados-gt/todosconectados-gt.github.io/issues) y selecciona "New Issue". Selecciona el botón "Get started" junto a "First Steps - Mobile Virtual Intern."
    1. Elabora un título conciso y descriptivo.
    2. Completa el template del issue de manera exhaustiva, marcando todas las casillas requeridas y proporcionando los detalles necesarios.
    3. Comparte un enlace a este issue en nuestro canal de Discord.
- Puedes consultar [este ejemplo](https://github.com/open-learning-exchange/open-learning-exchange.github.io/issues/3300) para ver cómo un issue sigue el template con una estructura clara.
- Una vez enviado, otros pueden proporcionar comentarios para guiar los próximos pasos.

**Nota**: Aunque crear un Pull Request no requiere aprobación previa, es mejor esperar la confirmación del issue por parte de nuestro equipo antes de trabajar en una solución. Si los cambios sugeridos no se alinean con los objetivos del proyecto, tu Pull Request puede no ser fusionado y tu trabajo no contará para el progreso de los "Primeros Pasos". Al buscar aprobación primero, puedes evitar esfuerzos y retrabajos innecesarios.

**Issues existentes:** También puedes trabajar en issues existentes. Si un issue está etiquetado como `mi` y `first step intern`, puedes solicitar trabajar en él enviándonos un mensaje en Discord. Si alguien más ya está asignado o ha expresado su intención de trabajar en él en la sección de comentarios del issue, no trabajes en ese issue; elige otro en su lugar.

_**Nota Especial**_:
- Los internos a menudo se apresuran en este proceso para completar sus "Primeros Pasos". Recuerda que estos pasos tienen como objetivo solucionar problemas reales y mejorar el flujo de trabajo. Tómate el tiempo para examinar los materiales de "Primeros Pasos" para encontrar problemas reales y investigar las mejores soluciones. También, asegúrate de que el issue no haya sido identificado ya.

## 4. Sincroniza Tu Repositorio

Antes de crear tu rama, sincroniza tu repositorio con los siguientes comandos (como te guiamos en el paso anterior):

1. Obtén los últimos cambios del repositorio principal:

   ```sh
   git fetch upstream
   ```

2. Cambia a tu rama `todos`:

   ```sh
   git checkout todos
   ```

3. Fusiona los cambios obtenidos de la rama `todos` del repositorio principal en tu rama `todos` local:

   ```sh
   git merge upstream/todos
   ```

4. Empuja la rama `todos` actualizada a tu repositorio bifurcado en GitHub:

   ```sh
   git push origin todos
   ```

**ATENCIÓN**: De ahora en adelante, para el resto de los Primeros Pasos, por favor usa la línea de comandos para crear ramas y hacer commits en lugar de usar la interfaz web de GitHub. Esto te dará práctica valiosa con comandos comunes de Git en tu terminal, lo cual es esencial para trabajar en código real que necesita ser probado localmente y no siempre puede ser editado directamente en GitHub.com.

## 5. Crear una Nueva Rama

**Cada vez que empieces a trabajar en un issue, necesitas crear una rama para mantener separados los issues en los que estás trabajando.** Asegúrate de usar un nombre descriptivo para tu rama de la siguiente manera: **issueNumber-nombre-descriptivo-de-la-rama**.

- Para crear y cambiar a una nueva rama desde `todos`, ejecuta los siguientes comandos:

  ```sh
  git checkout todos  # Asegúrate de estar en la rama todos
  git checkout -b <issueNumber-nombre-descriptivo-de-la-rama>
  ```

  Asegúrate de reemplazar `<issueNumber-nombre-descriptivo-de-la-rama>` con el nombre real de tu rama, sin los signos de menor (`<`) y mayor (`>`).

Más documentación sobre `git checkout` se puede encontrar [aquí](https://git-scm.com/docs/git-checkout).

Ahora puedes ir y hacer los cambios propuestos en tus archivos locales usando cualquier editor de texto que prefieras. También puedes usar VIM o Nano para editar archivos desde la terminal. [Esta guía sobre VIM](https://www.vim.org/docs.php) y [esta guía sobre Nano](https://www.nano-editor.org/docs.php) contienen más información sobre su uso adecuado. En el futuro, te recomendamos usar [Visual Studio Code](https://code.visualstudio.com/) para Planet, VIM para treehouse, y [Android Studio](https://developer.android.com/studio) para el desarrollo de Android.

NOTA: Usa `git branch` para ver en qué rama estás. Tu rama `todos` es la rama base de trabajo. Debe permanecer intacta por si necesitas revertir algunos cambios a una versión funcional. Asegúrate de estar en la rama correcta usando `git checkout <nombre-de-la-rama>` mientras haces los cambios propuestos en tus archivos locales y mientras haces commits.

Si todavía estás confundido, está bien. [Forking Workflow](https://www.atlassian.com/git/tutorials/comparing-workflows/forking-workflow) puede ser bastante desafiante al principio. Consulta el diagrama a continuación. Para un mejor contexto, la nueva rama que acabas de crear está dentro de tu "Forked GitHub IO".

![Diagrama del flujo del repositorio en GitHub](image/mi-repo-flowchart.png)

### 5.1. Vista Previa de Cambios Locales

Después de hacer modificaciones en tus archivos locales y antes de hacer un commit, es posible que quieras previsualizar los cambios localmente. Para configurar rápidamente un servidor HTTP local, puedes seguir [la guía de MDwiki aquí](https://dynalon.github.io/mdwiki/#!./faq.md#Q:_I_don't_want_to_install_nginx_or_apache_locally._What_is_the_fastest/easiest_way_to_setup_a_local_HTTP_server_to_get_started_with_MDwiki_?). Sin embargo, en lugar de usar el método obsoleto de Python mencionado en la guía, puedes usar el siguiente comando: `python3 -m http.server 8080`.

## 6. Crear un Commit y Empujar los Cambios

**NOTA**: Antes de hacer tu commit, configura la dirección de correo electrónico que asocias con tus commits de Git siguiendo las instrucciones en [Configurar tu dirección de correo electrónico en Git - GitHub Docs](https://docs.github.com/en/account-and-profile/setting-up-and-managing-your-personal-account-on-github/managing-email-preferences/setting-your-commit-email-address#setting-your-commit-email-address-in-git).

Usa los siguientes comandos para hacer commit y empujar tus cambios:

1. Verifica qué archivos en el directorio de trabajo han sido modificados:

   ```sh
   git status
   ```

2. Muestra los cambios en los archivos:
   - Para mostrar los cambios en archivos específicos:

     ```sh
     git diff <archivo1> <archivo2> <archivo3>...
     ```

   - Para mostrar todos los cambios en los archivos:

     ```sh
     git diff

     ```

   Verifica los cambios que has hecho, luego procede al siguiente paso.Claro, aquí está la continuación:

```
   Para entender la salida de `git diff`, consulta [Git Diff | Tutorial de Atlassian Git](https://www.atlassian.com/git/tutorials/saving-changes/git-diff).

3. Prepara los archivos modificados:
   - Para preparar archivos modificados específicos:

     ```sh
     git add <archivo1> <archivo2> <archivo3>...
     ```

   - Para preparar **todos** los archivos modificados que aparecen en `git status`:
     - **Precaución:** Antes de usar esto, revisa los archivos modificados listados en el paso anterior para asegurarte de no estar preparando cambios no deseados.

     ```sh
     git add .
     ```

4. Haz commit de los cambios preparados con un mensaje descriptivo:

   ```sh
   git commit -m "<tu_mensaje_de_commit>"
   ```

   (Consulta las directrices para mensajes de commit más abajo).

5. Empuja los cambios a tu nueva rama en GitHub:

   ```sh
   git push -u origin <issueNumber-nombre-descriptivo-de-la-rama>
   ```

   Para cualquier commit adicional en la misma rama después del primero, simplemente usa:

   ```sh
   git push
   ```

**SUGERENCIA**: Si sientes que has cometido algún error con los comandos de Git, consulta [Dangit, Git!?](https://dangitgit.com/) para errores comunes y sus soluciones.

### 6.1. Guía de Estilo para Mensajes de Commit

Dado que los commits que harás en este wiki markdown son bastante básicos, no es necesario imponer un estilo de commit detallado. Sin embargo, en el futuro, cuando empieces a trabajar en proyectos más complejos, es útil escribir tus mensajes de commit de una manera determinada. Aquí hay un artículo sobre [cómo escribir buenos mensajes de commit](https://chris.beams.io/posts/git-commit/).

Para ediciones en este wiki markdown, recomendamos que tus mensajes de commit consistan solo en la línea de asunto (consulta el artículo para más detalles sobre el asunto).

- Limita la línea de asunto a 50 caracteres
- No termines la línea de asunto con un punto
- Usa el modo imperativo en la línea de asunto

Aquí tienes un ejemplo de cómo escribir tu mensaje de commit:
`$ git commit -m "agregar guía de estilo para mensajes de commit y añadir sección raw.githack (soluciona #841)"`

**SUGERENCIA**: En tu mensaje de commit, si agregas una palabra clave como "fixes" o "resolves" seguida de "#" y el número del issue, una vez que tu pull request sea fusionado, el issue se cerrará automáticamente. Esto es útil porque ayuda a limpiar la sección de issues. Consulta más [aquí](https://help.github.com/articles/closing-issues-using-keywords/).

### 6.2. Raw.githack

Raw.githack es un aspecto importante del proceso de pull request. Después de que hagas commits en tu rama local y los empujes a tu rama remota, puedes ver estos cambios yendo a `https://raw.githack.com/<TuUsuario>/<TuUsuario>.github.io/<TuNombreDeRama>/index.html#!pages/mi/mi-10-steps.md` y navegando a la(s) página(s) que has cambiado. Si todo parece correcto, estás listo para crear un pull request.

Por ejemplo, [https://raw.githack.com/xyb994/xyb994.github.io/add-xyb994-profile/index.html#!pages/mi/mi-10-steps.md](https://raw.githack.com/xyb994/xyb994.github.io/add-xyb994-profile/index.html#!pages/mi/mi-10-steps.md) llevará a la página principal de Primeros Pasos – Interno Virtual Móvil:

![Página principal de los Primeros Pasos con enlace raw.githack](image/mi-raw-githack-first-steps-main-page.png)

Raw.githack facilita ver cómo se verá la página si tu rama se fusiona, así que no olvides incluir un enlace raw.githack en tu próximo paso, el pull request.

## 7. Crear un Pull Request y Eliminar tu Rama Después de Fusionar

Ahora sigue las instrucciones en [Tutorial de Creación de un Pull Request y Eliminación de una Rama](mi-github-pull-request.md) para crear tu pull request.

Ten en cuenta que un miembro del personal puede solicitar una revisión de código pidiéndote que modifiques algunos de tus cambios, o aceptar el pull request y cerrar el issue.

NOTA: Recuerda siempre sincronizar tu fork antes de comenzar a trabajar en un nuevo issue. Para sincronizar tu fork, puedes seguir el proceso en el [paso anterior](mi-github-and-repositories.md#Resumen_de_Pasos).

Este es un ejercicio para ayudarte a familiarizarte con los issues en GitHub, hacer commits y crear pull requests. Este es un proceso común en grandes proyectos de código abierto, ya que siempre hay margen para mejorar. Por lo tanto, te animamos a seguir este proceso y continuar publicando issues y resolviéndolos.

## 8. Comentar en un Issue Existente

Necesitarás hacer **al menos un comentario** en un issue que **no** hayas creado.

- Navega a la [pestaña de Issues del repositorio todosconectados-gt/todosconectados-gt.github.io](https://github.com/todosconectados-gt/todosconectados-gt.github.io/issues).
- Revisa algunos issues recientes y deja un comentario en aquellos donde puedas proporcionar *comentarios significativos y útiles*.
- En "Add a comment", escribe tu comentario con la sintaxis Markdown si es necesario, haz clic en la pestaña "Preview" para revisar y haz clic en el botón "Comment".

## 9. Enlaces Útiles

- [Guía Rápida para Issues en GitHub | GitHub Docs](https://docs.github.com/en/issues/tracking-your-work-with-issues/quickstart)
- [FAQ - Enlaces y Videos Útiles](mi-faq.md#Helpful_Links)
- [Cómo Contribuir al Código Abierto](https://opensource.guide/how-to-contribute/)

#### Regresar a [Primeros Pasos](mi-10-steps.md#Paso_6_-_Tutorial_de_Issues_en_GitHub)
