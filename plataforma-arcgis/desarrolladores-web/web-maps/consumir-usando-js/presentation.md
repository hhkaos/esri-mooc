<!-- .slide: class="title" -->

## Consumir web maps/scenes usando JavaScript
Plataforma ArcGIS para desarrolladores web

[desarrolladores.esri.es/moocs](http://desarrolladores.esri.es/moocs)

---

<!-- .slide: class="section" -->

## Cargarlo sin pintarlo

---

<!-- .slide: class="section" -->

## Web Scene

```js
require([
  "esri/views/SceneView",
  "esri/WebScene",
  "dojo/domReady!"
], function(SceneView, WebScene) {

  var scene = new WebScene({
    portalItem: {
      id: "3a9976baef9240ab8645ee25c7e9c096"
    }
  });

  var view = new SceneView({
    map: scene,
    container: "viewDiv"
  });
});
```
Ver en [js.arcgis.com](https://developers.arcgis.com/javascript/latest/sample-code/sandbox/sandbox.html?sample=webscene-basic)

---

<!-- .slide: class="section" -->

### Web map como: BD + BackOffice + API/ORM

<img src="https://docs.google.com/drawings/d/1OKpYpesHKMcRxxsL-ymvlvHsu-kK1M8HdZmosplzs5M/pub?w=900">

---

<!-- .slide: class="section" -->

## Web map como BD

<img src="https://docs.google.com/drawings/d/1b0t92GbRj2Q1xQHeg5_KnWkHkOqsoO9HEG0XLPfHBIo/pub?w=1364&amp;h=653">

---

<!-- .slide: class="section" -->

## Utiliza un webmap cuando...

1. Tengas que crear y mantener una <br>
   aplicación en varios lenguajes

2. Quieras aumentar la velocidad y reducir <br>
   el código de crear una aplicación

3. Te pidan un backoffice para poder <br>
   modificar el modelo geográfico

---

<!-- .slide: class="section" -->

## ¿Y si el modelo geográfico es insuficiente?

* Tienes dos opciones:
  * Ampliarlo con una *BD propia** y extender la API con una clase personalizada
  * Crear una app configurable como veremos más adelante

<small>También existe la posibilidad de almacenar los datos en un item</small>

---

<!-- .slide: class="section" -->

## Ventajas a nivel de desarrollo

* Algunas de las ventajas que proporcionan:
	* No necesitamos crear una base de datos para<br>
	 	almacenar los parámetros

	* Podemos reutilizar los usuarios y grupos de<br>
		nuestra organización para configurar quién tiene <br>
		acceso a cada plantilla.

	* Los usuarios que decidamos podrán crear, mantener<br>
		y publicar de sus aplicaciones web sin tener que<br>
		interrumpir al equipo de desarrollo.

---

<!-- .slide: class="section" -->

## Flujo de trabajo

> Para hacer efectivo esta nueva forma de trabajo lo
único que necesitaremos es que los usuarios encargados
de crear aplicaciones en nuestra organización aprendan:
* A usar la interfaz de configuración
* Y en caso de que los usemos, a crear webmaps.

---

<!-- .slide: class="section" -->


Enfocar Webmap como herramienta de productividad para el desarrollo (reutilización), no pensar tanto en casos en los que una organización controle el webmap que consume tu app (por posibles riesgos de que te borren capas que asumen que siempre estarán ahí, etc), o pensar bien cómo se tendría que hacer esa app (funcionalidad condicionada a que esté ese feature?, crearlo como plantilla configurable?).

---

<!-- .slide: class="section" -->

## Detalles

**Propiedades de alto nivel**

```javascript
{
  "authoringApp": "X",
  "authoringAppVersion": "Y",
  "version": "Z",
  "operationalLayers": [],
  "baseMap": {},
  "spatialReference": {},
  "bookmarks": [],
  "applicationProperties": {},
  "presentation": {},
  "table": {},
  "widget": {}
}
```

> Ver: [web map original](https://www.arcgis.com/sharing/rest/content/items/7d987ba67f4640f0869acb82ba064228/data?f=json) | [comentado](web-map-sample.json)

---

<!-- .slide: class="section" -->

## Referencias
* [Índice de propiedades](https://developers.arcgis.com/web-map-specification/objects/)
* [web-scene-sample.json](web-scene-sample.json)

---

<!-- .slide: class="questions centered" -->

## Preguntas

Para cualquier duda puedes usar los <br>[*issues* del proyecto](https://github.com/esri-es/moocs/issues) en Github

---


<!-- .slide: class="end" -->
