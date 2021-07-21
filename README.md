# postgres

Fix issue extension/postgis.control on OSX

After install postgis.
If you get the problem "ERROR:  could not open extension control file "/usr/local/share/postgresql/extension/postgis.control": No such file or directory" when you run command CREATE EXTENSION postgis;
You can folow commands below to fix that

brew install geos proj gdal libxml2 json-c
brew reinstall postgis --build-from-source

your version gets a specific postgis version!
