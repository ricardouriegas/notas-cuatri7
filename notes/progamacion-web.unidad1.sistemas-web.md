---
id: os35f1dcnqehv4blblfhyl5
title: Sistemas Web
desc: ''
updated: 1728395102928
created: 1727875166335
---
## Objetivo

El alumno configurara entornos de trabajo para desarrollar web.

## Temas

1. Introduccion a la Programacion Web
2. Configuracion de Servidores de Desarrollo Web
3. Configuracion de Servidores de Produccion

## Modelo Cliente-servidor

Estructura distribuida que divide tareas (o cargas de trabajo) entre proveedores de recursos o servicios (servidores) y los que solicitan los servicios (clientes)

![alt text](image.png)

## Internet

Conjunto descentralizado de redes de comunicacion interconectadas utilizan las familias de protocolos TCP/IP.

Es la red de redes, es decir, una red que no solo interconecta computadoras sino que tambien interconecta redes de computadoreas entre si.

### Origenes del Internet

El origen de internet data desde 1969 con la primera interconexion de computadoras conocida como Arpanet, entre tres universidades en Carolina (USA).

### Importancia del internet

A supuesto una revoluccion sin precedentes en el mundo de la informatica y de las comunicaciones.

Oportunidad de difusion mundialm un mecanismo de propagacion de la informacion y un medio de colaboracion e interaccion entre individuos y los ordenadores independientes de su localidad geografica.

## Que es la intranet
Red informatica que hace uso de la tecnologia del protocolo de internet para compartir informacion, sistemas operativos o servicios computacionales dentro de una organizacion

## Dominio de internet
Red de identificacion asociada a un frupo de dispositivos o equipos conectados a la red de Internet.

El proposito principal de los nombres de dominio en Internet y el sistema de nombres de dominio (DNS), es traducir las direcciones IP de cada nodo activo en la red a terminos momorizables y faciles de encontrar.

## World Wide Web
Sistema de distribucion de documentos de hipertexto o hipermedios interconectados y accesibles via internet

Desarrollado enre marzo de 1989 y 1990 por Tim Berners-Lee en el CERN en Ginebra, Suiza.

## Hypertext Transfer Protocol | HTTP

Protocolo de Transferencia de Hipertexto.

Protocolo de capa de aplicacion para la transmision de documentos de hipermedia (como HTML).

Diseñado para la comunicacion entre navegadores y servidores web, pero es de proposito general.

Sigue el modelo cliente-servidor.

Utiliza el puerto 80.

### Hypertext Transfer Protocol Secure | HTTPS
Version segura del protocolo HTTP que utiliza el protocolo SSL/TLS para cifrado.

Agrega cifrado, autenticacion e integridad al protocolo 

Utiliza el puerto 443.

## File Transfer Protocol | FTP
Protocolo de transferencia de archivos.

Es un protocolo usado en la capa de aplicacion

Es inseguro porque no esta cifrado.

Su version segura | cifrada es FTPS.

Los puertos que utiliza son:
- Puerto 21: para el control de la conexión (comandos).
- Puerto 20: para la transferencia de datos en modo activo.

## TCP/IP
Grupo de protocolos de red que haven posible la transferencia de datos en redes entre equipos informaticos e internet.

### TCP
Protocolo de control de trannsmision que permite establecer una conexion y el intercamvio de datos entre dos anfitrione. este protocolo proporciona un transporte fiable de datos

### IP
Protocolo de internet, untiliza direcciones en series de cuatro  octetos con formato de punto decimal (como por ejemplo '75.4.160.25'). Este protocolo lleva datos a otras maquinas de la red.

## Uniform Resource Identifier (URI)
Identificador de recursos uniforme
- Cdena de caracteres que identifica recursos en una red
- Los recursos son accesibles en una red o sistema

![alt text](image-1.png)

## Pagina web
Es una fuente de informacion adaptaba para la WWW y  accesibel mediante un navegador de internet.

