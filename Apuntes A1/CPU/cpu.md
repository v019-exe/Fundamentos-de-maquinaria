# Resumen de qué es el CPU

## CPU (Central Processing Unit)

El CPU es el cerebro del ordenador, donde se llevan a cabo la mayoría de las operaciones de procesamiento.

### Componentes del CPU

- Unidad de Control (UC)
+ Coordina y controla todas las operaciones del CPU
+ Interpreta las instrucciones del programa y emite señales para dirigir otras partes del procesador

- Unidad Aritmético-Lógica (UAL) o (ALU)
+ Realiza operaciones matemáticas (Suma, resta, multiplicación y división) y lógicas (AND, OR, NOT, XOR)
+ Se encarga de los cálculos y la manipulación de los datos

- Registros
+ Son pequeñas unidades de almacenamiento dentro del CPU, que guardan datos e instrucciones temporalmente.
+ Permiten un acceso rápido a los datos que están siendo procesados, esto acelera el procesamiento y rendimiento del CPU.

- Caché
+ Memoria de alta velocidad que almacena temporalmente datos e instrucciones que se usan con frecuencia.
+ Mejora el rendimiento al reducir el tiempo de acceso a la memoria principal.

## Funcionamiento del CPU

1. Ciclo de instrucción: El funcionamiento del CPU se divide en ciclos de instrucción. Se divide en varias etapas:
+ Fetch (Obtener): La UC obtiene la instrucción de la memoria (RAM) utilizando la dirección almacenada en el controlador de programa (PC), que indica la siguiente instrucción a ejecutar.
+ Decode (Decodificar): La UC decodifica la instrucción obtenedia para entender qe operación se debe realizar.
+ Execute (Ejecutar): La ALU o UAL realiza la operación especificadapor la instrucción. Esto puede implicar cálculos, comparaciones o mover datos entre registros.
+ Store (Almacenar): Si la operación genera un resultado, este se almacena en un registro o se envía de vuelta a la memoria RAM según sea necesario.
+ Update (Actualizar): El controlador de programa se actualiza para apuntar a la siguiente instrucción en la secuencia.

2. Interrupciones
+ El CPU puede recibir interrupciones de otros componentes del sistema (como dispositivos I/O) que requieren atención inmediata. Cuando esto pasa, el CPU pausa su ciclo actual, guarda su estado y atiende la interrupción antes de volver a su tarea original.