¿Por qué es importante escribir correctamente los contratos que se implementan en la red de Ethereum?
Porque no se puede alterar su código fuente una vez subido.

2.
¿Qué medida podemos tomar para controlar el gas en una llamada externa?
Establecer un límite de gas.

3.
¿Por qué conviene utilizar librerías?
Porque su código ya ha sido probado y auditado.

4.
¿Qué rol es habitual para el control de acceso a un contrato?
Owner

5.
¿Qué modificador define que una función puede recibir pagos en Ether?
payable

6.
¿En qué caso se diferencian tx.origin y msg.sender?
Cuando el contrato es llamado por otro contrato.

7.
¿Por qué no es bueno utilizar el timestamp del bloque para operaciones críticas?
Porque se puede manipular su valor.

8.
¿Qué tipo de dato era afectado por Overflow y Underflow?
int

9.
¿Qué función de web3 devela el contenido del almacenamiento del contrato?
getStorageAt

10.
¿Que característica tiene la llamada delegatecall?
No permite value como parámetro

11.
¿Qué debemos hacer para prevenir el problema del gas insuficiente?
Controlar el retorno de la llamada externa.

12.
¿Cómo se llama la función que puede enviar Ether salteando las funciones de recepción de Ether de los contratos?
selfdestruct

13.
¿Qué error facilita el ataque de reentrancy?
Modificar el estado del contrato al final de la función

14.
¿Qué característica deben tener dos funciones para que se pueda realizar un Reentrancy Cruzado?
Deben compartir el mismo estado

15.
¿Cómo se evita una denegación de servicio por reversión?
Separando las llamadas externas de la modificación del estado del contrato.

16.
¿Qué pasa si el límite de gas es menor al gas requerido por una función en tiempo de ejecución?
La función no se ejecutará en su totalidad y es probable que se revierta.
