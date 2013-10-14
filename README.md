Geolocation Plugin for Annotator
==================
##Geolocation Annotator Plugin

geolocation-annotator.js is a plugin for Annotator to know the current location of the annotation user.

The geolocation plugin uses the [HTML5 Geolocation API](http://www.w3.org/TR/geolocation-API/) and [Google Maps Image API](https://developers.google.com/maps/documentation/imageapis/) to show the maps with the location, in the next version it is going to use Google Maps and [Open Layer](http://openlayers.org/). The code is written in javascript/jquery, but you can translate to coffee using [js2coffee](http://js2coffee.org/), the language used in Annotator.

This plugin will be used in [Open Video Annotation tool](http://www.openvideoannotation.org/). 
A project supported by [Center for Hellenic Studies](http://chs.harvard.edu/), at [Harvard University](http://www.harvard.edu/) and the [Becas Talentia](http://www.juntadeandalucia.es/economiainnovacionyciencia/talentia/) program from the Junta de Andalucia, Spain.

##Live-Demo

There is a demo of the geolocation annotator plugin in the next webpage:

http://danielcebrian.com/geolocation-annotation/demo.html


##Installation

To use the tool you need to install the [Annotator plugin](https://github.com/okfn/annotator/) to annotate text. 

In addition add geolocation-annotator.min.js and geolocation-annotator.min.css CDN distributed file to your head tag, just after
videojs:

```html
	<head>
		<!-- Annotator -->
		<script src="http://ajax.googleapis.com/ajax/libs/jquery/1.7/jquery.min.js"></script>
		<script src="http://assets.annotateit.org/annotator/v1.2.7/annotator-full.min.js"></script>
		<link rel="stylesheet" href="http://assets.annotateit.org/annotator/v1.2.7/annotator.min.css">
	
		<!-- Geolocation Pluging -->
		<script src="src/geolocation-annotator.js"></script>
		<link href="src/geolocation-annotator.css" rel="stylesheet
	
	</head>
```

Furthermore, you will need to create an instance of Annotator with the plugin, as follow:

```js
	<script>
    	$('#airlock').annotator().annotator('addPlugin','Geolocation');
    </script>
```

Change #div_id for the real id where the Annotator is.

¡Caution! In orden to set your current position you will need to accept to use locations for the webpage in the browser.


##To-do

In the next version you can select between Google Maps or Open Layer.
