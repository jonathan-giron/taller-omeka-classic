---
title: Taller de Omeka. Ejercicio "Biblioteca imposible"
author: Jonathan Girón Palau
date: 2026
fontfamily: times
---

# Ejercicio: Biblioteca imposible

## Qué es esta colección

La *Biblioteca imposible* reúne cinco **portadas apócrifas**: memes que circularon en X (antes Twitter) y que toman el diseño de un libro real para mezclarlo con otra referencia de la cultura popular. Ninguno de estos libros existe, pero cada uno depende por completo de que reconozcamos el libro original.

Por eso son un material ideal para practicar Dublin Core. Obligan a distinguir entre:

- **el objeto que describimos** (la imagen-meme, publicada en una fecha y por una cuenta concretas),
- **la obra que cita** (el libro original, con su autor, editorial y año),
- **la fuente de donde la tomamos** (la URL en X).

> Pregunta guía del módulo 2: *¿estoy describiendo al objeto mismo o a una fotografía del objeto?* Aquí la pregunta es: **¿estoy describiendo el meme o el libro?**

## Los cinco ítems y su contexto

### 1. *El laberinto del fauno*, de Octavio Paz

- **Libro original:** *El laberinto de la soledad*, de Octavio Paz (1914-1998). Ensayo sobre la identidad mexicana publicado en 1950 por Cuadernos Americanos. En 1959 el Fondo de Cultura Económica publicó una edición revisada y aumentada, y desde entonces el libro lo edita el FCE. La portada del meme imita una edición del FCE, con el logotipo de la editorial bajo el título.
- **Referencia mezclada:** *El laberinto del fauno* (2006), película de Guillermo del Toro. El fauno sustituye a la ilustración original.
- **Para discutir:** dos "laberintos" mexicanos canónicos, uno literario y otro cinematográfico, y dos "Premios" (Nobel 1990 / Óscar). ¿Qué campo registra esa relación? → `dc.relation`.
- **Fuente:** <https://pbs.twimg.com/media/HDn-kMKWUAEfleQ.jpg>. Fecha de publicación en X: **2026-03-17**.

### 2. *La insoportable amsiedad del cheems*

- **Libro original:** *La insoportable levedad del ser*, de Milan Kundera (1929-2023). Novela escrita en checo y publicada por primera vez en 1984, en traducción francesa (Gallimard). En español la publica Tusquets en su colección **Andanzas**, cuyo diseño reproduce el meme: título en tipografía serif blanca sobre fondo oscuro, la leyenda "colección andanzas" en cursiva y una ilustración enmarcada.
- **Referencia mezclada:** *Cheems*, el perro shiba inu de un meme de internet, y su "amsiedad", la ortografía deliberadamente errónea típica de ese meme.
- **Para discutir:** el registro lingüístico. ¿Cómo se transcribe un título con faltas de ortografía intencionales? Se transcribe **tal cual** y, si hace falta, se añade una nota en `dc.description`.
- **Fuente:** <https://pbs.twimg.com/media/F5svDIqaQAAzNOf.jpg>. Fecha: **2023-09-10**.

### 3. *Amuleto* (Facultad de Economía), de Roberto Bolaño

- **Libro original:** *Amuleto*, de Roberto Bolaño (1953-2003), Anagrama, 1999. La narradora, Auxilio Lacouture, poeta uruguaya, queda encerrada en un baño de la **Facultad de Filosofía y Letras de la UNAM** durante la ocupación de Ciudad Universitaria por el ejército en septiembre de 1968. El meme reproduce el diseño de la colección **Compactos** de Anagrama.
- **Referencia mezclada:** una captura de pantalla del 16/08/2024 en la que un usuario dice haber quedado atrapado en un baño de la Facultad de Economía de la UNAM, y la cuenta @UNAM_MX responde "¿Sigues atrapado?".
- **Para discutir:**
  - *Ética y privacidad:* el autor del meme tachó el nombre del usuario. ¿Lo mantendríamos así al publicarlo? ¿Debería la descripción mencionar al usuario?
  - *Autenticidad:* no podemos verificar que la respuesta de @UNAM_MX sea auténtica y no un montaje. ¿Cómo se registra esa incertidumbre? En `dc.description`, con una frase como "no verificado".
  - Es el ítem con más capas: libro + tuit + respuesta institucional + 1968 + 2024.
- **Fuente:** <https://pbs.twimg.com/media/GVNrxI-WEAAJgxN.jpg>. Fecha: **2024-08-17**, un día después de la captura.

### 4. *La invención de la tradición*, de Eric Hobsbawm y Terence Ranger

- **Libro original:** *The Invention of Tradition*, editado por Eric Hobsbawm (1917-2012) y Terence Ranger (1929-2015), Cambridge University Press, 1983. En español la publicó Crítica (Barcelona) en su colección **Libros de Historia**, cuyo diseño reproduce el meme. Su tesis es que muchas tradiciones que parecen antiguas son invenciones recientes que crean un sentido de continuidad con el pasado.
- **Referencia mezclada:** una fotografía del **Desfile de Día de Muertos** de la Ciudad de México. El desfile se realizó por primera vez en 2016, inspirado en la secuencia inicial de la película de James Bond *Spectre* (2015), que mostraba un desfile que entonces no existía.
- **Para discutir:** es el ejemplo perfecto de la tesis del libro, y ahí está el chiste. El meme se publicó el 30 de octubre, en vísperas del Día de Muertos. ¿Qué pondríamos en `dc.coverage`: 2016, 1983 o 2024? Recordemos que *coverage* es el tema, no la fecha de creación.
- **Fuente:** <https://pbs.twimg.com/media/GbKWcuZakAEOTXe.jpg>. Fecha: **2024-10-30**.

