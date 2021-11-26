# Expresiones en Xpath

* / : Significa la raiz o root de todo el documento, tambien significa un salto entre nodos. Puedo navegar entre niveles

* // : Puedo ir por varios niveles en el esquema que construimos.

## Ejemplo:

Fuente de trabajo Quotes to Scrape:

* url ="http://quotes.toscrape.com/"

Quiero extraer el texto de mi nodo h1.

$x('//h1/a/text()').map(x => x.wholeText)
Devuelve en consola: ["Quotes to Scrape"]
La función map pertenece a Js y la estoy usando para que me muestre todo el texto de la selección de Xpath.

Existen otras expresiones

/… : Acceder a todos los nodos padre de x nodo.
/@atribute_name : Me permite extraer atributos
#Estoy trayendo todos los atributos class de los nodos span.
$x('//span/@class')
Para ser específicos con los datos a extraer se usan predicados.