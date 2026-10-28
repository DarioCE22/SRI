¿Qué es cURL?
cURL es una herramienta de línea de comandos y librería diseñada para transferir datos desde o hacia un servidor utilizando una gran variedad de protocolos de red sin necesidad de utilizar un navegador gráfico.

5 Ejemplos prácticos de uso de cURL

Obtener el código fuente HTML de una página web (Petición GET básica):
Descarga y muestra por pantalla el contenido del recurso indicado:
<img width="1284" height="808" alt="image" src="https://github.com/user-attachments/assets/0dd2a429-8b35-4e11-936c-514ee42bb7d0" />

Mostrar únicamente las cabeceras HTTP de respuesta (-I o --head):
Realiza una petición HEAD para inspeccionar el código de estado, el tipo de servidor y las cabeceras sin descargar el cuerpo HTML:
<img width="1278" height="803" alt="image" src="https://github.com/user-attachments/assets/72cf4d4d-4fbe-41d4-acd9-88550bb0e62e" />

Descargar y guardar el archivo en nuestro equipo (-o / -O):
Con -o guardamos la salida con el nombre que elijamos:
<img width="1287" height="801" alt="image" src="https://github.com/user-attachments/assets/545f4e5a-d79b-4c7a-a769-0aac23f88b0a" />

Seguir redirecciones automáticamente (-L o --location):
Si un servidor devuelve un código 301 o 302 (por ejemplo, de http a https o sin www a con www), la opción -L hace que curl siga la redirección hasta llegar a la página final:
<img width="1285" height="805" alt="image" src="https://github.com/user-attachments/assets/619d9db2-9256-4e0a-9f94-3e1e53523989" />

Enviar datos mediante una petición POST (-X POST -d):
Permite simular el envío de un formulario o datos JSON a una API o servidor web:
<img width="1286" height="801" alt="image" src="https://github.com/user-attachments/assets/8ca00d5f-c439-4b73-b7ef-79321f70103f" />
