# proyecto-sql-amedina
Primer proyecto/entregable del Máster de Data &amp; Analytics de ThePower

Lógica y Consultas SQL

INTRODUCCIÓN 

El objetivo de este proyecto es explorar y manipular una base de datos relacional que me han proporcionado. Es una base de datos que muestra un sistema de un videoclub (alquiler del peliculas), incluye información tanto del videoclub (empleados, direcciones, tiendas, clientes, alquileres, inventario, etc...) como de las peliculas (titulos, actores, idiomas, categorias, etc...). En el proyecto se realizan distintas queries/consultas, en base al siguiente enunciado:

[EnunciadoDataProject_SQL.Lógica.pdf](https://github.com/user-attachments/files/18040737/EnunciadoDataProject_SQL.Logica.pdf)

En el enunciado se solicitan, entre otrass cosas:

  - Consultas simples y avanzadas.
  - Uso de relaciones entre tablas mediante JOIN.
  - Implementación de subconsultas, vistas y estructuras temporales.
  - Documentación detallada de las consultas y su interpretación.

SOFTWARE UTILIZADO

  - pgAdmin4
  - DBeaver
    
PASO A PASO

  1. Configuración de la base de datos: Para que todo funcionara correctamente una vez descargada de la web.
  2. Analisis de la base de datos: Antes de empezar a trabajar con las consultas, revisé la base de datos y obtuve el diagrama ER (Con la base de datos abierta y ejecutada, pulsando Ctrl+Másyus+Intro; o click derecho sobre el "public" de la BD, y de nuevo, click, en "Obetener diagrama", para tener una visión más clara de las relaciones entre tablas para hacer las consultas.
  3. Ejecución de consultas: He realizado distintos tipos de consultas, desde las básicas en una sola tabla, hasta consultas en varias tablas mediante varios tipos de JOIN, así como consultas anidadas y CTEs     para casos más complejos. Para todas las consultas, antes de llegar a la respuesta definitiva, he ido haciendo ajustes para comprobar que los datos eran los deseados, esos ajustes han eliminado columnas innecesarias para responder al enunciado de la consulta, pero que si pueden ayudar en una comprensión del paso a paso y más a un nivel principiante

DOCUMENTACIÓN Y ENTREGA

Junto a cada consulta se han ido realizando comentarios explicativos, por simple que sea la consulta, para que se entienda como he llegado a la solución del enunciado, y para que sirva como documentación

Se ha preparado este mismo archivo para una explicación del proyecto

Archivo SQL generado con todas las queries (y enunciados), en un solo documento

ANALISIS DE LA BASE DE DATOS

Algunas tablas de la Base de Datos:

film: Proporciona información sobre las peliculas
category: Muestra las diferentes categorías de las peliculas
actor: Almacena los nombre de los actores que participan en las peliculas
rental: Registra los alquileres del videoclub con fecha y hora
customer: Guarda la información de los clientes del videclub
payment: Proporciona información sobre los pagos de los clientes
... Para ver el resto de tablas, revisa el diagrama ER

Algunas relaciones de la base de datos:

Cada pelicula (tabla film) puede pertener a varias categorias (film_category)
Los alquileres (rental) se vinculan con un cliente (customer) y al inventario (inventory)
Los pagos (payment) se asocian con los alquileres (rental)
... Para ver el resto de relacionces, revisa el diagrama ER

¿CÓMO EJECUTAR LAS QUERIES?

Primero de todo instala el Software mencionado anteriormente
Configura la conexión de la base de datos con ambos programas
Descarga el archivo SQL del repositorio
Importalo a DBeaver, o copia las consultas
Ejecutalas por separado para ver los resultados
** Cada consulta se ha identificado con su numero y enunciado con formato de comentario
Consulta los comentarios para enteder la solución de cada enunciado
Aquí hay un ejemplo de cómo se ven los resultados:

ARCHIVOS INCLUIDOS

  README.md: Este mismo archivo para documentar el proyecto
  Queries_Proyecto.sql: Archivo con todas las consultas comentadas siguiendo el enunciado 
  Esquema_BBDD: Archivo con el diagrama Entidad-Relacion

OBSERVACIONES

  Para poder trabajar con fechas y horas, he tenido que dividir los campos del tipo timestap

  Algunas de las relaciones necesitan un JOIN especifico para asegurar que el resultado de la consulta es el adecuado

¡Gracias por revisar este proyecto!