### 5. *Historia. Quinto grado*

- **Libro original:** los **Libros de Texto Gratuitos** de la SEP, editados por la Comisión Nacional de Libros de Texto Gratuitos (Conaliteg, fundada en 1959), en este caso el de Historia de quinto grado de primaria. La composición de la portada, con una bandera ondeando ante un cielo de nubes encendidas, evoca la iconografía patriótica de las portadas clásicas de los libros de texto.
- **Referencia mezclada:** dos gatos vestidos como **adelita y revolucionario**, con la bandera mexicana y un rifle, en alusión a la Revolución Mexicana, que se estudia en ese grado.
- **Autoría:** la propia imagen lleva una firma: "Por @co3ndu / Vía @neomexicanismos". Es el **único ítem con autor identificado**, y además distingue entre quien crea la imagen y quien la difunde. ¿`dc.creator` o `dc.contributor`/`dc.publisher`?
- **Para discutir:** el meme se publicó el 19 de noviembre, un día antes del aniversario de la Revolución (20 de noviembre).
- **Fuente:** <https://pbs.twimg.com/media/GctXMjDXwAAKSVL.jpg>. Fecha: **2024-11-19**.

## Nota sobre las fuentes y las fechas

Las imágenes se descargaron de X. Su nombre de archivo original (por ejemplo `GVNrxI-WEAAJgxN.jpg`) es el identificador del archivo en el servidor de imágenes de X, así que la URL `https://pbs.twimg.com/media/<identificador>.jpg` sigue mostrando la imagen. Ese identificador también codifica el momento en que se subió la imagen: de ahí salen las fechas de esta guía. En el caso de *Amuleto*, la fecha coincide con la de la captura que aparece dentro de la imagen.

Limitaciones que conviene decir en voz alta en el taller:

- La URL apunta a la **imagen**, no al **tuit**. Sin el tuit no sabemos qué cuenta lo publicó ni si es la publicación original o una republicación. Por eso, salvo en el ítem 5, `dc.creator` queda como "Desconocido".
- Las imágenes de X pueden borrarse en cualquier momento. ¿Qué implica eso para un repositorio que cita esa URL como fuente? → Conecta con la "A" de FAIR y con la preservación.

## Instrucciones para participantes

1. En tu sitio de Omeka.net, crea la colección **Biblioteca imposible** y describe al menos `Título` y `Descripción`.
2. Elige **dos** de los cinco ítems y créalos a mano: *Items → Add an Item*.
   - Tipo de elemento: **Imagen fija** (Still Image).
   - Llena los campos Dublin Core con ayuda de la ficha de abajo.
   - Sube la imagen y marca el ítem como **público**. Si no tienes los archivos de la sesión, descarga la imagen desde el enlace de **Fuente** de cada ítem (clic derecho → Guardar imagen).
   - Añade etiquetas, por ejemplo: `meme`, `portada apócrifa`, `parodia`, más el nombre del autor original.
3. *(Opcional, para quien termine antes)* Importa los cinco ítems de golpe con el plugin **CSV Import** usando `biblioteca_imposible.csv`. Al mapear las columnas, marca `Tags` como etiquetas (separador: coma), `File` como archivo (contiene la URL de la imagen en X, porque CSV Import no acepta archivos locales) e `Item Type` como tipo de elemento. El separador de valores múltiples en `Subject` es el punto y coma. Compara: ¿qué ganaste y qué perdiste al importar en lugar de describir a mano?
4. Asigna los ítems a la colección.

## Ficha modelo (ítem 4)

| Campo | Valor |
|---|---|
| Title | La invención de la tradición [portada apócrifa con el Desfile de Día de Muertos] |
| Subject | Memes; Parodia; Portadas de libros; Día de Muertos; Tradiciones inventadas |
| Description | Meme que reproduce el diseño de la colección Libros de Historia (Editorial Crítica) para el libro de Eric Hobsbawm y Terence Ranger, sustituyendo la ilustración por una fotografía del Desfile de Día de Muertos de la Ciudad de México, celebrado desde 2016 a partir de la película *Spectre* (2015). Ironiza sobre la tesis del libro. |
| Creator | Desconocido |
| Source | https://pbs.twimg.com/media/GbKWcuZakAEOTXe.jpg |
| Publisher | X (Twitter) |
| Date | 2024-10-30 |
| Contributor | Girón Palau, Jonathan (catalogación) |
| Rights | Derechos no evaluados (http://rightsstatements.org/vocab/CNE/1.0/) |
| Relation | Hobsbawm, Eric y Terence Ranger (eds.). *The Invention of Tradition*. Cambridge University Press, 1983. |
| Format | image/jpeg |
| Language | es |
| Type | Still Image |
| Identifier | 04_La_invencion_de_la_tradicion.jpg |
| Coverage | Ciudad de México; 2016- |

## Ideas para el Ejercicio 3 (exhibición)

Exhibición sugerida: **"Juzgar un libro por su portada: memes y cultura editorial en español"**.

- **Página 1. Introducción:** bloque de texto. ¿Qué es una portada apócrifa? ¿Por qué el chiste solo funciona si reconocemos el diseño editorial?
- **Página 2. Colecciones editoriales como marca:** galería con Andanzas, Compactos, Libros de Historia y FCE. El diseño de colección como lenguaje visual.
- **Página 3. La UNAM en el meme:** archivo con texto. *Amuleto*: 1968/2024, el baño como espacio literario y como chiste.
- **Página 4. Tradiciones inventadas:** archivo con texto con Hobsbawm y el libro de texto gratuito. Historia nacional, patria y cultura pop.
- **Página 5. ¿Quién es el autor de un meme?:** texto. Autoría, derechos y anonimato (enlaza con el Ejercicio 4).
