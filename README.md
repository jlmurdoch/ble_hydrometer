# BLE Hydrometer

This is my attempt at a low power hydrometer running on the following hardware:
- XIAO nRF54LM20A
- 3.7V 150mAh LiPo rechargable cell

Features:
- Deep sleep for power saving
  - GRTC wake-up
- Blink LED on wake
  - PWM RGB LED
- BLE results via the BTHome format, containing:
  - IMU reading for tilt
  - Stateful storage of monotonic counter during deep sleep (GPREGRET1)
  - Basic battery state: Voltage
  - Optional: nPM1300 Fuel Gauge: Current Discharge + Battery Remaining

TODO: 
- More power tuning

Warning: Do NOT use this example with a non-rechargable battery