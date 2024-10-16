# Unidades funcionales

## ¿Qué es un ordenador?
Un ordenador es una máquina que el objetivo es recibir unos datos, procesarlos y ofrecer los resulatdos de este procesamiento de una manera automática.

Nosotros conocemos los ordendores por ordenadores de sobremesa o portátiles, los ordenadores están en todas partes (PC, cajeros, teléfonos, etc.).

## Unidades funcionales de un ordenador
El funcionamiento de un ordenador se basa en la arquitectura **Von Neumann**, que establece una serie de unidades funcionales que, gràcias a su conexión, permanente consiguen un funcionamiento coordinado bajo un control central.

### CPU (Central Processing Unit)
Se conoce como microprocesador y es un circuito integrado (chip) formado por:
+ Unidad aritmético-lógica (UAL): Realiza las operaciones necesarias (matemáticas y lógicas) para ejecutar una instrucción.
+ Unidad de control (UC): Dirije el resto de las unidades para su correcto funcionamiento.
+ Registros: Memorias rápidas y de poca capacidad para almacenar datos de manera temporal. El almacenamiento de datos en el ordenador se realiza a través del código binario. El binario es un sistema de numeración que utiliza 2 números, que son el 0 y el 1.

### Unidad de memoria (UM)
Sus elementos almacenan la información en el ordenador.

### Unidad de entrada/salida (UI/UO)
Formada por los elementos utilizados para introducir, almacenar y mostrar la información (Periféricos).

### Buses
Un bus es una via que comunica 2 puntos. Todas las unidades funcionales necesitan comunicarse entre sí, por lo que se utilizan los buses para comunicarse. Físicamente puede ser un cable o un canal de circuito.

+ Bus de datos: Transfiere datos entre los elementos del ordenador
+ Bus de direcciones: Transfiere direcciones entre la unidad de control y la unidad de memoria.
+ Bus de control: Emite las señales decontrol que gobiernan el funcionamiento de las unidades funcionales.

### Unidad de memoria (UM) definición
La unidad de memoria está formada por la memoria principal (RAM), **es un dispositivo de almacenamiento volátil de capacidad limitada y de alta velocidad.**, utilizado para el almacenamiento de instrucciones de los programas y sus correspondientes datos.

Los datos se pueden encontrar almacenados en unas celdas llamadas posiciones de memoria que están numeradas de manera consecutiva. Esta numeración se conoce como dirección de memoria y permite acceder a los datos de manera directa.

| Dirección de Memoria | Valor  | Acceso                 |
|----------------------|--------|------------------------|
| $$0x0000$$           | $$10$$ | ↓                      |
| $$0x0001$$           | $$20$$ | ↓                      |
| $$0x0002$$           | $$30$$ | ↓                      |
| $$0x0003$$           | $$40$$ | ↓                      |
| $$0x0004$$           | $$50$$ | ↓                      |
| $$0x0005$$           | $$60$$ | ↓                      |
| $$0x0006$$           | $$70$$ | ↓                      |
| $$0x0007$$           | $$80$$ | ↓                      |
| $$0x0008$$           | $$90$$ | ↓                      |
| $$0x0009$$           | $$100$$| ↓                      |

#### Acceso a los datos
El acceso a los datos se realiza a través de las direcciones de memoria. Cuando se necesita acceder a un valor, se utiliza la dirección correspondiente, como se muestra a continuación:
$$[Dirección]\rightarrow[Valor]$$

- Por ejemplo:
  - $$0x0000 \rightarrow 10$$
  - $$0x0001 \rightarrow 20$$
  - $$0x0002 \rightarrow 30$$

#### Jerarquía de la memoria
La memoria se organiza en diferentes niveles en función de su velocidad, capacidad y coste.

Los niveles de memoria son:

+ Registros: Memorias de alta velocidad, baja capacidad integradas en el procesador; se utilizan para el almacenamiento intermedio de los datos, especialmente en la UC y la UAL.

+ Caché: Memoria intermedia entre la UM y la CPU, permite accelerar el acceso a datos- Cuando se accede a un dato,, este se copia en la cajita para que podamos acceder mas tarde a el de manera más rápida. Tiene diferentes niveles
1. L1
2. L2
3. L3
4. L4

+ Principal (RAM): La memoria principal, es decir la memoria RAM, es la memoria principal del ordenador, se usa para almacenar datos y programas de manera temporal.

