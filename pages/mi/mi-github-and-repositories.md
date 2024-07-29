# Repositorios Git: Una Guía para Clonar, Configurar y Sincronizar Forks

## Objetivos

- Aprender a **usar Git desde la línea de comandos**
- Comprender cómo configurar y sincronizar un repositorio con el flujo de trabajo de fork

## Introducción

En GitHub, el código de software se organiza en repositorios, cada uno representando un proyecto diferente. Por ejemplo, has estado trabajando en uno de nuestros repositorios, **todosconectados-gt.github.io**. Te animamos a explorar nuestros otros repositorios en GitHub [aquí](https://github.com/open-learning-exchange), pero recuerda: **mira, no toques**. Si eres nuevo en Git o GitHub, echa un vistazo a [esta introducción](https://www.freecodecamp.org/news/introduction-to-git-and-github/).

Como se mencionó anteriormente, en el [flujo de trabajo de fork](mi-github-and-markdown.md#2.3_Introduction_to_Forking_Workflow), haces un fork de un repositorio para trabajar en él de manera independiente del repositorio principal, y luego envías tus cambios de vuelta al repositorio original mediante una solicitud de extracción (pull request). Completaste este proceso en github.com en el Paso 1. En este paso, profundizaremos y utilizaremos la línea de comandos para sincronizar tu repositorio fork con el repositorio principal de OLE.

El diagrama a continuación muestra la estructura del flujo de trabajo de fork para todosconectados-gt.github.io, con un repositorio principal central, forks individuales y copias locales en tu máquina.

![Relación de Repositorios](image/mi-repo-diagram.png)

## Términos Importantes

En este paso, encontrarás algunos términos comunes, como:

- `master`/`main`: nombre de la rama por defecto de un repositorio
- `upstream`: el repositorio del que hiciste el fork
- `origin`: tu propio fork del repositorio upstream
Tanto `upstream` como `origin` se consideran **[remotos](https://git-scm.com/docs/git-remote)**. Además, recuerda que un repositorio puede contener múltiples ramas.

## 1. Clonar Tu Repositorio de GitHub

Tanto las URLs HTTPS como SSH te permiten acceder a los mismos repositorios remotos, pero utilizan diferentes protocolos. Puedes elegir cualquiera según tu preferencia:

- **HTTPS:** Más fácil de configurar para principiantes, no requiere claves SSH.
- **SSH:** Más seguro, requiere que tengas claves SSH configuradas en tu máquina y añadidas a tu cuenta de GitHub.

Para más detalles, consulta [Clonando un repositorio | GitHub Docs](https://docs.github.com/en/repositories/creating-and-managing-repositories/cloning-a-repository).

#### Para clonar con SSH

1. [Verifica que tienes claves SSH existentes en tu máquina](https://docs.github.com/en/authentication/connecting-to-github-with-ssh/checking-for-existing-ssh-keys).
2. [Añade la clave SSH a tu cuenta de GitHub](https://docs.github.com/en/authentication/connecting-to-github-with-ssh/adding-a-new-ssh-key-to-your-github-account).

### 1.2 Clona Tu Repositorio

1. Abre una ventana de línea de comandos/terminal y visita tu repositorio `<TuUsuario>.github.io` en GitHub.
2. Haz clic en el botón verde "<> Code" para obtener la URL del repositorio. Copia el enlace HTTPS o SSH.
3. En tu interfaz de línea de comandos (CLI), escribe `git clone ` y pega el enlace copiado. Debería verse algo como:
   - **HTTPS:** `git clone https://github.com/<TuUsuario>/<TuUsuario>.github.io.git`
   - **SSH:** `git clone git@github.com:<TuUsuario>/<TuUsuario>.github.io.git`
4. Presiona Enter. Si el repositorio se clona correctamente, ahora puedes `cd` en tu directorio `<TuUsuario>.github.io` para ver su contenido.

## 2. Explicación Sobre Repositorios y el Proceso de Sincronización

![URL de Clonación de GitHub](image/mi-forking-and-updating-a-repo.png)

El paso anterior creó un clon de tu repositorio en tu sistema operativo.

Ahora, hay tres niveles de repositorios a tener en cuenta:

1. **Repositorio Upstream en GitHub:** `todosconectados-gt.github.io`
2. **Tu Fork en GitHub:** `<TuUsuario>.github.io`
3. **Tu Clon Local del Sistema:** `<TuUsuario>.github.io`

Estos repositorios deben estar consistentemente sincronizados y actualizados entre sí, ya que todos contribuimos al repositorio upstream (todosconectados-gt.github.io). Es crucial mantener los cambios separados y evitar mezclarlos entre repositorios. Diferencias significativas pueden causar conflictos y evitar que realices operaciones `git push/pull` sin problemas.

### 2.1 Recursos

- [Ayuda de GitHub: Sincronizando un Fork](https://help.github.com/articles/syncing-a-fork/)
- [Documentación de Git](https://git-scm.com/doc)

Siguiendo estos pasos, te asegurarás de que tus repositorios estén constantemente actualizados y evitarás conflictos (consulta el diagrama a continuación).

![URL de Clonación de GitHub](image/mi-sync-a-fork.png)

## 3. Configura un Repositorio Remoto para Tu Fork

Para obtener actualizaciones del repositorio upstream, configúralo de la siguiente manera:

1. Abre tu línea de comandos/terminal y navega al directorio del repositorio:

  ```bash
  cd <TuUsuario>.github.io
  ```

2. Lista el repositorio remoto configurado actualmente:

  ```bash
  git remote -v
  ```

  Esto debería mostrar:

  ```bash
  origin  https://github.com/<TuUsuario>/<TuUsuario>.github.io.git (fetch)
  origin  https://github.com/<TuUsuario>/<TuUsuario>.github.io.git (push)
  ```

3. Añade el repositorio upstream:

  ```bash
  git remote add upstream https://github.com/todosconectados-gt/todosconectados-gt.github.io.git
  ```

4. Verifica que el repositorio upstream esté configurado correctamente:

  ```bash
  git remote -v
  ```

  Esto debería mostrar:

  ```bash
  origin  https://github.com/<TuUsuario>/<TuUsuario>.github.io.git (fetch)
  origin  https://github.com/<TuUsuario>/<TuUsuario>.github.io.git (push)
  upstream  https://github.com/todosconectados-gt/todosconectados-gt.github.io.git (fetch)
  upstream  https://github.com/todosconectados-gt/todosconectados-gt.github.io.git (push)
  ```

  Si notas que las URLs del upstream son incorrectas, usa `git remote rm upstream` y repite "3. Añadir el repositorio upstream".

## 4. Sincroniza Tu Fork

1. Obtén cualquier cambio del repositorio remoto llamado `upstream` a tu repositorio local:

   ```bash
   git fetch upstream
   ```

2. Cambia a la rama master de tu repositorio local:

   ```bash
   git checkout master
   ```

3. Combina el upstream/master con la rama actual en tu repositorio local:

  ```bash
  git merge upstream/master
  ```

  Si aparece el editor Vim para el mensaje de commit, usa `:wq` (**w**rite y **q**uit) para salir con el mensaje por defecto.

4. Empuja las actualizaciones realizadas a tu repositorio en GitHub:

  ```bash
  git push origin master
  ```

## Resumen de Pasos

En general, sigue estos comandos en tu línea de comandos, pero consulta arriba si hay errores o preguntas adicionales sobre por qué estás escribiendo alguno de los siguientes comandos:

#### Clona tu repositorio de GitHub `<TuUsuario>.github.io`

1. Abre tu línea de comandos/terminal y encuentra el directorio correcto.
2. Copia el enlace HTTPS o SSH desde tu repositorio en el sitio de GitHub.
3. En la línea de comandos, escribe `git clone *pega tu enlace HTTPS o SSH aquí*`.

#### Comprende que hay tres niveles de un repositorio en GitHub

- el upstream ([todosconectados-gt.github.io](https://github.com/todosconectados-gt/todosconectados-gt.github.io))
- Tu `<TuUsuario>.github.io` en GitHub
- Tu `<TuUsuario>.github.io` en tu sistema operativo.

Estos necesitan estar sincronizados y revisados constantemente.
El **repositorio upstream** es al que estamos contribuyendo.

#### Configura el repositorio upstream a tu fork

1. `cd <TuUsuario>.github.io.`
2. `git remote -v` consulta arriba para asegurarte de que estás empujando y obteniendo a tu propio repositorio en GitHub como origin.
3. `git remote add upstream https://github.com/todosconectados-gt/todosconectados-gt.github.io.git`
4. `git remote -v` los origins deberían permanecer igual, pero ahora también deberías estar obteniendo y empujando a OLE como upstream.

#### Sincroniza Tu Fork

1. `git fetch upstream` - para obtener ramas del repositorio upstream ([más info](https://git-scm.com/docs/git-fetch))
2. `git checkout master` - para cambiar a la rama `master` ([más info](https://git-scm.com/docs/git-checkout))
3. `git show-branch` - para ver ramas y los cambios realizados en ellas ([más info](https://git-scm.com/docs/git-show-branch))
4. `git merge upstream/master` - Tu repositorio ahora debería estar sincronizado con upstream/master ([más info](https://git-scm.com/docs/git-merge))

#### Asegúrate de que tu repositorio esté actualizado

1. `git diff` - para comparar diferentes versiones del mismo archivo ([más info](https://git-scm.com/docs/git-diff))
2. `git status` - para ver los cambios realizados en la rama, si la rama está actualizada con master ([más info](https://git-scm.com/docs/git-status))
3. `git pull` - para sincronizar el repositorio local con el repositorio remoto ([más info](https://git-scm.com/docs/git-pull))
4. `git push` - para empujar las actualizaciones que realizaste en los repositorios locales a los repositorios en GitHub ([más info](https://git-scm.com/docs/git-push))

**NOTA**: Los desarrolladores deben sincronizar siempre su fork y asegurarse de que sus repositorios estén actualizados con GitHub cada vez que comiencen a trabajar. De esta manera, como equipo, podemos minimizar la pérdida de datos y ahorrar tiempo.

#### Si te encuentras necesitando rebasar tu repositorio fork, los siguientes dos enlaces deberían ayudarte

- [Rebase](https://git-scm.com/docs/git-rebase)
- [Ramas y Rebase](https://git-scm.com/book/en/v2/Git-Branching-Rebasing)

**NOTA**: Aunque rebase y merge son similares, hay una diferencia entre ellos. El merge toma todos los cambios en una rama y los fusiona en otra rama en un solo commit. El rebase mueve el punto de partida de la rama a otro lugar. Por ejemplo, si rebasas tu rama a la rama master, entonces tu rama ahora incorpora todos los cambios realizados en master, y cada vez que master cambia, tu rama también cambia. En contraste, el merge es un cambio único.

Para más información sobre las diferencias entre merging y rebasing (y cuándo usar cada uno), [consulta esto](https://www.atlassian.com/git/tutorials/merging-vs-rebasing)

Si deseas comprender cómo funciona la sincronización con el fork, aquí hay un útil [video](https://www.youtube.com/watch?v=-zvHQXnBO6c)

## Enlaces Útiles

- [Configurar un repositorio remoto para un fork | GitHub Docs](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/working-with-forks/configuring-a-remote-repository-for-a-fork) - Puedes sincronizar los cambios realizados en el repositorio original con un fork.
- [Sincronizando un fork | GitHub Docs](https://help.github.com/articles/syncing-a-fork/) - Sincroniza un fork de un repositorio para mantenerlo actualizado con el repositorio upstream.
- [Tutorial de GitHub](http://product.hubspot.com/blog/git-and-github-tutorial-for-beginners) - Una introducción a Git y GitHub para principiantes de HubSpot.
- [Git-it Workshop](http://jlord.us/git-it/) - Se ejecuta en tu terminal para trabajar y proporciona un enfoque práctico para aprender Git y los repositorios de GitHub.
- [Ayuda de Git](https://git-scm.com/) - Una enciclopedia de flujos de trabajo útiles de git y explicaciones de la terminología.
- [Otros enlaces y videos útiles](mi-faq.md#Helpful_Links)

#### Regresar a [Primeros Pasos](mi-10-steps.md#Step_5_-_Git_Repositories:_A_Guide_to_Cloning,_Configuring,_and_Syncing_Forks)
