<!-- .slide: class="title" -->

## Introducción a los webmaps
[Plataforma ArcGIS para desarrolladores web](https://esri-es.github.io/moocs/plataforma-arcgis/desarrolladores-web/)

[![octocat](../../template/octocat.png)](http://esri-es.github.io/)

---

<!-- .slide: class="section" -->
## Qué es un webmap
> Es el término usado en la plataforma ArcGIS para denominar la represetanción
  de un mapa en formato **JSON**

---

<!-- .slide: class="section" -->

## Información contenida
* **Metadatos**: título, descripción, autor, fecha de <br>
creación y modificación, etiquetas, valoraciones, etc.

* **Información de referencia**: mapa base, referencia <br>
espacial, extensión inicial, etc.

* **Capas operacionales**: URLs de los servicios, orden <br>
de las capas,simbología/renderizadores, configuración de<br>
popups, opacidad, etc.

* **Otros**: marcadores, etc.

---

<!-- .slide: class="section" -->

## [Webmap de ejemplo](http://www.arcgis.com/sharing/rest/content/items/1a40fa5cc1ab4569b79f45444d728067?f=json)

```javascript
{
	"id": "1a40fa5cc1ab4569b79f45444d728067",
	"owner": "acarroll73",
	"orgId": "nzS0F0zdNLvs7nc8",
	"created": 1317674957000,
	"modified": 1346084228000,
	"guid": null,
	"name": "ecological_footprints_1316885358916",
	"title": "Ecological Footprints of Nations",
	"type": "Web Map",
	"typeKeywords": ["Web Map", "Explorer Web Map", "Map", "Online Map", "ArcGIS Online"],
	"description": "Código HTML de con la descripción",
	"tags": ["Global Footprint", "ecological footprint", "sustainability", "nations", "carbon footprint"],
	"snippet": "The ecological footprints of the world's nations as calculated by the Global Footprint Network",
	"thumbnail": "thumbnail/ecological_footprint.jpg",
	"documentation": null,
	"extent": [
		[-142.5586, -52.0525],
		[94.9219, 73.8737]
	],
	"spatialReference": null,
	"accessInformation": "Global Footprint Network",
	"licenseInfo": null,
	"culture": "en-us",
	"properties": null,
	"url": null,
	"access": "public",
	"size": 75992,
	"appCategories": [],
	"industries": [],
	"languages": [],
	"largeThumbnail": null,
	"banner": null,
	"screenshots": [],
	"listed": false,
	"commentsEnabled": false,
	"numComments": 0,
	"numRatings": 6,
	"avgRating": 3.5,
	"numViews": 170294
}
```

---

<!-- .slide: class="section" -->

## Por qué son importantes

1. Lenguaje común de la plataforma

2. Son fáciles y rápidos de crear/editar por<br>
todo tipo de usuarios

3. Se pueden compartir entre usuarios con <br>diferentes roles

4. Incremento de la productividad:
  * Ahorran líneas de código
  * Sencillo de mantener/actualizar
  * Reutilizable entre aplicaciones, SDKs, etc

---

<!-- .slide: class="section" -->

## Creación y consumo

* Creación/edición:
  * [ArcGIS Online](https://doc.arcgis.com/en/arcgis-online/create-maps/make-your-first-map.htm), [Portal for ArcGIS](http://server.arcgis.com/en/portal/latest/use/make-your-first-map.htm), [ArcGIS Pro](http://pro.arcgis.com/en/pro-app/help/mapping/map-authoring/author-a-web-map.htm) y [API REST](http://resources.arcgis.com/en/help/arcgis-rest-api/index.html#/Add_Item/02r30000008q000000/)
  * APIs, SDKs y AppBuilders (*Próximamente*)

* Consumo:
  * Apps: [ArcGIS Online](https://doc.arcgis.com/en/arcgis-online/create-maps/make-your-first-map.htm), [Portal for ArcGIS](http://server.arcgis.com/en/portal/latest/use/make-your-first-map.htm), [ArcGIS Pro](http://pro.arcgis.com/en/pro-app/help/mapping/map-authoring/author-a-web-map.htm), <br>[Operations Dashboard](http://doc.arcgis.com/en/operations-dashboard/windows-desktop/author/faqs-author.htm#anchor17), [Collector](https://doc.arcgis.com/en/collector/android/create-maps/create-and-share-a-collector-map.htm), ...
  * APIs y SDKs: [JavaScript](https://developers.arcgis.com/javascript/jshelp/intro_agstemplate_amd.html), [iOS](https://developers.arcgis.com/ios/swift/guide/viewing-web-map.htm), [Java](https://developers.arcgis.com/java/guide/build-a-web-mapping-app.htm), [Xamarin](https://developers.arcgis.com/xamarin/quartz/forms/guide/open-an-existing-map.htm), [.NET](https://developers.arcgis.com/net/desktop/guide/access-maps-and-content-from-your-portal.htm), ...
  * Plantillas: [aplicaciones configurables](https://www.arcgis.com/home/gallery.html#c=esri&t=apps&o=modified&f=configurable), [storymaps](https://storymaps.arcgis.com/en/), etc.
  * App Builders: [Web AppBuilder](http://doc.arcgis.com/en/web-appbuilder/create-apps/make-first-app.htm) y [AppStudio](https://appstudio.arcgis.com/#do_more)

---

<!-- .slide: class="section" -->

## Consideraciones

* El fichero puede ocupar desde unos pocos <br>
bytes hasta pocos KB

* Los cambios en un webmap se propagan entre <br>
todas las aplicaciones que los consuman

---

<!-- .slide: class="questions centered" -->

## Preguntas

Para cualquier duda puedes usar los <br>[*issues* del proyecto](https://github.com/esri-es/moocs/issues) en Github

---


<!-- .slide: class="end" -->
