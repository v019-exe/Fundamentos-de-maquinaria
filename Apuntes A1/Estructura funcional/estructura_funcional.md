# Esquema funcional y estructura de un ordenador

## Sistema informático

Un sistema informático es un conjunto de elementos necesarios para la realización y explotación de aplicaciones informáticas, se incluyen 3 tipos, programas, maquinaria y humanos.

En un sistema informático hay elementos constitutivos interelacionados entre si:

- Parte lógica: Hardware, todo aquello que se puede ver y tocar en el mundo de la informática (monitores, impresoras, ratón, teclado, etc.)

- Parte lógica: Software, tiene su origen en las ideas (conceptos) y está formado por todo aquello que usamos en el campo de la informática que no se puede ni ver ni tocar (programas, SO, etc.)

- Parte humana: Este elemento es esencial que forma parte de la informática o de un sistema informático. Sin las personas que están a cargo de la informática no habría ni parte lógica ni física.

## Funcionalidad
Su función principal es el procesamiento de datos.

## Características
+ Hace una acción a la vez.
+ Puede hacer cálculos matemáticos: suma, resta, multiplicación, división, etc.
+ Puede realizar operaciones lógicas: AND, OR, NOT, XOR, etc.
+ Opera a alta velocidad.
+ Es exacto y preciso, hace exactamente lo que se le indica.
+ Es eficiente, puede trabajar sin parar.
+ Tiene capacidad de manipular grandes cantidades de información.
+ Es fiable, tiene la capacidad de verificar la exactitud de sus operaciones internas, es decir, autocomprobación.
+ Puede manipular símbolos
+ Cada vez son mas pequeños y mas utiles y menos costosos.

## Definiciones

+ Maquinaria (Hardware): Todo aquello que podemos ver y tocar (Monitores, impresoras, ratón, teclado, etc.)

+ Programas (Software): Hace referencia a los elementos que no tienen existencia física, como las ideas, conceptos, programas y las aplicaciones.

+ Usuario y programador: El usuario es el que utiliza el sistema informático, es decir, el que interactúa con él. El programador es el que escribe los programas que se utilizan en el sistema informático. Escrito en un lenguaje de programación para que los ordenadores puedan entenderlo.

+ Datos y información: Los datos son hechos o materiales originales que no han sido modificados. La información es el producto de los datos ya procesados.

+ Documentación: Es el conjunto de instrucciones o manuales de procedimiento que enseñan al usuario como se tiene que utilizar el ordenador y los programas informáticos.

## Elementos principales

+ Dispositivos de entrada: Su función principal consiste en permitir la entrada de datos en el ordenador.

+ Dispositivos de salida: Su función principal consiste en sacar la información al exterior del ordenador.

+ Dispositivos de entrada/salida: Son todas las maquinas de configuración de las cuales permiten hacer funciones de entrada y salida (Cintas mágneticas, unidades de discos mágneticos o unidades opticomágneticas, etc.)

```mermaid
graph TD;
    A[Dispositivos de entrada] --> B[Dispositivos de procesamiento];
    B --> C[Dispositivos de salida];
    D[Dispositivos de entrada/salida] --> B;
    B --> D;
```

### Dispositivos de procesamiento
También conocidos como UCP (Unidad central de procesamiento) o CPU. Es la parte más importante de un ordenador, en el que se manipula la información. Los dispositivos de procesamiento son los que se encargan de coordinar y llevar a cabo todas las operaciones de tipo lógico y matemático.

+ Procesador (microprocesador): Cerebro del ordenador, coordina y dirige la faena que se tiene que hacer en cada momento.
+ CU (Unidad de cntrol): Se encarga de governar el resto de las unidades, es decir, interpreta las instrucciones y controla la ejecución y la secuencia.

+ ALU (Unidad Aritmético-Lógica): Realiza operaciones matemáticas y lógicas.


```mermaid
flowchart TD;
    A[CPU] --> B[Procesador];
    B --> C[Unitat de control CU];
    B --> D[Unitat aritmètica i lògica ALU];
    B --> E[Memòria principal];
    E --> B;
```

## Unidades funcionales

+ Unidades de entrada
+ Unidades de procesamiento y almacenamiento
+ Unidades de salida
+ Unidades entrada/salida

Definimos como unidades funcionales del ordenador como el conjunto de elementos de maquinaria imprescindibles para que el ordenador funcione.

Se pueden clasificar en 3 tipos:

+ CPU
+ Memoria principal
+ I/O

Todos los elementos que forman las unidades funcionales necesitan algún tipo de comunicación para funcionar correctamente, a esto se le llama bus y se consigue con el bus del sistema.

También para la comunicación entre estos dispositivos y otras máquinas sea eficiente, a veces hace falta que otras máquinas las gestionen. Esto es lo que hacen los controladores. Son dispositivo que gestionan el funcionamiento de determinadas máquinas y hacen la comunicación entre elementos de las unidades funcionales y dispositivos periféricos.

