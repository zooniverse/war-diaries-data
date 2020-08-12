# Data

## /diaries

## /groups

JSON exports of the [Group models](https://github.com/zooniverse/wd3/blob/master/app/models/group.rb), one per diary, named by the group ID eg. `GWD0000001.json`. These can be used to look up diary metadata for a given group/diary.

## /results

Aggregated results for each diary, named by diary group ID eg. `GWD0000001.json`. Each file is an array of [Result models](https://github.com/zooniverse/wd3/blob/master/app/models/result.rb), where a Result represents the consensus for a single tag on a page of the diary (diaryDate, place, activity, person etc.)

## places.csv

A gazetteer built from the data added by volunteers using the Place tag and the geonames.org geolocation service.
Columns are:

- `Label`: Free text labels entered by volunteers for this place.
- `Name`: Place name.
- `Identifier`: Text string used to match volunteer entries for aggregation/consensus.
- `GeoID`: geonames ID identified by volunteers as the linked place.
- `Lat`: Latitude
- `Long`: Longitude.