+ Secundaria o memoria de disco: Formada por los discos duros del ordenador, es una memoria de alta capacidad no volátil, lo que significa que guarda la información de manera permanente.

+ Auxiliar: Esta memoria se usa como copias de seguridad, pudiendo ser situados en medios extraibles o en red, como cinta magnética, disco duro extraible o almacenamiento en red.

### Unidad central de procesamiento (CPU)
Tambien conocida como CPU, es la unidad central de procesamiento del ordenador. Se encarga de procesar la información que llega al equipo. Existen otros chips en el ordenador que sirven de soporte al procesador, pero este es el que aporta la mayor carga. La CPU está compuesta por:

+ UAL: se encarga de realizar operaciones aritméticas y lógicas.

#### UAL
Se pueden clasificar en tres tipos:

| **Su ámbito**                   | **Descripción**                                                  |
|---------------------------------|-----------------------------------------------------------------|
| **Genéricos**                   | Pueden realizar diferentes operaciones.                          |
| **Específicos**                 | Només pueden realizar un tipo de operación.                     |
| **El número de operandos**      |                                                                 |
| **Monádicos**                   | Només una entrada, por ejemplo, el negador.                     |
| **Diádicos**                    | Dues entradas, por ejemplo, el operador suma.                   |
| **Triádicos**                   | Tres entradas, por ejemplo, el condicional.                     |
| **Su capacidad de operar**      |                                                                 |
| **Serie**                       | Reciben la información en una secuencia de bits y la procesan uno a uno hasta acabar toda la serie. |
| **Paralelo**                    | Reciben la información en bloques de bits, que procesan de manera simultánea. |

### UC
La UC es el centro nervioso del ordenador, ya que coordina el resto de unidades funcionales.

Su función principal, realizar la búsqueda, carga y interpretación de las instrucciones de los programas que se encuentran almacenadas en la memoria para después emitir la secuencia adecuada de ordenes y que se ejecuten correctamente.

## I/0

| **TIPOS**                       | **FUNCIÓN**                                                   | **EJEMPLOS**                                |
|---------------------------------|--------------------------------------------------------------|---------------------------------------------|
| **Periféricos de entrada**      | Con ellos el usuario introduce la información al ordenador.   | teclado, ratón, escáner                     |
| **Periféricos de salida**       | Se utiliza el ordenador para mostrar la información al usuario.| monitor, impresora, altavoces               |
| **Periféricos de E/S**          | Se usan para establecer una comunicación entre dos o más ordenadores. | enrutador, switch, tarjeta de red           |
| **De almacenamiento**           | Se encargan de guardar los datos para que la CPU pueda usarlos una vez eliminados de la memoria principal. | disco duro, memoria USB, CD/DVD             |

## Periféricos

## Intercambio de información entre periféricos y CPU

Los periféricos intercambian información con el ordenador gracias a un sistema que consta de dos partes:

| **Parte**      | **Descripción**                                                                                                 |
|----------------|-----------------------------------------------------------------------------------------------------------------|
| **Interfaz**   | Gestiona el intercambio de información entre el periférico y la CPU. Adapta la información específica de cada dispositivo a un conjunto de señales normalizadas que actúan como interlocutor del periférico y la máquina. |
| **Controlador** | Se ocupa directamente del periférico. Es un sistema electrónico o mecánico que solo interactúa con el propio periférico, para que el cual cosa puede deducir que es específico de éste. |

## Técnicas de gestión de E/S

La gestión de la E/S es uno de los pilares fundamentales en el rendimiento de un ordenador, ya que todos los dispositivos que se conectan al equipo compiten por el uso de la CPU para poder operar. Para facilitar la comunicación interna del módulo de E/S, la CPU y la memoria existen diversas técnicas:

| **Técnica**                      | **Descripción**                                                                                  |
|----------------------------------|--------------------------------------------------------------------------------------------------|
| **E/S programada**               | Puede realizarse en serie o en paralelo; la CPU y el módulo de E/S intercambian los datos.    |
| **E/S por interrupciones**       | El procesador espera que el módulo de E/S esté preparado, lo cual aumenta el tiempo de manera considerable. |
| **E/S por acceso directo a memoria (DMA)** | Permite al módulo de E/S comunicarse sin interrupciones para liberar una gran carga de trabajo.     |

