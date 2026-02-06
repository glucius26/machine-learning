# API Query Building Assignment
---

## USGS Earthquake Queries

### Query 1: Earthquakes of atleast 7.0 Magnitude in the last year.
**URL:**
```
https://earthquake.usgs.gov/fdsnws/event/1/query?format=geojson&minmagnitude=7.0&starttime=2025-01-01&endtime=2026-01-01&limit=5
```

**Parameters used:**
- `format`: geojson
- `parameter2`: minmagnitude = 7.0
- `parameter3`: starttime = 2025-01-01
- `parameter4`: endtime = 2026-01-01
- `parameter5`: Limit = 5

**Result:** An overview of 5 earthquakes of magnitude 7.0 or higher over the last year.

---

### Query 2: A list of earthquakes in 2026.
**URL:**
```
https://earthquake.usgs.gov/fdsnws/event/1/query?format=geojson&starttime=2026-01-01&endtime=2026-02-05
```

**Parameters used:**
- `format`: geojson
- `parameter2`: starttime = 2026-01-01
- `parameter3`: endtime = 2026-02-05

**Result:** A very long list on all earthquakes in 2026.

---

### Query 3: A list of 10 earthquakes, 30 degrees latitude minimum, sorted by magnitude
**URL:**
```
https://earthquake.usgs.gov/fdsnws/event/1/query?format=geojson&minlatitude=30.0&limit=10&orderby=magnitude
```

**Parameters used:**
- `format`: geojson
- `parameter2`: minlatitude = 30.0
- `parameter3`: limit = 10
- `parameter4`: orderby = magnitude

**Result:** A list of 10 earthquakes from a minimum of 30 latitude, sorted by magnitude.

---

## Open Library Queries

### Query 4: A list of every warrior cats box set
**URL:**
```
https://openlibrary.org/search.json?author=erin+hunter&title=warriors,box&fields=title,author_name,first_publish_year
```

**Parameters used:**
- `parameter1`: author=erin+hunter
- `parameter2`: title=warriors,box
- `parameter3`: fields=title,author_name,first_publish_year

**Result:** A list of every warriors box collection with author, title, and publish year data.


### Query 5: A list of all james patterson books
**URL:**
```
https://openlibrary.org/search.json?author=james+patterson&fields=title
```

**Parameters used:**
- `parameter1`: author=james+patterson
- `parameter2`: fields=title

**Result:** A list of all the titles of books published by james patterson

### Query 6: A list of Edgar Allan Poe works
**URL:**
```
https://openlibrary.org/search.json?author=edgar+allan+poe&fields=title,first_publish_year&limit=10
```

**Parameters used:**
- `parameter1`: author=allan+poe
- `parameter2`: fields=title,first_publish_year
- `parameter3`: limit=10

**Result:** A list of 10 texts by Edgar Allan Poe