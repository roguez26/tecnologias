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
```
public class CustomerManager
```
Ejemplo incorrecto:
```
public class customerManager
```

* Se utilizará la convención de nombrado camelCase para el nombramiento de parámetros de los métodos y variables locales.
Ejemplo correcto:
```
public void ProcessOrder(int orderId, string customerName)
{
    int totalItems = 5; 
    double totalPrice = 99.99;
}
```
Ejemplo incorrecto:
```
public void ProcessOrder(int OrderId, string CustomerName)  
{
    int TotalItems = 5;
    double TotalPrice = 99.99; 
}
```
* Cuando se nombre una interfaz se debe de iniciar con una “I” mayúscula.
Ejemplo correcto:
```
public interface IDataProcessor
```
Ejemplo incorrecto:
```
public interface DataProcessor
```
* Los identificadores de variables deben de comenzar con una letra o un guión bajo. A su vez, estos no deben de tener dos guiones bajos debido a que está reservado para los identificadores generados por el compilador y no se debe de usar para separar palabras (“snake_case”).
Ejemplo correcto:
```
private int orderNumber = 123;
private int _tempValue = 0;
```
Ejemplo incorrecto:
```
int __hiddenValue = 100;
string customer_name = "Jane Doe";
```
* Los campos de instancia privados comienzan con un guión bajo y el resto del texto se escribe en camelCase.
Ejemplo correcto:
```
private int _orderCount;
```
Ejemplo incorrecto:
```
private int orderCount;
```
* Usar PascalCase para nombrar miembros públicos de tipo, campos, propiedades, eventos y funciones locales.
Ejemplo correcto:
```
public string CustomerName { get; set; }
```
Ejemplo incorrecto:
```
public int orderCount;
```
* Utilizar PascalCase/UpperCamelCase para el nombrado de constantes, evitar el uso de “Screaming Caps”. 
Ejemplo correcto:
```
public const int MaxItems = 100;
```
Ejemplo incorrecto:
```
public const int MAX_ITEMS = 100; 
```
* Se podrán usar palabras reservadas para nombres de identificadores, solo si es necesario y se deberá de utilizar el prefijo “@”.
Ejemplo correcto:
```
private int @int = 10;
```
Ejemplo incorrecto:
```
private int int = 10;
```
* Utilizar nombres con significado y descriptivos para variables, métodos, clases y espacios de nombre. Evitar el uso de abreviaciones a excepción de las que son nombres.
Ejemplo correcto:
```
private string customerEmailAddress;
```
Ejemplo incorrecto:
```
private string str;
```
* No omitir los modificadores de acceso
Ejemplo correcto:
```
public int orderCount;
```
Ejemplo incorrecto:
```
int orderCount;
```
Los nombres de las clases deben de ser sustantivos simples, completos y singulares.
Ejemplo incorrecto:
```
```
Ejemplo correcto:
```
public class Customer
{
}
public class Data
{
}
```


