# geotext

Geotext extracts country and city mentions from text. This repos is a forked of https://github.com/elyase/geotext, which seems to be abandoned.

## Usage

```
from geotext import GeoText

# list cities
places = GeoText("London is a great city")
places.cities
# "London"

# list countries


# filter by country code
result = GeoText('I loved Rio de Janeiro and Havana', 'BR').cities
# 'Rio de Janeiro'


# identify mentions countries from the cities in the text
GeoText('New York, Texas, and also China').country_mentions
# OrderedDict([(u'US', 2), (u'CN', 1)])
```