# Predicados Xpath

* [predicado] :Para encontrar nuestra información debemos ser más especificos, para ello sirve los predicados.

## Predicados :

* n : Hace referencia al n elemento de la lista.
* last(): Al último elemento de la lista.
* @atribute_name : Al usarse como predicado me trae todos los nodos que contienen este atributo
* @atribute_name="" : Al usarse como predicado me trae todos los nodos que contienen este atributo, incluso el value de este atributo.

## Ejemplos:

* Para extraer solo uno de los div del div container usamos un predicado

$x('/html/body/div/div[1]')
# Devuelve [div.row.header-box]

$x('//span[@class="text"]/text()').map(x=>x.wholeText)
Devuelve (10) ["“The world as we have created it is a process of o…cannot be changed without changing our thinking.”", "“It is our choices, Harry, that show what we truly are, far more than our abilities.”", "“There are only two ways to live your life. One is… The other is as though everything is a miracle.”", "“The person, be it gentleman or lady, who has not …ure in a good novel, must be intolerably stupid.”", "“Imperfection is beauty, madness is genius and it'…be absolutely ridiculous than absolutely boring.”", "“Try not to become a man of success. Rather become a man of value.”", "“It is better to be hated for what you are than to be loved for what you are not.”", "“I have not failed. I've just found 10,000 ways that won't work.”", "“A woman is like a tea bag; you never know how strong it is until it's in hot water.”", "“A day without sunshine is like, you know, night.”"]