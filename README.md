# "Describe Your Espresso" DE1app DSx plugin

<span style="color:red">**WARNING: DON'T USE WITH CURRENT DE1 APP VERSIONS (OLDER THAN 1.37) This was a DSx-only plugin and has been superseded by the [skin-independent extension](https://github.com/ebengoechea/de1app_plugin_DYE) that is distributed automatically with the base app.**</span>

"Describe Your Espresso" (DYE) is a [DSx](https://www.diy.brakel.com.au/dsx/](https://www.diy.brakel.com.au/dsx/) plugin for the [Decent DE1 app](https://github.com/decentespresso/de1app](https://github.com/decentespresso/de1app).

It improves the default shot logging functionality in the Insight and DSx skins, allowing users to edit, modify and use shot metadata such as beans, grinder, EY & TDS or espresso description.

By Enrique Bengoechea (with lots of copy/paste/tweak from Damian, John and Johanna's code!)

Plugin [manual available on Decent Diaspora site](https://3.basecamp.com/3671212/buckets/7351439/documents/3344125879) (Decent owners only): 

Code released under GPLv3 license. See LICENSE file.

## Installation

1. Ensure you have DE1 app v1.34 stable or higher, and DSx version v4.39 or higher.
2. Copy this file "describe_your_espresso.dsx" to the "de1plus/skins/DSx/DSx_Plugins" folder.
3. Restart the app with DSx as skin.
4. After initial install, updates can be done from within the app, on the "Describe Your Espresso Settings" page.

## Features

1. "Describe your espresso" accesible from DSx home screen with a single click, for both next and last shots.

2. All main description data in a single screen for easier data entry.
    - Irrelevant options ("I weight my beans" / "I use a refractometer") are removed.
    
3. Facilitate data entry in the UI:
    - Numeric fields can be typed directly, using clicker arrows, or double tapping on them to launch a full-page numeric-pad.
    - Keyboard return in non-multiline entries take you directly to the next field.
    - Choose categories fields (bean brand, type, grinder, etc) from a list of all previously typed values.
    - Star-rating system for Enjoyment
    - Mass-modify past entered categories values at once.
    
4. Description data from previous shots can now be retrieved and modified:
    - A summary is shown on the History Viewer page, below the profile on both the left and right shots.
    - When that summary is clicked, the describe page is open showing the description for the past shot, which can be modified

5. Create a SQLite database of shot descriptions.
    - Populate on startup
    - User decides to store only shot descriptions or shot description+shot series.
    - Update whenever there are new shots or shot data changes
    - Update (synchronize) on startup when a shot file has been added, changed or deleted on disk, or trigger synch from the settings page.
    
6. "Filter Shot History" page callable from the history viewer to restrict the shots being shown on both 
left and right listboxes.

7. Upload shot files to Miha's Visualizer repository, either automatically when finished, or on demand with a button press. 

8. Configuration page allows defining settings and launch database maintenance actions from within the app. 

9. TBD Add new description data: other equipment, beans details (country, variety), detailed coffee ratings like
		in cupping scoring sheets, etc.
