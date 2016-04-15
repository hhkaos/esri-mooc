<!-- .slide: class="title" -->

## Introducción a las plantillas
Plataforma ArcGIS para desarrolladores web

[desarrolladores.esri.es/moocs](http://desarrolladores.esri.es/moocs)

---

<!-- .slide: class="section" -->

## Qué es una plantilla

> Es el esqueleto de una aplicación (web vacía o con valores por defecto) que se intancia a partir de un item de la organización que se recibe como párametro por URL.

---

<!-- .slide: class="section" -->

## Qué significa que se instancia

> Qué se auto-configura a partir de los valores de configuración contenidos en un item.

---

<!-- .slide: class="section" -->
## Valores de configuración
Es frecuente que entre estos valores se incluyan:
* Título de la aplicación
* Logotipo de la empresa
* Webmap utilizado
* etc.

> Aunque la configuración de cada plantilla es diferente<br>
y viene determinada por el autor de la misma.

---

<!-- .slide: class="section" -->

## Para qué se usan las plantillas
* Las plantillas tiene como objetivo:
	1. **Aumentar la independencia** de los usuarios no<br>
		desarrolladores pudiendo crear ellos mismos<br> aplicaciones web que cubran necesidades <br>frecuentes de la organización.
	2. **Mejorar la productividad** del equipo de <br>
	desarrollo permitiéndoles centrarse en crear <br>
	aplicaciones que resuelvan nuevas necesidades

---

<!-- .slide: class="section" -->
## Plantillas predeterminadas
> En ArcGIS Online y Portal for ArcGIS hay alojadas más<br>
de [20 plantillas](https://github.com/Esri?query=template-js). Estas cubren casos de uso más comunes en cualquier organización

* Contar historias ([storymaps](https://storymaps.arcgis.com))
* Recopilar o editar datos geofráficos
* Comparar mapas o capas
* Explorar o resumir datos
* Mostrar contenido de redes sociales
* Acceder a información cercana
* Calcular rutas u obtener direacciones

---

<!-- .slide: class="section" -->
## Plantillas personalizadas
> Cualquier organización puede modificar estas plantillas o incluir otras nuevas (como veremos en otra lección).

---

<!-- .slide: class="section" -->
## Cómo se crea un item de aplicación

* Para crear un item de aplicación que permita<br>
	instanciar una plantilla podemos usar:
	* Interfaz web del Editor de mapa
	* *Pestaña mi contenido* (* Sólo algunas plantillas)
	* API REST

---

<!-- .slide: class="section" -->
## Contenido de un item de aplicación

Sacar algo de aquí
https://docs.google.com/drawings/d/1iek8Igocexriv770nUcb8eSTLpaR0HZxGah_ZsmtzdU/edit
```
{
	//...

	"type": "Web Mapping Application",
	"url": "https://hhkaos2.maps.arcgis.com/apps/MapJournal/index.html?appid=ddf48b0d9d2543f9bea156af2050d6c6",
	"itemControl": "admin",
	"typeKeywords": ["Configurable", "JavaScript", "Map", "Mapping Site", "Online Map", "Web Map"],
	//...
}
```

---

<!-- .slide: class="section" -->

## Demo

---

<!-- .slide: class="section" -->

## Otras referencias

* [Plantillas registradas en ArcGIS Online por esri_en <- Esri Default](http://www.arcgis.com/home/search.html?t=content&q=tags:ArcGIS%20web%20application%20template)

---

<!-- .slide: class="questions centered" -->

## Preguntas

Para cualquier duda puedes usar los <br>[*issues* del proyecto](https://github.com/esri-es/moocs/issues) en Github

---


<!-- .slide: class="end" -->
