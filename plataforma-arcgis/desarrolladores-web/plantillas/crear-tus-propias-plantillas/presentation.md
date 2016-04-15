<!-- .slide: class="title" -->

## Crear tus propias plantillas
Plataforma ArcGIS para desarrolladores web

[desarrolladores.esri.es/moocs](http://desarrolladores.esri.es/moocs)

---

<!-- .slide: class="section" -->

## Recursos y herramientas
Podemos crearlas :
* https://github.com/Esri/application-boilerplate-js
* Web AppBuilder

## Cómo se registra

---

<!-- .slide: class="section" -->

## Cuándo crear una plantilla
Ventajas y limitaciones
* Si tenemos un tipo de interfaz que usamos mucho con datos distintos,

---

<!-- .slide: class="section" -->

## Ventajas y limitaciones de cada tipo
* Configurable:
	* Por ejemplo: titulo, logotipo, textos, visibilidad.
	* Ejemplos: Swipe, ...
* Auto-configurable:
	* Podremos elegir una capa de un servicio que se incluya en el webmap
	* Ejemplos: Geoform, MapJournal

que recibe un webmap y puede una aplicación. aplicaciones genérica que necesita Es el término usado en la plataforma ArcGIS para denominar la represetanción
  de un mapa en formato **JSON**

---

<!-- .slide: class="section" -->

## Integración con una orgazanicación

> Las plantillas se pueden registrar como items especiales en una organización para facilitar que los usuarios puedan crear instancias a partir de la interfaz del editor de mapas.

---

<!-- .slide: class="section" -->
## De qué se compone una plantilla

* Código fuente (HTML, CSS y JS)
* Item de aplicación (webmap, parámetros adicionales de configuración)


## Tipos de plantillas
* Configurables:  
	* Los parámetros de configuración son estánticos y se especifican en [formato JSON](http://doc.arcgis.com/es/arcgis-online/create-maps/configurable-templates.htm)
	* La interfaz de configuración la proporciona ArcGIS Online (o Portal por
	ArcGIS)
	* La configuración de cada aplicación instanciada se almacenada en los datos
	del item y siguen siempre la estructura del JSON especificado anteriormente.

* Auto-configurables:
	* Los parámestros de configuración pueden ser dinámicos
	* La interfaz de configuración se proporciona con el código de la aplicación
	* La estructura almacenada por cada instancia la definimos desde nuestra
	interfaz y por tanto
	almacenada no siempre tiene la misma estructura ya que puede depender de los
	datos del webmaps.

## Qué tecnología debo usar
La que mejor se adapte a los requisitos de tu app:
Si necesitas:
* Webmap: API JS
* Análisis: API JS
* Renderizadores avanzados:
* Móvil: leaflet, calcite,
* Basada en formularios: esri-angular

## Datos de las instancias
Configurable:
* Item: tipo Web Mapping Application
* Data: en el atributo **source** se indica el **item id** de la plantilla
de donde se recuperarán datos de configuración.

Al ser de tipo **Web Mapping Application** es obligatorio que en las keywords
tenga la tecnología (JavaScript) y el tipo de plantilla (purpose), que en nuestro
caso será Configurable

---

<!-- .slide: class="section" -->

## Otras referencias
* [Documentación sobre cómo añadir una plantilla a ArcGIS Online](
https://doc.arcgis.com/en/arcgis-online/share-maps/add-items.htm#ESRI_SECTION1_0D1B620254F745AE84F394289F8AF44B)
* [Cómo crear plantillas configurables](http://desarrolladores.esri.es/crear-plantillas-parametrizables-en-arcgis/)

*[Video tutorial: cómo crear plantillas configurables]
http://desarrolladores.esri.es/granada-bike-tour/

https://doc.arcgis.com/en/arcgis-online/create-maps/create-app-templates.htm

https://github.com/Geo-Developers/youtube-video-tour
