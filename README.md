# semaforosSO
Codigos sobre semaforos en Python y C++


Repositorio acerca de las barreras en python, primero se importa el módulo de hilos de Python y la función sleep del módulo de tiempo. Además, se define un objeto mutex (bloqueo mutuo) que se usa para sincronizar el acceso a una variable compartida.

La clase Hilo se define como una subclase de threading.Thread, lo que significa que cada objeto Hilo es un subproceso que se puede ejecutar simultáneamente con otros subprocesos. Cada objeto Hilo tiene una propiedad "id" que se establece en la creación del objeto.

La función "run" se define para cada objeto Hilo y se ejecuta cuando se llama al método "start" del objeto. El método "acquire" del objeto mutex se llama al principio de la función "run" para bloquear el acceso a la variable compartida "d". Luego, el hilo llama a la función sleep con un valor que depende del valor de su propiedad "id". Finalmente, el hilo imprime un mensaje que muestra su propiedad "id" y el valor actual de "d".

Fuera de la definición de la clase Hilo, se define la variable "d" con un valor de 1 y se crea una lista de tres objetos Hilo con diferentes valores de "id". Luego, se inicia cada hilo en la lista con el método "start", lo que hace que cada hilo ejecute su función "run" en paralelo con los otros hilos.


Video explicativo.

Python: https://youtu.be/6Ej4hOZdKBk

Barreras usando hilos: https://youtu.be/h7EZS91UjUw

C: 
