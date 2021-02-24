# Scrapear webs para aprender idiomas

Para aprender idiomas, la web [www.languagepod101.com](https://www.languagepod101.com/) propone una misma metodología independientemente del idioma. Esta consiste en **aprender cada día una palabra nueva** y usar dicha palabra en un par de frases. Además de la palabra en el idioma que se quiera aprender (el turco en el caso de nuestro notebook) y las frases donde usarla, también aparece su traducción al inglés. 

Vamos a scrapear la web que nos propone las palabras en turco ([www.turkishclass101.com](www.turkishclass101.com)) yendo día a día a lo largo de un periodo de tiempo que nosotros determinemos para poder **sacar un archivo Excel** con una tabla donde aparezcan la lista de palabras, su traducción y las frases donde se usan (con su traducción igualmente).

Vamos a hacer este scraping usando la librería [autoscraper](https://github.com/alirezamika/autoscraper), que facilita el web scraping al aprender las reglas del scraping de una URL dada, y devuelve los elementos con una estructura similar de esa URL u otras URLs con contenido similar.


### Ejecución del código
En este notebook se explica paso a paso cómo hacer el web scraping, pasar los datos a un formato tabular y guardarlos en formato csv. Si se quiere correr el código directamente solo hará falta ejecutar la importación de librerías, la inicialización del autoscraper y la función final que engloba todos los pasos intermedios. 

Los inputs que necesita la función son: 
- Fecha de inicio del scraping (string en formato día-mes-año)
- Fecha de fin del scraping (string en formato día-mes-año)
- Carpeta donde queremos guardar el archivo (puede ser un string vacío)
- Nombre del archivo (string)
