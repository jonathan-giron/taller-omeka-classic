---
title: Taller de Omeka. Colecciones y exhibiciones
author: Jonathan Girón Palau
date: 2026
fontfamily: times
---

## Colecciones

Las **colecciones** son agrupaciones de elementos de Omeka. Pueden utilizarse en diversos contextos que resulten más apropiados para tu archivo digital.

En Omeka Classic, **un elemento solo puede pertenecer a una colección** (pero pueden pertenecer a distintas exhibiciones). Las colecciones, por supuesto, pueden contener múltiples elementos. El concepto de colecciones en Omeka tiene su origen en las colecciones de museos y archivos; no se puede colocar un documento en más de una caja física. Sin embargo, no es necesario seguir una interpretación tradicional de colección, como por propietario o donante.

Las **colecciones no tienen jerarquía** por defecto, a menos que instales el plugin **Collection Tree** para crear colecciones anidadas. Los elementos dentro de las colecciones **no tienen un orden establecido**, a menos que instales el plugin **Item Order** y reorganices manualmente tus elementos.

### Consideraciones para el diseño de colecciones

**Flexibilidad conceptual:** Aunque Omeka emula la lógica física de archivos y museos, puedes organizar tus colecciones según criterios académicos más flexibles: períodos históricos, temas de investigación, géneros literarios, metodologías, o cualquier otra lógica que sirva a tu proyecto.

**Limitación de pertenencia única:** Recuerda que cada elemento solo puede estar en una colección. Planifica cuidadosamente tu estructura organizativa. Si necesitas que los elementos aparezcan en múltiples agrupaciones, considera usar **etiquetas** como sistema complementario de organización.

**Extensibilidad mediante plugins:** Los plugins **Collection Tree** e **Item Order** pueden agregar funcionalidades importantes si tu proyecto requiere jerarquías complejas u organización secuencial específica.

- describir nuestra colección mediante el esquema de metadatos DC (como mínimo el campo título)

### Agregar elementos a colecciones

Para agregar elementos a colecciones, **primero debes crear la colección**. 

Los elementos **pueden agregarse a una colección** desde la página de edición del elemento o desde la página de navegación de elementos.


#### Imagen miniatura y elemento destacado

La **imagen miniatura** de una colección se deriva automáticamente del archivo principal del elemento creado más recientemente en la colección. Sin embargo, si tienes un elemento marcado como **"destacado"** (featured), la miniatura corresponderá al elemento destacado creado más recientemente en la colección.

## Exhibiciones

Las **exhibiciones** se componen de **páginas**, generalmente una página inicial que introduce tu exhibición y páginas posteriores compuestas por elementos de tu base de datos de Omeka Classic que deseas destacar y/o relacionar entre sí. Las exhibiciones de Exhibit Builder pueden ser tan cortas como una página o consistir en múltiples páginas. Puedes hacer que las páginas de una exhibición sean jerárquicas.

El diseño de las exhibiciones en Exhibit Builder es personalizable, con páginas compuestas por unidades más pequeñas llamadas **bloques**. Hay **cuatro tipos básicos de bloques de contenido** que vienen con Exhibit Builder:

- **Archivo con texto** (file with text)
- **Galería** (gallery)  
- **Texto** (text)
- **Archivo** (file)

**Para poder crear una exhibiciones** primero se tiene que instalar el plugin Exhibit Builder

--

## Configurar nuestra página (apariencia)

> En el plan gratuito de Omeka.net solo están disponibles los temas **Berlin** y **Seasons**; las opciones de configuración descritas abajo pueden variar según el tema.

## Temas en Omeka Classic

Los **temas** determinan el aspecto y la sensación del lado público de tu sitio Omeka. Explora nuestros temas y nuestro directorio de ejemplos para ver la variedad de diseños y personalizaciones disponibles.

La mayoría de los temas tienen varias configuraciones que pueden ser personalizadas en el panel de administración por los superusuarios del sitio. Si quieres personalizar aún más un tema, o crear el tuyo propio, puedes hacerlo editando los archivos en el lado del servidor.

### Gestión de temas

El **tema activo** se muestra en la parte superior, con una vista previa de la apariencia del tema, un resumen de sus características, y un botón para configurar el tema.

Si el tema activo está desactualizado, verás un mensaje bajo el resumen del tema activo que dice "Una nueva versión de este tema está disponible. Obtén la nueva versión." La frase "Obtén la nueva versión" es un enlace a la página donde puedes descargar la última versión de tu tema. Para actualizar, simplemente sigue las instrucciones de instalación, reemplazando la carpeta del tema desactualizado con la nueva.

Los **temas inactivos** no te solicitarán actualizar. Puedes considerar eliminar los temas inactivos para simplificar tu instalación de Omeka una vez que hayas terminado de personalizar su diseño.

### Configuración de un tema

Las configuraciones te permiten tomar decisiones sobre el aspecto de tu sitio, incluyendo agregar un logo y texto de página de inicio, gestionar elementos destacados, y agregar texto de pie de página.

Las configuraciones que hagas son **únicas para cada tema** y se guardarán con ese tema. Para configurar tu tema, haz clic en el botón "Configurar tema" debajo del gráfico del tema para personalizar tu sitio.

### Opciones de configuración de **Encabezado y Pie de página**:

* **Archivo de Logo**: Puedes subir una imagen que reemplazará el título del sitio en el encabezado de tu sitio web. En muchos temas, este logo estará alineado a la izquierda, con márgenes alrededor. Muchos temas recomiendan un ancho máximo para tu logo de 500px, y algunos tienen una altura máxima requerida de 150px.

* **Fondo del Encabezado**: Sube un archivo de imagen que se mostrará en la parte superior de tu sitio web, detrás del título de tu sitio o logo.

* **Texto del Pie de Página**: Una caja de texto habilitada para HTML donde puedes ingresar texto para un pie de página del sitio que aparezca en cada página. Ten en cuenta que los códigos cortos no funcionarán en este campo, ni tampoco las imágenes codificadas en HTML u otros multimedia.

* **Mostrar Copyright en el Pie de Página**: Marca esta casilla si deseas mostrar la información de copyright de tu sitio en el pie de página. La información de copyright del sitio se encuentra en la sección de Configuraciones Generales.

* **Usar Búsqueda Avanzada para Todo el Sitio**: Marca esta casilla para permitir que los visitantes del lado público busquen en todo el sitio, incluyendo elementos, colecciones y archivos, y para usar métodos booleanos al buscar.