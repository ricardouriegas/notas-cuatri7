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

---

## Casos de uso funcionales
### Caso de uso 1: Registro de usuarios
- **Actor**: Usuario no registrado
- **Precondicion**: El usuario no debe tener una cuenta registrada en el sistema
- **Descripcion**: Permitir que un usuario se registre en el sistema proporcionando su nombre, correo electronico y una contraseña segura.
#### Flujo principal
1. Elsuaurio  accede al formualrio de regsitro 
2. El usuario introduce su nombre. correo electronico y contraseña
3. El sistema valida que el correo no este registrado previamente
4. El sistema valida la complejidad de la contraseña
5. El sistema almacena los datos y envia un correo verificacion
6. El usuario recibe el correo y confirma su cuenta haciendo clic en el enlace de activacion
#### Excepciones
- 3a .El correo ya esta registrado: El sistema muestra un mensaje de error
- 4a. La contraseña no cumple con los criterios: El sistema solicita una contraseña mas segura

**Postcondicion**: El usuario se registra con exito y puede inicia sesion despues de verificar su cuenta por correo

### Caso de uso 2: Iniciar sesion
- **Actor**: Usuario registrado
- **Precondicion**: El usuario debe haberse resgistrado previemente haber confirmado su cuenta
- **Descripcion**: Permitir que un usuario registrado inicie sesion en el sistema usando su correo electronico y contraseña
#### Flujo principal
1. El usuairo accede a la pagina de inicio de sesion 
2. Intrudce su correo electronico y contrasema
3. El sistema valida las credenciales
4. El sistema otorga acceso a la cuenta del usuaria

#### Excepciones
- 3a. Credenciales incorrectas: El sistema muestra un mensaje de error
- 3b. El usuario intenta iniciar sesion multiples veces con credenciales oncorrectas: El sistema bloquea temporalmente la cuenta.

**Postcondicion**: El usuario inicia sesion exitosamente y accede a su cuenta

### Caso de uso 3: Busqueda de libros
- **Actor**: Usuario registrado
- **Precondicion**: El catalogo de libros debe de estar disponible en el sistema
- **Descripcion**: Permitir que los usuarios busquen libros por titulo, autor o categoria en el catalogo de la biblioteca
#### Flujo principal
1. El usuario accede al catalogo de libros
2. El usuario introduce el criterio de busqueda (titulo, autor, categoria)
3. El sistema muestra una lista de libros que coinciden con el criterio de busqueda
4. El usuario selecciona un libro para ver mas detalles.

#### Excepciones
- 3a. No se encuentran libros que coincidan con el criterio: El sistema muestra un mensaje indicando que no hay resultados.

**Postcondicion**: El usuario viualiza los resultados de la busqueda y puede acceder a la informacion del libro.

### Caso de uso 4: Reserva de libros
- **Actor**: Usuario registrado
- **Precondicion**: El usuario debe haber iniciado sesion en el sistema. El libro debe de estar disponble para reserva
- **Descripcion**: Permitir que los usuarios reserven libros disponibles para recogerlos en la biblioteca en una fecha determinada

#### Flujo principal
1. El suaurio busca un libro y lo selecciona
2. El sistema muestra si el el libro esta disponible para reservar
3. El usuario selecciona la opcion de "Reserva"
4. El sistema solicita al usuario elegir una fecha de recogida
5. El sistema confirma la reserva del libro y muestra la fecha de recogida.

#### Excepciones 
- 2a. El libro no esta disponible: El sistema muestra un mensaje indicando que el libro no esta disponible para
- 5a. El usuario no selecciona una fecha de recogida: El sistema no permite proceder con la reserva

**Postcondicion**: El usuario ha reservado el libro exitosamente y puede recogerlo en la fecha seleccionada.

### Caso de uso 5: Notificaciones
- **Actor**: Sistema. Usuario registrado
- **Precondicion**: El usuario debe haber realizado una reserva o estar en una lista de espera
- **Descripcion**: El sistema debe enviar notificaciones automaticas por correo electronico cuando una reserva este lista para recogerse o cuando un libro reservado este disponible

#### Flujo principal
1. El usuario reserva un libro
2. El sistema monitorea el estado de la reserva
3. Cuando el libro esta disponible para recogida, el sistema envia una notificacion por correo electronico al usuario
4. El usuario recibe el correo y procede a la bibilioteca a recoger el libro

#### Excepciones
- 4a. El correo no se entrega correctamente: El usuario no recibe la notificacion pero puede consultar el estado de su reserva en el sistema

**Postcondicion**: El usuario recibe una notificacion por correo electronico cuando su reserva esta lista

### Caso de uso 6: Historial de reservas
- **Actor**: Usuario registrado
- **Precondicion**: El usuario debe haber iniciado sesion en el sistema y tener un historial de reservas
- **Descripcion**: Permitir que los usuarios consulten su historial de reservas, incluyendo el estado de cada una (pendiente, recogido, devuelto).

#### Flujo principal
1. El usuairo accede a su cuenta
2. El usuario selecciona la opcion "historial de reservas"
3. El usuario muestra una lista de todas las reservas realizada por el usuario, junto on su estado 
4. El usaurio puede filtrar las reservas por estado o fecha

#### Excepcciones
- 3a. El usuario no tiene reservas en su historial. El sisteam muestra un mensaje indicando que no hay reservas

