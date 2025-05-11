# Introducción a Blockchain

Este repositorio contiene los ejemplos utilizados en el seminario de Blockchain de la asignatura de [Negocio Electrónico][1].

## Tipos de nodos

_REVISAR_

- **Nodos Completos (Full Nodes):** Almacenan toda la blockchain, verifican transacciones y bloques.
- **Nodos Ligeros (Light Nodes):** Sólo guardan una parte de la blockchain y consultan a nodos completos para verificar.
- **Nodos Mineros (Mining Nodes):** Compiten para crear nuevos bloques en redes PoW (_Proof-of-Work_) resolviendo problemas criptográficos.
- **Nodos de Validación (Validator Nodes):** Validan transacciones y proponen bloques en redes PoS (_Proof-of-Stake_) u otros mecanismos de consenso.
- **Masternodes:** Nodos especiales con funciones adicionales (transacciones privadas, gobernanza, etc.).
- **Nodos de Archivo (Archive Nodes):** Almacenan todo el historial de la blockchain, desde el inicio.

## Mecanismos de Consenso

_REVISAR_

Permiten validar las transacciones y asegurar la red.

- **_Proof-of-Work_ (PoW):** Los mineros compiten para resolver problemas
  criptográficos complejos. El primer minero en encontrar la solución puede
  añadir un nuevo bloque a la cadena. Ejemplo: Bitcoin.

- **_Proof-of-Stake_ (PoS):**  Los validadores son seleccionados (a menudo de
  forma probabilística, con mayor probabilidad para aquellos que han apostado
  una mayor cantidad de criptomonedas) para proponer y validar nuevos bloques.
  La capacidad de validar está ligada a la cantidad de criptomonedas que poseen
  y están dispuestos a "apostar" o bloquear como garantía. Ejemplo: Ethereum.

## Contenido de un bloque

_REVISAR_

- **Número de bloque:** Identificador único del bloque.
- **Hash del bloque:** Identificador único del bloque, generado a partir de su contenido.
- **Hash del bloque anterior:** Identificador único del bloque anterior, asegurando la
  integridad de la cadena.
- **Marca de tiempo:** Fecha y hora en que se creó el bloque.
- **Nonce:** Número aleatorio utilizado en el proceso de minería para encontrar un hash válido.
- **Transacciones:** Lista de transacciones incluidas en el bloque.
- **Merkle Root:** Hash que representa todas las transacciones en el bloque, utilizado para verificar la integridad de las transacciones.
- **Dificultad:** Nivel de dificultad para encontrar un nuevo bloque, ajustado periódicamente.
- **Tamaño del bloque:** Tamaño total del bloque en bytes.

_NOTA_

Problema: Soft fork vs Hard fork

- https://www.geeksforgeeks.org/hard-fork-vs-soft-fork-in-blockchain/

## Árbol de Merkle

_REVISAR_

Utilizado para organizar y verificar grandes cantidades de datos de manera eficiente.

Podemos utilizalo para almacenar las transacciones dentro de un bloque.

- https://es.wikipedia.org/wiki/%C3%81rbol_de_Merkle

- [Merkle proofs explained](https://medium.com/crypto-0-nite/merkle-proofs-explained-6dd429623dc5b)

## Simuladores de Blockchain

- https://andersbrownworth.com/blockchain/. [GitHub](https://github.com/anders94/blockchain-demo/)
- https://blockchain-sim-test.web.app
- https://blockchaindemo.io/

## Vídeos

- [Introducción a las tecnologías Blockchain. Parte I](https://canal.uned.es/video/646488c86ff5a73b9e6a73c2). Víctor García Pastor. UNED.
- [Introducción a las tecnologías Blockchain. Parte II](https://canal.uned.es/video/646488c86ff5a73b9e6a73c7). Víctor García Pastor. UNED.

## Referencias

- [¿Qué es el Blockchain?](https://www.ibm.com/es-es/topics/blockchain). IBM.
- [Blockchain: La revolución industrial en Interner](https://libroblockchain.com/). Alex Preukschat. Gestión 2000.
- [Bitcoin: Un Sistema de Efectivo Electrónico Usuario-a-Usuario](https://bitcoin.org/files/bitcoin-paper/bitcoin_es_latam.pdf). Satoshi Nakamoto.

## Créditos

El código utilizado en este seminario está basado en el código desarrollado por
[José Antonio Torres Ariaza](https://www.ual.es/persona/535053495455545772).
Sólo se han modificado pequeños detalles para crear el proyecto en
Flask.

[1]: https://www.ual.es/estudios/grados/presentacion/plandeestudios/asignatura/4015/40153316