# Example CityJSON

## Source data
- old CityGML 2 from 2017: https://3d.hel.ninja/data/citygml/
- CRS is EPSG:3879

## Processing
- Using https://github.com/citygml4j/citygml-tools version 2.2.0
- Remove appearances
-- '"C:\apps\citygml-tools-2.2.0\citygml-tools.bat" remove-apps %1 --log-file=%1_log.txt'
- Convert to CityJSON
-- '"C:\apps\citygml-tools-2.2.0\citygml-tools.bat" to-cityjson %1 --pretty-print --log-file=%1_log.txt'

## Example CityJSON files
- CRS is set manually for the alternative file with suffix

## Tested and ok
- https://ninja.cityjson.org/
- (https://github.com/cityjson/Up3date)https://github.com/cityjson/Up3date also works ok in Blender 4.0.1
- FME 2022.2.2 and 2024.0 inspectors on Mac
- Azul 1.1.1 Mac https://github.com/tudelft3d/azul

## Known incompatibilities
- CityJSON Loader-plugin 0.8.1 on QGIS 3.34.2 fails to load these examples.
- Rhino 8.3 Mac / Grasshopper
  
## TODO
- Get new "Official CityJSON" from Helsinki 3DCityDB.
- Set bounds
