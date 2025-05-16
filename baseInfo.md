
# Base Teórica 

# Bloque 

Un Bloque tiene un Hash asociado, la blockchain está formada por varios bloques, los bloques tienes registrados el hash del bloque anterior, de esta forma, podemos encontrar los fllos de una manera rápida.

El Hash de un bloque viene determinado por el número del bloque, los datos y el Nonce.

## Árbol de Merkle
Se establece un árbol, que tiene 3 niveles, estos tres niveles están conformados por un nodo raiz y varios nodos hoja, los nodos padre son siempre la unión de los dos nodos hijos que tiene.
De esta forma, la complejidad para comprobar si un bloque o nodo pertenece a una blockchain es del **log2(X)** 