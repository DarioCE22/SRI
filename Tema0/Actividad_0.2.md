| Característica | TCP (Transmission Control Protocol) | UDP (User Datagram Protocol) |
| :--- | :--- | :--- |
| **Conexión** | Orientado a conexión (requiere saludo inicial). | No orientado a conexión (envía sin avisar). |
| **Fiabilidad** | Fiable: garantiza que los datos lleguen mediante acuses de recibo (ACK) y retransmite paquetes perdidos. | No fiable: no confirma la recepción ni reenvía paquetes perdidos (Best effort). |
| **Orden** | Garantiza que los paquetes se entreguen en el mismo orden en que se enviaron (usa números de secuencia). | Los datagramas pueden llegar desordenados. |
| **Velocidad y Sobrecarga** | Más lento, mayor sobrecarga (cabecera mínima de 20 bytes) y control de flujo/congestión. | Muy rápido, baja latencia y ligero (cabecera fija de solo 8 bytes). |
---
2. ¿Qué aplicaciones usan TCP?
Aplicaciones donde la integridad de los datos es crítica y no se puede perder ni un solo byte:
HTTP / HTTPS
SMTP, POP3, IMAP
SSH y Telnet
FTP / SFTP

3. ¿Qué aplicaciones usan UDP?
Aplicaciones en tiempo real o consultas rápidas donde prima la velocidad sobre la pérdida ocasional de algún paquete:
DNS
DHCP
Streaming de vídeo/audio en directo y VoIP
Videojuegos online multijugador.
NTP y TFTP.

4. ¿Qué capa almacena el puerto?
La Capa de Transporte

5. ¿Qué capa almacena la dirección IP?
La Capa de Red o Capa de Internet

6. ¿Qué es el Three-way handshake?
Es el mecanismo de negociación en tres pasos que utiliza TCP para sincronizar y establecer una conexión fiable entre cliente y servidor antes de empezar a enviar datos:
SYN (Synchronize): El cliente envía un segmento SYN al servidor solicitando iniciar la conexión e indicando su número de secuencia inicial
SYN-ACK (Synchronize-Acknowledge): El servidor recibe la petición, acepta abrir la conexión y responde con un segmento SYN-ACK, confirmando el paquete del cliente y enviando su propio número de secuencia
ACK (Acknowledge): El cliente confirma la respuesta del servidor enviando un segmento ACK. En este instante la conexión queda establecida y comienza la transferencia de datos.
