#Wedding invitation map brought online
This project takes a physical illustrated map and turns it into an interactive online map, embedded in the wedding website.

![BeforeAfter](https://raw.github.com/nixta/ahc/master/BeforeAfter.png)

See the map live [here](http://nixta.github.io/ahc/).

The map makes use of ArcGIS.com WebMaps, the ArcGIS Javascript API, and an original illustration by [Emma Trithart](http://www.emmatrithart.com).

##The Process

The original PSD was brough into Illustrator and the base outline turned into vector graphics. That vector outline was exported to DWG format, brought into ArcGIS Desktop and exported to a Shapefile.

ArcGIS Desktop editing tools were used to move and resize the outline appropriately to overlay the wedding location.

Roads were drawn by hand in a dedicted polyline shapefile. They were redrawn to more precisely overlay the actual road network (important now that they were in context of an actual map) and styled to match the original illustration.

Additional point shapefiles were used to mark interesting locations from the original map (Hotel, Tree, Polo club and of course the Rings).

These shapefiles were then published to ArcGIS Online from ArcGIS Desktop and combined in a WebMap. Symbology was all derived from the original Photoshop document.

The WebMap was generated to have multiple symbology styles at varying scale levels.

Lastly, a custom web page was put together to consume and display the WebMap and to properly offset the label graphics.

###References
The following tools were used to generate this map:
* [ArcGIS Online](http://www.arcgis.com)
* [Esri JavaScript API](https://developers.arcgis.com/en/javascript/)
* Adobe Illustrator
* Adobe Photoshop
* [ArcGIS for Desktop](http://www.esri.com/software/arcgis/arcgis-for-desktop)

These blog posts came in handy when processing the original Photoshop version of the map:
* http://blogs.esri.com/esri/arcgis/2008/06/18/migrating-illustrator-file-ai-archives-to-arcgis/
* http://ngmdb.usgs.gov/Info/dmt/docs/DMT08_Wunderlich.pdf
