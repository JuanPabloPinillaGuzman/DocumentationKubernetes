# DocumentationKubernetes

##Opción 1: Usar el instalador oficial (recomendada)

Esta es la forma más sencilla y segura.

1. Descargar cURL

Ve a la página oficial: https://curl.se/windows/

Busca la sección "Win64 - Generic" si tu sistema es de 64 bits (lo más probable).

Si tu Windows es de 32 bits, descarga la opción Win32.

Descarga el archivo ZIP que dice algo como:

curl-8.x.x-win64-mingw.zip

2. Extraer el archivo

Descomprime el .zip en cualquier carpeta, por ejemplo:

C:\curl

3. Configurar la variable de entorno

Para poder usar cURL desde cualquier parte de la terminal:

Presiona Windows + R, escribe:

sysdm.cpl


y presiona Enter.

Ve a Opciones avanzadas → Variables de entorno.

En la sección Variables del sistema, selecciona Path y haz clic en Editar.

Haz clic en Nuevo y agrega la ruta:

C:\curl\bin


Guarda los cambios y cierra todo.

4. Verificar la instalación

Abre CMD o PowerShell y ejecuta:

curl --version


Si ves la versión, ¡listo! ✅

Opción 2: Instalarlo con Winget (más rápido, solo Windows 10/11)

Si tienes Windows 10 o Windows 11, puedes instalarlo con Winget (el gestor de paquetes oficial de Microsoft).

Abre PowerShell como administrador.

Ejecuta:

winget install curl


Espera a que finalice la instalación.

Verifica con:

curl --version

Opción 3: Verificar si ya lo tienes

En Windows 10 y 11, cURL viene preinstalado.
Antes de instalarlo, prueba en CMD o PowerShell:

curl --version
