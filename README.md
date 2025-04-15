
PASO A PASO: Ejecutar el Proyecto Hugo en Otro Computador (Windows)

1. INSTALAR HERRAMIENTAS NECESARIAS
------------------------------------

A. Instalar Git:
   - Visita https://git-scm.com/downloads
   - Descarga e instala Git según tu sistema operativo.
   - Verifica con: git --version

B. Instalar Hugo (versión extendida) usando Chocolatey:
   - Abre PowerShell como ADMINISTRADOR
   - Ejecuta este comando (copia y pega completo):

     Set-ExecutionPolicy Bypass -Scope Process -Force; `
     [System.Net.ServicePointManager]::SecurityProtocol = `
     [System.Net.ServicePointManager]::SecurityProtocol -bor 3072; `
     iex ((New-Object System.Net.WebClient).DownloadString('https://community.chocolatey.org/install.ps1'))

   - Una vez instalado Chocolatey, ejecuta:

     choco install hugo-extended -y

   - Verifica que Hugo esté instalado:

     hugo version

2. CLONAR EL PROYECTO DESDE GITHUB
-----------------------------------

- Abre Git Bash o una terminal y escribe:

  git clone https://github.com/tu-usuario/upz-la-flora.git
  cd upz-la-flora

(Reemplaza el enlace con el de tu repositorio real)

3. ABRIR EN VISUAL STUDIO CODE
-------------------------------

- Abre la terminal en la carpeta del proyecto y ejecuta:

  code .

- Esto abrirá el proyecto en Visual Studio Code.

4. PROBAR EL SITIO WEB LOCALMENTE
----------------------------------

- Ejecuta en la terminal:

  hugo server

- Se mostrará un mensaje como:

  Web Server is available at http://localhost:1313/

- Abre esa dirección en tu navegador.

5. CADA VEZ QUE QUIERAS PROBAR CAMBIOS:

- Ve a la carpeta del proyecto y ejecuta:

  hugo server

¡LISTO! Ahora puedes ver tu sitio Hugo corriendo localmente.
