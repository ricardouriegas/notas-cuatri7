---
id: udse3f1jf6apgthkhau89wr
title: Actividad1
desc: ''
updated: 1728939459619
created: 1728592829446
---
## Funcional
- Pantalla de Login
  - Botón de olvide mi contraseña
  - Botón de olvide mi correo
  - Botón de registro
  - Botón de enviar formulario
- Pantalla modificar perfil
  - Modificar/añadir número telefónico
  - Modificar contraseña
- Pantalla de registro
  - Pedir correo
  - Contraseña

## No Funcional
- Barra de búsqueda para buscar el libro necesario
- Al buscar, que aparezca el catálogo de libros
- Menú al desplegar un libro
  - Sinopsis del libro
  - Revisar disponibilidad del libro
  - Portada del libro
- Que permita realizar una solicitud 
  - Solicitar fecha de salida y entrada

## No funcional
- Verificación de correo.
- Recuperación de contraseña después de tres intentos fallidos.
- Que aparezcan los libros más destacados hasta arriba.
- La fecha no puede ser más de 1 mes

## Sistema de reservas de libros en una bibliotea
### Requisitos funcionales
1. Registro de usuario
   - El sistema debe permitir a los usuarios registrarse proportcionando su nombre correo electronico credenciales de acceso
2. Iniciar sesion
   - Los usurios registrados deben poder iniciar sesion en el sistema con su correo electronicao y contrasena
3. Busqueda de libros:
   - Los usuariods debenpoder buscar libros por titulo, autor  o el catalogo de la biblioteca
4. Reserva de libros 
   - El sistema debe permitir a los usuarios reservar libros disponibles para recogerlos en la bibilioteca en una fecha determinada
5. Notificacion:
   - El sistema debe de enviar notificaciones por el corrreo electronico cuando la reserva este lista para recogerse o cuando un libro reservado este disponible
6. Historial de reserva
   - Los usuarios deben poder ver el historial de sus reservas anteriores y su estado (pendiente, recogido, devuelto)
7. Administracion de invetnario:
   - Los bibliotecarios deben poder añadir, eliminar o modificar  los registros de libros disponibles 
8. Devoluciones de los libros:
   - El sistema debe de registrar la devolucion de libros por parte de los usarios y actualizar la disponibilidad de los libros en el catalogo.

### Requisitos no funcionales
1.Seguridad:
   - El sistema debe implementar autenticacion segura (por ejemplo HTTPS y  encriptacion de contraseñas) para proteger la informacion de los usuarios
2. Rendimiento:
   - El sistema debe ser capaz de gestionar hasta 1000 consultas simultaneas de busquedas sin comprometer la velocidad de respuesta.
3. Disponibilidad
   - El sistema debe estar disponible el 99.9% del tiempo con un maximo de 1 hora de inactividad al mes
4. Usabilidad:
   - La interfaz debe ser intuitiva y facil de usar, permitiendo a que lo suaurios encuentren y reserven libros en menos de 3 pasos 
5. Compatibilidad
   - El sistema debe ser compatible con los navegadores web mas utilizados (chrome, firefox y safari) y con dispositivos moviles
6. Escalabilidad
   - El sistema dbe eser capaz de apliarse para soportar hhasta 10,000 usuarios simiultaneos sin afectur su rendimiento
7. Tiempos de respuest  
   - Las consultas de busqueda deben devolver resultados en menos de 2 segundos 
8. Cumplimiento legal
   - El sistema debe de cumplir con las regulaciones locales de proteccion de datos, como ley de proteccion de datos personales (GDPR en la union Europea o equivalente en la region)