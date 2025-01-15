# Pagura.Valentin.Final.Java.2024
Aplicación de Gestión de Productos
Descripción General
Esta aplicación es un sistema de gestión de inventario desarrollado en JavaFX que permite administrar diferentes tipos de productos (Electrónicos y Alimentos) en un entorno gráfico intuitivo. La aplicación implementa operaciones CRUD (Crear, Leer, Actualizar y Eliminar) para gestionar el inventario de manera eficiente.
Estructura del Proyecto
La aplicación está organizada en varias clases principales:
Clases Base

Producto (Abstracta): Clase base que define las propiedades comunes de todos los productos:

ID
Nombre
Precio
Stock
Método abstracto getCategoria()



Clases de Productos

Alimento:

Hereda de Producto
Atributos adicionales:

Fecha de vencimiento
Indicador de producto perecedero




Electronico:

Hereda de Producto
Utiliza el enum TipoElectronico para categorizar los productos en:

COMPUTADORA
TELEFONO
TABLET
TELEVISION
ELECTRODOMESTICO
OTRO





Gestión de Datos

GestorDeProductos: Implementa la interfaz CRUD para manejar las operaciones sobre los productos
Interfaz CRUD: Define las operaciones básicas (crear, leer, actualizar, eliminar)

Interfaz Gráfica y Funcionalidades
Ventana Principal
La interfaz principal muestra:

Una tabla con las columnas:

ID
Nombre
Precio
Stock
Categoría


Panel lateral con botones:

Agregar Producto
Eliminar Producto
Actualizar Producto



Operaciones Principales
1. Agregar Producto
Al hacer clic en "Agregar Producto":

Se abre una ventana modal
Permite seleccionar el tipo de producto (Electrónico o Alimento)
Campos para ingresar:

Nombre
Precio
Stock
Campos específicos según el tipo de producto



2. Actualizar Producto
Para actualizar un producto:

Seleccionar el producto en la tabla
Clic en "Actualizar Producto"
Se abre una ventana modal con los datos actuales
Modificar los campos deseados
Confirmar la actualización

3. Eliminar Producto
Para eliminar:

Seleccionar el producto en la tabla
Clic en "Eliminar Producto"
Confirmar la eliminación en el diálogo de confirmación

Manejo de Errores
La aplicación incluye:

Validación de campos numéricos
Mensajes de error claros
Confirmación antes de eliminar productos
Manejo de excepciones para productos duplicados

Características Técnicas

Desarrollado en JavaFX
Uso de Properties para binding bidireccional
Implementación de patrones de diseño:

Herencia
Polimorfismo
Interfaz CRUD


Manejo de tipos enumerados
Interfaz gráfica responsiva

Instrucciones de Uso

Iniciar la aplicación
Para agregar productos:

Clic en "Agregar Producto"
Seleccionar tipo
Llenar los campos requeridos
Confirmar


Para modificar:

Seleccionar producto en la tabla
Clic en "Actualizar Producto"
Modificar campos
Guardar cambios


Para eliminar:

Seleccionar producto
Clic en "Eliminar Producto"
Confirmar eliminación
