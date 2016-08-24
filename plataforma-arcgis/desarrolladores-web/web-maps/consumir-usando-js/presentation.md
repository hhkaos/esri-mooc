<!-- .slide: class="title" -->

## Consumir web maps/scenes <br>usando JavaScript
Plataforma ArcGIS para desarrolladores web

[desarrolladores.esri.es/moocs](http://desarrolladores.esri.es/moocs)

---

<!-- .slide: class="section" -->

## Cargarlo sin pintarlo

```js
webmap.load()
  .then(function() {
    var layer = webmap.allLayers.find(function(layer) {
     return layer.id === "orp_sensor_4775";
    });
    return layer.load();
  })
  .then(function(featureLayer) {
    var query = new Query();
    query.where = 'OBJECTID = 1';
    return featureLayer.queryFeatures(query);
  })
  .then(function(result) {
    console.log(result.features);
  })
  .otherwise(function(error) {
    console.error(error);
  });
```
Ver ejemplo: [asyncronous-web-map-load.html](asyncronous-web-map-load.html)

---

<!-- .slide: class="section" -->

## Clase: WebMap

```js
require([
  "esri/views/MapView",
  "esri/WebMap",
  "dojo/domReady!"
], function(SceneView, WebScene) {

  var webmap = new WebMap({
    portalItem: {
      id: "e691172598f04ea8881cd2a4adaa45ba"
    }
  });

  var view = new MapView({
    map: webmap,
    container: "viewDiv"
  });
});
```
Ver en [js.arcgis.com](https://developers.arcgis.com/javascript/latest/sample-code/sandbox/sandbox.html?sample=webmap-basic)

---

<!-- .slide: class="section" -->

## Clase: WebScene

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

> Quieras `aumentar la velocidad y reducir las líneas de código` de crear una aplicación

---

<!-- .slide: class="section" -->

### 81 mapas en 60 líneas JS

<iframe src="gallery.html" style="width:100%;height:550px"></iframe>

> Ver código fuente: [gallery.html](https://github.com/esri-es/moocs/blob/gh-pages/plataforma-arcgis/desarrolladores-web/web-maps/introduccion/gallery.html)

---

<!-- .slide: class="section" -->

## Utiliza un webmap cuando...

> `Te pidan un backoffice` para poder modificar el modelo geográfico

---

<!-- .slide: class="section" -->

### 81 mapas + backoffice en 60+2 líneas JS

<iframe src="gallery-edit.html" style="width:100%;height:550px"></iframe>

> Ver código fuente: [gallery-edit.html](https://github.com/esri-es/moocs/blob/gh-pages/plataforma-arcgis/desarrolladores-web/web-maps/introduccion/gallery-edit.html)

---

<!-- .slide: class="section" -->

### Utiliza un webmap cuando tengas que...

> * `Mantener coherencia` entre varias aplicaciones
* Crear una misma app para `varias plataformas`

---

<!-- .slide: class="section" -->

### Web app + App Nativa

<iframe src="http://www.nerjamap.com/" style="width:100%; height:550px"></iframe>

App Nativa: [QR](images/nerja-guide-qr.png) | [AppStudio Standard](arcgis-appstudio://hhkaos2@www.arcgis.com?id=9f731456db7746759a62b5ceebe9e340) - Editar [web map](https://hhkaos2.maps.arcgis.com/home/webmap/viewer.html?webmap=230d2efb94a148c49507f4730c221bbe) | [app](http://hhkaos2.maps.arcgis.com/apps/MapTour/index.html?appid=b73182a581604ccfacaf00792a2562d3&edit)

---

<!-- .slide: class="section" -->

### ¿Y si el modelo geográfico es insuficiente?

* Tienes dos opciones:
  * Ampliarlo con una *BD propia** y extender <br>
    la API con una [clase personalizada](https://developers.arcgis.com/javascript/3/jshelp/intro_javascript_classes.html)

  * Crear una app configurable como veremos <br>
    más adelante

<small>**Nota**: También puedes almacenar los datos en un item</small>

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
