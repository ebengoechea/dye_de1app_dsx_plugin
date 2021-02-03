# "Describe Your Espresso" DE1app DSx plugin

"Describe Your Espresso" (DYE) is a DSx plugin for the Decent DE1 app.

It improves the default shot logging functionallity in the Insight and DSx skins, allowing users to edit, modify and use
shot metadata such as beans, grinder, EY & TDS or espresso description.

By Enrique Bengoechea (with lots of copy/paste/tweak from Damian, John and Johanna's code!)

Decent DE1app: [https://github.com/decentespresso/de1app](https://github.com/decentespresso/de1app)

DSx skin: [https://www.diy.brakel.com.au/dsx/](https://www.diy.brakel.com.au/dsx/)

Plugin [manual available on Decent Diaspora site](https://3.basecamp.com/3671212/buckets/7351439/documents/3344125879) (Decent owners only): 

## Installation

1. Ensure you have DE1 app v1.31 stable (except for fontawesome symbols, which may need to be downloaded manually) 
or higher, and DSx version v4.39 or higher.
2. Copy this file "describe_your_espresso.dsx" to the "de1plus/skins/DSx/DSx_Plugins" folder.
3. Restart the app with DSx as skin.

## Features

1. "Describe your espresso" accesible from DSx home screen with a single click, for both next and last shots.
2. All main description data in a single screen for easier data entry.
    * Irrelevant options ("I weight my beans" / "I use a refractometer") are removed.
3. Facilitate data entry in the UI:
    - Numeric fields can be typed directly.
    - Keyboard return in non-multiline entries take you directly to the next field.
    - Choose categories fields (bean brand, type, grinder, etc) from a list of all previously typed values.
    - Star-rating system for Enjoyment
    - Mass-modify past entered categories values at once.
    
4. Description data from previous shot can now be retrieved and modified:
    - A summary is shown on the History Viewer page, below the profile on both the left and right shots.
    - When that summary is clicked, the describe page is open showing the description for the past shot, 		which can be modified.

5. Create a SQLite database of shot descriptions.
    - Populate on startup
    - User decides what is to be stored in the database.
    - Update whenever there are new shots or shot data changes
    - Update on startup when a shot file has been added, changed or deleted on disk.
    
6. "Filter Shot History" page callable from the history viewer to restrict the shots being shown on both 
    left and right listboxes.

7. Upload shot files to Miha's Visualizer repository with a button press.

8. Configuration page allows defining settings and launch database maintenance actions from within the app. 

9. TBD Add new description data: other equipment, beans details (country, variety), detailed coffee ratings like
		in cupping scoring sheets, etc.
T
his code is released under GPLv3 license. See LICENSE file under the DE1 source folder in github.
