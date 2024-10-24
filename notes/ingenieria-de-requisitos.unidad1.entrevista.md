---
id: ugw5xjya7isrjb9crcv572e
title: Entrevista
desc: ''
updated: 1729714250818
created: 1729627576982
---
## Elicitacion de requisitos: Identifiacacion de necesidades

- La elicitacion de requisitos es una fase critica del desarrollo de sisteamas en la cual se identifican y capturan las necesidades y expectativas de los skateholders (usuario finales, clientes equipo tecnico, etc.)
- Su objetivo es asegurar que el sistema final cumpla con los requerimientos reales
- Existen varias tecnicas para recopilar estos requisitos, y entre mas comunes se encuentran las entrevistas, cuestionarios y prototipos.

## Identifiacacion de las necesidades

Antes de iniciar el procesode elicitaciono, es fundamental comprender quienes son los stakeholders y cuales son sus intereses. Por ejemplos de necesidades pueden incluir:

- Optimizacion de procesos 
- Solucion a problemas actuales
- Automatizacion de tareas manuales
- Cumplimiento normativo o legal

El objetivo es transformar estas necesidades en requisitos claros y comprensibles. La calidad de los requisitos es determinante para el exito del proyecto.

## Tecnicas de elicitacion
### 1. Entrevistas
Las entrevistas son una tecnica directa de recopilaciono de informacion, donde un analista interactua con los stakeholders para conocer sus necesidades

#### Tipos de entrevistas:
- Estructuradas: Preguntas predefinidas, similares para todos los entrevistas
- Semi-estructuradas: Combinand preguntas preparadas con la libertad de explorar otras areas segun avance la conversacion
- No estructuradas: Conversion abierta donde los temas surgen organicamente

#### Ventajas:
- Permiten obteneer informaicon detallada y especifica
- Facilitan la contruccion de relaciones con los stakeholders

#### Desventajas:
- Consumen tiempo 
- La calidad de los resultados depende de la habilidad del entrevistador

#### Ejemplo
Un analista entrevista a los bibliotecarios para conocer las necesidades del sistema de reservas, identifiacando cuantos ejemplares tienen disponibles y como gestionan las devoluciones.

#### Fase 1: Preparacion de la entrevista
El analista define el objetivo de la entrevista y prepara las preguntas clave para asegurarse de cubrir todos los aspectos relevantes.

Objetivos:
Identifiacar los procesos actuales de gestion de reservas, prestamos y devoluciones, asi como las principales necesidades y expectativas del sistema.

#### Preguntas predefinidas
Sobre las reservas:
- Como gestionan las reservas actualmente?
- Cuantos libros se pueden reservar al mismo tiempo por usuario?
- Cuales son los criterios para reservar un libro? (por ejemplo, disponibilidad, fecha limite)

Sobre los prestamos y devoluciones:
- Como registran actualmente las devoluciones de libros?
- Que sucede si un usuario no devuelve un libro a tiempo?
- Como manejan los libros danados o perdidos?

Sobre la disponibilidad:
- Que porcentaje de libros suele estar reservado o prestado en un momento dado?
- Con que frecuencia actualizan el inventario de libros?
- Les gustaria una funcion que notifique automaticamente la devolucion de libros?

#### Realizacion de la entrevista
Dialogo simulado:
- Analista: "Buenos dias, podria explicarme como llevan a cabo las reservas actualmente?"
- Bibliotecario 1: "Ahora lo hacemos de forma manua. Registramos la solicitud en una hoja de calculo y marcamos si el libro este disponible o no"
- Analista: "Han tenido problemas con la disponibilidad de libros?"
- Bibliotecario 2: "Si, a veces los usuarios reservan libros que ya estan prestados, lo que genera confusion"
- Analista: "Que les pareceria si el sistema pudiera bloquear automaticamnete la reserva de un libro que ya esta prestado?"
- Bibliotecario 1: "Eso seria ieal. Evitaria errores y nos ahorraria mucho trabajo"
- Analista: "Como gestionan actualmente las devoluciones de libros?"
- Bibliotecario 2: "Escanemaos el codigo de barras del libro, pero a veces tenemoms problemas si no se puede leer"
- Analista: "les gustaria que el sistema permitiera una opcion manual para estos casos?"
- Bibliotecario 1: "Si, definitivamente seria util"

