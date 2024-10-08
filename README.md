# 2024_2C_SC-304_-GRUPO4
# Componentes visuales y librerías a utilizar en nuestro proyecto 
## Integrantes
- Alexander Torres Lopez
- Marvin Gago Reyes
- Andrey Ureña Chaves
## Como método de interfaz vamos a utilizar JFrame: 
JFrame es una clase utilizada en Swing para generar ventanas sobre las cuales añadir distintos objetos con los que podrá interactuar o no el usuario. JFrame posee algunas nociones típicas de una ventana como minimizar, cerrar, maximizar y poder moverla.
# Librerías a utilizar: 

## java.io.FileWriter:
se utiliza para escribir datos orientados a caracteres en un archivo . Es una clase orientada a caracteres que se utiliza para el manejo de archivos en Java. 

## java.io.IOException: 
Indica que se ha producido algún tipo de excepción de E/S. Esta clase es la clase general de excepciones producidas por operaciones de E/S fallidas o interrumpidas.

## java.util.Date: 
Esta clase representa una instancia específica de fecha y hora. O el paquete java.time en su lugar para trabajar con fechas y horas en Java de manera más efectiva.

## java.util.Scanner: 
La clase Scanner se utiliza para analizar datos de entrada en Java. Proporciona métodos para leer diferentes tipos de datos primitivos y cadenas de texto de una variedad de fuentes de entrada, archivos, o cadenas de texto. Es especialmente útil para dividir y procesar la entrada del usuario.

## javax.swing.JOptionPane: 
JOptionPane es una clase que pertenece al paquete javax.swing y se utiliza para mostrar cuadros de diálogo simples en aplicaciones Java Swing. Estos cuadros de diálogo pueden ser utilizados para mostrar mensajes, pedir al usuario que ingrese datos, o mostrar opciones al usuario.

## java.util: 
El paquete java.util es un conjunto de clases y interfaces de utilidad proporcionadas por Java para realizar diversas tareas comunes, como manejo de colecciones (ArrayList, HashMap, etc.), manipulación de fechas y horas, generación de números aleatorios, escaneo de entrada, entre otros. 

## java.util.HashMap: 
HashMap es una implementación de la interfaz Map que almacena pares clave-valor. Permite el acceso rápido a los valores a través de una clave y no mantiene un orden específico de los elementos. Es eficiente para operaciones de búsqueda, inserción y eliminación de elementos.

## java.util.Random:
La clase Random se utiliza para generar números aleatorios en Java. Proporciona métodos para generar valores aleatorios de diferentes tipos, como enteros, números en coma flotante y valores booleanos. Es útil en aplicaciones que requieren generar datos aleatorios, como juegos, simulaciones y pruebas.

# Plan de proyecto con responsables por tarea (en Git)
| nombre del estudiante | tarea|
|-----------------------|------|
|Marvin Gago Reyes|Lista de Participantes,Listado de Eventos,Registro de Resultados,Consulta de Participantes,Consulta de Resultados
|Alexander Torres Lopez| Registro de Eventos,Actualización y Eliminación de Eventos,Registro de Participantes,Actualización y Eliminación de Participantes
|Andrey Ureña Chaves|Programación de Partidos,Calendario de Partidos,Historial de Resultados,Consulta de Eventos
|Todos|Grafo de Equipos, Árbol de Clasificación 
# Diagrama de clases 
# Clases:
1.	Usuario
  - Estática: No
  - Atributos:
    - Privados:
        - nombre: String
        - email: String
        - tipoUsuario: String (puede ser "administrador" o "espectador")
  - Métodos:
  	- Públicos:
         - getNombre(): String
          - getEmail(): String
         - getTipoUsuario(): String
         - setNombre(nombre: String): void
         - setEmail(email: String): void
         - setTipoUsuario(tipoUsuario: String): void
2.	Evento
   - Estática: No
   - Atributos:
       - Privados:
          - nombre: String
          - fecha: Date
          - ubicacion: String
          - participantes: DoubleLinkedList<Participante>
          - partidos: Queue<Partido>
   - Métodos:
     - Públicos:
       - getNombre(): String
       - getFecha(): Date
       - getUbicacion(): String
       - getParticipantes(): DoubleLinkedList<Participante>
       - getPartidos(): Queue<Partido>
       - setNombre(nombre: String): void
       - setFecha(fecha: Date): void
       - setUbicacion(ubicacion: String): void
       - addParticipante(participante: Participante): void
       - removeParticipante(participante: Participante): void
       - addPartido(partido: Partido): void
        - removePartido(partido: Partido): void
