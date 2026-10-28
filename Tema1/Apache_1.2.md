1. IfModule

Para qué se usa: Es un contenedor condicional que aplica las directivas que tiene en su interior únicamente si el módulo de Apache especificado está cargado y activo

3. LoadModule
 
Para qué se usa: Carga un módulo dinámico en la memoria de Apache para añadir funcionalidades extra al servidor.

5. Include (o IncludeOptional)   

Para qué se usa: Permite incluir otros archivos de configuración dentro del fichero principal apache2.conf, facilitando una organización modular

6. Directory

Para qué se usa: Agrupa un bloque de directivas que se aplicarán exclusivamente a un directorio físico del sistema de archivos del servidor y a todos sus subdirectorios.

5. Files 

Para qué se usa: Aplica directivas de configuración o control de acceso a archivos específicos según su nombre, independientemente del directorio en el que se encuentren.

6. Location

Para qué se usa: Aplica directivas de configuración en función de la URL solicitada por el navegador

7. VirtualHost

Para qué se usa: Encapsula directivas que se aplican a un sitio web o dominio específico, permitiendo alojar múltiples páginas web distintas dentro de un único servidor Apache.

8. ¿Qué son los ficheros .htaccess?

Son archivos de configuración distribuida por directorio. Permiten modificar el comportamiento de Apache dentro de un directorio concreto y sus subdirectorios sin necesidad de tener permisos de administrador para editar los ficheros principales de /etc/apache2/, y sin tener que reiniciar el servicio Apache para que los cambios surtan efecto. Para que funcionen, la directiva AllowOverride del directorio padre debe estar configurada con un valor distinto de None.   
