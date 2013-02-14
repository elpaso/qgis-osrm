qgis-osrm
=========

QGIS OSRM python plugin


Introduction
------------

This page is about the develoment of a new QGIS Python plugin wich will retrieve data from an OSRM web service and display the result in QGIS.

OSRM stands for Open Source Routing machine (http://www.project-osrm.org), it is an amazing fast routing server for OSM data.

The new plugin will connect to a given, user defined, OSRM server and download routes, turn-by-turn instructions and reverse geoconding informations. Start, middle and end waypoints will be added by the user by clicking on the map canvas. 

 
The project is articulated in steps, the first step will deliver a working plugin with very basic functionalities. The following steps add more options until a full-fledged, configurable and API-expandable plugin will be built.

A fast routing machine as OSRM opens a lot of interesting possibilities, catchment areas calculation is one of those. 

Steps
-----

1. working prototype: this is the first development step, aimed to produce a working plugin that allows the user to download a route with start and end points, display the route in QGIS and save it into a memory layer. No options available.
2. Basic GUI: basic GUI to configure  and save the server URL and the line style, append/overwrite mode switch will also be available. 
3. Full GUI: multiple OSRM server support, servers can be stored in the user preferencese, changed and retrieved, a default server can be set and changed in the options dialog. Full GUI support for all OSRM options (zoom etc.). Support for storage options other than a memory layer (SpatiaLite).
4. Python API: complete support for all OSRM options through a fully documented Python library, this step is the foundation to add more interesting functions to this plugin. Batch geocoding and routing available via API (not in the plugin GUI). The plugin code will be rewritten as needed to use the new API, to also serve as an example about using the API itself.


License
-------


The code will live on GitHub and will be released with GPL GNU General Public Licence

