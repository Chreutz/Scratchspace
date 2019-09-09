# Low-cost FFB wheel and pedals for simracing (no fancy name yet)

## Wheel

- Stepper-based, for cost reasons
  - Nema 34, probably
  - Requires very quick control loop
    - 50 Poles
    - 300 RPM => 600+ Hz sample rate on output
  - Dual H bridge 
    - Current feedback
    - PWM directly driven by MCU
      - 600 Hz * 1024 PWM = 600+ kHz base frequency
- DIY Optical/Magnetic hybrid encoder
  - 3D printed disc incorporating:
    - 10 position absolute optical encoder
    - 10 pairs of disc magnets for an AS5311 for absolute position in each optical inteval
- MCU in wheel with high speed serial connection
  - 4 position slip ring (https://www.aliexpress.com/item/32824982200.html)
    - Power
    - TX
    - RX
    - GND

## Pedals

- Mechanicals based solely on 3D printed parts
- Syringes for hydraulic/pneumatic springs?
  - Possibly pressure sensor?
    - https://www.aliexpress.com/item/33054432260.html
- Encoder/pot or LC?
  - Which is cheapest?
  - Non-linear response?
    - Calibration of encoder/pot


