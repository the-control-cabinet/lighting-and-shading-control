# 01 Lighting strategy

[← Back to README](../README.md)

| Function | Rule (draft) |
|---|---|
| **Occupancy on** | Presence (BLE room + motion) AND lux below threshold, so lights on at scene level |
| **Vacancy off** | No presence for 10 min (rooms) / 2 min (circulation), so fade off |
| **Daylight harvesting** | Dim artificial light as measured lux rises (where dimmable) |
| **Schedules** | Night mode (low level in circulation), holiday mode (presence simulation) |
| **Manual override** | Respected for a timeout (e.g. 2 h), then back to automatic |
| **Energy** | Lighting energy estimated per circuit for the energy dashboard |
