Database tutorial
=====

This is short tutorial for those who want to work with the 3D City Database.

1. Requirements and setup
----------

Do everything by yourself?
* Download and install PostgreSQL version 9.1 or higher
* Download and install PostGIS extension for PostrgeSQL of version 2.0 or higher
* Download and install 3D City Database Importer/Exporter from [here](http://www.3dcitydb.net/3dcitydb/downloads/)
* Create an 3D City Database instance by using the SQL scripts. Read the [manual](http://www.3dcitydb.net/3dcitydb/documentation/)
* Start the Importer/Exporter (needs Java RE), connect to your database, import CityGML files
* Import takes a long time

Do mostly everything by yourself?
* Download and install PostgreSQL version 9.1 or higher
* Download and install PostGIS extension for PostrgeSQL of version 2.0 or higher
* Download and install 3D City Database Importer/Exporter from [here](http://www.3dcitydb.net/3dcitydb/downloads/)
* Unzip and restore the database dump (see chapter 4)
* On command line restoring works with: <pre>psql -h localhost -p 5432 -U [your_username] -d [your_database_name] -f [location_of_dump].sql</pre>
* Restoring takes a long time

Do some parts yourself?
* Download and install docker. Using [Windows](https://docs.docker.com/installation/windows/)?
* Get [this](https://github.com/vpicavet/docker-pggis) docker image which provides an installed PostgreSQL server with all spatial extensions
* Follow the instructions of the README.
* Unzip the database dump and put it into a folder */data/restore* to restore the dump automatically when starting the docker image (like described in the README)
* Restoring takes a long time

I just want to start!
* We could provide a Linux VM with a running systems (PostgreSQL, 3DCityDB, Importer/Exporter) but the VM would be huge.
* Contact us if you want to work with an VM.


2. What can you do with the database
----------

* CityGML import and export
* KML/COLLADA export
* Setup your own WFS
* Do spatial analysis with PostGIS


3. What else can we do during the weekly meetings
----------

* Explain the database schema to you
* Explain the different APIs of stored procedures


4. SQL Dump
----------

You can download the SQL dump of the Berlin LoD2 model from our FTP server. 
You can use an FTP client software like [FileZilla](https://filezilla-project.org/) or enter the address in your browser
Please contact Felix to get the server address!


5. Contact
----------

fkunde[at]virtualcitysystems.de
or
use the issues section of this GitHub repo, so that questions and answers are visible to everybody