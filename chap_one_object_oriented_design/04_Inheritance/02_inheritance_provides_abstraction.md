## Inheritance provides abstraction

Exploremos la palabra más larga en argot orientado a objetos. El polimorfismo es la capacidad de
tratar una clase de manera diferente dependiendo de qué subclase se implementa. Ya hemos
Lo veo en acción con el sistema de piezas que hemos descrito. Si tomamos el diseño un poco.
Además, probablemente veríamos que el objeto de la Junta puede aceptar un movimiento del jugador y
Llame a la función de movimiento en la pieza. El tablero no necesita saber nunca qué tipo de pieza.
se trata de Todo lo que tiene que hacer es llamar al método de movimiento, y la subclase apropiada
cuida de moverlo como un caballero o un peón.

El polimorfismo es bastante bueno, pero es una palabra que rara vez se usa en Python
programación. Python va más allá de lo que permite que una subclase de un objeto sea
tratado como una clase padre. Un tablero implementado en Python podría tomar cualquier objeto que
tiene un método de movimiento, ya sea una pieza de alfil, un carro o un pato. Cuando se llama mover,
el obispo se moverá diagonalmente en el tablero, el auto conducirá a algún lugar y el
El pato nadará o volará, dependiendo de su estado de ánimo.

Este tipo de polimorfismo en Python se denomina tipificación de pato: "Si
camina como un pato o nada como un pato, es un pato ". No nos importa si realmente es un pato
(Herencia), solo que nada o camina. Gansos y cisnes podrían fácilmente ser capaces de
proporcionar el comportamiento de pato que estamos buscando. Esto permite a los futuros diseñadores
crear nuevos tipos de aves sin especificar realmente una jerarquía de herencia para
Aves acuáticas. También les permite crear comportamientos de entrada completamente diferentes que
Los diseñadores originales nunca planearon. Por ejemplo, los futuros diseñadores podrían
para hacer un pingüino caminando, nadando que trabaje con la misma interfaz sin
Alguna vez sugiriendo que los pingüinos son patos.