3.	Participante
  -	Estática: No
  -	Atributos:
    - Privados:
        -	nombre: String
        -	edad: int
        -	equipo: String
  -	Métodos:
    -	Públicos:
          -	getNombre(): String
          -	getEdad(): int
          -	getEquipo(): String
          -	setNombre(nombre: String): void
          -	setEdad(edad: int): void
          -	setEquipo(equipo: String): void
4.	Partido
  -	Estática: No
  - Atributos:
    -	Privados:
        -	evento: Evento
        -	participantes: List<Participante>
        -	fecha: Date
  -	Métodos:
     - Públicos:
          -	getEvento(): Evento
          -	getParticipantes(): List<Participante>
          -	getFecha(): Date
          -	setEvento(evento: Evento): void
          -	setParticipantes(participantes: List<Participante>): void
          -	setFecha(fecha: Date): void
5.	Resultado
  -	Estática: No
  -	Atributos:
    -	Privados:
          -	partido: Partido
          -	participante: Participante
          -	puntuacion: int
  -	Métodos:
    -	Públicos:
        -	getPartido(): Partido
        -	getParticipante(): Participante
        -	getPuntuacion(): int
        -	setPartido(partido: Partido): void
        -	setParticipante(participante: Participante): void
        -	setPuntuacion(puntuacion: int): void

# Diseño de interfaces
1. Gestión de Eventos
- Registro de Eventos:
  - Campos: Nombre, Fecha, Ubicación, Lista de Participantes (selector múltiple)
  - Botones: Guardar, Cancelar
- Listado de Eventos:
  - Tabla con columnas: Nombre, Fecha, Ubicación, Participantes, Acciones (Editar, Eliminar)
- Actualización de Eventos:
  - Similar al formulario de registro con datos precargados.
- Eliminación de Eventos:
  - Confirmación antes de eliminar.
2. Gestión de Participantes
- Registro de Participantes:
  - Campos: Nombre, Edad, Equipo
  - Botones: Guardar, Cancelar
- Listado de Participantes:
  - Tabla con columnas: Nombre, Edad, Equipo, Acciones (Editar, Eliminar)
- Actualización de Participantes:
    - Similar al formulario de registro con datos precargados.
- Eliminación de Participantes:
    - Confirmación antes de eliminar.
3. Programación de Eventos
- Programación de Partidos:
  - Campos: Evento (selector), Equipos (selector múltiple), Fecha, Hora
  - Botones: Guardar, Cancelar
- Calendario de Partidos:
  - Vista de calendario con partidos programados (eventos por día)
4. Resultados de Partidos
- Registro de Resultados:
  - Campos: Evento (selector), Partido (selector), Resultado
  - Botones: Guardar, Cancelar
- Historial de Resultados:
  - Lista de resultados en orden inverso (último partido jugado primero)
5. Consulta de Participantes
- Búsqueda de Participantes:
  - Campo de búsqueda
  - Botón: Buscar
- Lista de Participantes:
  - Tabla con columnas: Nombre, Edad, Equipo
6. Consulta de Eventos
- Lista de Eventos:
  - Tabla con columnas: Nombre, Fecha, Ubicación
  - Botón: Ver Detalles
- Detalles del Evento:
  - Información del evento
  - Lista de Participantes
  - Calendario de Partidos
7. Consulta de Resultados
- Lista de Resultados:
  - Selección de evento
  - Lista de resultados por evento
8. Grafo de Equipos
- Visualización del Grafo:
  - Gráfico interactivo mostrando nodos (equipos) y aristas (partidos jugados)
9. Árbol de Clasificación
- Visualización del Árbol Binario:
  - Gráfico interactivo mostrando la clasificación de equipos por victorias
- Consideraciones Técnicas
- Interfaz Amigable:
  - Uso de colores y tipografías claras.
  - Diseño responsivo.
  - Persistencia de Datos:
  - Utilización de archivos para almacenar datos.
- Desempeño:
  -   Optimización de las operaciones para manejar grandes cantidades de datos eficientemente
