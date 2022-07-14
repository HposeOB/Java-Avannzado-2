
# Patrones de diseño

## Patrones creacionales:

* **Factory Method:**
  * Es un patrón que proporciona una interfaz para crear objetos en una superclase, mientras permite a las subclases alterar el tipo de objetos que se crearán. 
  * Se utiliza cuando no conoces las dependencias y los  tipos exactos de objetos con los que trabajarás.
  * Cuando quieras ofrecer a los usuarios de tu biblioteca o framework una forma de extender sus componentes internos. 
  * Cuando quieras ahorrar recursos del sistema mediante la reutilización de objetos existentes en lugar de reconstruirlos cada vez.
  * Es un patrón que evita el acoplamiento.
  * Cumple el principio de responsabilidad única.
  * Cumple el principio de abierto/cerrado.

* **Abstract Factory:**
  * Es un patrón que nos permite producir familias de objetos relacionados sin especificar sus clases concretas.
  * Se utiliza cuando el código debe funcionar con familias de productos relacionados pero no desees que dependa de las clases concretas de esos productos.
  * Puedes tener la certeza de que los productos que obtienes son compatibles entre si.
  * Evitas un acoplamiento fuerte entre productos concretos y el código cliente.
  * Cumple el principio de responsabilidad única.
  * Cumple el principio abierto/cerrado.

* **Builder:**
  * Nos permite construir objetos complejos paso a paso.
  * Nos permite producir distintos tipos y representaciones de un objeto empleando el mismo código de construcción.
  * Se utiliza para eviar tener un constructor telescópico.
  * Construir árboles con el patrón composite u otros objetos complejos.
  * Puedes construir objetos paso a paso, aplazar pasos de la contrucción o ejecutar pasos de forma recursiva.
  * Puedes reutilizar el mismo código de construcción al contruir varias representaciones de productos.
  * Cumple el principio de responsabilidad única.

* **Prototype:**
  * Nos permite copiar objetos existentes sin que el código dependa de sus clases.
  * Se utiliza cuando quieres reducir la cantidad de subclases que solo se diferencian en la forma en la que se inicializan sus propios objetos.
  * Puedes clonar objetos sin acoplarlos a sus clases concretas.
  * Evitas un código de inicialización repetido clonando prototipos prefabricados.
  * Creas objetos complejos con más facilidad.
  * Obtienes una alternativa a la herencia al tratar con preajustes de configuración para objetos complejos.
  
* **Singleton:**
  * Nos permite asegurarnos de que una clase tenga una única instancia, a la vez que proporciona un punto de acceso global a dicha instancia.
  * Se utiliza cuando una clase tan solo deber tener una instancia disponible para todos sus clientes, por ejemplo, un único objeto de base de datos compartido por distinatas partes del programa.
  * Cuando necesitas un control más estricto de las variables locales.
  * Puedes tener la certeza de que una clase tiene una única instancia.
  * Obtienes un punto de acceso global a dicha instancia.
  * El objeto singleton solo se inicializa cuando se requiere por primera vez.
  
## Patrones estructurales:

* **Adapter:**
  * Permite la colaboración entre objetos con interfaces incompatibles.
  * Se utiliza cuando quieres reutilizar varias subclases existentes que carezcan de alguna funcionalidad común que no pueda añadirse a la superclase.
  * Cumple el principio de responsabilidad única.
  * Cumple el principio de abierto/cerrado.

* **Bridge:**
  * Permite dividir una clase grande o un grupo de clases estrechamente relacionadas, en dos jerarquías separadas (abstracción e implementación) que pueden desarrollarse independientemente la una de la otra.
  * Se utiliza cuando quieres dividir y organizar una clase monolítica que tenga muchas variantes de una sola funcionalidad (por ejemplo, si la clase trabaja con varios servidores de bases de datos).
  * Cuando necesitas extender una clase en varias dimensiones ortogonales (independientes).
  * Cuando necesitas poder cambiar implementaciones durante el tiempo de ejecución.
  * Puedes crear clases y aplicaciones independientes de la plataforma.
  * El código cliente funciona con abstracciones de alto nivel.
  * Cumple el principio de responsabilidad única.
  * Cumple el principio de abierto/cerrado.

* **Composite:**
  * Permite componer objetos en estructuras de árbol y trabajar con esas estructuras como si fueran objetos individuales.
  * Se utiliza cuando quieres que el código cliente trate elementos simples y complejos de la misma forma.
  * Todos los elementos definidos por el patrón Composite comparten la misma interfaz común.
  * Puedes trabajar con estructuras de árbol complejas con mayor comodidad: utiliza el poliformismo y la recursión a tu favor.
  * Cumple el principio abierto/cerrado.
  
* **Decorator:**
  * Permite añadir funcionalidades a objetos colocando estos objetos dentro de objetos encapsuladores especiales que contienen estas funcionalidades.
  * Se utiliza cuando necesitas asignar funcionalidades adicionales a objetos durante el tiempo de ejecución sin descomponer el código que utililza esos objetos.
  * Cuando resulte extraño o no sea posible extender el comportamiento de un objeto utilizando la herencia.
  * Puedes extender el comportamiento de un objeto sin crear una nueva subclase.
  * Puedes añadir o eliminar responsabilidades de un objeto durante el tiempo de ejecución.
  * Puedes combinar varios comportamientos envolviendo un objeto con varios decoradores.
  * Cumple el principio de responsabilidad única. Puedes dividir una clase monolítica que implementa muchas variantes posibles de comportamiento, en varias clases más pequeñas.
  
* **Facade:**

  
