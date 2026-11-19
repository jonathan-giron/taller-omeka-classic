---
title: Taller de Omeka. Objetos digitales
author: Jonathan Girón Palau
date: 2026
fontfamily: times
---

# Objetos digitales (items)

## Elementos (Items): Los componentes fundamentales

Los **elementos** o **ítems** constituyen la unidad básica de cualquier proyecto en Omeka. Estos objetos digitales representan la materia prima de nuestro repositorio y pueden incluir prácticamente cualquier tipo de material: documentos históricos digitalizados, fotografías, grabaciones de audio, videos, manuscritos, obras de arte, testimonios orales, mapas antiguos, o cualquier otro recurso digital que queramos preservar y compartir.

La flexibilidad de Omeka permite que estos elementos se adapten a una amplia variedad de proyectos académicos y culturales. Desde repositorios sencillos que facilitan la consulta y descarga de documentos organizados temáticamente, hasta complejas narrativas digitales que culminan en exhibiciones virtuales interactivas, recursos educativos multimedia, o publicaciones académicas enriquecidas.

### Organización jerárquica: De elementos a narrativas

Los elementos no existen de forma aislada, sino que pueden **organizarse en colecciones** según criterios temáticos, cronológicos, tipológicos o metodológicos. Estas colecciones, a su vez, sirven como material base para crear **exhibiciones** – espacios curatoriales donde los elementos se combinan con textos interpretativos para construir argumentos académicos, narrativas históricas, o experiencias educativas.

Es importante entender que lo que Omeka denomina "exhibición" trasciende el concepto museológico tradicional. Estas exhibiciones pueden funcionar como **recursos educativos interactivos**, **publicaciones académicas digitales**, **argumentos de investigación visualizados**, o **experiencias narrativas multimedia**.

### Tipologías de elementos predefinidas

Omeka Classic incluye **16 tipos de elementos predefinidos** que cubren la mayoría de necesidades de proyectos académicos y culturales:

- **Dataset**: Conjuntos de datos, bases de datos
- **Email**: Correspondencia digital, comunicaciones
- **Evento**: Conferencias, performances, acontecimientos históricos
- **Hipervínculo**: Enlaces a recursos externos
- **Recurso interactivo** Recursos que requieren de la interacción con el usuario para ser entendidos y ejecutados (páginas web, servicios de chat, entornos de realidad virtual)
- **Lección**: Materiales educativos, tutoriales
- **Imagen en movimiento**: Videos, documentales, películas
- **Historia oral** Recursos que contienen información histórica obtenida a partir de entrevistas con personas
- **Persona**: Biografías, perfiles de individuos
- **Objeto físico**: Artefactos, obras de arte, especímenes
- **Servicio**: Recursos o servicios digitales
- **Software**: Aplicaciones, programas, código
- **Sonido**: Grabaciones de audio, música, testimonios orales
- **Imagen fija**: Fotografías, pinturas, dibujos, mapas
- **Texto**: Obras literarias, ensayos, artículos
- **Sitio web**: Referencias a sitios completos

### Personalización y extensibilidad

Si los tipos predefinidos no se ajustan completamente a las necesidades específicas del proyecto, Omeka permite **modificar los tipos existentes** o **crear tipos completamente nuevos**. Esta flexibilidad asegura que la plataforma pueda adaptarse a las particularidades de cualquier disciplina o metodología de investigación, desde estudios literarios hasta antropología visual, desde historia oral hasta archivos de arte contemporáneo.

## Guía de metadatos Dublin Core en Omeka Classic

### Campos fundamentales de descripción

| Campo | Definición | Recomendaciones de uso |
|-------|------------|------------------------|
| **dc.title** | Nombre del elemento que estás describiendo | Establece convenciones consistentes: mayúsculas/minúsculas, información suplementaria entre corchetes, etc. |
| **dc.creator** | Persona u organización principalmente responsable de crear el elemento (artista, autor) | Utiliza vocabularios controlados: Library of Congress Name Authority File (LCNAF), Union List of Artist Names (ULAN), o Virtual International Authority File (VIAF) |
| **dc.contributor** | Persona u organización que contribuyó al recurso (ilustrador, editor, traductor) | Usa los mismos vocabularios controlados que para dc.creator |
| **dc.date** | Punto o período temporal asociado con el elemento (fecha de creación original) | Emplea el estándar internacional: 2017-01-01. Consulta la nota W3C sobre formatos de fecha y hora |
| **dc.description** | Descripción en texto libre del elemento | Espacio ideal para información que no encaja en campos más estructurados |
| **dc.rights** | Información sobre el estatus legal del elemento | Usa descripciones estándar: licencias Creative Commons o declaraciones de RightsStatements.org |
| **dc.subject** | Tema del elemento que describes | Vocabularios controlados recomendados: Library of Congress Subject Headings (LCSH) o Thesaurus for Graphic Materials (TGM) |
| **dc.coverage** | Ubicación espacial o temporal que trata el elemento (no dónde/cuándo se creó, sino de qué lugar/época trata) | Espacial: Thesaurus of Geographic Names (TGN). Temporal: formato estructurado similar a dc.date |
| **dc.publisher** | Persona u organización responsable de hacer disponible el elemento | Vocabularios controlados: LCNAF, ULAN, o VIAF |
| **dc.relation** | Cita de un elemento relacionado | Incluye URL si aparece en otra colección digital |
| **dc.source** | Cita de dónde se encontró este elemento (institución, recurso impreso) | Incluye URL si aparece en otra colección digital |
| **dc.format** | Medio físico, formato de archivo, o dimensiones del elemento | Vocabulario controlado recomendado: Art & Architecture Thesaurus (AAT) |
| **dc.type** | Naturaleza o género del elemento | Vocabulario controlado: DCMI Type Vocabulary |
| **dc.language** | Idioma del elemento | RFC 5646: Tags for Identifying Languages. Ejemplo: inglés estadounidense = en-US. ¡Mantén consistencia! |
| **dc.identifier** | Referencia inequívoca al elemento | Nombre de archivo o URI |

### Consideraciones prácticas para proyectos académicos

**Consistencia:** Establece convenciones claras desde el inicio del proyecto. Define formatos estándar para nombres, fechas, y terminología específica de tu disciplina.

**Vocabularios controlados:** Aunque puede parecer tedioso, el uso de autoridades establecidas facilitará enormemente la búsqueda, interoperabilidad, y profesionalismo de tu colección.

**Información contextual:** Los campos `dc.description`, `dc.coverage`, y `dc.relation` son especialmente valiosos para preservar el contexto académico e histórico de los elementos.

**Derechos y acceso:** El campo `dc.rights` es crucial para proyectos que serán públicos. Define claramente qué pueden hacer los usuarios con tus materiales.

### Ejemplo práctico

**Para una carta histórica:**
- `dc.title`: "Carta de Octavio Paz a Alfonso Reyes, 15 de marzo de 1950"
- `dc.creator`: "Paz, Octavio, 1914-1998"
- `dc.date`: "1950-03-15"
- `dc.type`: "Text" (vocabulario DCMI Type; en la interfaz en español corresponde al tipo de elemento "Texto")
- `dc.language`: "es-MX"
- `dc.coverage`: "México--Historia--Siglo XX"
- `dc.rights`: "Copyright © Fundación Octavio Paz"


