---
id: udse3f1jf6apgthkhau89wr
title: Actividad1
desc: ''
updated: 1728592833071
created: 1728592829446
---
# Sistema de Reservación de Libros en una Biblioteca

## 1. Funcionalidades que debe tener el sistema (Requisitos Funcionales):

### Registro de Usuarios
- Permitir a los usuarios registrarse con una cuenta.
- Autenticación mediante nombre de usuario y contraseña.
- Permitir la recuperación de contraseñas.

### Búsqueda de Libros
- Motor de búsqueda avanzado que permita encontrar libros por:
  - Título
  - Autor
  - ISBN
  - Categoría
  - Año de publicación
- Filtrado por disponibilidad en la biblioteca.

### Consulta de Disponibilidad
- Ver si un libro está disponible o actualmente prestado/reservado.
- Ver las fechas de devolución estimadas para los libros que están prestados.

### Reservación de Libros
- Permitir a los usuarios reservar un libro que esté disponible.
- Opción de hacer cola para libros prestados (espera en lista).
- Notificación cuando el libro reservado está disponible para recoger.

### Gestión de Préstamos
- Ver historial de préstamos y reservas activas.
- Renovación automática o manual de préstamos, si el libro no tiene más reservas.
- Cancelación de reservas si ya no es necesario.

### Notificaciones y Recordatorios
- Notificaciones por correo electrónico o SMS sobre:
  - Fecha de devolución próxima.
  - Disponibilidad de un libro reservado.
  - Recordatorios para renovar o devolver un libro.

### Perfil del Usuario
- Gestión de información personal (correo electrónico, dirección, etc.).
- Ver multas o sanciones por devoluciones tardías.

### Integración con Catálogo Digital
- Acceso a libros electrónicos (si el servicio está disponible).
- Permitir la descarga o el préstamo digital de materiales electrónicos.

### Gestión por Parte del Bibliotecario
- Agregar, eliminar o actualizar libros en el sistema.
- Gestión de reservas, historial de usuarios y préstamos.

### Reportes y Estadísticas
- Generar reportes sobre:
  - Libros más solicitados.
  - Historial de préstamos por usuario.
  - Datos de ocupación de los libros.

---

## 2. Características de calidad importantes (Requisitos No Funcionales):

### Usabilidad
- Interfaz intuitiva y fácil de usar, tanto para usuarios como para bibliotecarios.
- Adaptación a dispositivos móviles (diseño responsivo).
- Fácil acceso a la información con el menor número de clics.

### Rendimiento
- Tiempos de carga mínimos al buscar libros o consultar información.
- Manejo eficiente de grandes volúmenes de datos.

### Disponibilidad
- El sistema debe estar disponible 24/7 para que los usuarios puedan hacer reservas en cualquier momento.
- Tolerancia a fallos para evitar tiempos de inactividad.

### Seguridad
- Protección de datos personales y de la privacidad de los usuarios.
- Autenticación segura y cifrado de contraseñas.
- Prevención contra ataques como SQL injection o accesos no autorizados.

### Escalabilidad
- Capacidad de crecimiento a medida que aumentan los usuarios o libros en el catálogo.
- Integración de nuevas funcionalidades sin afectar el rendimiento.

### Mantenibilidad
- Código fácil de actualizar y mantener.
- Documentación clara para futuras modificaciones o adiciones al sistema.

### Compatibilidad
- Compatible con diferentes navegadores web y sistemas operativos.
- Integración con sistemas existentes, como gestión de préstamos físicos o catálogos externos.

### Accesibilidad
- Cumplimiento de estándares de accesibilidad para personas con discapacidades (ej. navegación por teclado, compatibilidad con lectores de pantalla).

---

## Discusión en Grupo y Presentación de Resultados:

### Preguntas clave para discutir en grupo:
1. ¿Qué funcionalidades serían esenciales y cuáles opcionales para la biblioteca específica?
2. ¿Qué características de calidad son más prioritarias para la implementación inicial del sistema?
3. ¿Cómo asegurar la facilidad de uso y escalabilidad del sistema a medida que se expande la biblioteca?
4. ¿Qué tecnologías o plataformas serían más adecuadas para garantizar el rendimiento y la seguridad del sistema?

### Presentación de resultados:
- Exponer las funcionalidades acordadas y cómo mejoran la experiencia de los usuarios.
- Resaltar las características de calidad y justificar su priorización (seguridad, rendimiento, etc.).
- Proponer un plan de acción para la implementación inicial y abordar posibles desafíos de escalabilidad y mantenimiento.
