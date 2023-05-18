1. ¿Qué es una coroutine en Kotlin y cómo se diferencia de un hilo
tradicional?
Las corrutinas nos permiten nos permiten escribir codigo asincrono. A diferencia de un hilo tradicional 
el programador puede decidir cuando se suspende y se reanuda.

2. ¿Cuál es la importancia de la suspensión en las coroutines y cómo se
implementa?
La suspension permite el hilo que estaba siendo utilizado se libera para que otras acciones puedan utilizarlo. Para implementarlas es necesario
agregar las dependencias requeridas, y utilizando la palabra clave "suspend". Para poder ejercutar la funcion suspendida tenemos que utilizar las funciones como launch o async 

3. ¿Cuál es el propósito del Dispatcher en las coroutines y cómo se elige
uno adecuado para cada tarea?

EL dispatcher nos permite seleccionar el hilo en el que se ejecutara una coroutine.Elegir el adecuado dependera de la tarea que 
querramos realizar, el dispatchers.Main nos permite actualizar la interfaz. EL dispatchers.IO para opciones de entrada 
y salida de datos. El dispatchers.Default es util para tareas de computacion intensiva. 

4. ¿Cuál es el propósito y el uso de la función async en las coroutines?

La funcion async es un constructor que nos permite lanzar coroutines de manera asíncrona se obtiene el resultado
utilizando el objeto Deferred, y obtenemos el resultado la función await(). Y es útil cuando se
deben ejecutar tareas concurrentes y combinar los resultados.