**UCP, Memoria central, controladora, I/O**
```mermaid
flowchart TD;
    A[UCP] --> B[Memoria central];
    B --> A;
    A --> C[Controladora];
    C --> D[Unidad de entrada/salida];
    D --> C;
    D --> B;
    B --> D;
    C --> B;
    C --> A;
```
**Entrada, procesador, memoria, UC, ALU**

```mermaid
flowchart TD;
    A[Entrada] --> B[Memoria principal: Datos e instrucciones];
    B --> C[Unidad de control];
    B --> D[Unidad aritmética y lógica ALU];
    C --> E[Procesador central CPU];
    D --> E;
    B --> F[Memoria masiva];
    F --> B;
    E --> G[Salida];
```

**UCP, Unidad de control, memoria, periféricos, buses de datos y control**
```mermaid
flowchart TD;
    A[UCP CPU] --> B[UC Unidad de control];
    B --> C[Memoria principal MP];
    C --> D[Memoria secundaria o masiva];
    D --> C;
    C --> E[Bus de datos];
    E --> F[Periféricos];
    F --> G[Unidad de entrada];
    G --> F;
    F --> H[Unidad de salida];
    H --> F;
    F --> C;
    C --> A;
    A --> B;
    A --> E;
    E --> D;
```

## Memoria principal y sus elementos

La memoria principal o central, es el dispositivo electronico en el cual se situan los datos o instryucciones que manipulará la ALU o los resultados que se obtengan de estos tratamientos.

La memoria principal tiene una capacidad límitada y en determinados momentos el precio de las memorias principales han estado mas elevados que otros componentes de maquinaria. Por esto y otros factores, esta memoria complementa con la memoria externa o memoria secundaria.

### Elementos de la memoria principal

La memoria principal está formada por celdas o posiciones de memoria numeradas de manera consecutiva. Dichas celdas son capaces de mantener la información almacenada en ellas mientras esté el ordenador en funcionamiento.

Cada celda tiene un nombre que se denomina como posición de memoria y un identificador único que se denomina dirección de memoria.

```mermaid
graph LR
    1["1"] --> 2["2"] --> 3["3"] --> 4["4"] --> 5["5"] --> 6["6"] --> 7["7"] --> 8["8"] --> 9["9"] --> 10["100"]
    
    %% Flechas explicativas
    memDir([Dirección de memoria]) --> 1
    memPos([Posición de memoria]) --> 7
```

+ Registro de dirección de memoria: Antes de realizar cualquier operación de lectura o escritura en la memoria, se tienen que colocar la dirección de la celda que se utilizará en la operación de este registro, tanto como si es para grabar la dirección en un registro o como si es para extraer datos.

+ Registro de información o intercambio de memoria (RIM): Este registro recibe la información obtenida de la lectura de la memoria. Este registro tiene que contener la información que queremos escribir y guardar en la memoria.

+ Selector de memoria o descodificador: Este dispositivo se activa cada vez que se produce una orden de lectura o escritura. Conecta la celda de memoria, indicada por la dirección de registro de la dirección de memoria con el registro de información de memoria. El cual lo hace posible el hacer transferencias de datos en un sentido o en otro (memoria a RIM, RIM a memoria).

Hay 3 parámetros para medir la velocidad de respuesta de una memoria:

+ TA (Tiempo de acceso): Es el tiempo máximo que se tarda en leer o escribir el contenido de una posición de memoria.

+ Tiempo de ciclo (TC): El tiempo mínimo entre 2 lecturas.

+ Ancho de banda (AB): Es el número de palabras que se transfieren entre la memoria y la CPU en cada unidad de tiempo.

$$
AB = 1 / TC
$$

**Secuencia de pasos para leer o escribir un dato en la memoria principal**

1. Leer: Para leer un dato se siguen los pasos siguientes:
+ Se pone la dirección de memoria en el registro de dirección.
+ Mediante el descodificador, se accede a la dirección de memoria.
+ Se situan los datos en el registro de datos.

2. Escribir: Para escribir un dato se siguen los pasos siguientes:
+ Se transfiere la dirección en la qeu se escribirá en el registro de dirección.
+ Se transfieren los datos al registro de información.
+ Se descodifica la dirección de memoria.
+ Se pasa el contenido del registro de información a la dirección que contiene el registro de dirección.

## CPU

Como hemos mencionado anteriormente, el CPU es el cerebro del ordenador, es el encargado de coordinar y dirigir la ejecución de todas las operaciones de procesamiento.

Está formada por:
+ Registros
+ ALU
+ CU

