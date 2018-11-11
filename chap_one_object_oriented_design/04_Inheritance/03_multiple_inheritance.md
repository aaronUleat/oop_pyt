## Multiple inheritance

Cuando pensamos en la herencia de nuestro propio árbol genealógico, podemos ver que heredamos
características de más de un padre. Cuando extraños le dicen a una madre orgullosa que ella
su hijo tiene "los ojos de su padre", ella responderá típicamente como "sí, pero él
tengo mi nariz ".

El diseño orientado a objetos también puede presentar dicha herencia múltiple, lo que permite una
subclase para heredar la funcionalidad de varias clases padre. En la práctica, múltiples
La herencia puede ser un negocio difícil, y algunos lenguajes de programación (la mayoría
En particular, Java) lo prohíbe estrictamente. Sin embargo, la herencia múltiple puede tener sus usos.
La mayoría de las veces, se puede usar para crear objetos que tienen dos conjuntos distintos de comportamientos.
Por ejemplo, un objeto diseñado para conectarse a un escáner y enviar un fax de la
El documento escaneado se puede crear heredando de dos escáneres separados y
Objetos de fax.

Mientras dos clases tengan interfaces distintas, normalmente no es perjudicial para una
subclase para heredar de ambos. Sin embargo, se ensucia si heredamos de dos
Clases que proporcionan interfaces superpuestas. Por ejemplo, si tenemos una moto.
clase que tiene un método de movimiento, y una clase de barco que también presenta un método de movimiento,
y queremos fusionarlos en el vehículo anfibio definitivo, ¿cómo funciona el
¿La clase resultante sabe qué hacer cuando llamamos mover? A nivel de diseño, esto necesita
por explicar, y en el nivel de implementación, cada lenguaje de programación tiene
diferentes formas de decidir a qué método de clase padre se llama, o en qué orden.

A menudo, la mejor manera de lidiar con esto es evitarlo. Si tienes un diseño que aparece como
Esto, probablemente lo estás haciendo mal. Retroceda un paso, analice nuevamente el sistema, y
Vea si puede eliminar la relación de herencia múltiple en favor de algún otro
Diseño asociativo o compuesto.

La herencia es una herramienta muy poderosa para extender el comportamiento. También es uno de los más
Avances comerciales de diseño orientado a objetos sobre paradigmas anteriores. Por lo tanto,
a menudo es la primera herramienta que buscan los programadores orientados a objetos. De todos modos, eso
Es importante reconocer que poseer un martillo no convierte los tornillos en clavos.
La herencia es la solución perfecta, porque una relación obvia es una relación, pero se puede abusar de ella.
Los programadores a menudo usan la herencia para compartir código entre dos tipos de objetos que son
Sólo a distancia, sin relación es una relación a la vista. Si bien esto no es necesariamente
un mal diseño, es una excelente oportunidad para preguntar por qué decidieron diseñar que
manera, y si una relación diferente o patrón de diseño hubiera sido más
adecuado.