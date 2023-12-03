# Example CityJSON

## Source data
- old CityGML 2 from 2017: https://3d.hel.ninja/data/citygml/
- CRS is EPSG:3879

## Processing
- Using https://github.com/citygml4j/citygml-tools
- Remove appearances
-- '"C:\apps\citygml-tools-2.2.0\citygml-tools.bat" remove-apps %1 --log-file=%1_log.txt'
- Convert to CityJSON
-- '"C:\apps\citygml-tools-2.2.0\citygml-tools.bat" to-cityjson %1 --pretty-print --log-file=%1_log.txt'

## Viewing
- Use https://ninja.cityjson.org/

## TODO
- Set CRS
