# Operadores en Xpath

Hay una forma de filtrar más avanzada y es con operadores lógicos.

## Operadores lógicos en Xpath :

Cabe notar que los operadores se están usando dentro del predicado.

!=
<>
and
or
not
Ejemplo:

Usando el operador != diferente, le estoy diciendo que me
traiga todos los nodos span que tienen clase diferente a Texto.

$x('//span[@class!="text"]')

Usando operador not me devuelve todos los nodos que no tienen el atributo class.

$x('//span[not(@class)]'
