---
id: 8r0v90zcihg21cuazfh4zx0
title: Modelado De Requisitos
desc: ''
updated: 1731443185235
created: 1731443185235
---

- El **modelo de requisitos** es el proceso de crear representaciones visuales de los requisitos de un sistema para facilitar la comprension, comunicacion y validacion de las necesidades de los usuarios
- Utiliza diferentes tipos de diagramas y tecnicas para capturar las funciones, restricciones, procesos y flujos de trabajo del sistema, y permite al equipo de desarrollo traducir estas necesidades en un diseño tecnico y funcional

## Objetivos del modelado de requisitos
- Clarificar y organizar requisitos: Los modelos ayudan a estructurar los requisitos de manera que sea mas facil de entender para todos los involucrados
- Comunicacion efectiva: Permite que los desarrolladores , analistas y usuarios tengan una vision comun de lo que debe hacer el sistema
- Validacion de requisitos: facilita la deteccion temprana de errores o inconsistencias en los requisitos, evitando malentendidos y cambios costosos en etapas avanzadas del proyecto.

## Tecnicas de modelado de requisitos
- Las tecnicas de modelado de requisitos son herramientas y metodos que ayudan a estructurar, visualizar y comprender los requisitos del sistema
- Estas tecnicas facilitan la comunicacion entre los equipos y las partes interesadas asegurando que todos tengan una vision clara de como debe funcionar el sistema

## 1. Diagrama de casos de uso
- Los diagramas de casos de uso son una tecnica visual de modelado que representa como los usuarios (actores) interactuan con un sistema, mostrando las diferentes funcionalidades que ofrece
- Cada funcionalidad o interaccion que el sistema permite se denomina caso de uso
- Los diagramas de caso de uso son utiles en la fase de analisis de requisitos, ya que facilitan la comprension de los objetivos del sistema desde el punto de vista del usuario

### Elementos clave en un diagrama de casos de uso
- Actores: representan a los uaurio y otros sistemas que intractuan con el sistema que estamos modelando. Pueden ser:
  - Primarios: Quieres inician una accion en el sistema (ejemplo , el usuario)
  - Secundarios: Sistemas o personas que apoyan la ejecucion del caso de uso pero no iniciar la accion (ejemplo un sistema de autenticacion)
- Casos de uso: son las funcionalidades o acciones que sistema permite realizar a los actores, como registrar usuario, iniciar sesion o buscar libros. Se representan con un ovalo en el diagrama
- Relaciones:
  - Asociacion: Represnta la initeraccion directa entre un actor y un caso de uso. Se indica con una linea simple que conecta al actor y al caso de uso
  - Include: Representa la inclusion obligatoria de un caso de uso en otro. Se usa cuando un caso de uso necesita la funcionalidad de otro para completarse. Ejemplo el caso de uso de buscar libro inclye mostrar detalles del libro
  - Extend: Represetna una realicon opcional o condicional entre casos de uso. Se usa cuando un caso de uso amplia el comportamiento de otro en situaciones especificar. Ejemplo solicitar renovacion podra extender a reservar libro si  el usuario cumple ciartos criterios
  - Generalizacion: Indica que un actor o caso de uso puede tener subtipos. Ejemplo, un actor usuario podria tener subtipos como usuario regular y administrador.
- Sistema: Se representa mediante un rectagulo que delimita el alcance del sistema y contine los casos de uso. Los actores se colocan fuera del sistema.

Ventajas del diagrama de casos de uso:
- facilita la comunicacion entre usuario, clientes y  desarrolladores
- permite identificar las funcionalidades clave desde el inicio del proyecto
- Proporciona una vision de alto nivel  de las interaccion el sistema
