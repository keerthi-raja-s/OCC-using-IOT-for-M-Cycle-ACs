# IoT-for-M-Cycle-AC

| #  | Component                                                 | Typical spec / part number\*              |  Qty  | Unit cost (₹) | Sub-total (₹) | Purpose                        |
| -- | --------------------------------------------------------- | ----------------------------------------- | :---: | ------------: | ------------: | ------------------------------ |
| 1  | **Edge MCU**                                              | ESP32-S3 DevKit-C (Wi-Fi/BLE, 2 MB PSRAM) |   1   |           450 |           450 | Local PID + failsafe control   |
| 2  | **Outdoor / indoor T-RH-P sensor**                        | BME280 break-out (I²C)                    |   1   |           280 |           280 | Comfort & weather feedback     |
| 3  | **Occupancy radar**                                       | S-110 60 GHz mmWave module                |   1   |           950 |           950 | Live occupant count            |
| 4  | **CO₂ sensor**                                            | MH-Z19C NDIR, 400–5 000 ppm               |   1   |         1 450 |         1 450 | Proxy for metabolic load / IAQ |
| 5  | **Window / door status**                                  | Magnetic reed or Hall switch              |   4   |            50 |           200 | Envelope open/closed logic     |
| 6  | **Fan & pump current sense**                              | INA219 0–3 A ±1 %                         |   2   |           120 |           240 | Real-time power & fault detect |
| 7  | **Water-temp probes**                                     | DS18B20 waterproof 1 %                    |   2   |           120 |           240 | Sump & SAT verification        |
| 8  | **Sump level switch**                                     | PP float switch, N/O                      |   1   |            90 |            90 | Dry-run protection             |
| 9  | **LoRa-WAN node**                                         | RAK3172 STM32WL                           |   1   |           690 |           690 | Low-power sensor backhaul      |
| 10 | **RS-485 isolator**                                       | Modbus-RTU (MAX3485 + ISO)                |   1   |           350 |           350 | VFD/PLC field-bus              |
| 11 | **VFD – supply fan**                                      | 1.5 kW, 415 V, Modbus                     |   1   |         4 000 |         4 000 | Variable airflow control       |
| 12 | **VFD – exhaust fan**                                     | 1.5 kW, 415 V, Modbus                     |   1   |         4 000 |         4 000 | Exhaust balancing              |
| 13 | **VFD – water pump**                                      | 0.75 kW, 240 V, Modbus                    |   1   |         3 200 |         3 200 | Wetting rate modulation        |
| 14 | **Edge gateway**                                          | Raspberry Pi CM4-2G + carrier             |   1   |         7 500 |         7 500 | Node-RED / MQTT broker         |
| 15 | **LTE/Wi-Fi hat**                                         | 4G CAT-4, GNSS                            |   1   |         2 500 |         2 500 | Cloud back-haul & OTA          |
| 16 | **12 V @ 5 A PSU**                                        | DIN-rail, 85-264 VAC in                   |   1   |           900 |           900 | Sensor & MCU rail              |
| 17 | **24 V @ 5 A PSU**                                        | DIN-rail                                  |   1   |         1 100 |         1 100 | Field-bus & relay rail         |
| 18 | **Industrial enclosure**                                  | ABS IP-65, 300 × 400 × 150 mm             |   1   |         1 500 |         1 500 | Control panel housing          |
| 19 | **Shielded CAT-6 patch**                                  | 3 m, RJ-45                                |   3   |           150 |           450 | Gateway ↔ switch links         |
| 20 | **Sensor cable**                                          | 4-core, shielded, 0.5 mm²                 |  30 m |          25/m |           750 | Low-noise runs                 |
| 21 | **Cable glands & ferrules**                               | assorted M16–M20                          | 1 set |           500 |           500 | IP-rated entries               |
| 22 | **Mini-breakers & relays**                                | 2-pole C-curve, 6 A                       | 1 set |           800 |           800 | Protection & manual bypass     |
|    | ***Estimated hardware total***                            |                                           |       |               |  **₹ 32 140** | \~ US \$ 385                   |
|    | Project-management, wiring consumables & 10 % contingency |                                           |       |               | **+ ₹ 3 200** |                                |
|    | **Grand total (excl. GST)**                               |                                           |       |               |  **₹ 35 300** |                                |
