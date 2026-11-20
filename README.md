# Taller de Omeka Classic

Materiales del taller de Omeka Classic, 2026.

## Contenido del repositorio

| Archivo / carpeta | Contenido |
|---|---|
| `README.md` | Objetivos, ejercicios y agenda del taller (este documento) |
| `1 Introducción.md` | Qué es Omeka, variantes, comunidad y principios FAIR |
| `2 Primeros pasos.md` | Estructura de un sitio, ejemplos y registro en Omeka.net |
| `3 Objetos digitales.md` | Ítems, tipos de elemento y guía de metadatos Dublin Core |
| `4 Colecciones y exhibiciones.md` | Colecciones, Exhibit Builder y temas |
| `imaagenes gral/Ejercicio/Biblioteca imposible/` | Guía del ejercicio y CSV para importar los ítems con CSV Import |
| `imaagenes gral/DC_Metadata.xml` | Ejemplo de registro Dublin Core (ejercicio *Palestina*) |
| `imaagenes gral/*.png` | Capturas de pantalla de Omeka.net |
| `imaagenes gral/Tutorial.md` y `Ejercicio/HTML/` | Material de apoyo y fragmentos HTML de ejemplo |

**Sobre las imágenes de los ejercicios:** las imágenes de terceros no se incluyen en este repositorio.

## Objetivos de Aprendizaje

Al finalizar el taller, los participantes serán capaces de:

- Identificar y describir las ventajas y limitaciones de Omeka Classic como plataforma para proyectos digitales
- Comprender los elementos fundamentales de un proyecto en Omeka (elementos, colecciones, exhibiciones)
- Evaluar críticamente proyectos existentes de humanidades digitales realizados con Omeka
- Crear contenido básico en la plataforma (subir elementos, organizar colecciones)
- Diseñar una narrativa digital simple mediante exhibiciones
- Fortalecer su confianza como colaboradores potenciales en proyectos de humanidades digitales

## Estructura del Taller

**Ejercicio 1:** Análisis crítico de un proyecto existente (30 minutos)

Equipos de 3-4 personas; cada equipo analiza un sitio distinto: Cleveland Historical, un sitio del directorio de Omeka Classic <https://omeka.org/classic/directory/> y uno de la UNAM.

Guía de observación:

1. **Objeto y propósito:** ¿qué colecciona el sitio, para quién y con qué argumento?
2. **Estructura:** ¿cuántas colecciones hay y con qué lógica se agrupan? ¿Hay exhibiciones y página "Acerca de"?
3. **Metadatos:** abre dos ítems. ¿Qué campos Dublin Core usan? ¿Son consistentes? ¿Se dice de dónde viene el objeto (`source`) y qué se puede hacer con él (`rights`)?
4. **Decisiones curatoriales:** ¿quién habla en las exhibiciones? ¿Qué queda fuera?
5. **FAIR en la práctica:** Omeka Classic puede entregar sus metadatos en formatos legibles por máquinas, no solo como página web. Ve a la lista de ítems del sitio (la dirección termina en `/items/browse`) y agrega al final `?output=dcmes-xml` (Dublin Core en XML) o `?output=json`. Ejemplo: <https://clevelandhistorical.org/items/browse?output=dcmes-xml>. Si aparece código en lugar de la página, el sitio es interoperable: otros sistemas pueden recolectar sus datos. Después revisa si los ítems dicen bajo qué licencia se pueden reutilizar (campo `Rights`).
6. **Sostenibilidad:** ¿el sitio está vivo? Busca fechas, enlaces rotos e imágenes caídas.

Producto: una fortaleza, una debilidad y una decisión que el equipo copiaría.

**Ejercicio 2:** Creación de elementos en Omeka (45 minutos)

- Configuración básica de un sitio en el plan gratuito (Free) de Omeka.net
- Subida y descripción de elementos (textos, imágenes, documentos)
- Aplicación de metadatos Dublin Core
- Uso de etiquetas y organización básica
- Opcional: importación por lotes con CSV Import

**Ejercicio 3:** Colecciones y exhibiciones (40 minutos)

- Creación de colecciones temáticas
- Diseño de una exhibición narrativa
- Vista previa y ajustes de presentación

**Ejercicio 4:** Reflexión sobre roles colaborativos (20 minutos)

Dinámica "¿Quién hizo este sitio?": a partir del sitio que cada quien armó, se reconstruyen los roles que intervinieron, aunque los haya cumplido una sola persona.

| Rol | Pregunta guía | ¿Qué hiciste tú hoy que pertenece a este rol? |
|---|---|---|
| Investigación / curaduría | ¿Qué argumento cuenta la exhibición? | |
| Catalogación / metadatos | ¿Quién decide vocabularios y convenciones? | |
| Derechos y ética | ¿Podemos publicar esto? ¿Hay personas identificables? ¿Quién es el autor de un meme? | |
| Diseño / experiencia de usuario | ¿Se entiende la navegación? | |
| Gestión técnica | Plugins, respaldos, actualizaciones | |
| Preservación | ¿Qué pasa con el sitio en 5 años? (plugins Exports y Static Site Export) | |

Cierre (5 minutos): cada persona escribe en una tarjeta un proyecto que le gustaría hacer, qué rol asumiría y qué rol necesitaría de alguien más.

## Agenda sugerida (3 horas)

| Bloque | Minutos |
|---|---|
| Introducción (módulo 1) | 20 |
| Ejercicio 1: análisis crítico | 30 |
| Primeros pasos y creación del sitio en Omeka.net (módulo 2) | 20 |
| Ejercicio 2: ítems y Dublin Core (módulo 3) | 45 |
| Ejercicio 3: colecciones y exhibiciones (módulo 4) | 40 |
| Ejercicio 4: roles colaborativos | 20 |
| Cierre | 5 |


## Materiales Necesarios

- Computadora con acceso a internet
- Navegador web actualizado
- Cuenta en el plan gratuito (Free) de Omeka.net o acceso a una instancia de práctica de Omeka Classic
- Correo electrónico para activar la cuenta


## Resultados Esperados
Al concluir el taller, cada participante tendrá:

Productos tangibles:

- Un sitio Omeka básico con al menos 5 elementos catalogados
- Una colección temática organizada
- Una exhibición simple con narrativa coherente

<a rel="license" href="https://creativecommons.org/licenses/by-nc/4.0/deed.es"><img alt="Creative Commons License" style="border-width:0" src="https://licensebuttons.net/l/by-nc/4.0/88x31.png" /></a><br />Este tutorial fue elaborado por Jonathan Girón Palau bajo una licencia <a rel="license" href="https://creativecommons.org/licenses/by-nc/4.0/deed.es">Creative Commons Atribución/Reconocimiento-NoComercial 4.0 Internacional</a>.
