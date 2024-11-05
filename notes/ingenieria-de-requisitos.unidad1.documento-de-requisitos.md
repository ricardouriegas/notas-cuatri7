---
id: 45qwxe0mg7wmkrncopn7yuj
title: Documento De Requisitos
desc: ''
updated: 1730838129119
created: 1729716081325
---
# Sistema de Reservas de Biblioteca.
## 1. Introducción
### Propósito del documento:
Este documento tiene como objetivo describir los requisitos funcionales y no funcionales del *Sistema de Reservas de Biblioteca*. Los requisitos aquí documentados se han elaborado mediante entrevistas y sesiones de validación con los bibliotecarios, con el propósito de asegurar que el sistema cubra sus necesidades operativas.

### Alcance del sistema:
El sistema permitirá gestionar de manera eficiente las reservas y devoluciones de libros, facilitar el seguimiento del inventario, y enviar notificaciones automáticas. La solución mejorará la experiencia tanto de los usuarios como del personal bibliotecario.

## 2. Requisitos Funcionales
*RF1. Registro de Usuarios:*
* *Descripción:* El sistema permitirá que los usuarios se registren proporcionando su nombre. correo electrónico y una contraseña segura.
* *Validación:* El sistema verificará que el correo no esté registrado previamente y que la contraseña cumpla con los criterios de seguridad.

*RF2. Inicio de Sesión:*
* *Descripción:* El sistema permitirá que los usuarios registrados inicien sesión usando su correo y contraseña.
* *Regla:* Si se ingresan credenciales incorrectas tres veces. La cuenta se bloqueará temporalmente.

*RF3. Búsqueda de Libros:*
* *Descripción:* Los usuarios podrán buscar libros por título, autor o categoría.
* *Regla:* Si no se encuentran libros que coincidan con los criterios, se mostrará un mensaje informativo.

*RF4. Reserva de Libros:*
* *Descripción:* Los usuarios registrados podrán reservar libros disponibles y selccionar una fecha para su recogida.
* *Reglas:* 
    * Si el libro ya esta resevado, no se permitirá otra reserva hasta que se devuelva.
    * El sistema establecerá un *tiempo límite de 5 días* para recoger la reserva, después del cual el libro quedará disponible nuevamete.

*RF5. Gestión de Devoluciones:*
* *Descripción:* El bibliotecario podrá registrar la devolución de libros mediante escaneo del código de barras o introducción manual.
* *Regla:* El sistema actualizará la disponibilidad del libro automáticamente.

*RF6. Envío de Notificaciones*
* *Descripción:* El sistema enviará notificaciones automáiticas cuando: 
    * Un libro reservado esté listo para ser recogido.
    * La reserva esté próxima a vencer.

*RF7. Historial de Reservas*
* *Descripción:* Los usuarios podrán consultar su historial de reservas y ver el estado (pendiente, recogido, devuelto).
* *Regla:* Se permitirá filtrar las reservas por estado y fecha.

*RF8. Administración del inventario*
* *Descripción:* Los bibliotecarios podrán añadir, modificar o eliminar libros del catálogo.
* *Regla:* Si los datos introducidos son incompletos, el sistema mostrará un mensaje de error.

## 3. Requisitos No Funconales
*RNF1. Seguridad - Autenticación segura*
* *Descripción:* El sistema HTTPS y cifrado de contraseñas para proteger las credenciales de los usuarios.
* *Regla:* Si se intenta acceder desde una conexión no segura, se bloqueará la operación.

*RNF2. Usabilidad - Interfaz Intuitiva*
* *Descripción:* El proceso de búsqueda y reserva de libros debe completarse en *menos de tres pasos.*
* *Regla:* El diseño debe ser intuitivo y accesible desde dispositivos móviles y navegadores.

*RNF3. Compatibilidad - Navegadores y Dispositivos*
* *Descripción:* El sistema debe ser compatible con *Chrome, **Firefox, **Safari* y funcionar correctamente en dispositivos móviles.
* *Regla:* Si no se encuentran libros que coincidan con los cirterios, se mostrara un mensaje informativo.

*RNF4. Escalabilidad - Manejo de Usuarios Simultáneos*
* *Descripción:* El sistema debe soportar hasta *10,000* usuarios simultáneos sin afectación del rendimiento.

*RNF5. Rendimiento - Respuesta rápida*
* *Descripción:* Las consultas de búsqueda deben devolver resultados en *menos de 2 segundos*.

*RNF6. Alta disponibilidad*
* *Descripción:* El sistema debe estar disponible el *99.9% del tiempo, con un máximo de **1 hora de inactividad* mensual.

*RNF7. Cumplimiento Legal - Protección de Datos*
* *Descripción:* El sistema debe cumplir con normativas de protección de datos personales, permitiendo que los usuarios soliciten la eliminación de su información en cualquier momento.

## 4. Casos de Uso Principales
*CU1: Registro de Usuario*
* *Actor:* Usuario no registrado
* *Descripción:* El usuario se registra porporcionando sus datos personales y recibe un correo de activación para confirmar su cuenta.

*CU2: Reserva de Libro*
* *Actor:* Usuario registrado
* *Descripción:* El usuario busca un libro, verifica su disponibilidad y selecciona una fecha para la recogida.

*CU3: Devolución de Libro*
* *Actor:* Bibliotecrio 
* *Descripción:* El bibliotecario registra la devolución mediante escaneo del código de barras o entrada manual.

*CU4: Envío de notificaciones*
* *Actor:* Sistema
* *Descripción:* El sistema envía notificaciones automáticas cuando una reserva está lista para ser recogida.

## 5. Riesgos identificados
* *R1:* El usuario no recoge el libro reservado tiempo.
  * *Mitigación:* Se establecerá un tiempo límite para las reservas.
* *R2:* El sistema no lee correctamente el código de barras.
  * *Mitigación:* Se habilitará la opción de registro manual de devoluciones.
* *R3:* Sobrecarga del servidor en horas pico.
  * *Mitigación:* Se implementarán servidores de respaldo para distribuir la carga.

## 6. Aprobación del Documento
Este documento ha sido revisado y validado con los bibliotecarios. Con la aprobación de está versión, se procederá al desarrollo del sistema de reservas.

| Nombre | Rol | Firma | Fecha |
| :-|:-|:-|:-|
| Bibliotecario 1 | Responsable de reservas | | 
| Bibliotecario 2 | Encargado de Inventario | | 
| Analista de Sistemas | Encargado del Proyecto | |

## 7. Conclusión
Este documento refleja los requisitos funcionales y no funcionales para el sistema de reservas de biblioteca. La implementación de este sistema permitirá optimizar la gestión de reservas, devoluciones e inventario, mejorando la experiencia del usuario y del personal de la biblioteca.

## 8. Anexos
* Prototipo de la interfaz (si aplica)
* Diagrama de Casos de Uso (si aplica)
* Manual preliminar del Usuario (si aplica)