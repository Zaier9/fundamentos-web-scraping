# Robots.txt

Los archivos robots.txt exiten como una forma de administrar una página web. Proporciona información a los rastreadores de los buscadores sobre las páginas o los archivos que pueden solicitar o no de tu sitio web.
Principalmente, se utiliza para evitar que tu sitio web se sobrecargue con solicitudes.
En el contexto de webscraping, le dice al scraper que puede y no extraer. Es decir hasta donde puede llegar. Ya que infrigir en la violación
de estas directivas puede acarrear un problema legal con el sitio web al que estamos scrapeando.

## Robots.txt contiene entre otros elementos:

**USER-AGENT:** Identificadores de quienes acceden a tu sitio web, puede ser un archivo.py hasta un googlebot.

## DIRECTIVAS

**ALLOW:** Utiliza esta directiva para permitir a los motores de búsqueda rastrear un subdirectorio o una página, incluso en un directorio que de otro modo no estaría permitido
**DISALLOW:** Utiliza esta directiva para indicar a los motores de búsqueda que no accedan a archivos y páginas que se encuentren bajo una ruta específica


Ejemplo:

url/robots.txt
Pro ejemplo:

//Robots.txt file from http://www.nasa.gov
//All robots will spider the domain

User-agent: *
Disallow: /worldbook/
Disallow: /offices/oce/llis/