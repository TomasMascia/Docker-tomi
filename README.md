Docker, Let's Encrypt, Nginx y Digital Ocean

(LEER ATENTAMENTE EL TRABAJO PRÁCTICO DESDE INICIO A FIN)

Requisitos previos para el trabajo práctico:

Tener instalado Docker Compose.
Tener instalado Docker.
Tener instalado Git.
Utilizar el repositorio visto en el bloque de Web Server Nginx. https://www.youtube.com/watch?v=TdCkRm43PsU 
https://github.com/pablokbs/peladonerd/tree/master/varios/1

Tener usuario con permisos de Docker.
Crear cuenta en https://www.noip.com/es-MX para tener un registro A gratuito y poder redireccionar nuestra aplicación.
Tener cuenta con créditos gratuitos en Digital Ocean.
Tener acceso al workflow de Gitlab para subir el repositorio.
Tener una aplicación web simple/estática para utilizar.

ACLARACIONES: Realizar todo en una misma carpeta llamada “my-app”.

No utilizar en lo posible ChatGPT u otras IAs. Consultar en foros como StackOverflow o distintas páginas de Google.

Cada comando ejecutado en consola debe tener una breve descripción.

Documentar el proceso de cómo se fue desarrollando el script, las funcionalidades, instalaciones y requisitos en un README.md del proyecto en Gitlab.

Al final del script, ejecutar un mensaje de que el script terminó con éxito.

Realizar el script SECUENCIAL y CONTINUO, sin menú interactivo.

Jerarquía de archivos (para tener de ejemplo):
my-app/
├── README.md               	
├── setup.sh       
├── app/ 
   ├── index.html
   └── docker-compose.yml

Para realizar las pruebas se recomienda usar una vm local con Ubuntu. El script tendrá que estar alojado en un repositorio para así clonarlo y poder hacer seguimiento de avances.




El trabajo práctico integra los temas de Docker, Let's Encrypt y Digital Ocean. El mismo va a consistir en levantar una máquina virtual en Digital Ocean e integrar los conocimientos de Let's Encrypt y Docker.

1. Levantar una VM con ubuntu server. 
2. Crear una llave SSH para poder conectarse a la VM. 
3. Configurar la VM con un script escrito en bash para que el mismo se pueda reutilizar: 
1. Configurar la zona horaria en Argentina.
2. Configurar el nombre del host como “bootcampwebexperto”.
3. Crear un usuario sudo que se llame webexperto.
4. Crear un usuario para conectarse vía ssh.
5. Que actualice las dependencias.
6. Validar si está instalado docker y sino instalarlo.
7. Validar si está instalado docker-compose y sino instalarlo.
8. Crear grupo docker e iniciar el servicio.
9. Instalar mc.
10. Instalar vim.
11. Instalar net-tools.
12. Crear un usuario nginx y dar permisos de docker.

4. Con el usuario nginx, clonar el repositorio que se explica en el siguiente video en la home del usuario. TU SITIO CON SSL GRATIS en DOCKER - Nginx Proxy.
5. Crear un archivo dentro del repositorio de su aplicación web a elección para que muestre el contenido de la misma.
6. Clonar dentro de ese usuario un repositorio suyo con una app dockerizada en compose.
7. Servir con nginx el contenido de la aplicación web en el puerto 80 y que dirija automáticamente al 443 con certificados.