**Postcondiciion**: El usuario consulta el historial de reservas

### Caso de uso 7: Administracion de invetarios
- **Actor**: Bibliotecario
- **Precondicion**: El Bibiliotecario debe haber iniciado sesion en el sisteam con permito de administracion
- **Descripcion**: Permitir a los bibliotecarios añadir, lliminar o modificar los registrados de libros desponibles en el catalogo de la biblioteca

#### Flujo principal
1. El bibliotecario accede a la seccion de adminstracion de invetarios
2. El bibliotecario selecciona la opcion de "añadir", "eliminar" o "modificar" un libro
3. El sistema solicita los detalles del libro
4. El bibliotecario intrudce o actualiza la informacion requerida
5. El sistema confirma la accion y actualiza el catalogo de libros

#### Excepciones
- 3a. El bibliotecario introduce datos incorrectos o incompletos. El sistema muestra un mensaje de error y no permite continuar

**Postcondicion**: El bibliotecario gestiona el catalogo de libros de la biblioteca

### Caso de uso 8: Devoluciones de los libros
- **Actor**: Usuario registrado, bibliotecario
- **Precondicion**: El usuario debe haber tomado prestado un libro y estar en proceso de devolucion
- **Descripcion**: Registrar la devolucion de libros por parte de los usuarios y actualizar la disponibilidad de los libros en el catalogo

#### Flujo principal
1. El usuario acude a la bilioteca para devolver un libro
2. El bibliotecario escanea el codigo de barras del libro 
3. El sistema actualiza el estado del libro a "disponible" en el catalogo
4. El sistema notifica al usuario que la devolucion ha sido exitosa

#### Excepciones
- 2a El sistema no puede leer el codigo de barras: El bibliotecario ingresa manuealmente la informacion

**Postcondicion**: El libro se devuelve correctamente y se actualiza la disponibilidad en el catalogo

## Caso de uso no funcionales
### Caso de uso 1: Seguridad - Autenticacion segura
- **Actor**: Usuario, Sistema
- **Precondicion**: El sistema debe tener certificados HTTPS y protocolos de seguridad activos
- **Descripcion**: Proteger las credenciales de los usuarios mediante autenticacion segura y encriptacion de contraseñas

#### Flujo principal
1. El usuario accede a la pagina de inicio de sesion mediante un elace HTTPS
2. El usuario introduce su correo y contraseña
3. El sisteam encripta las credenciales antes de enviarlas al servidor
4. El servidor verifica las credenciales y permite el acceso al usuario

#### Excpeciones
- 2a. Si la conexion no es segura, el sistema bloquee la operacion y muestra un mensaje de alerta
- 3a. Si la contraseña se ingresa incorrectamente mas de 3 veces, el sistema bloquea la cuenta temporalmente

**Postcondicion**: El usuario accede al sistema de manera segura sin comprometer la informacion personal

### Caso de uso 2: Rendimiento - Manejo de consultas simultaneas
- **Actor**: Usuario, Sistema
- **Precondicion**: El sistema debe ser capaz de gestionar multiples consultas simultaneas
- **Descripcion**: Garantizar que el sistema pueda manejar hasta 1000 consultas simultaneas sin comprometer la velocidad de respuesta

#### Flujo principal
1. Los usuario acceden al sistema y realizan consultas de busqueda
2. El sistema proesa todas las solicitudes simultaneamente utilizando recursos optimizados del servidor
3. Los resultados se develven a cada usuario en tiempo real sin interrupciones

#### Excepciones
- 2a. Si el limite de consultas se supera, el sistema distribuye la carga en un servidor alterno

**Postcondicion**: Las busquedas se completan sin comprometer la velocidad de respuesta

### Caso de uso 3: Disponibilidad - Alta disponibilidad del sistema
- **Actor**: Usuario, sistema
- **Precondicion**: El sistema debe tener configuraciones de respaldo y monitorieo
- **Descripcion**: Garantizar que el sistema este disponible el 99.9% del tiempo con un maximo de 1 hora de inactividad al mes

#### Flujo principal
1. El sistema monitorea su disponibilidad continuamente
2. Si se deteca una posible falla, el sistema activa un servidor de respaldo automaticamente
3. El administrador recive notificaciones si se produce un  caida inesperada

#### Excepciones
- 2a. Si el sisteam excede la hora de inactividad mensual, se despliega un mensaje explicando la situacion al usuario

**Postcondicion**: El sistema se mantiene operativo caso todo el tiempo sin afectar a los usuarios

### Caso de uso 4: Usavilidad- interaaz intuitiva
- **Actor**: Usuario
- **Precondicion**: El sistema debe estar diseñado con principio s de UX/UI simples
- **Descripcion**: Los usuarios deben encontrar y reservar libros en menos de 3 pasos

#### Flujo principal
1. El usuario accede al catalogo de libros desde la pagina principal
2. Intruduce el titulo o autor del libro en la barra de busqueda
3. Selecciona el ibro hace clic en "Reservar"

#### Excepciones
- 3a. Si el proceso de reserva escede los tres pasos, se detecta como un problema de usabilidad

**Postcondicion**: El usuario completa la reserva de forma sencilla y rapida

### Caso de uso 5: Compatibilidad - Navegadores y dispositivos