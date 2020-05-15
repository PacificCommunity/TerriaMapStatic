Terria Map Static
==========
![Terria logo](terria-logo.png "Terria logo")

This is a static HTML (serverless) version of [Terria Map](https://github.com/TerriaJS/TerriaMap).

That means you can create your own working version just by forking this repository!

Features missing in this serverless version:

- No CORS proxy, so you can only use services that have CORS enabled, or through an existing CORS proxy.
- No authenticated proxy service.
- No Proj4 conversion service, so some files may not display, such as GeoJSON files using an obscure projection.
- No server-side OGR2OGR service, so the user can't drag Shapefiles or other non-standard format files into the browser. GeoJSON, CSV and KML still work.

## Updating this repository

How this version is made:

1. Check out https://github.com/TerriaJS/TerriaMap
2. `npm install`
3. `gulp release`
4. This repository is the contents of the `wwwroot/build` directory.

Test at: http://staticmap.pacificdata.org
