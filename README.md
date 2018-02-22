# Daylight Calendar ICS

This is a dynamically generated .ics calendar that you can host and subscribe to in Google Calendar, iCal, or other calendar software.

## Options

- [Find your geo coordinates](http://mygeoposition.com/)
- [Find your GMT offset](http://en.wikipedia.org/wiki/List_of_UTC_time_offsets#mediaviewer/File:World_Time_Zones_Map.png)
- Determine which zenith setting you prefer
  - Default: `90.83`
  - Civil Twilight: `96`
    - _Conventionally used to signify twilight_
  - Nautical Twilight: `102`
    - _The point at which the horizon stops being visible at sea_
  - Astronomical Twilight: `108`
    - _The point when Sun stops being a source of any illumination_
- You can also change the year
    
## Instructions

- Upload `daylight.php` to your server (or skip this step and use the one hosted on [gearside.com](https://gearside.com/calendars/daylight.php))
- Point your calendar to the file and use query parameters for the options above.
  - Latitude: `lat`
  - Longitude: `lng`
  - GMT: `gmt`
  - Zenith: `z`
  - Year: `year`

## Examples

#### Basic
`https://gearside.com/calendars/daylight.php?lat=43.1234&lng=-76.1234&gmt=-5`

#### Advanced
`https://gearside.com/calendars/daylight.php?lat=43.1234&lng=-76.1234&gmt=-5&z=108`

## Notes

Calendar software caches remote .ics files (like this one), so when replacing it you can "bust" the cache by adding another query parameter of random characters such as `&sdfgsfd`.

- [More information available at Gearside.com](https://gearside.com/google-daylight-calendar/)