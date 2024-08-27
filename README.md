# Estándar de codificación para Tecnologías de Software

## Introducción

El propósito del presente estándar es establecer un conjunto de reglas y guías que sirvan como pauta para la consistencia, claridad y calidad del código en el proyecto que se va a realizar durante el curso actual. Estas reglas fueron seleccionadas para facilitar la lectura, el mantenimiento y la seguridad del código, y al mismo tiempo, minimizar los errores y que se mejore la colaboración entre los desarrolladores. Este estándar cubre aspectos clave como el nombrado de variables, constantes, clases, métodos, propiedades y namespaces. Estilo e indentación, basados en la guía que Microsoft provee para el lenguaje C#; así como, el uso de comentarios, el uso correcto de estructuras de control, manejo de excepciones, niveles de logueo y prácticas seguras de construcción.

## Propósito 

### Propósito general

El propósito general del presente trabajo es crear un estándar de codificación para el lenguaje de programación C# que sirva como guía para el equipo durante la construcción del proyecto de software “NOMBRE DEL PROYECTO”, asimismo, que permita a externos entender las reglas de estilo y decisiones de construcción que se tomaron.

### Propósitos específicos
* Definir reglas claras y consistentes de sintaxis, nomenclatura y estilo para la codificación.
* Fomentar la legibilidad y la comprensión del código.
* Promover la coherencia y la calidad del código en todo el proyecto.

### Reglas de nombrado
* Se utilizará la convención de nombrado PascalCase/UpperCamelCase para el nombramiento de **clases**, **interfaces**, **structs**, **delegates**, **constantes** y **nombres de métodos**

Ejemplo correcto:
`public class CustomerManager`
Ejemplo incorrecto:
`public class customerManager`

* Se utilizará la convención de nombrado camelCase para el nombramiento de parámetros de los métodos y variables locales.
Ejemplo correcto:
`public void ProcessOrder(int orderId, string customerName)
{
    int totalItems = 5; 
    double totalPrice = 99.99;
}`
Ejemplo incorrecto:
`public void ProcessOrder(int OrderId, string CustomerName)  
{
    int TotalItems = 5;
    double TotalPrice = 99.99; 
}`
