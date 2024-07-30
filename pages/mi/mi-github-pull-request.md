# Crear una Solicitud de Extracción

Una solicitud de extracción (pull request) es una propuesta para fusionar modificaciones de una rama a otra. Permite a los colaboradores revisar y discutir los cambios propuestos antes de integrarlos en la base de código principal. [Esta guía sobre Solicitudes de Extracción](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/about-pull-requests) contiene más información sobre su uso adecuado.

## 1. Abrir una Solicitud de Extracción

Ahora, ve a tu repositorio bifurcado en GitHub visitando `https://github.com/<TuNombreDeUsuario>/<TuNombreDeUsuario>.github.io`. GitHub detectará que recientemente has subido una nueva rama.

1. Haz clic en el botón "Compare & pull request" como se destaca en la captura de pantalla a continuación. Si no aparece, ve a la pestaña 'Pull requests' y haz clic en el botón "New pull request".

   ![Botón Compare & Pull](image/mi-initiate-pull-request.png)

2. **Sigue el <span style="color:red;">template de la solicitud de extracción</span> cuidadosamente y completa los detalles necesarios en la descripción.**

   ![Template de Solicitud de Extracción](image//mi-pr-title-and-description.png)

   Hay algunas cosas a tener en cuenta antes de hacer clic en el botón "Create pull request". Asegúrate de:
      - agregar el título y el número de problema (cuando sea aplicable) en el campo de título
      - marcar las casillas de verificación
      - escribir la descripción
      - agregar el enlace de vista previa de RawGitHack
      - verificar que cumples con los requisitos para los que estás creando esta solicitud de extracción

3. Envía la solicitud de extracción.
4. Una vez redirigido a la nueva solicitud de extracción creada, completa las tareas listadas bajo "Después de Crear la Solicitud de Extracción" marcando cada casilla a medida que las terminas.
5. Publica el enlace a tu solicitud de extracción en nuestro canal de Discord junto con cualquier enlace requerido.

    Un miembro de nuestro equipo revisará tus cambios y te notificará en Discord. Los revisores a menudo proporcionan comentarios, así que prepárate para abordar sus sugerencias o correcciones. Si recibes comentarios, realiza los cambios necesarios en tu rama navegando al archivo en tu repositorio bifurcado o haciendo clic en la pestaña "Files changed" de la solicitud de extracción, seleccionando "...", y luego "Edit file". Deja un comentario en la solicitud de extracción una vez que hayas terminado, y no olvides notificarnos en Discord. Cualquier actualización que realices en tu rama se reflejará automáticamente en la solicitud de extracción.

6. Espera a que tu solicitud de extracción sea fusionada. Una vez fusionada, procede a eliminar tu rama.

**NOTA**: ¡Solo elimina tu rama después de que tu solicitud de extracción haya sido fusionada con éxito!

## 2. Eliminar la Rama

Después de que tu solicitud de extracción haya sido aprobada y fusionada, es posible que quieras eliminar la rama asociada para mantener tu repositorio local y remoto (<TuNombreDeUsuario>.github.io en GitHub) limpio y libre de ramas obsoletas.

- Para eliminar la rama en tu repositorio remoto, haz clic en el botón "Delete branch" en tu solicitud de extracción (ver la imagen a continuación).

  ![Eliminar Rama Fusionada](image/mi-delete-merged-branch.png)

- Para eliminar la rama de tu repositorio local, utiliza el comando `git branch -d <NombreDeTuRamaLocal>`. Asegúrate de no estar actualmente en la rama que deseas eliminar. Para obtener más información sobre cómo eliminar una rama localmente, ve [aquí](https://tecadmin.net/delete-git-remote-and-local-branch/).
