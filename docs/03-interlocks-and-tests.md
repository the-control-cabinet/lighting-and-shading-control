# 03 Interlocks and tests

[← Back to README](../README.md)

| Interlock | Rule |
|---|---|
| Cooling vs open blinds | When the aircon is cooling a room in full sun, close its blinds first |
| Heating vs solar gain | If solar gain has the room > 1 °C above setpoint, don't call for heat; prefer shading |
| Occupant comfort | Never close blinds fully on an occupied room without a glare or overheat reason |

| Test | Pass when |
|---|---|
| Occupancy on/off | Lights follow presence within 30 s / the timeout |
| Daylight | Lights stay off when lux is above threshold |
| Summer gain | Blinds close when sun + cooling + over-temperature |
| Winter gain | Blinds open when sun + heating + under setpoint |
| Override | Manual action holds for its timeout |
