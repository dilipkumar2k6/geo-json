# Summary
- GeoJSON is a geospatial data interchange format based on JavaScript Object Notation (JSON)
- It defines several types of JSON objects and the manner in which they are combined to represent data about geographic features, their properties, and their spatial extents.
- GeoJSON uses a geographic coordinate reference system, World Geodetic System 1984, and units of decimal degrees.
# Example
```
   {
       "type": "FeatureCollection",
       "features": [{
           "type": "Feature",
           "geometry": {
               "type": "Point",
               "coordinates": [102.0, 0.5]
           },
           "properties": {
               "prop0": "value0"
           }
       }, {
           "type": "Feature",
           "geometry": {
               "type": "LineString",
               "coordinates": [
                   [102.0, 0.0],
                   [103.0, 1.0],
                   [104.0, 0.0],
                   [105.0, 1.0]
               ]
           },
           "properties": {
               "prop0": "value0",
               "prop1": 0.0
           }
       }, {
           "type": "Feature",
           "geometry": {
               "type": "Polygon",
               "coordinates": [
                   [
                       [100.0, 0.0],
                       [101.0, 0.0],
                       [101.0, 1.0],
                       [100.0, 1.0],
                       [100.0, 0.0]
                   ]
               ]
           },
           "properties": {
               "prop0": "value0",
               "prop1": {
                   "this": "that"
               }
           }
       }]
   }               
```
# Geometry Object
- Position
- Point
- MultiPoint
- LineString
- MultiLineString
- Polygon
- MultiPolygon
- GeometryCollection



# Reference 
https://www.youtube.com/watch?v=8RPfrhzRw2s
https://tools.ietf.org/html/rfc7946
https://geojson.io/
