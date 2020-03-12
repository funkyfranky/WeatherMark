# WeatherMark Script for DCS World
Version 1.0
By funkyfranky (2018)

Features:
---------
* Offers easy access to weather data at all points of the map.
* Reports temperature, QFE pressure, wind direction and strength, wind strength classification according to Beaufort scale.
* Output of weather data in metric or imperial units.
* Optionally, the altitude can be specified at which the weather data is evaluated.
* Works with static and dynamic weather.
* Works with all current and future maps (Caucasus, NTTR, Normandy, PG, ...)

## Prerequisite:
* This script requires **DCS 2.5.1 or higher**.
* Note that the script uses only the pure DCS API, i.e. **NO** other framework like MIST, MOOSE, etc required.

## Load the script:
1. Download the script and save it anywhere on your hard drive.
2. Open your mission in the mission editor.
3. At a new trigger:
    * TYPE   "4 MISSION START"
    * ACTION "DO SCRIPT FILE"
    * OPEN --> Browse to the location where you saved the script and click OK.
4. Save the mission and start it.
5. Have fun :)

## Basic Usage:
1. Place a mark on the F10 map.
2. As text enter "weather report".
3. Click somewhere else on the map to submit the new text.
4. The original mark will disappear and a new mark with the weather data at the point the mark was set is created.

## Options:
* Type "weather report, imperial" to get weather report in imperial units independent of default unit system.
* Type "weather report, metric" to get weather report in metric units independent of default unit system.
* Type "weather report, alt 1000" to get weather report at that location but at an ASL altitude of 1000 meters for feet, depending on default unit system.
* Type "weather report, alt 1000, imperial" to get weather at that location at an altitude of 1000 feet independent of default unit system.
* Type "weather report, alt 1000, metric" to get weather at that location at an altitude of 1000 meters independent of default unit system.
* Type "weather set, metric" to set the default unit system to metric units.
* Type "weather set, imperial" to set the default unit system to imperial units.
* Type "weather laste" will create a LASTE report (A-10C, on GND level +0,+2000ft,+6000ft and +12000ft).

## NOTE
* All keywords are **CaSE inSenSITvE**.
* Instead of "weather report" you can also type "weather request" or "weather mark". All three commands are equivalent.
* Commas are the speparators between options ==> They are IMPORTANT!
