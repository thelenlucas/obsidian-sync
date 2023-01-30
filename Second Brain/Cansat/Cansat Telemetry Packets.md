---
tags: Cansat_2023
---

For the Mission, the [[Cansat Software System]] will be sending these packets as 1Hz to the [[Cansat Ground System]]. These packets will be formatted:

```
TEAM_ID,MISSION_TIME,PACKET_COUNT,MODE,STATE,ALTITUDE,HS_DEPLOYED,PC_DEPLOYED,MAST_RAISED,TEMPERATURE,VOLTAGE,GPS_TIME,GPS_ALTITDUDE,GPS_LATITUDE,GPS_LONGITUDE,GPS_SATS,TILT_X,TILT_Y,CMD_ECHO
```

| Field         | Width/Precision | Variable Type    |
| ------------- | --------------- | ---------------- |
| TEAM_ID       | 4 Digit Number  | u16              |
| MISSION_TIME  | 2 ints, 1 float | 2xu8, 1xf32     |
| PACKET_COUNT  |                 | u16              |
| MODE          | Toggle (F/S)    | u8 (conv. later) |
| STATE         |                 | u8 (conv.)       |
| ALTITUDE      | 0.1m            | f32              |
| HS_DEPLOYED   | P/N Toggle      | u8               |
| TEMPERATURE   | 0.1 degrees     | f32              |
| VOLTAGE       | 0.1V            | f32              |
| GPS_TIME      | 2 ints, 1 float | 2xu16, 1xf16     |
| GPS_ALTITUDE  | 0.1m            | f32              |
| GPS_LATITUDE  | 0.0001 degrees  | f32              |
| GPS_LONGITUDE | 0.0001 degrees  | f32              |
| GPS_SATS      |                 | u8               |
| CMD_ECHO      | String          | u8 array?                 |
