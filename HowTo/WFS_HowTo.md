Web Feature Service tutorial
=====

This is short tutorial for those who want to use the Web Feature Service interface of the 3D City Database.

1. Requirements and setup
----------

How To?
* See database tutorial for database setup
* Install a Java Servlet Container, e.g. Tomcat
* Download the WFS from [here](http://www.3dcitydb.net/3dcitydb/dwfs/)
* Copy the JDBC drivers to the lib folder of your Tomcat
* Copy the war file to the webapps folder of your Tomcat
* Further details can be found in the [3DCityDB manual](http://www.3dcitydb.net/3dcitydb/documentation/)

I just want to start!
* We provide a WFS under: http://berlin3d-wfs.virtualcitymap.de/wfs
* GetCapabilities <pre>http://berlin3d-wfs.virtualcitymap.de/wfs?request=GetCapabilities&service=WFS</pre>
* GetFeature example --> use the WFS GUI: http://berlin3d-wfs.virtualcitymap.de/wfsclient
<pre>
&lt;?xml version="1.0" encoding="UTF-8"?&gt;
&lt;wfs:GetFeature service="WFS" version="2.0.0" xmlns:wfs="http://www.opengis.net/wfs/2.0"&gt;
  &lt;wfs:StoredQuery id="http://www.opengis.net/def/query/OGC-WFS/0/GetFeatureById"&gt;
    &lt;wfs:Parameter name="id"&gt;BLDG_0003000e007d8955&lt;/wfs:Parameter&gt;
  &lt;/wfs:StoredQuery&gt;
&lt;/wfs:GetFeature&gt;
</pre>


2. What can you do with the WFS
----------

* Display the information in the viewer
* Render the geometry, e.g. by converting it to OBJ (note: this WFS is not designed for rendering)


3. What else can we do during the weekly meetings
----------

* Explain the CityGML XSD schema
* Show ways how to parse CityGML