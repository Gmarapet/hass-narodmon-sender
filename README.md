# 🌦️ Narodmon Integration for Home Assistant
Send weather sensor and camera data from your Home Assistant to [Narodmon.ru](https://narodmon.ru) — the community weather monitoring network.

This custom integration lets you:
- Select compatible sensors (temperature, humidity, etc.);
- Aggregate data (average/min/max);
- Skip unavailable sensors automatically;
- Get Home Assistant notifications about broken sensors;
- Send data at custom intervals;
- Use or override Home Assistant coordinates;
- Authorize using MAC address only.

## Installation
### HACS (recommended)
1. Open **HACS → Integrations → Custom repositories**
2. Add `https://github.com/Gmarapet/hass-narodmon-sender` with category `Integration`
3. Find **Narodmon** and install it
4. Restart Home Assistant

### Manual
1. Download latest ZIP from [Releases](https://github.com/Gmarapet/hass-narodmon-sender/releases)
2. Extract folder `narodmon` into `/config/custom_components/narodmon`
3. Restart Home Assistant

## Configuration
1. Go to **Settings → Devices & Services → Add Integration → Narodmon**
2. Enter:
   - MAC address (auto-detected, editable)
   - Latitude / Longitude (from HA by default)
   - Update interval in seconds
3. Add sensor groups and choose aggregation type.

## Example data
```
ID=AA:BB:CC:DD:EE:FF
LAT=55.7522
LON=37.6156
temperature=22.1
humidity=43.7
pressure=1009.2
```

## Developer Info
Repo: [https://github.com/Gmarapet/hass-narodmon-sender](https://github.com/Gmarapet/hass-narodmon-sender)
Author: @Gmarapet
License: MIT
