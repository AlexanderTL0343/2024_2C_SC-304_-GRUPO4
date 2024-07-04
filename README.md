# 2024_2C_SC-304_-GRUPO4
# 2024_4C_SC-304_HE_K_GRUPO-1
# Componentes visuales y librerías a utilizar en nuestro proyecto 
## Como método de interfaz vamos a utilizar JFrame: 
JFrame es una clase utilizada en Swing para generar ventanas sobre las cuales añadir distintos objetos con los que podrá interactuar o no el usuario. JFrame posee algunas nociones típicas de una ventana como minimizar, cerrar, maximizar y poder moverla.
# Librerías a utilizar: 
## java.util.Date: 
Esta clase representa una instancia específica de fecha y hora. O el paquete java.time en su lugar para trabajar con fechas y horas en Java de manera más efectiva.

## java.util.Scanner: 
La clase Scanner se utiliza para analizar datos de entrada en Java. Proporciona métodos para leer diferentes tipos de datos primitivos y cadenas de texto de una variedad de fuentes de entrada, archivos, o cadenas de texto. Es especialmente útil para dividir y procesar la entrada del usuario.

## javax.swing.JOptionPane: 
JOptionPane es una clase que pertenece al paquete javax.swing y se utiliza para mostrar cuadros de diálogo simples en aplicaciones Java Swing. Estos cuadros de diálogo pueden ser utilizados para mostrar mensajes, pedir al usuario que ingrese datos, o mostrar opciones al usuario.

## java.util: 
El paquete java.util es un conjunto de clases y interfaces de utilidad proporcionadas por Java para realizar diversas tareas comunes, como manejo de colecciones (ArrayList, HashMap, etc.), manipulación de fechas y horas, generación de números aleatorios, escaneo de entrada, entre otros. 

## java.util.ArrayList: 
Esta clase implementa una lista de tamaño variable que proporciona operaciones para agregar, eliminar y acceder a elementos en la lista. Es parte del paquete java.util.

## java.util.HashMap: 
HashMap es una implementación de la interfaz Map que almacena pares clave-valor. Permite el acceso rápido a los valores a través de una clave y no mantiene un orden específico de los elementos. Es eficiente para operaciones de búsqueda, inserción y eliminación de elementos.

## java.util.Random:
La clase Random se utiliza para generar números aleatorios en Java. Proporciona métodos para generar valores aleatorios de diferentes tipos, como enteros, números en coma flotante y valores booleanos. Es útil en aplicaciones que requieren generar datos aleatorios, como juegos, simulaciones y pruebas.

## java.util.regex.Pattern:
Esta clase se utiliza para representar un patrón de expresión regular, que es una secuencia de caracteres que define un conjunto de cadenas de texto. Proporciona métodos para compilar y aplicar expresiones regulares a cadenas de texto para realizar operaciones de coincidencia, búsqueda y reemplazo de texto.

# Plan de proyecto con responsables por tarea (en Git)
| nombre del estudiente | tarea|
|-----------------------|------|
|santiago|Módulo Usuario,CRUD Usuarios,Seguimiento de usuarios,Persistencia en CSV,Árbol comentarios Árbol comentarios,Formulario crear 
|Marvin|Módulo Mensajes,Crear mensajes,Comentar mensajes (árbol binario),Persistencia en CSV,Validaciones,Seleccionar usuario
|Alexander|Módulo Feed,Construir feed con Cola,Mostrar mensajes y comentarios,Destruir cola al finalizar,Formato identado comentarios,Mostrar cola feed
|Sebas|Interfaz Usuarios,Formularios CRUD,Búsqueda y seguimiento,Validaciones,Testing,Integración módulos
|Todos|Interfaz Mensajes,Interfaz Feed 

# Diseño de interfaces
- Inicio
  - Crear Cuenta
  - Iniciar sesion
- Iniciar sesion
  - Correo
  - Contraseña
  - Aceptar
  - Volver
- Crear Cuenta
  - Nombre
  - Apellido
  - Correo
  - Contraseña
  - Aceptar
  - Volver
- Inicio 2
  - Feed
  - Administrar Perfil
  - Cambiar de usuario
- Feed
  - Crear Publicacion
  - Editar Publicacion
  - Eliminar Publicacion
  - Volver
- Administrar Perfil
  - Nombre
  - Editar Perfil
  - Eliminar Cuenta
  - Volver
  - Correo
  - Seguir
  - Dejar De Seguir
  - Usuarios Seguidos
- Dejar De Seguir
  - Correo
  - Aceptar
  - Volver
- Editar Perfil
  - Nombre
  - Apellido
  - Aceptar
  - Volver
- Seguir
  - Correo
  - Aceptar
  - Volver
- Eliminar Cuenta
  - Aceptar
  - Volver
  - Escribir CONFIRMAR
- Crear Publicacion
  - Escribir Publicacion 
  - Volver
  - Publicar
- Editar Publicacion
  - Escribir Publicacion 
  - Volver
  - Publicar
  - ID Publicacion
- Eliminar Publicacion
  - Volver
  - Aceptar
  - ID Publicacion