Se presenta generalmente en formato HTML y puede contener hiperenlaces a otras paginas web, constituyendo la red enlazada de la WWW.

## Sitio Web
- Conjunto de paginas web tipicamente comunes a un dominio de Internet o subdominio en la WWW en internet
- Su principal objetivo es entregar informacion
- Consumir el contenido es la tarea mas importante 
- Tienen varias paginas interconectadas y comunmente tienen un gestor de contenidos.

## Aplicacion Web
- Tiene como objetivo que el usuario realice una tarea o un proceso.
- Tambien puede referirse como un programa se utiliza desde el navegador.
- Ejemplos: servicios de banca en linea. Google drive, sitios de venta de retail, etc.

## Portal web
Es un sitio web cuya caracterisitca fundamental es la de serir de puerta de entrada (unica) para ofrecer al usuario, de forma facil e integrada el acceso a una serie de recursoss y de servicios relacionados a un mismo tema.

## Diferencias entre sistios web y aplicaciones web

Sitio Web | Aplicacion Web
--- | ---
Los sitios web son fuentes de informacion, mientras que las aplicaciones se centran en la realizacion de acciones | Una aplicaion web puede ser parte de un sitio en un proyecto pero no alreves. <br> Las funciones y tareas de una aplicacion son muchas mas y tienen un nivel de complejidad mas elevadas.

### HyperText Markup Language | HTML
- Lenguaje de mercado de hipertexto
- Se usa para la elaboracion de paginas web 
- Permite las estructuracion las paginas con un lenguaje basado en etiquetas.

## Cascading Style Sheets | CSS
Lenguaje e diseño para definir y crear la presentacion de un documento estructurado escrito en HTML.

Creado para separa r el contenido del documento y la forma en que se presenta.

## JavaScript | JS
- Lenguaje de programacion interpretado
- Codigoque se usa principalmente del lado del cliente, porque lo puede ejeuctar el navegador
- Permite mejoras en la interfaz del usuario
- Estandas ECMAScript

## Tencologias / Lenguajes del Lado del Servidor
- PHP
  - Laravel | Symfony | CodeIgniter | CakePHP
- ASP .NET (ASP .NET)
  - ASP .NET MVC | Razos Pages | Web API
- Python
  - Django | Flask | Fast API
- Java
  - JSP | Spring Boot
- JavaScript (Node JS)
  - ExpressJS | NestJS

## Funcionamiento de la web
El priemr paso consiste en traducir la parte nombre del servidor de la URL en una direccion IP usando la bse de datos distribuida de internet conocida como DNS. Esta direccion IP es necesaria para contactar con el servidor web y poder enviarle paquetes de datos.

## Funcionamiento de la WEB
El siguiente paso es enviar uuna peticion HHTP al servidor web solicitando el recurso. En el caso de una pagina web tipica primero ses solicita el texto HTML y luego es imediatmamente analizado por el navegador, el cual, despues hace peticiones adicionalespara los graficos y otros ficheros que formen parte de la pagina.

Al recibir los ficheros solicitados desde el servidor web, el navegador represente (renderiza) la pagina tal y como se descruibe en el codigo HTML, el CSS y otros lenguajes web.


## Configuracion de Servidores de Desarrollo Web
### Servidor Web
Progama informatico que procesa una apliacion del lado del sservifor realizando conexiones bidireccionales y/o unidireccioinales sincronas o asincronas con el cliente y generados o cediendo una respuesta en cualquier lengaje o aplicacion del lado del cliente.

### Servidor Web - Ejemplos 
- Apache
- Cherokee 
- Nginx 
- IIS (Internet Information Services)
- Lighttpd 
- Kestrel 

```HTML
<!-- Peticion get -->
<form action="pagina.php" method="get">
  <input type="text" name="nombre">
  <input type="submit" value="Enviar">
</form>
```
