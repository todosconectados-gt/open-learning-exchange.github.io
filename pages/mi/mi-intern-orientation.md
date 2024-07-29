# Orientación para Pasantes Virtuales Móviles

## ¡Bienvenido al Equipo de Pasantes Móviles de OLE!

¡Felicidades! Has completado los primeros pasos y has sido seleccionado para unirte al equipo de pasantes virtuales móviles de Open Learning Exchange. Por favor, recuerda que esperamos que los pasantes dediquen al menos 24 horas a la semana durante un mínimo de 3 meses para trabajar en los temas de Open Learning Exchange. Si actualmente no tienes suficiente tiempo, estaremos encantados de tenerte más adelante cuando tengas tiempo.

## Conoce al Equipo

Lo primero es conocer al equipo, comenzando con el CTO [dogi](https://github.com/dogi), luego los [líderes y miembros actuales del equipo de pasantes](#!./pages/mi/mi-team.md). Después de tener la reunión inicial con dogi, puedes unirte a <http://talk.ole.org> durante la sesión de Google Meet para conocer a los pasantes actuales, conocerse y preguntarles en qué han estado trabajando.

## Familiarízate con los Proyectos y Problemas Actuales

Normalmente, los pasantes eligen el proyecto en el que quieren trabajar en función de su experiencia. Si te cansas de un proyecto en particular, hay una oportunidad de cambiar. Echa un vistazo a nuestros proyectos actuales a continuación; si alguno en particular te interesa, hay una buena posibilidad de que puedas trabajar en ellos.

**Proyectos Móviles Activos**

- [myPlanet](https://github.com/open-learning-exchange/myplanet)
  - Una aplicación para Android que se sincroniza con Planet para guardar datos para uso sin conexión y enviar datos de uso.
- [Remote](https://github.com/treehouses/remote/)
  - Una aplicación para Android que se comunica con un servidor móvil Raspberry Pi sin cabeza que ejecuta una imagen de treehouses a través de Bluetooth.

## Algunas Cosas que Debes Saber...

### Convertirse en Miembro de la Organización en GitHub

Una vez que hayas sido oficialmente incorporado como pasante virtual, recibirás invitaciones por correo electrónico para unirte a las organizaciones de GitHub: [open-learning-exchange](https://github.com/open-learning-exchange), [ole-vi](https://github.com/ole-vi) y [treehouses](https://github.com/treehouses).

Al recibir estas invitaciones, por favor, acéptalas de inmediato. Una vez aceptadas, márcate como miembro público en la [lista de colaboradores de OLE](https://github.com/orgs/open-learning-exchange/people).

### Transición a los Repositorios de OLE y Adopción del Flujo de Trabajo con Ramas de Características

A partir de ahora, trabajarás directamente en los repositorios de OLE en lugar de tus propios repositorios bifurcados. Seguiremos el [Flujo de Trabajo con Ramas de Características](https://www.atlassian.com/git/tutorials/comparing-workflows/feature-branch-workflow), que permite una mejor colaboración y gestión del código.

Es importante tener en cuenta que con este flujo de trabajo, tienes el potencial de hacer cambios más significativos, por lo que siempre debes verificar la rama en la que estás trabajando. Además, realiza commits con frecuencia y crea solicitudes de extracción temprano en el proceso de desarrollo. Esto permite a otros pasantes virtuales revisar tu código y proporcionar retroalimentación, asegurando que te mantengas en el camino correcto desde el principio.

### Revisión de Solicitudes de Extracción y Problemas

Una de tus responsabilidades como pasante es revisar y ayudar a los pasantes prospectivos con sus problemas / solicitudes de extracción en [open-learning-exchange/open-learning-exchange.github.io](https://github.com/open-learning-exchange/open-learning-exchange.github.io). Para comenzar una revisión, navega a la pestaña 'Files changed' en una solicitud de extracción. Familiarízate con las funciones de revisión de GitHub consultando la [documentación sobre Revisiones en GitHub](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/reviewing-changes-in-pull-requests/about-pull-request-reviews).

Asegúrate de ser consciente de nuestra diversa comunidad al comunicar comentarios. Consulta [**Una guía para revisar código y tener tu código revisado**](https://github.com/thoughtbot/guides/tree/main/code-review#code-review) para obtener consejos sobre el uso de lenguaje inclusivo y fomentar un entorno de apoyo.

Debes verificar que se cumplan las siguientes condiciones:

- [x] el número de problema está incluido en el título y la descripción de la solicitud de extracción en el formato `(fixes #IssueNumber)`, cuando sea aplicable
- [x] no hay archivos o líneas innecesarios en la pestaña "Files changed"
- [x] hay una rama para el parche
- [x] la solicitud de extracción realmente soluciona el problema
- [x] los cambios se renderizan correctamente en la vista previa de rawgit
- [x] sin conflictos de fusión
- [x] los commits están asociados con la cuenta de GitHub

Cada vez que comentes en un problema o revises una solicitud de extracción, envía un mensaje a los involucrados en el [Servidor de Discord](https://discord.gg/mtgGD4EnYW) con un enlace al problema / solicitud de extracción. Además, si encuentras algún problema que deba abordarse con una solicitud de extracción, no olvides usar la opción `Request changes` al crear tu revisión.

### Fusionar una Solicitud de Extracción

Para fusionar una solicitud de extracción, sigue estos pasos:

1. **Requisito de Aprobación:** Asegúrate de que al menos dos miembros del equipo hayan aprobado la solicitud de extracción y no haya solicitudes de cambios pendientes de otros. Sin embargo, hay una excepción para los pasantes virtuales que se añaden a `mi-team.md`: deben fusionar su solicitud de extracción durante su entrevista inicial.

2. **Proceso de Fusión:**
   - Selecciona "Squash and Merge"
   - **Título del Commit:** Elimina todos los mensajes de commit en la descripción extendida. Mantén el título del commit conciso, claro y en minúsculas.
   - **Cierre de Problemas:** Si es aplicable, incluye "(fixes #IssueNumber)" en el título para [cerrar automáticamente el problema asociado](https://docs.github.com/en/issues/tracking-your-work-with-issues/linking-a-pull-request-to-an-issue#linking-a-pull-request-to-an-issue-using-a-keyword). Si olvidas esto, cierra manualmente el problema y vincúlalo a la solicitud de extracción original. Un ejemplo de un buen título de commit: "update vi-configuration.md (fixes #1530) (#1557)", donde "1530" es el número del problema y "1557" es el número de la solicitud de extracción.

3. **Notificación:** Después de fusionar una solicitud de extracción, menciona al autor en el [servidor de Discord](https://discord.gg/mtgGD4EnYW). Asegúrate de incluir un enlace a la solicitud de extracción y el ID del commit para referencia.

### Registro de Entrada/Salida

Normalmente, realizamos registros de entrada y salida verbales (similares a los "[stand-up meetings](https://en.wikipedia.org/wiki/Stand-up_meeting)"). Si la comunicación verbal no es posible, puedes usar el siguiente formato de texto en nuestro canal de Discord *vi-lounge*:

```
# Registro de Entrada
¿Qué hice la última vez?
-

¿Cuál es mi objetivo para hoy?
- Enumera en qué estás trabajando - considera enlazar a los problemas

¿Qué obstáculos están en el camino de nuestro progreso?
- Enumera cualquier problema
```

```
# Registro de Salida
Lo que trabajé hoy
- Considera enlazar a la solicitud de extracción cuando sea aplicable

¿Qué fecha y hora vamos a encontrarnos contigo la próxima vez?
- por ejemplo, miércoles 10am EDT
```

## Formar una Rutina de Trabajo y Horario

### Rutina Diaria Recomendada

Mientras eres libre de trabajar a tu propio ritmo, te recomendamos seguir esta rutina diaria básica:

- Revisa los canales de Discord y tus mensajes privados en Discord.
- Únete a la [sesión de Google Meet de OLE](http://talk.ole.org) si puedes, para que puedas seguir en qué está trabajando todo el mundo y obtener ayuda rápidamente.
- Regístrate verbalmente o escribe un mensaje en el canal vi-lounge de Discord con el formato mencionado anteriormente.
- Revisa cualquier problema o solicitud de extracción que se haya agregado o cambiado en [open-learning-exchange.github.io](https://github.com/open-learning-exchange/open-learning-exchange.github.io) desde la última vez que revisaste.
- Cierra problemas con `(fixes #IssueNumber)` en el mensaje de commit de fusión squash de la solicitud de extracción.
- Trabaja en tus problemas y escribe en el canal de Discord del repositorio respectivo cada vez que te enfrentes a problemas.
- Realiza commits con frecuencia y crea solicitudes de extracción lo antes posible, para que puedas obtener retroalimentación mientras trabajas.

### Horario Semanal

Nuestra sesión de Google Meet se puede unirse en [http://talk.ole.org](http://talk.ole.org). A medida que iniciamos nuestro programa de pasantías virtuales, podríamos dividirnos en varias sesiones de Google Meet o usar Discord para comunicación sincrónica.

## ¡Comunica, Comunica, Comunica!

La comunicación es clave para el éxito en una pasantía remota. No dudes en ponerte en contacto en Discord si tienes preguntas, inquietudes o necesitas orientación. Estamos aquí para apoyarte en cada paso del camino.

Si no estás seguro de qué tareas abordar a continuación o encuentras obstáculos que te impiden trabajar, háznoslo saber. Es mejor comunicarse abiertamente en lugar de dejarnos adivinando. Recuerda, cuanto más inviertas en esta pasantía, más obtendrás de ella.

Adaptarse al trabajo remoto requiere autodisciplina e iniciativa, pero no estás solo. Estamos aquí para ayudarte a navegar por este viaje, así que no dudes en pedir ayuda o consejo. ¡Tu éxito es nuestra prioridad!
