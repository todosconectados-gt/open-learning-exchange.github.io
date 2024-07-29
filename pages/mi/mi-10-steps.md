
# Primeros Pasos – Interno Virtual Móvil

## La Visión General

¡Bienvenido a los primeros pasos para convertirte en un Interno Virtual Móvil de OLE! Tratamos estos primeros pasos como un proceso de selección para demostrar que puedes seguir instrucciones básicas antes de pasar a proyectos más complejos y equipos más grandes. Piensa en esto como la entrevista para la pasantía.

Si eres seleccionado para la pasantía después de completar los pasos, serás invitado oficialmente a unirte al equipo de internos móviles de OLE. Te agregaremos a nuestro canal de Discord para Internos Virtuales y te asignaremos a un equipo específico para trabajar en el desarrollo y mejora del software de OLE. Nuestros proyectos móviles actuales son:

1. **[myPlanet](https://github.com/open-learning-exchange/myplanet)**: Una aplicación de Android que se sincroniza con Planet para guardar datos para uso offline y enviar datos de uso.
2. **[Remote](https://github.com/treehouses/remote)**: Una aplicación de Android que se comunica con un servidor móvil Raspberry Pi sin pantalla que ejecuta la imagen de treehouses vía Bluetooth.

Si eres seleccionado después de completar estos pasos, trabajarás con tu equipo en una asignación, y las asignaciones cambiarán semanalmente. Durante esta pasantía, tendrás la oportunidad de trabajar con varios softwares y lenguajes, incluyendo **[Git](https://git-scm.com/)**, **[GitHub](https://github.com/)**, **[Markdown](https://daringfireball.net/projects/markdown/)**, **[Línea de Comandos/Terminal](https://www.w3schools.com/whatis/whatis_cli.asp)**, **[Scripts de Línea de Comandos/Terminal](https://www.codecademy.com/articles/command-line-commands)**, **[Vim](https://www.vim.org/)**, **[CouchDB](http://couchdb.apache.org/)**, **[Base de datos Realm](https://en.wikipedia.org/wiki/Realm_(database%29)**, **[Java](https://www.tutorialspoint.com/java/index.htm)**, **[Android Studio](https://en.wikipedia.org/wiki/Android_Studio)** y **[Kotlin](https://kotlinlang.org/)**.

**NOTA**: Esta es una pasantía no remunerada e intensiva que requiere al menos 24 horas de trabajo por semana. Puedes encontrar más información sobre la pasantía en nuestro [FAQ](mi-faq.md#General_Internship_Questions). Si tienes preguntas adicionales, no dudes en preguntar en el servidor de Discord.

## Los Pasos

La codificación social es una gran parte de cualquier proyecto de código abierto y colaborativo, y Open Learning Exchange (OLE) no es diferente. En la siguiente serie de pasos, aprenderás sobre Markdown, Vagrant, Docker, Git, GitHub, problemas de GitHub, solicitudes de extracción de GitHub, etc. También se te presentará la biblioteca digital de OLE, [Planet](https://github.com/open-learning-exchange/planet), y su aplicación complementaria de Android, [myPlanet](https://github.com/open-learning-exchange/myplanet).

**Estos pasos pueden parecer simples, pero esperamos un trabajo de alta calidad, lo que podría requerir tiempo adicional. Queremos ver que puedes usar, o aprender a usar, estas herramientas de manera efectiva, incluyendo escribir problemas claros de GitHub, usar comandos básicos de Git, crear solicitudes de extracción adecuadas, navegar por myPlanet, etc. Seguir los pasos pasivamente es lo mínimo; en cambio, apunta a impresionarnos con una excelente etiqueta de GitHub y un Markdown bien estructurado.**

Aprovecha la oportunidad de leer más sobre las herramientas y lenguajes que usamos para profundizar tu comprensión y reducir la confusión. **¡Trata estos pasos como oportunidades de aprendizaje!** Las habilidades de GitHub y Markdown que practiques en los primeros pasos son cruciales tanto para esta pasantía como para una futura carrera en desarrollo de software.

El MDwiki ofrece muchos recursos para ayudarte a completar estos pasos. Encontrarás una lista de enlaces útiles al final de cada paso. :)

**También nos gustaría que nos mantuvieras actualizados regularmente en el canal de Discord a medida que completes estos pasos. Te pediremos que envíes mensajes, enlaces y capturas de pantalla en el camino, que usaremos para rastrear tu progreso. Por favor, asegúrate de no omitir esto, ya que es crucial para nosotros rastrear tu trabajo.**

Una parte importante de estos pasos es identificar problemas o sugerir mejoras para este MDwiki. A medida que completes los pasos, toma nota de cualquier problema que encuentres o ideas para mejoras. Esto ayuda a mejorar el MDwiki y estos pasos para futuros internos.

Aunque no hay una fecha límite oficial para completar estos pasos, la mayoría de los candidatos exitosos los completan en 7-8 días. ¡Buena suerte!

## FAQ - Preguntas Frecuentes

**[Nuestra página de FAQ](mi-faq.md)** es un recurso integral que contiene respuestas a preguntas comunes sobre la pasantía y los Primeros Pasos. También presenta enlaces adicionales útiles y tutoriales en video destinados a familiarizarte con las herramientas y lenguajes esenciales para nuestro trabajo.

Si tienes consultas generales sobre la pasantía y no puedes encontrar la información que necesitas en la página de FAQ, no dudes en contactarnos a través de Discord. Intenta evitar los mensajes directos ya que otros podrían tener la misma pregunta.

Para preguntas técnicas no cubiertas en el FAQ, además de contactarnos en Discord, Google y Stack Exchange son excelentes recursos suplementarios para explorar. :)

## Paso 0 - Requisitos Previos

Para participar en la pasantía, necesitarás lo siguiente:

1. Una computadora portátil o de escritorio con al menos 8GB de RAM.
2. Un dispositivo Android (teléfono o tableta) con un mínimo de 3GB de RAM y que ejecute Android 9 "Pie" o posterior, y/o una Chromebook.
   - Si no tienes un dispositivo Android físico o Chromebook, puedes usar una [Raspberry Pi 4](https://emteria.com/kb/hardware#raspberry-pi-4b) [o 5](https://emteria.com/kb/hardware#raspberry-pi-5) con al menos 8GB de RAM como una alternativa experimental.
3. [Discord](https://discord.com/download) instalado tanto en tu dispositivo Android como en tu computadora portátil o de escritorio para facilitar la comunicación y el intercambio de capturas de pantalla.
4. Una conexión a internet estable.

**Una vez que hayas confirmado que cumples con los requisitos mencionados anteriormente, saluda a todos en el canal de Discord y háznos saber que has llegado al Paso 0.**

## Paso 1 - Markdown y Flujo de Trabajo de Forking

Sigue las instrucciones en [Crear Tu Página de Perfil de GitHub: Una Guía de Markdown y Flujo de Trabajo de Forking](mi-github-and-markdown.md).

**Recuerda: Solo procede al siguiente paso una vez que hayas completado todas las instrucciones y enviado la solicitud de extracción para tu perfil.**

## Paso 2 - Aplicación myPlanet

myPlanet es una aplicación de Android disponible en la Play Store. Encuéntrala e instálala allí usando [este enlace](https://play.google.com/store/apps/details?id=org.ole.planet.myplanet).

#### Inscribirse en la Prueba Beta

Únete como beta tester para ayudarnos a mejorar la aplicación:

- **Desde un Teléfono:**
  Únete en Google Play en Android en [la página de detalles de la app de myPlanet](https://play.google.com/store/apps/details?id=org.ole.planet.myplanet). Desplázate hacia abajo, en "Únete a la beta", toca Unirse.
- **Desde una Computadora Portátil o de Escritorio:**
  Únete en la web a través de [este enlace](https://play.google.com/apps/testing/org.ole.planet.myplanet).

Después de inscribirte, puede haber un retraso antes de que puedas actualizar a la versión beta de la aplicación.

#### Probando la aplicación

Una vez que hayas **instalado la versión beta** de la aplicación, lánzala y concede los permisos necesarios. Toca el ícono de engranaje en la esquina superior derecha después de pasar la pantalla de introducción. Mantén las configuraciones por defecto y toca "SYNC". Espera a que se complete, luego "INICIAR SESIÓN COMO INVITADO" y explora la aplicación durante al menos 15 minutos.

Toma capturas de pantalla e intenta hacer que la aplicación falle. Después de la exploración, actualízanos en Discord: "Estoy en el paso 2, pasé aproximadamente xx minutos en la aplicación myPlanet y falló al navegar a ..." o "Estoy en el paso 2, pasé aproximadamente xx minutos en la aplicación myPlanet y no falló."

Los detalles sobre la falla pueden tardar hasta 24 horas en aparecer en la Consola de Google Play en nuestro lado.

## Paso 3 - Construir myPlanet en Android Studio

Sigue la guía en [myPlanet y Android Studio](mi-myplanet-and-android-studio.md) para clonar el repositorio de myPlanet desde GitHub y construir la aplicación myPlanet con Android Studio.

## Paso 4 - Conectar la aplicación myPlanet a Planet

Sigue la guía en [Conectar myPlanet a Planet](mi-step4.md).

## Paso 5 - Repositorios de Git: Una Guía para Clonar, Configurar y Sincronizar Forks

Sigue las instrucciones en [Repositorios de Git: Una Guía para Clonar, Configurar y Sincronizar Forks](mi-github-and-repositories.md).

## Paso 6 - Tutorial de Issues en GitHub

- Sigue el tutorial en [GitHub Issues](mi-github-issues.md) para crear al menos un issue. Publica un enlace en el canal de Discord cada vez que crees un issue o comentes en el issue de otra persona. Se te anima a publicar tantos issues como puedas para mejorar la página, así como para práctica personal.
- Ningún issue es demasiado grande o pequeño para ser presentado, y está bien si no sabes cómo solucionarlo por ti mismo. Si sabes cómo resolver un issue, asegúrate de proporcionar una descripción detallada de tu investigación y muestra cómo solucionarlo. Está bien presentar un issue sobre errores menores y cambios muy pequeños, pero no hagas que este sea el caso para todos los issues que presentes.
- También puedes trabajar en issues que no hayas creado. Asegúrate de haber creado al menos un issue, resuelto, comentado en un issue que no creaste y haber realizado un pull request con la solución que fue aceptada.

**HINT**: Puedes seguir tu progreso con el número de pull requests y issues [aquí](../track-first-steps-progress.md).

## Paso 7 - Tomar un Curso en myPlanet, Jardinería de Cursos

Sigue la guía en [Tomar un Curso en myPlanet, Jardinería de Cursos](mi-myplanet-course.md).

## Paso 8 - Crear Issues y Pull Requests

En este paso, tu objetivo es crear, comentar y resolver issues en GitHub para mejorar nuestra Wiki de Markdown. Esto es lo que necesitarás hacer:

1. **Crear Issues**:
   - Crea 3 nuevos issues en nuestro repositorio de GitHub sobre los Primeros Pasos para Internos Móviles o el Manual de Usuario de myPlanet.
   - Cada issue debe centrarse en un problema o mejora específica.
     - Asegúrate de que **al menos un issue** aborde la reducción de contenido, como enlaces muertos, contenido repetitivo, detalles excesivos, o la posibilidad de referenciar documentación oficial externa en los Primeros Pasos para Internos Móviles.
     - Asegúrate de que **al menos un issue** se trate de poblar o mejorar la página del [Manual de Usuario de myPlanet](#!pages/manual/myplanet/overview.md).

2. **Comentar en Issues**: Proporciona comentarios útiles en al menos 3 issues existentes que no creaste. Esto podría ser para dar retroalimentación, sugerir soluciones, hacer preguntas o aclarar el issue.

3. **Resolver Issues con Pull Requests**: Resuelve los 3 issues haciendo los cambios necesarios en ramas separadas derivadas de `master` en tu repositorio, y envía un pull request distinto para cada uno.

Sigue el **mismo proceso** descrito en el paso [GitHub Issues](mi-github-issues.md), trabajando para mejorar nuestra documentación para futuros internos. Para que tus pull requests sean aceptados, deben ser aprobados por al menos otros dos miembros/equipos de OLE. Después de crear un pull request, anúncialo en el chat de Discord para solicitar revisiones. Es posible que necesites hacer correcciones adicionales basadas en los comentarios.

Recuerda, incluso los issues pequeños valen la pena ser abordados. Mantén tus issues enfocados y concisos. Si tus pull requests necesitan aprobaciones adicionales, sigue trabajando en otras tareas mientras esperas.

Así como tu aprendizaje con esta Wiki fue posible gracias a los esfuerzos de internos anteriores, ahora recurrimos a ti para continuar esa tradición y ayudar a futuros internos a dar sus Primeros Pasos. Ayúdanos a hacer que esta documentación sea clara y útil para aquellos que la sigan.

**NOTA**: Si bien agregar detalles puede ser útil, es importante recordar que menos es a menudo más. Con el tiempo, esta guía de Primeros Pasos se ha vuelto abultada con demasiada información, dificultando su seguimiento. A medida que trabajas en mejorar esta guía, concéntrate en simplificar las instrucciones y eliminar cualquier contenido innecesario. El objetivo es crear una guía clara y concisa que los futuros internos virtuales puedan entender y usar fácilmente.

**NOTA**: Mientras esperas que dos miembros del equipo OLE aprueben tus Pull Requests, puedes seguir creando más Issues y Pull Requests (con aprobación, sugerimos). Todos contarán para tu total final de Issues/PR. La aprobación de PR puede llevar tiempo, así que no permitas que un proceso de aprobación/arreglo largo te detenga en tu progreso en los "Primeros Pasos".

Una vez que completes el Paso 8 tendrás:

- 5 pull requests aceptados (uno en el paso 1, uno en el paso 6 y tres en el paso 8)
- 4 comentarios hechos en issues que no creaste (uno en el paso 6 y tres en el paso 8)
- 4 issues creados (uno en el paso 6 y tres en el paso 8)

**HINT**: Puedes seguir tu progreso con el número de pull requests y issues [aquí](../track-first-steps-progress.md).

## Paso 9 - Ser parte del equipo

Lo siguiente es añadirte a la lista de internos virtuales que se encuentra en [mi-team.md](mi-team.md) y crear un pull request. Envíanos un mensaje ("@okurole_25668", "@dogi" y "@vi-mobile") en el canal de Discord para que podamos organizar una reunión y agregarte al equipo lo antes posible.

Asegúrate de leer el [documento de orientación para internos](mi-intern-orientation.md) antes de la reunión.
