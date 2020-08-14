


````python

import pandas as pd
import geopandas

df=geopandas.read_file('mexican_states.geojson')
d1=df.iat[6,-1]

m=folium.Map(location=[26, -99.156], zoom_start=4.5)
folium.GeoJson(d1,name='geojson').add_to(m)
m

```
