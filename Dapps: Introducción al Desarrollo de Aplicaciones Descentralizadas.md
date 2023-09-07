1.
¿Cuáles son las principales características de una DApp?
Resistentes a censura, resilientes y transparentes.

2.
¿Qué es una DApp?
Es una aplicación que posee la mayor cantidad de componentes descentralizados.

3.
¿Cuáles son las 3 capas descentralizables de una aplicación?
Persistencia, lógica de negocios y cliente

4.
Aunque OpenSea es un marketplace para activos descentralizados, esta puede no considerarse una DApp en su totalidad debido a que...
Su backend está centralizado, y aunque indexa datos de distintos blockchain, podría censurar su información.

5.
Un ethereum provider de conexión a un nodo de blockchain...
Funciona como intermediario para firmar transacciones y mensajes, es el medio por el cual te auténticas de forma segura

6.
¿Cuál de los siguientes NO es un ethereum provider?
Binance

7.
Hardhat es...
Un entorno de desarrollo que nos permite compilar, probar y desplegar contratos inteligentes.

8.
¿Porqué es necesario evitar subir nuestras llaves privadas en el repositorio?
Porque la llave privada permite firmar cualquier transacción. Exponer públicamente una llave privada es comprometer irrecuperablemente una cuenta

9.
¿Cuál de las siguientes opciones NO es una alternativa a Hardhat?
Alchemy

10.
EIP significa ________ y es _______
Ethereum Improvement Proposal / es un documento con las especificaciones de mejora a alguna de las partes del protocolo de Ethereum

11.
¿Qué es un ERC?
Es una propuesta preliminar para un EIP, se discute en el GitHub oficial de los EIPs y significa Ethereum Request for Comments

12.
¿Qué es Open Zeppelin?
Un set de herramientas para mantener la seguridad de contratos inteligentes. Su principal producto es Contracts, una librería de Smart Contracts estándar, seguros y previamente auditados

13.
¿Cuál de las siguientes opciones es la forma de instanciar un ERC721 de Open Zeppelin?
// SPDX-License-Identifier: MIT pragma solidity ^0.8.0; import "@openzeppelin/contracts/token/ERC721/ERC721.sol"; contract PlatziPunks is ERC721("PlatziPunks", "PLPKS") { }
REPASAR CLASE
14.
La extensión ERC721Enumerable...
Extiende al ERC721 y agrega funcionalidad para obtener el balance de cada address y sus tokens

15.
¿Qué regresa la función tokenURI del ERC712 Metadata?
Debe regresar una URL, que a su vez, regresa un JSON donde están los atributos del NFT, como su imagen o características

16.
Una técnica para codificar la metadata on-chain sin apuntar a un servidor externo es...
Construir una URL base64 en el Smart Contract que resuelva a un archivo JSON. Se puede hacer lo mismo para la imagen

17.
El ADN de PlatziPunks es una forma de expresar los atributos del NFT de forma numérica, ¿cómo se aplica el algoritmo de los atributos?
Se toma un entero “aleatorio” de 256 bits, y se divide en rebanadas de 2 dígitos que expresan cada atributo. Se obtiene el módulo con respecto a la longitud de propiedades disponibles y así se obtiene un índice en el arreglo.

18.
¿Cuál es una razón válida para usar un ADN en lugar de guardar en memoria cada atributo para cada NFT?
Guardar cada atributo es costoso y redundante. Eso ocuparía mucho espacio en memoria, consumiendo mucho gas

19.
¿Por qué no existen los números aleatorios en Blockchain y la máquina virtual de Ethereum?
Porque el consenso requiere determinismo. Un número aleatorio rompe con esta regla y desestabiliza el consenso

20.
¿Cómo podemos acceder a información no determinista en la blockchain?
A través de un oráculo como Chainlink, que hace el procesamiento no determinista off-chain y lo reinserta a través de una transacción

21.
Una forma de realizar tests en JavaScript a nuestro contrato inteligente con Hardhat es utilizando ________ y ________
ethers.js y chai

22.
¿Con qué funciones en Solidity se puede añadir ruido de forma DETERMINISTA a una pieza de información?
keccak256()

23.
¿Cuál de las siguientes no es una red de prueba?
Infura

24.
¿Cómo interactuar con un Smart Contract desde Etherscan?
Este tiene que ser verificado subiendo los archivos fuente a Etherscan. Una forma de hacerlo es con el flatten de Hardhat

25.
¿Porqué es que servicios como Open Sea pueden indexar nuestro NFT?
Porque cumple con el estándar ERC721, y eso permite a todas las plataformas de NFT leer y procesar sus atributos
