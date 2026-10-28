1. Directivas de identificación

- ServerName
  
  Uso: Define el nombre de dominio y el puerto que el servidor utiliza para identificarse a sí mismo.
  
  Valor por defecto: No tiene un valor activo por defecto.
  
  Dónde se define: En los archivos de cada sitio virtual

- ServerAdmin
  
  Uso: Dirección de correo electrónico del administrador que Apache incluye en los mensajes de error enviados al cliente.
  
  Valor por defecto: webmaster@localhost.
  
  Dónde se define: /etc/apache2/sites-available/000-default.conf.

- ServerTokens
  
  Uso: Controla qué información sobre el servidor se envía en la cabecera Server: de las respuestas HTTP.
  
  Valor por defecto: Full
  
  Dónde se define: /etc/apache2/conf-available/security.conf.

3. Directivas de localización de ficheros

- DocumentRoot
  
  Uso: Directorio raíz del sistema de ficheros desde el cual Apache sirve los documentos web al público.

  Valor por defecto: /var/www/html.

  Dónde se define: /etc/apache2/sites-available/000-default.conf.

- ErrorLog

  Uso: Especifica la ruta del archivo donde Apache registra todos los errores de diagnóstico y fallos de procesamiento.
  
  Valor por defecto: ${APACHE_LOG_DIR}/error.log
  
  Dónde se define: /etc/apache2/apache2.conf y puede personalizarse dentro de /etc/apache2/sites-available/000-default.conf.

- CustomLog

  Uso: Establece la ruta y el formato del archivo de registro donde se guardan todas las peticiones realizadas al servidor.
  
  Valor por defecto: ${APACHE_LOG_DIR}/access.log combined
  
  Dónde se define: /etc/apache2/sites-available/000-default.conf.

- ServerRoot

  Uso: Directorio base donde se alojan los ficheros de configuración, errores y registros principales del servidor Apache.
  
  Valor por defecto: "/etc/apache2".
  
  Dónde se define: /etc/apache2/apache2.conf

6. Directivas de control de la conexión

- Timeout

  Uso: Tiempo máximo que Apache espera por la recepción o envío de paquetes durante una petición antes de dar la conexión por fallida.
  
  Valor por defecto: 300
  
  Dónde se define: /etc/apache2/apache2.conf.

- KeepAlive

  Uso: Habilita o deshabilita las conexiones HTTP persistentes
  
  Valor por defecto: On.
  
  Dónde se define: /etc/apache2/apache2.conf.

- MaxKeepAliveRequests

  Uso: Número máximo de peticiones permitidas durante una única conexión persistente antes de cerrarla
  
  Valor por defecto: 100.
  
  Dónde se define: /etc/apache2/apache2.conf.

- KeepAliveTimeout

  Uso: Tiempo que Apache esperará por la siguiente petición de un mismo cliente en una conexión persistente antes de cerrar la conexión.
  
  Valor por defecto: 5
  
  Dónde se define: /etc/apache2/apache2.conf.

7. Otras directivas

- LogLevel

  Uso: Controla el nivel de detalle de los mensajes que se registran en el archivo ErrorLog
  
  Valor por defecto: warn.
  
  Dónde se define: /etc/apache2/apache2.conf.

- LogFormat

  Uso: Define la estructura o plantilla de datos que utilizará la directiva CustomLog al escribir en los archivos de acceso.
  
  Valor por defecto: Define los alias combined, common, referer y agent
  
  Dónde se define: /etc/apache2/apache2.conf.
