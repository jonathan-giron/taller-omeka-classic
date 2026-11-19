---
title: Taller de Omeka. Introducción
author: Jonathan Girón Palau
date: 2026
fontfamily: times
---

# Introducción

Omeka es una plataforma de código abierto diseñada para crear repositorios digitales accesibles desde la web. Su objetivo principal es facilitar la publicación de colecciones digitales y exposiciones en línea para archivos, bibliotecas, museos y otras entidades vinculadas al patrimonio cultural.

Fue creado en el Roy Rosenzweig Center for History and New Media (Universidad George Mason) y se distribuye bajo licencia GPL v3, lo que permite su uso, modificación y adaptación sin restricciones económicas. Está especialmente orientado a usuarios no técnicos, ya que su interfaz prioriza la gestión de contenidos sobre la necesidad de programación.

Omeka emplea estándares abiertos, como el esquema Dublin Core para la descripción de ítems, y admite otros vocabularios como BIBO, Dublin Core Type, y FOAF. También es compatible con OAI-PMH, lo que permite compartir recursos con otros sistemas mediante recolección de metadatos. Gracias a su arquitectura basada en plugins y temas, puede ampliarse fácilmente con funciones adicionales —por ejemplo, mapas interactivos, cronologías o visores de imágenes— y ajustarse visualmente a cada proyecto.

Omeka se describe a sí mismo como una "plataforma web gratuita, flexible y de código abierto para la publicación y exhibición de colecciones de bibliotecas, museos, archivos y materiales académicos".


## Desarrollo y comunidad

Omeka nació en el Roy Rosenzweig Center for History and New Media (RRCHNM) de la George Mason University, el mismo centro donde surgieron otros proyectos de referencia como:
- Zotero - Sistema de gestión de referencias bibliográficas
- Otros proyectos de humanidades digitales: <https://rrchnm.org/our-work/>

Actualmente Omeka es mantenido por **Digital Scholar**, una organización sin fines de lucro que desarrolla el software y administra el servicio Omeka.net. Al momento de esta edición (noviembre de 2026), la versión vigente es **Omeka Classic 3.2.2** (septiembre de 2026), y el plugin Exhibit Builder va en la versión 3.11.1.


## Características principales

- Software libre y gratuito - No dependes de grandes plataformas comerciales
- Sin conocimientos avanzados de programación requeridos
- Utiliza estándares y protocolos ampliamente aceptados
- Puede ejecutarse localmente en tu propio servidor o en servidores de Omeka en la nube
- Comunidad activa de usuarios y amplia documentación:
	- <https://omeka.org/classic/docs/>
	- <https://www.rubenalcaraz.es/manual-omeka/introduccion-omeka.html>
	- <https://programminghistorian.org/es/lecciones/?search=omeka>
	- <https://info.omeka.net/build-a-website/change-site-navigation/>


## Las tres variantes del proyecto Omeka

Actualmente el proyecto Omeka se divide en tres productos:

- **Omeka Classic:** plataforma de publicación web para construir y compartir colecciones digitales y exhibiciones. Se descarga desde omeka.org y se instala en un servidor propio.
- **Omeka S** (Semantic), lanzada en 2017: pensada para instituciones que administran varios sitios desde una sola instalación y enfocada en la conexión de las colecciones con la web semántica (Linked Open Data). También se instala en un servidor propio.
- **Omeka.net:** servicio de alojamiento en la nube que ofrece Omeka Classic ya instalado. Cualquier persona con una cuenta puede crear o colaborar en un sitio sin administrar un servidor. Tiene un plan gratuito y varios planes de pago.

Este material se basa en Omeka Classic, la versión más establecida y accesible para proyectos académicos y culturales. Para el taller usaremos el plan gratuito de Omeka.net.


## Funcionalidades principales

- Permite crear archivos <colecciones organizadas>
- Permite crear exhibiciones <narrativas curatoriales>
- Gestión profesional de metadatos



# Omeka y los principios FAIR:

<https://omeka.org/news/2025/08/13/omeka-and-FAIR/>


Arquitectura técnica orientada a la interoperabilidad

