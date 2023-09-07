1.
¿Cómo se le conoce al área de estudio de dispositivos de cálculo abstractos (Máquinas)?
Teoría de Autómatas.

2.
Es el modelo de máquina computacional más común, cuyo diseño está implementado en las computadoras modernas.
Arquitectura de Von Neumann.

3.
¿Qué significa Σ en la definición de un Autómata Finito Determinista (DFA)?
Es el conjunto de posibles estados en los que se puede encontrar un autómata.
REPASAR CLASE
4.
¿Qué es una máquina de Turing?
Es la máquina mínima teórica que puede resolver cualquier problema computable.

5.
¿Qué es el instruction set en la arquitectura x86?
Es una lista de instrucciones proveída por el fabricante, con las cuales se puede programar un microcontrolador.

6.
¿A qué se refiere la virtualización de una máquina?
Es la creación de una versión no física de dicha máquina, utiliza software en lugar de hardware.

7.
La Máquina Virtual de Ethereum es una...
Process Virtual Machine.

8.
Un compilador…
Se encarga de transformar instrucciones en un lenguaje de programación de alto nivel en instrucciones (bytecode) para una máquina objetivo.

9.
Una máquina de stack…
Utiliza una pila donde deposita y lee valores.

10.
El memory word es…
El tamaño en bytes de lo que cabe en una unidad de memoria. En la EVM es de 32 bytes.

11.
¿Cuál de las siguientes afirmaciones sobre la EVM es FALSA?
Los elementos de la memoria y el stack inician en null.

12.
¿Cuál es la diferencia principal entre memory y storage?
El storage es no volátil, mientras que la memory es volátil

13.
¿Cómo se define el entorno de ejecución de Ethereum?
Ξ(e, g, F, I) ≡ (e’, g’ , F’ , o)
REPASAR CLASE
14.
¿Qué representa g y g' en el entorno de ejecución de Ethereum?
Representa el gas disponible al inicio y al final de la ejecución.

15.
El storage en Ethereum está representado por…
Un Merkle Patricia Tree.

16.
Cada address en Ethereum tiene su propio storage.
Cierto

17.
La forma en la que se validan las modificaciones al storage en la blockchain de Ethereum es…
Computando las transacciones, modificando el state y guardando el root hash en el nuevo bloque.

18.
Un Merkle Tree es ideal para guardar el estado porque…
El hash del root representa todos los cambios en todas las hojas del árbol, lo que facilita verificar que el árbol es correcto con poca información.

19.
Un ejemplo de un problema NO decidible es…
Un loop infinito.

20.
¿Qué es el gas?
Es una unidad de medida que representa el costo computacional de la ejecución de la EVM.

21.
¿Cuándo se consume el gas?
Se consume con cada instrucción que ejecuta la EVM

22.
Las variables pueden ser empaquetadas en memoria y storage dependiendo de su orden.
Cierto

23.
¿Cuál es la diferencia principal entre el creation bytecode y el runtime bytecode?
El creation bytecode incluye el constructor y código que guarda el runtime bytecode en storage. El runtime bytecode es el que se guarda on chain.

24.
¿Cómo sabe la EVM qué función de Solidity queremos ejecutar?
Se envía el selector de la función y sus parámetros codificados en el calldata.

25.
¿Cuál de las siguientes funciones NO consume gas de forma estática?
ADD
REPASAR CLASE
26.
¿Cuál de las siguientes funciones NO consume gas de forma dinámica?
PUSH1

27.
El error "Out of Gas" se muestra cuando…
El gas restante durante la ejecución es menor o igual a 0, sin importar que el código no haya terminado de ejecutarse.

28.
¿Cuál es el recurso más costoso en la EVM?
El storage

29.
¿Qué es el costo de expansión de memoria?
Es el costo de extender el arreglo de memoria para almacenar más información.

30.
¿Qué hace la instrucción JUMPI?
Cambia el valor del program counter, permitiendo ciclos y condiciones.
