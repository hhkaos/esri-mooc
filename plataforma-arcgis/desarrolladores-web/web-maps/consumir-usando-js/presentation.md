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

## Referencias
* [Índice de propiedades](https://developers.arcgis.com/web-map-specification/objects/)
* [web-scene-sample.json](web-scene-sample.json)

---

<!-- .slide: class="questions centered" -->

## Preguntas

Para cualquier duda puedes usar los <br>[*issues* del proyecto](https://github.com/esri-es/moocs/issues) en Github

---


<!-- .slide: class="end" -->
