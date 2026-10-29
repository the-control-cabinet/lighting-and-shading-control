# Lighting and Solar-Shading Control: BMS Strategies on Home Hardware (Design Stage)

**Lighting control and façade/solar-shading control written as BMS strategies and implemented on existing home equipment: occupancy- and daylight-driven lighting, time schedules and scenes on the lighting systems, and motorised blinds that manage solar gain in coordination with heating and cooling, so the blinds help the HVAC rather than fighting it.**

[![YouTube](https://img.shields.io/badge/YouTube-The%20Control%20Cabinet-red?logo=youtube)](https://www.youtube.com/channel/UC5Cupmz7vlfcodpCX7k8iuQ)
[![Portfolio](https://img.shields.io/badge/Portfolio-the--control--cabinet-24292f?logo=github)](https://github.com/the-control-cabinet/the-control-cabinet)
![Domain](https://img.shields.io/badge/BMS-lighting%20%26%20shading-blue)
![Status](https://img.shields.io/badge/Status-Design%20stage-yellow)

> **The short version:**
> - **Lighting:** occupancy (BLE presence + motion), daylight (lux sensors), time schedules and scenes; vacancy timeouts and minimum light levels.
> - **Shading:** motorised blinds driven by sun position, solar gain, room temperature and the HVAC mode. Close against **summer** gain when cooling or overheating; open for **winter** gain when heating; never fight the occupant (manual override with a timeout).
> - **Coordination:** a heating/cooling/shading interlock: no cooling with blinds open to full sun; no heating while solar gain is overheating the room.
> - **Kit already in place:** smart lighting on several local APIs, motorised blinds (local hub API), BLE presence, lux sensors.

**Portfolio position:** Automation level · lighting and façade control. Inputs from: [BLE presence](https://github.com/the-control-cabinet/esp32-ble-presence-network) · [Evohome zones](https://github.com/the-control-cabinet/evohome-heating-controls-ramses-integration) · [aircon](https://github.com/the-control-cabinet/localtuya-portable-aircon-dp-map). Rules shared with: [FDD](https://github.com/the-control-cabinet/fdd-rules-heating-plant) · [sequence of operation](https://github.com/the-control-cabinet/heating-sequence-of-operation)

---

## Documents

| Doc | Contents |
|---|---|
| [01 Lighting strategy](docs/01-lighting-strategy.md) | Occupancy, daylight, schedules, scenes |
| [02 Solar-shading strategy](docs/02-shading-strategy.md) | Sun position, gain, HVAC coordination |
| [03 Interlocks and tests](docs/03-interlocks-and-tests.md) | HVAC coordination and functional tests |

## Roadmap
- [ ] Window/façade orientation register
- [ ] Lighting occupancy + daylight on 2 rooms
- [ ] Shading rules on one sun-facing room (shadow mode first)
- [ ] HVAC coordination interlocks
- [ ] Energy and comfort comparison

## Skills demonstrated (as built)
| Skill | Evidence |
|---|---|
| Lighting control | Occupancy, daylight harvesting, schedules, overrides |
| Façade/shading control | Sun-position and gain-based blind control |
| HVAC coordination | Shading/heating/cooling interlocks |
| Commissioning | Functional tests per strategy |

📺 [The Control Cabinet on YouTube](https://www.youtube.com/channel/UC5Cupmz7vlfcodpCX7k8iuQ)

*Built and documented by James · part of [The Control Cabinet BMS portfolio](https://github.com/the-control-cabinet/the-control-cabinet). MIT Licence.*
