[View the Map](https://deefinder200.github.io/poecile-map/map.html)

# Overview
* A simple visualization of the contact zone between Black-capped Chickadees and Carolina Chickadees. Designed to be just an html and css file.
* Can plot locations of last 30 iNaturalist observations of Poecile (Chickadees) that Need ID that an account has not reviewed.
* Can add Observations to the map. This will update the URL which you could use to share with others. More details about the URL below.
* Includes a measurement tool to help in determining distance between observation and contact zone. Carolina Chickadees are moving north at a rate of 1km/year [1] and this contact zone is from 2020 [2].

[1] Found in McQuillan et al. 2015. "Second, the hybrid zone is moving rapidly northward at a rate of approximately 10 km/decade, with P. carolinensis moving into territory historically occupied by P. atricapillus and displacing them (Bronson et al. 2003a; Reudink et al. 2007; Taylor et al. 2014a)."

[2] https://www.sibleyguides.com/bird-info/black-capped-chickadee/black-capped-carolina-chickadee/

# Observation Colors
* orange: Observation with picture
* blue: Observation with audio
* green: Observation with both picture and audio
* pink: Specific observation added to map

# URL
Uses URL to control initial load of map i.e. `map.html#loadcurrent=false&observationid=344329184`. Variables can be added together with a `&` between key-value pairs.

**Variables**
* **loadcurrent**: By default, the map will load the current observations that Need ID. If you pass `loadcurrent=false` then the map will not load the current observations (unless `viewerid` is used).
* **viewerid**: Load current observations that Need ID for iNaturalist username.
* **observationid**: A comma-separated string of observation IDs to add to the map. These will be shown in pink. For example, `observationid=344329184` or `observationid=344447956`
* **loadchickadeecontactzone**: By default, the map will load the contact zone between Black-Capped and Carolina chickadees. If you pass `loadchickadeecontactzone=false` then the zone will not be displayed.

# TODOs
* Update popups with more features - picture, sound, etc.
* UX improvements - load more observations, hide reviewed observations, etc.
* Update contact zone for 2025 by adding 5km to northern most points - ideally add a slider to control contact zone for a given year