Branched Oak Sailing

A single-page web app for sailing Buen Camino on Branched Oak Lake: depth contours from Nebraska Game and Parks, live wind from Open-Meteo with animated wind arrows on the map, GPS position and track recording, marks with notes and stories, and checklists for slip life.

Everything is in index.html. There is no build step and nothing to install.

Putting it on GitHub Pages

1. Create a free account at github.com if you do not have one.
2. Click the plus sign in the top right, then New repository. Name it branched-oak (any name works). Leave it Public. Click Create repository.
3. On the new repository page, click "uploading an existing file". Drag index.html and this README.md into the box. Click Commit changes.
4. Click Settings (top of the repository), then Pages in the left sidebar. Under Build and deployment, set Source to "Deploy from a branch", Branch to "main" and folder to "/ (root)". Click Save.
5. Wait a minute or two, then reload the Pages settings page. It shows the address, which will look like https://YOURNAME.github.io/branched-oak/

Open that address on your phone. In Safari, tap Share, then Add to Home Screen, so it opens full screen like an app.

Updating

Open index.html in the repository on github.com, click the pencil icon, paste the new contents, and commit. The site updates within a minute or two.

How the depth data works

The page asks the Game and Parks Lake Contours service for Branched Oak Lake each time it opens and caches the result on the phone. Depths are relative to the survey pool (the 3 ft contour is at 1281.0 ft elevation, so the survey surface is about 1284 ft). Buen Camino draws 2.5 ft; the 3 ft line is drawn in red and the 6 ft line in orange.

Data sources

Contours: Nebraska Game and Parks Commission, Lake Contours (https://www.nebraskamap.gov/maps/outdoornebraska::lake-contours)
Weather: Open-Meteo (https://open-meteo.com)
Basemap: Esri World Imagery and OpenStreetMap
Map library: Leaflet
