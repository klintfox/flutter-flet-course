# Flutter Flet y Python


## Flutter
Es un framework de desarrollo de aplicaciones de código abierto creado por Google, que permite construir aplicaciones nativas de alto rendimiento para móviles, web y escritorio a partir de una única base de código.

Con Flutter, puedes crear interfaces de usuario hermosas, rápidas y nativas para Android, iOS, Windows, macOS, Linux y la web. Flutter se destaca por su alto rendimiento, su fácil integración con plataformas nativas, y su capacidad para crear aplicaciones con diseños personalizados.

Características clave de Flutter
Desarrollo multiplataforma: Es posible crear aplicaciones para Android, iOS, Web, Windows, macOS y Linux utilizando un solo código base.

Alto rendimiento: Flutter se compila directamente a código nativo, lo que proporciona un rendimiento superior al de otras soluciones de desarrollo multiplataforma como React Native.

Hot Reload: Una característica que permite ver los cambios realizados en el código de inmediato sin tener que reiniciar la aplicación. Esto acelera el proceso de desarrollo y pruebas.

UI rica y flexible: Flutter proporciona un conjunto de widgets personalizables que permiten crear interfaces visualmente atractivas y adaptables a las necesidades de la aplicación.

Integración con plataformas nativas: Puedes acceder fácilmente a las APIs y funcionalidades de dispositivos nativos utilizando plataformas de canales para interactuar con el código nativo (Java, Kotlin, Swift, Objective-C).

Dart como lenguaje de programación: Flutter usa Dart, un lenguaje de programación también desarrollado por Google, conocido por su facilidad de uso, seguridad de tipo y rendimiento optimizado para la compilación a código nativo.

## Flet 
Es un framework de desarrollo que permite crear aplicaciones móviles y web usando Python y Flutter. Flet combina la potencia de Flutter para crear interfaces visuales y el poder de Python para manejar la lógica de la aplicación, lo que facilita la creación de aplicaciones multiplataforma con solo un lenguaje de programación.

Este proyecto utiliza Flet para generar aplicaciones modernas y funcionales para Android, iOS, Web y más, con una experiencia de desarrollo sencilla y rápida.

## Ventajas de usar Flet con Flutter
Desarrollo Rápido: Crea aplicaciones móviles y web de forma rápida y sencilla utilizando solo Python. Flet se encarga del backend utilizando Flutter.
Multiplataforma: Desarrolla aplicaciones para Android, iOS, y Web sin necesidad de escribir código específico para cada plataforma.
Interfaces Modernas: Utiliza los widgets de Flutter para construir interfaces visuales ricas y atractivas.
Fácil Integración con Python: Aprovecha la flexibilidad de Python para manejar bases de datos, APIs, procesamiento de datos, etc.
Sin Dependencias Adicionales: No necesitas aprender o trabajar con Java, Swift o JavaScript. Solo con Python.
Requisitos previos
Antes de comenzar, asegúrate de tener las siguientes herramientas instaladas en tu sistema:


### Pasos para instalar y configurar Flutter en Windows
1. Descargar e instalar Flutter

** Descargar Flutter:**

- Ve al sitio web oficial de Flutter: flutter.dev.
- En la sección de Windows, haz clic en el enlace para descargar el archivo ZIP de Flutter. Por ejemplo, el archivo descargado podría ser flutter_windows_v3.x.x-stable.zip.
- Extraer el archivo ZIP:

- Extrae el archivo ZIP en una ubicación en tu máquina. Es recomendable que lo extraigas en un directorio como C:\flutter (sin espacios en el nombre del directorio) para evitar problemas con las rutas.

- La estructura de tu directorio debería ser algo así:
```sh
C:\flutter\
```

2. Configurar las variables de entorno

- Para que Flutter funcione correctamente desde la terminal, debes agregar Flutter a tu variable de entorno PATH.
- Abrir la configuración de las variables de entorno:
- Haz clic con el botón derecho en el botón de Inicio y selecciona Sistema.
- En la ventana de Sistema, haz clic en Configuración avanzada del sistema.
- Luego, selecciona Variables de entorno.
- Agregar Flutter al PATH:
- En la ventana de Variables de entorno, bajo Variables del sistema, busca la variable Path y haz clic en Editar.
- En la ventana de edición de la variable Path, haz clic en Nuevo y agrega la ruta de la carpeta bin dentro del directorio donde extrajiste Flutter. En este caso, agregarás:
```sh
C:\flutter\flutter\bin
```

- Haz clic en Aceptar en todas las ventanas para guardar los cambios.
- Verificar que Flutter está correctamente agregado al PATH:

- Abre una terminal de PowerShell o CMD y escribe (ambos en modo administrador)
```sh
flutter --version
```

- Si Flutter está bien configurado, deberías ver la versión instalada de Flutter.

3. Instalar las dependencias de Android SDK y el NDK
Configurar el SDK de Android:

- Abre una terminal y ejecuta:
```sh
flutter doctor
```

- Si es la primera vez que ejecutas flutter doctor, este comando descargará e instalará las dependencias necesarias, como el Android SDK y el NDK.
- Aceptar las licencias de Android:
- Para que Flutter funcione con Android, necesitas aceptar las licencias de Android. Para ello, ejecuta el siguiente comando en la terminal:
```sh
flutter doctor --android-licenses
```

- Luego, presiona y (sí) para aceptar todas las licencias.

4. Instalar Visual Studio (para desarrollo de Windows)

- Si planeas desarrollar aplicaciones para Windows, necesitas instalar Visual Studio con las herramientas necesarias:

**Descargar Visual Studio:**
- Ve a visualstudio.com y descarga Visual Studio Community Edition.
- Durante la instalación, selecciona los componentes de Desarrollo de escritorio con C++.

5. Verificar la instalación

- Verificar la instalación de Flutter:
- Después de instalar todo lo necesario, abre una terminal y ejecuta:
```sh
flutter doctor
```
- Este comando verificará si hay algún problema con la configuración de Flutter. Si todo está correcto, verás algo como esto:

```sh
[√] Flutter (Channel stable, 3.x.x, on Microsoft Windows [version 10.0.xxxx.x], locale en-US)
[√] Android toolchain - develop for Android devices (Android SDK version 34.x.x)
[√] Android Studio (version 2024.x)
[√] Visual Studio - develop for Windows apps (version 16.x)
[√] Connected device (1 available)
[√] Network resources
```

- Si encuentras algún problema, el comando flutter doctor te indicará qué necesitas corregir.

6. Crear tu primer proyecto Flutter

**Crear un nuevo proyecto Flutter:**

- Una vez que Flutter esté configurado, puedes crear tu primer proyecto ejecutando:
```sh
flutter create my_first_app
```

- Ir a la carpeta creada
```sh
cd my_first_app
```

**Ejecutar el proyecto:**

- Para ejecutar la aplicación, conecta un dispositivo o abre un emulador Android, y luego corre:
```sh
flutter run
```

7. Solucionar problemas comunes

- Si encuentras algún problema durante la instalación, puedes buscar ayuda usando el comando:
```sh
flutter doctor -v
```

-Esto te proporcionará más detalles y mensajes de error que pueden ayudarte a diagnosticar cualquier problema de configuración.

### Generar APK en proyecto Python 

- Asegurarse de tener el archivo requeriments.txt creado en la raiz del proyecto en caso contrarios puedes ejecutar el comando
```sh
pip freeze > requirements.txt
```

- Una vez que generar el archivo o lo crees bajo la codificación UTF-8 ejecuta el siguiente comando para generar el .apk
```sh
flet build apk --verbose
```
