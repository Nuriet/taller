# Ejemplos de textos.

 ## 1. Argentina Manuscrita.

Texto: [Argentina Manuscrita. Rui Díaz de Gúzman](http://www.cervantesvirtual.com/obra-visor/historia-argentina-del-descubrimiento-poblacion-y-conquista-de-las-provincias-del-rio-de-la-plata--0/html/ff57d7e8-82b1-11df-acc7-002185ce6064_12.html "Argentina Manuscrita. Rui Díaz de Gúzman")

## 2. Texto de Servicio CTS (Canonical Text Service) 
[Pausanias, Description of Greece](https://scaife.perseus.org/reader/urn:cts:greekLit:tlg0525.tlg001.perseus-eng2:1.1.1-1.1.5/ "Pausanias, Description of Greece")


@@ -47,7 +47,7 @@ When the application is loaded, a table prompt window is displayed asking for th

<img src="./../imgs/welcome.png" alt="prompt image" height="300" />

## 4 Application layout
## 4 Application Layout

<img src="./../imgs/layout.png" alt="app layout image" height="400" />

@@ -151,7 +151,7 @@ The setting section is used to set additional options and rules:

<img src="./../imgs/columns.png" alt="columns image" height="150" />

## 7 Map control
## 7 Map Control

The map control menu is located in the bottom-left part of the map and has two subsections:

@@ -160,12 +160,20 @@ The map control menu is located in the bottom-left part of the map and has two s

<img src="./../imgs/mapcontrol.png" alt="mapcontrol image" height="400" />

## 8 config files
## 8 Deployment
HGA is a client-side application that does not require its own server to run. To deploy your own copy of HGA:
 - clone the repository
 - create a ‘config_api.json’ file in ‘app/configs’ with your Google API key and client ID (see below)
 - install npm and node
 - install npm dependencies `npm install`
 - build the application `npm run build`
 - deploy the `dist` folder to your server

When deploying your own version of HGA, you can use the included config files (json formatted) to customise the content and rules of the application. There are 4 config files:

- **Config.json** - various areas of customisation such as colors, default options etc.;
- **Config_api.json** - Google API ID and key (note that this file has to be created; it is not in the repository!);
  `{ "apiKey": YOUR GOOGLE API KEY, "clientId": YOUR CLIENT ID }`
- **Basemaps.json** - a list of base layers (WMS or tile services);
- **Mapoverlays.json** - other auxiliary layers in GeoJSON or WMS format (modern countries, etc.).
- **config.json** - various areas of customisation such as colors, default options etc.;
- **config_api.json** - Google API ID and key (note that this file has to be created; it is not in the repository!);
 `{ "apiKey": YOUR GOOGLE API KEY, "clientId": YOUR CLIENT ID }`
- **basemaps.json** - a list of base layers (WMS or tile services);
- **papoverlays.json** - other auxiliary layers in GeoJSON or WMS format (modern countries, etc.).
