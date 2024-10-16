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
