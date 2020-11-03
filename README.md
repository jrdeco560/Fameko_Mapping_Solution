# Fameko_Mapping_Solution

Fameko_mapping_creation

Ghana Post GPS data + OpenAddresses(OA) data compiled for use in Fameko

Targets
Ghana, addresses added based on OpenAddresses

Usage
Option 1:
Download file from releases to data folder for Fameko and it will auto load.
Option 2:
Download file from releases to phone and open it. Fameko will copy file into its data folder and load it. This will leave a copy of the file in the Downloads folder.

Deactivate the default WA map file to ensure search pulls results from this file.
Restart app after changes otherwise search may not work properly. Restarting is done by opening recent apps and flicking upward on app in Android.

Data
OpenAddresses provides data downloads at (http://results.openaddresses.io/).
OpenStreetMap extracts retrieved from (https://download.geofabrik.de)

Processing
Processing.py
OA data is loaded into Postgresql, filtered with sql, exported to osm xml format and merged with OSM state extracts while converting to osm.pbf. See docs/processing_script_usage and processing.py file.

Fameko 
Move files to Fameko_map folder and run Fameko Map Creator. 
