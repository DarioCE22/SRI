1. ¿Quién, dónde y cuándo se crea el primer servidor web?
Fue creado por Tim Berners-Lee en el CERN a finales del año 1990.

2. ¿Qué es la pila de protocolos usados por HTTP?
Es el conjunto de protocolos organizados por capas sobre los que se apoya HTTP para transmitir la información:
Capa de Aplicación: HTTP / HTTPS
Capa de Transporte: TCP
Capa de Internet / Red: IP
Capa de Acceso a la Red / Enlace: Ethernet, Wi-Fi, fibra óptica

3. ¿Componentes de una URL?
Tomando como ejemplo https://www.ejemplo.com:8080/tienda/productos.php?categoria=redes&id=5#detalles
Esquema o protocolo: https://
Host o Nombre de dominio (FQDN): www.ejemplo.com
Puerto (opcional): :8080
Ruta (Path): /tienda/productos.php
Cadena de consulta (Query String / Parámetros): ?categoria=redes&id=5
Fragmento (Anchor): #detalles

4. ¿Pasos en la recuperación de una página web mediante HTTP?
El usuario introduce la URL en el navegador.
El navegador realiza una consulta DNS para traducir el nombre de dominio a una dirección IP.
El navegador establece una conexión TCP con el servidor web en esa IP mediante el saludo de tres vías.
El navegador envía un mensaje HTTP Request.
El servidor web localiza o procesa el recurso solicitado y devuelve un mensaje HTTP Response con el código de estado, las cabeceras y el cuerpo del documento HTML.
El navegador interpreta el HTML y solicita recursos adicionales si los hay. Finalmente, se cierra o se reutiliza la conexión.

5. Diferencia entre páginas dinámicas y estáticas:
Páginas estáticas: Son archivos almacenados tal cual en el disco del servidor. El servidor simplemente los lee y los envía al cliente sin modificarlos; todos los usuarios ven exactamente el mismo contenido.
Páginas dinámicas: El contenido se genera "al vuelo" en el momento de la petición mediante un lenguaje de servidor y consultas a bases de datos. El resultado HTML cambia según el usuario, la hora o los datos enviados en un formulario.

6. ¿Cómo usar telnet para acceder a un servidor web?
Abriendo una terminal, conectándose al puerto 80 del servidor mediante el comando telnet <dominio_o_IP> 80 y, una vez conectado, escribiendo manualmente la petición HTTP:
GET / HTTP/1.1
Host: www.ejemplo.com

7. Request. Métodos principales:
GET: Solicita un recurso al servidor
POST: Envía datos en el cuerpo de la petición para ser procesados por el servidor
HEAD: Idéntico a GET, pero solicita únicamente las cabeceras de respuesta, sin el cuerpo de la página
PUT: Sube o reemplaza completamente un recurso en una ruta específica del servidor.
DELETE: Solicita al servidor que elimine un recurso determinado.

8. Response. Códigos de estado:
Se dividen en 5 categorías según su primer dígito:
1xx (Informativos): La petición ha sido recibida y el proceso continúa
2xx (Éxito): La petición fue recibida, entendida y aceptada con éxito
3xx (Redirección): El cliente debe realizar una acción adicional para completar la petición
4xx (Errores del cliente): La petición contiene sintaxis incorrecta o no puede cumplirse
5xx (Errores del servidor): El servidor falló al intentar cumplir una petición válida

9. Content-Type. Tipos principales (MIME Types):
Indican al navegador qué tipo de contenido viaja en el cuerpo del mensaje:
Texto: text/html, text/css, text/plain.
Imágenes: image/jpeg, image/png, image/gif, image/svg+xml, image/webp.
Aplicación / Datos: application/javascript, application/json, application/xml, application/pdf, application/octet-stream
Multimedia: audio/mpeg, video/mp4.