```mermaid
graph TB
    %% Bloques principales
    registrosDatos[Registros de datos] --> busInterno[Bus de datos interno]
    busInterno --> registrosDirecciones[Registros de direcciones]
    busInterno --> ALU[Unidad aritmética y lógica]
    ALU --> registrosEspecificos[Registros específicos]
    busInterno --> registrosEspecificos

    %% Unidad de control conectada
    unidadControl[Unidad de control] --> busControlExterno[Bus de control externo]
    busInterno --> unidadControl

    %% Buses externos
    registrosDirecciones --> busDireccionesExterno[Bus de direcciones externo]
    unidadControl --> busDireccionesExterno
    registrosEspecificos --> busDatosExterno[Bus de datos externo]
    busInterno --> busDatosExterno

    %% Relaciones externas
    busDireccionesExterno -.-> busDatosExterno
    busDireccionesExterno -.-> busControlExterno
```

### Los registros

Dentro del procesador hay unas zonas reservadas para el almacenamiento de pequeñas cantidades de información. Son los registros internos.

Se denomina registro un conjunto de bits que se manipulan en bloque.

Podemos diferenciar 2 tipos de registros internos:

+ Registros internos de uso general: El procesador usa estos registros para el almacenamiento temporal de datos o direcciones de memoria, es decir la posición de memoria que se almacenan los datos. Podemos encontrar los siguientes:

+ Registros internos de datos: Se usan para almacenar datos que el procesador solicita frecuentemente.

+ Registros internos de dirección: Se puede guardar la dirección de memoria donde se encuentra el dato.

Registros internos específicos, podemos indicar los siguientes:
+ Contador de programa: Uno de los registros que lleva a cabo el control de las instrucciones del programa que se ejecutan es el contador de programa. Se trata de un registro específico que está pendiente de la instrucción del programa que se ejecuta o el próximo a ejecutar.

+ Puntero de pila: dentro de la RAM, hay una zona destinada al almacenamiento de información temporal, es decir pila o stack. Es un registro que mantiene la dirección de un dato que está almacenado en la pila.

+ Indicador de resultado: Cada bit del registro indicador de resultado (flag register, FLAGS) contiene información sobre el resultado de la última operación efectuada en la ALU. El numero de bits del FLAGS y su significado varían de un procesador a otro.

+ Registro de instrucción: La unidad de control tiene una referencia permanente de la instrucción en curso mediante el registro de instrucción. Mantiene el código de la instrucción que se está ejecutando.

### ALU
La unidad aritmética y lógica gestiona las operaciones elementales de tipo aritmético (sumas, restos, etc etc.) y, también, las de tipo lógico (operaciones en las que el resultado es verdadero o falso).

Esta unidad tiene dos entradas para los operandos y una salida para el resultado. El procesador se dirige a las entradas ALU cuyos registros debe realizarse la operación. El resultado aparece a la salida de la ALU y se recoge en un registro o se envía al autobús. Muchos procesadores dirigen la salida de la ALU hacia el acumulador.

Podemos encontrar los siguientes:

+ Circuitos operacionales: Circuitos necesarios para hacer las operaciones con los datos procedentes de los registros de entrada.

+ Registro de entrada: Almacena datos o operandos que intervienen en una instrucción antes de la realización de la operación por parte del circuito operacional.

+ Registro acumulador: Almacena los resultados númericos del circuito operacional.También está conectado a los registros de entrada para la retroalimentación, en caso de operaciones encadenadas y tiene una conexión con el bus de datos para enviar los resultados a la memoria principal o a la UC.

+ Registro de estado: Registro que almacena algunas condiciones de situaciones esdevenidas en la ultima operación hecha y que tenemos que tener en cuenta en las operaciones siguientes.

### Buses
+ Bus de datos: Mueve los datos entre los dispositivos del maquinario de entrada, de salida y de almacenamiento.
+ Bus de direcciones: Está vinculado al bloque de control de la CPU para prender y colocr los datos en el subsistema de memoria durante la ejecución de los procesos de computo.

+ Bus de control: Transporta señales de estado de las operaciones hechas por el CPU con el resto de unidades.

### Unidad de control

La unidad de control hace una serie de operaciones básicas para el funcionamiento del procesador:

+ Interpreta las instrucciones del programa que llegan a la memoria del sistema.
+ Dirige los registros adecuados hacia la ALU.
+ Controla los buses internos.
+ Ordena a la ALU efectuar la operación indicada en el programa.
+ LLeva de la memoria los datos necesarios y envia los datos resultantes.
+ Gestiona los buses externos de comunicación con la memoria externa y los periféricos.

```mermaid
graph TB
    %% Bloques principales
    reloj[Reloj] --> secuenciador[Secuenciador]
    secuenciador --> contadorP[Contador de programa]
    secuenciador --> microordenes[Microórdenes]
    secuenciador --> descodificador[Descodificador]
    descodificador --> registroInstruccion[Registro de instrucción]
    registroInstruccion --> bus[BUS]
    secuenciador --> bus
    
    %% Conexiones adicionales
    contadorP --> secuenciador
    registroInstruccion --> descodificador
```