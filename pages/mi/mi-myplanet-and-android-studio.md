# Paso 3 - myPlanet y Android Studio

## Preparación

Sigue [Clonar un repositorio - GitHub Docs](https://docs.github.com/en/repositories/creating-and-managing-repositories/cloning-a-repository) para clonar el [repositorio de myPlanet de OLE](https://github.com/open-learning-exchange/myplanet) en tu máquina local.

## 1. Descargar y Abrir Android Studio

- Si ya tienes Android Studio instalado, asegúrate de que esté actualizado.
- Si no, visita [Instalar Android Studio | Android Developers](https://developer.android.com/studio/install) y sigue los pasos proporcionados para instalar Android Studio.
- Inicia Android Studio en tu computadora. Si es la primera vez que usas Android Studio, puede que tarde un momento en configurar la configuración inicial.

## 2. Abrir el Proyecto

- En la pantalla de bienvenida, haz clic en el botón "Open". Alternativamente, si ya tienes un proyecto abierto, puedes ir a "File" > "Open..." desde la barra de menú superior.
- Aparecerá un cuadro de diálogo de archivos. Navega a la ubicación donde está la carpeta del repositorio de tu proyecto.

## 3. Construcción de Gradle

Después de importar el proyecto, Android Studio realizará una construcción de Gradle, lo cual puede tardar unos momentos. Gradle es el sistema de construcción para proyectos de Android y descargará cualquier dependencia necesaria para el proyecto.

## 4. Configurar el Emulador

Para evitar sobrescribir la aplicación en tu dispositivo físico y para asegurar que se envíen los informes de fallos, necesitamos configurar un emulador de Android para este paso. Abre 'Tools' > 'Device Manager.'
![Device Manager](image/mi-device-manager-location.png)

Haz clic en el icono + para crear un nuevo dispositivo virtual. Deberías ver este cuadro emergente:
![Virtual Device](image/mi-virtual-device-configuration.png)

Sigue las instrucciones para seleccionar un hardware, haz clic en siguiente y elige una imagen del sistema. Continúa y finaliza la configuración. Puedes cambiar el nombre del dispositivo si lo deseas.

## 5. Seleccionar Configuración de Ejecución

En la barra de herramientas de Android Studio, selecciona la configuración de ejecución deseada del menú desplegable. En nuestro caso sería `app`.
![Run Configuration](image/mi-app-run-configuration.png)

## 6. Ejecutar la Aplicación

Haz clic en el botón verde "Run" para instalar y lanzar la aplicación en el emulador.

## 7. Lanzamiento de la Aplicación

Después de instalar la aplicación en tu emulador, se iniciará automáticamente. Acepta cualquier solicitud de permiso para continuar. Una vez que la aplicación esté en funcionamiento, toma una captura de pantalla desde tu emulador y compártela en el canal de Discord para hacernos saber que completaste el paso 3.

## Enlaces Útiles

- https://github.com/open-learning-exchange/myplanet?tab=readme-ov-file#getting-started-for-interns

#### Volver a [Primeros Pasos](mi-10-steps.md#Step_3_-_Build_myPlanet_in_Android_Studio)
