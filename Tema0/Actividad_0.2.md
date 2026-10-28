| Característica | TCP (Transmission Control Protocol) | UDP (User Datagram Protocol) |
| :--- | :--- | :--- |
| **Conexión** | Orientado a conexión (requiere saludo inicial). | No orientado a conexión (envía sin avisar). |
| **Fiabilidad** | Fiable: garantiza que los datos lleguen mediante acuses de recibo (ACK) y retransmite paquetes perdidos. | No fiable: no confirma la recepción ni reenvía paquetes perdidos (Best effort). |
| **Orden** | Garantiza que los paquetes se entreguen en el mismo orden en que se enviaron (usa números de secuencia). | Los datagramas pueden llegar desordenados. |
| **Velocidad y Sobrecarga** | Más lento, mayor sobrecarga (cabecera mínima de 20 bytes) y control de flujo/congestión. | Muy rápido, baja latencia y ligero (cabecera fija de solo 8 bytes). |