Omeka Classic está construido desde sus fundamentos para facilitar la interoperabilidad y reutilización de datos a través de metadatos estructurados. Su arquitectura técnica implementa de manera concreta los Principios FAIR (Findable, Accessible, Interoperable, Reusable | en español: Encontrable, Accesible, Interoperable, Reutilizable).

¿Qué son los Principios FAIR?

Los Principios Guía FAIR surgieron de un taller inicial en Leiden en 2014, fueron articulados, refinados y publicados en Scientific Data en 2016. Estos principios fueron diseñados para facilitar la creación y publicación de datos de investigación y colecciones que sean accesibles y reutilizables tanto para el descubrimiento humano como automatizado.

Los cuatro pilares FAIR:

F - Findable (Encontrable)
- Los datos deben tener identificadores únicos y persistentes
- Deben estar descritos con metadatos ricos
- Los metadatos deben estar registrados en recursos de búsqueda
A - Accessible (Accesible)
- Los datos deben ser recuperables mediante protocolos estandarizados
- Los protocolos deben ser abiertos y gratuitos
- Los metadatos deben permanecer accesibles incluso cuando los datos ya no estén disponibles
I - Interoperable (Interoperable)
- Los datos deben usar lenguajes formales y compartidos para la representación del conocimiento
- Deben emplear vocabularios que sigan los principios FAIR
- Deben incluir referencias cualificadas a otros datos
R - Reusable (Reutilizable)
- Los datos deben estar ricamente descritos con atributos precisos y relevantes
- Deben publicarse con licencias claras de uso
- Deben incluir información detallada sobre su procedencia


Características FAIR en Omeka Classic:

Encontrabilidad (Findable):
- Utiliza el esquema de metadatos Dublin Core para estructurar la descripción de elementos, archivos y colecciones
- Los metadatos pueden ser registrados en recursos de búsqueda determinados por el usuario
Accesibilidad (Accessible):
- Protocolo HTTPS y API REST estándar
- Sistema de autenticación y autorización
- Política de preservación de metadatos determinada por el usuario
Interoperabilidad (Interoperable):
- Formatos de salida estándar: atom, dcmes-xml, json, omeka-xml y rss2. Se obtienen agregando `?output=<formato>` a una página de ítems o colecciones, por ejemplo `/items/browse?output=dcmes-xml`
- Todos accesibles mediante API
- Plugin disponible OAI-PMH Repository para intercambio de metadatos
- Plugin LC Suggest para vocabularios estructurados
Reutilización (Reusable):
- Licencias de uso determinadas por el usuario
- Metadatos de procedencia mediante Item Type metadata
- Cumplimiento de estándares comunitarios específicos del dominio

Preservación (plugins nuevos, abril de 2026):
- **Exports:** permite descargar los metadatos de ítems, colecciones, archivos y exhibiciones en CSV o JSON, útil para respaldos o para depositarlos en un repositorio institucional.
- **Static Site Export:** genera una copia "plana" del sitio público que puede reconstruirse con Hugo como sitio estático, útil para conservar proyectos que ya no se actualizan.
- Ver: <https://omeka.org/news/2026/04/30/new-preservation-plugins-for-omeka-classic/>

Dimensión social de los principios FAIR

Es importante reconocer que este trabajo es tanto social como técnico. Todo el trabajo de descripción y datos ocurre en un contexto, y ese contexto es esencial para gobernar la forma en que los datos se forman, publican y reutilizan.
El consenso sobre estándares de descripción debe lograrse dentro de una comunidad de práctica para que los miembros de esa comunidad inviertan y desplieguen métodos compartidos de representación del conocimiento dentro de su campo.

### Relevancia para las humanidades digitales

La adopción de los principios FAIR en Omeka representa un paso importante hacia la democratización de la gestión de datos académicos en las humanidades. Permite que:
- Investigadorxs publiquen datos según estándares internacionales
- Las colecciones digitales sean más fácilmente descubiertas y reutilizadas
- Se facilite la colaboración interdisciplinaria
- Se preserve el patrimonio cultural digital para futuras generaciones

Esta aproximación convierte a Omeka no solo en una herramienta de publicación, sino en una plataforma para la ciencia abierta en humanidades.



