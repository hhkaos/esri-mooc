<!-- .slide: class="title" -->

## Introducción a las apps configurables
Plataforma ArcGIS para desarrolladores web

[desarrolladores.esri.es/moocs](http://desarrolladores.esri.es/moocs)

---

<!-- .slide: class="section" -->

## Qué es una app configurable

> Las también llamadas en ocasiones **plantillas**, son un mecanismo
que permite a usuarios de una organización crear y configurar
**aplicaciones web** sin necesidad de escribir código

---

<!-- .slide: class="section" -->

## [Demo](http://www.arcgis.com/home/webmap/viewer.html?url=https://services1.arcgis.com/nCKYwcSONQTkPA4K/ArcGIS/rest/services/ServicioSanitariosGalicia/FeatureServer/1&source=sd)

> Crear una aplicación lista para usar a partir de la app configurable
"**Basic Viewer**" desde el editor de mapa.

---

<!-- .slide: class="section" -->
## Valores de configuración
Es frecuente que entre estos valores se incluyan:
* Título de la aplicación
* Logotipo de la empresa
* Webmap utilizado
* etc.

> Aunque la configuración de cada aplicación es diferente<br>
y viene determinada por el autor de la misma.

---

<!-- .slide: class="section" -->

## Para qué se usan las apps configurables
* Estas apps tienen como objetivo:

	1. **Aumentar la independencia** de los usuarios no<br>
		desarrolladores dándoles la posibilidad de crear<br> aplicaciones web que cubran necesidades <br>frecuentes de la organización.

	2. **Mejorar la productividad** del equipo de <br>
	desarrollo permitiéndoles centrarse en crear <br>
	aplicaciones que resuelvan **nuevas** necesidades

	3. Acortar el tiempo de desarrollo proporcionando el <br>
		 código fuente (repo en Github & ZIP) que puede ser <br>
		 extendida y personalizada con modificaciones propias

---

<!-- .slide: class="section" -->
## Apps configurables creadas por Esri
> En ArcGIS Online y Portal for ArcGIS tienen por defecto alojadas más
de [20 apps configurables](https://github.com/Esri?query=template-js). Estas cubren
algunos de los casos de uso más comunes en cualquier organización.

* Contar historias ([storymaps](https://storymaps.arcgis.com))
* Recopilar o editar datos geofráficos
* Comparar mapas o capas
* Explorar o resumir datos
* Mostrar contenido de redes sociales
* Acceder a información cercana
* Calcular rutas u obtener direacciones

---

<!-- .slide: class="section" -->
## Apps configurables personalizadas
> Cualquier organización puede descargar y modificar el código de estas
plantillas o incluir otras nuevas en la organización.

---

<!-- .slide: class="section" -->
## Formas de configurar una app

> Para configurar una **aplicación lista para usar** a partir de una app configurable
necesitamos crear un item en la organización para almacenar los parámetros.

* Esto se puede hacer de tres formas:
	* Desde la interfaz web del [Editor de mapa](http://www.arcgis.com/home/webmap/viewer.html) (visto)

	* Desde la pestaña "**[mi contenido](http://arcgis.com/home/content.html)**"<br>
	<small>(*Sólo con plantillas auto-configurables*)</small>

	* Usando la [API REST](http://resources.arcgis.com/en/help/arcgis-rest-api/index.html#/Add_Item/02r30000008q000000/)

---

<!-- .slide: class="section" -->
## Demo

> Crear una aplicación desde la pestaña **mi contenido** y usando la **API REST**

---

<!-- .slide: class="section" -->
## Webmaps & Apps configurables

> En los datos de una App configurable lista para usar siempre se guarda
el ID del webmap a partir del cual fue generada y se
suele utilizar como base en el código de la plantilla.

> Sin embargo en las auto-configurables depende del autor de la plantilla

---

<!-- .slide: class="section" -->

## Otras referencias

* [Plantillas incluidas en ArcGIS Online y Portal](http://www.arcgis.com/home/search.html?q=tags%3AArcGIS%20web%20application%20template%20owner%3Aesri_en&t=content&sortField=modified&sortOrder=desc)
* [Cómo crear aplicaciones web a partir de webmaps](https://doc.arcgis.com/en/arcgis-online/create-maps/create-map-apps.htm)
* [Crear items usando la API REST](http://resources.arcgis.com/en/help/arcgis-rest-api/index.html#/Add_Item/02r30000008q000000/)
* [Más sobre storymaps](https://storymaps.arcgis.com/)

---

<!-- .slide: class="questions centered" -->

## Preguntas

Para cualquier duda puedes usar los <br>[*issues* del proyecto](https://github.com/esri-es/moocs/issues) en Github

---


<!-- .slide: class="end" -->