## Redaccion de requisitos
- Requisito 1: El sistema debe impedir la reserva de un livro que ya este prestado o reservado
- Requisito 2: El sistema debe permitir registrar devoluciones mediante un escaneo, con opcion manual en caso de error en el codigo 
- Requisito 3: El sistema debe enviar notificaciones automaticas a los usuarios cuando una reserva este lista para ser recogida
- Requisito 4: El sistema debe limitar la cantidad de reservas simultaneas por usuairo a un maximo de 3 libros

### Validacion de requisitos ocn los bibliotecarios
La validacion de requiasitos es una fase crucial en la ingenieria de requisitos para asegurarse de que las necesidades identificadas se alinean correctamente con las expectativas y el contexto del usuario ( en este caso, los bibliotecarios). Esto minimiza malentendidos y errores antes de comenzar con el desarrollo del sistema.

#### Pasos para la validacion de requisitos con los bibliotecarios
1. Preparar el documento de requisitos

    El analista crea un documento que incluye los requisitos funcionales y no funcionales extraidos de las entrevistas. Cada requisitos debe ser claro, detallado y comprensible para los bibliotecarios

    - Requisitos funcionales:
      - RF1; El sistema debe bloquear automaticamente la reserva de libros que ya esten preparados 
      - RF2: El sistema debe permitir registrar devoluciones mediante escaneo y opcion manual en caso de error 
      - RF3: Se enciara una notificacion automatica cuando un libro reservado este listo para ser recogido 
    - Requisitos no funcionales:
      - RNF1: La interfaz del sistema debe ser intuitiva y accesible desde dispositivos moviles y navegadores web
      - RNF2: Las reservas deben realizarse en menos de 3 pasos.

2. Planificar la sesion de validacion

    El analista organiza una reunion con los bibliotecarios para discutir los requisitos. Esta sesion puede ser presencial o virtual

    - Objetivos de la sesion:
      - confirmar que los requisitos reflejan correctamente las necesidaes
      - Identificar requisitos adicionales o realizar ajustes si es necesario
      - Detectar incosistencias, ambiguedades o requisitos inalcanzables
    - Materiales necesarios
      - Documento de requisitos
      - Protoptipos o bocetos de la interfaz, si estan disponibles
      - Lista de preguntas para validar la comprension

### Realizacion de la sesion de validacion
- Dinamica de la reunion
  - IntroduccionL El analista explica el objetivo de la sesion y como se organizara
  - Revision de requisitos: El analista lee cada requisito y explica su proposito
  - Analista: "Les parece adecuado que el sistema bloquee automaticamente la reserva de libros que ya estan prestados?"
  - Bibliotecario 1: "Si, eso es justo lo que necesitamos"

- Discusion de posibles ajustes:
  - Bibliotecario 2: Seria util que el sisstema tambien nos mostrara una lista de libros proximos a ser devueltos"
  - Analista: Perfecto. Incluire ese requisito en la lista final
- Identificacion de riesgos:
  - Bibliotecario 1: " A veces los usuarios no recogen los libros reservados, Poremos establecer un tiempo limite para la reserva?
  - Analista: Esa es una buena sugerencia. Agregaremos esa funcionalidad.

### Ajustar los requisitos identificados
- Con base en los comentarios obtenidos durante la sesion, el analista hace los ajustes necesarios. Algunos cambios podrian incluir:
  - Agregar requisitos: 
    - El sistema debe permitir establecer un tiempo limite para recoger reservas
  - Modificar requisitos
    - Añadir una lista de libros proximos a ser devueltos para facilitar la gestion

### Obtener la aprobacion formal
- Una vez ajustados los requisitos, se elabora una version final del documento
- El analista lo envia a los bibliotecarios para su revision y aprobacion final

**Seguimiento posterior**

- El analista se asegura de estar disponible para resolver dududas adicionales y programar futuras validacion es si surgen cambios en los requistos durante el desarrollo del proyecto

# Actividades pendientes

- [ ] pantalla de inicio
- [ ] implementar ver transacciones en el modo admin
- [ ] hacer la tabla de reporte en la pagina de devolver libro (cuando le des a devolver libro debe mostrar la tabla para que tu hagas el repo?rte; si esta roto entonces no se aumenta la cantidad disponible, sino pues si aumenta)
- [ ] En la base de datos; 3 dias habiles para ir por el libro cuanod se reserva
- [ ] mandar un correo cuando se hace la reserva mostrando el rango de tiempo que puedes por el libro
- [ ] cuando le de reservar un boton de verificacion y verificar que no halla mas de 3 reservas pendientes hechas por el usuario
- [ ] _que la pantalla del catalogo se divida en paginas_