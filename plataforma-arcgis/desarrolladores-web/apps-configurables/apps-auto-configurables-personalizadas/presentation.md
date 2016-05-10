<!-- .slide: class="title" -->

## Apps auto-configurables personalizadas
Plataforma ArcGIS para desarrolladores web

[desarrolladores.esri.es/moocs](http://desarrolladores.esri.es/moocs)

---

<!-- .slide: class="section" -->
## Aplicaciones *auto-configurable*
<small>```Purpose: Self-configurable```</small>

* **Pros**: los parámetros se pueden definir <br>
dinámicamente y con total flexibilidad. <br>
Ej: podemos configurar la aplicación en base<br>
a los servicios incluidos en un webmap, etc.

* **Cons**: No disponen de un editor por defecto

* **Algunos ejemplos**: [Geoform](http://www.arcgis.com/home/item.html?id=931653256fd24301a84fc77955914a82),
[MapJournal](http://www.arcgis.com/home/item.html?id=da029c7670514be1b5a10b60825cd8da),
[MapTour](http://www.arcgis.com/home/item.html?id=91d75e9b375e4e9b9b3a4004544bfadf),<br>
[Swipe & SpayGlass](http://www.arcgis.com/home/item.html?id=7dca95087c8941ce9feef3776a1354a6),
[Impact Summary](http://www.arcgis.com/home/item.html?id=5b5f03c0b2c04fc4bfca1ce761a01249), etc.

---

<!-- .slide: class="section" -->
## Tipos de plantillas

* Auto-configurada (typeKeywords: ["**selfConfigured**"]):
	* Los parámestros de configuración pueden ser dinámicos
	* La interfaz de configuración se proporciona con el código de la aplicación
	* La estructura almacenada por cada instancia la definimos desde nuestra
	interfaz y por tanto
	almacenada no siempre tiene la misma estructura ya que puede depender de los
	datos del webmaps.

---

<!-- .slide: class="section" -->
## Configuración y visualización
<small>Apps configurables</small>

*
 para usa para visualizar datos prose intancia a partir de un item de la organización que se recibe como párametro por URL.

---

<!-- .slide: class="section" -->

## Metadatos: App configurable vs App configurable RTU
Tanto plantllas como instancias son ```"type": "Web Mapping Application"```
* Plantillas (Metadatos: typeKeywords: "configurable"):
	* Configurable:
		* Data: objeto JSON definiendo los parámetros de configuración
	* selfConfigured:
		* Data: vacío
* Instancia (Metadatos: typeKeywords: "Ready To Use")
	* Configurable & selfConfigured:
		* Data: configuración establecida

---

<!-- .slide: class="section" -->

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

## Recursos y herramientas
Podemos crearlas :
* https://github.com/Esri/application-boilerplate-js
* Web AppBuilder para usuarios no desarrolladores

---

<!-- .slide: class="section" -->

## ¿Qué tecnología debo usar?
La que mejor se adapte a los requisitos de tu app:
* Webmap: API JS + [angular-esri-map]

Si necesitas:
* Análisis: API JS
* Renderizadores avanzados:
* Móvil: leaflet, calcite,
* Basada en formularios: esri-angular
