Ejercicio 1: Crea un directorio llamado dir1 y otro llamado dir2
<img width="1258" height="794" alt="image" src="https://github.com/user-attachments/assets/1bb0d9f5-d214-4712-a881-73ab6299aa20" />

Ejercicio 2: Diferencia entre ambos bloques y su equivalencia con Require

Se evalúan primero las directivas Deny y después las Allow

Como en Apache gana la última regla que coincida y por defecto lo que no coincida se permite, solo el equipo 192.168.1.100 tendrá acceso permitido y el resto será denegado.

Equivalencia en Apache 2.4 con Require:

Directory /var/www/example1
    
  Require ip 192.168.1.100
    
/Directory

Bloque 2 (Order Allow, Deny):

Se evalúan primero las directivas Allow y en segundo lugar las Deny

Al evaluarse Deny from All al final, machaca el permiso anterior y deniega el acceso a absolutamente todo el mundo

Equivalencia en Apache 2.4 con Require:

Directory /var/www/example1

  Require all denied

/Directory

Ejercicio 3: Configuración para dir1 (a, b, c y d)
<img width="1263" height="799" alt="image" src="https://github.com/user-attachments/assets/0c4127bb-a880-4160-bd1c-43a7b2e79f27" />

Ejercicio 4: Acceso a dir1 permitido a marisma.intranet pero NO desde 10.3.0.101
<img width="1258" height="809" alt="image" src="https://github.com/user-attachments/assets/586bd21b-c776-4a32-b870-908321603214" />

Ejercicio 5: Acceso a dir2 permitido a 10.3.0.100/8 pero NO a marisma.intranet
<img width="1267" height="792" alt="image" src="https://github.com/user-attachments/assets/9230679d-bca6-4816-839f-1a551295a050" />
