---
id: 45qwxe0mg7wmkrncopn7yuj
title: Documento De Requisitos
desc: ''
updated: 1730752718636
created: 1729716081325
---
## Introduccion 
Proposito del documento:

Este docuento tiene como objeticovo descrivir los requisitos funcionales y no funcionales del sistema de reservas de biblioteca. Los requisitos aqui dcoumentados se han elaborado mediante entrevistas y sesiones de validacion con los bibliotecarios, con el proposito de asegurar que el sistema cuba sus necesidades operativas

Alcance del sistema

El sistema permitira gestionar de manera eficiente las reservas y devoluciones de libros, facilitar el seguimiento de l inventario, y enviar notificaciones automaticas. La solucion mejorara la experiencia tanto de los usuario  como del personal bibliotecario


## Requisitos funcionales
RF1. Registro de usuario
- Descripcion: El sistema permitira que los uarios se registren proporcionando su nombre correo elelctronico y una contrasena segura
- Validacion: El sistema verificara que el correo no este registrado previmiente y que la contrasena cmpla con los criterios de seguridad

RF2. Inicio de sesion
- Descripcion: El sistema permitira que los usuarios registrados inician sesion usando su correo y contrasena
- Regla: Si se ingresan credenciales incorrectas res vees, la cuenta se bloqueara temporalmente

RF3.  Busqueda de libros
- Descripcion: Los libros podran buscar libros por titulo, autor o categoria
- Regla: Si no se encuentran libros que coincidan con los criterios, se mostrara un mensaje informativo

RF4. Reserva de libros
- Descripcion: Los usuarios registrados podran reservar libros disponibles y seleccionar una fecha para su recogido 
- ReglasL 
  - Si el libro ya esta reservado, no se permitira otra reserva hasta que se devuelva.
  - El sistema establecea un tiempo limite de 5 dias para recoger la reserva, despues del cual el libro quedara disponible nuevamente

RF5. Gestion de devoluciones
- Descripcion: El bibliotecario podra registrar la devolucion de libros mediante escaneo del codigo de barras o intruccion manual
- Regla: El sistema actualizara la disponibilidad del ibro automaticamente

RF6. Envio de notificaciones
- Descripcion: El sistema enviara notificaciones automaticas cuando:
  - Un libro reservado este listo para ser recogido
  - La reserva este proxima a vencer

RF7. Historial de Reservas
- Descripcion: Los usuarios podran consultar su historial de reservas y ver el estado (pendiente, recodigo, devuleto)
- Regla: Se permitira filtrar las reservas por estado y fecha

RF8. Administracion del inventario
- Descripcion: Los bibliotecarios podran anadir, modificar o eliminar livros del catalogo.
- Regla: Si los datos intrucidos son incompletos, el sistema mostrara un mensaje de error.

3. Requisitos no funcionales

RNF1. Seguridad - autenticacion segura
- Descripcion: El sistema utilizara HTTPS y cifrado de contrasenas para proteger las credenciales de los usuarios
- Regla: si se intenta acceder desde una conexion no segura, se bloqueara la operacion

RNF2. Usabilidad - interfaz intuitiva
- Descripcion: El proceso de busqueda y reserva de libros debe completarse en menos de tres pasos
- Regla: El diseno debe ser intuitivo y accesible desde dispositivos mobiles y navegadores

RNF3. Compatibilidad - Navegadores y dispositivos
- Descripcion: El sistema debe ser compatible con chrome, firefox, safari y funcionar correctamente en dispositivos mobiles.
- Regla: 