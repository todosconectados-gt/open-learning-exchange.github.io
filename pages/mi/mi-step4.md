# Conectando myPlanet a Planet

## Antecedentes

Usamos la infraestructura de naciones/comunidades porque nuestro software a menudo se despliega en áreas sin acceso a internet. Las naciones son servicios en la nube conectados a internet. Las comunidades, generalmente ejecutadas localmente en Raspberry Pis y/o laptops, operan en una red interna y a veces no están conectadas a internet. Las naciones, al estar conectadas a internet, facilitan la comunicación entre nosotros (con acceso a internet) y los usuarios en las comunidades (sin acceso a internet). Sin embargo, para que una comunidad se sincronice con una nación, debe conectarse a internet para permitir el intercambio bidireccional de datos.

## Conectando myPlanet a la Nación Virtual Interns "vi"

[Video tutorial para esta sección](https://www.youtube.com/watch?v=Gm194qUNz0o)

En este paso, conectarás nuestra aplicación móvil, myPlanet, a la nación "vi" de Planet. Para establecer la conexión, sigue las instrucciones a continuación:

- **Configuración**: Haz clic en el ícono de engranaje en la esquina superior derecha para abrir el cuadro de diálogo de configuración.
  - Activa la configuración "manual".
  - Selecciona "https".
  - Ingresa lo siguiente para "planet ip": `planet.vi.ole.org`.
  - Para "server pin", envía `-get_vi_nation_pin` en el [canal de Discord de internos móviles](https://discord.com/channels/1079980988421132369/1131244649902772235) y recibirás un DM con el PIN del bot YAGPDB.
  - Haz clic en "SYNC" y permite que el proceso de sincronización se complete.

  ![Captura de pantalla del popup de dirección del servidor](image/mi-server-address-popup.png)

- **Crear una Cuenta de Usuario**: Después de sincronizar, haz clic en "BECOME A MEMBER" y completa la información requerida para crear una cuenta. Guarda tus credenciales en algún lugar, ya que las necesitarás para futuros inicios de sesión.

- **Iniciar Sesión**: Usa el nombre de usuario y la contraseña que acabas de crear para iniciar sesión en myPlanet. Ahora has conectado con éxito la aplicación myPlanet al servidor de Planet.

**NOTA**: Si encuentras problemas durante el inicio de sesión, prueba lo siguiente:
1. Re-Sincronizar: inicia manualmente la sincronización presionando el ícono de sincronización en la esquina superior izquierda de la aplicación. Después de sincronizar, intenta iniciar sesión nuevamente.
2. Borrar datos de la aplicación: Borra los datos de la aplicación myPlanet en la página de información de la aplicación de Android. Intenta los pasos de configuración nuevamente.
3. Si el problema persiste, contáctanos en Discord con los detalles.

- **Explora**: Haz clic y explora las características básicas de la aplicación, háznoslo saber en el canal de Discord si notas algún problema.

Toma una captura de pantalla de la página de inicio de la aplicación myPlanet en tu dispositivo y compártela en el canal de Discord para hacernos saber que has completado el paso 4.

#### Volver a [Primeros Pasos](mi-10-steps.md#Step_4_-_Connect_myPlanet_app_to_Planet)
