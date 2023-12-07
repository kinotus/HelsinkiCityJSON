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
- 

## Tested with
- Use https://ninja.cityjson.org/
- [B](https://github.com/cityjson/Up3date)https://github.com/cityjson/Up3date also works ok in Blender 4.0.1
- FME 2022.2.2 and 2024 inspectors
- Known problem; QGIS 3.34 with cityjson-plugin fails to load this example data.

## TODO
- Set bounds
