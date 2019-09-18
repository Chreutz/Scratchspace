# Low-cost FFB wheel and pedals for simracing (no fancy name yet)

## Wheel

- Stepper-based, for cost reasons
  - Nema 34, probably
  - Requires very quick control loop
    - 50 Poles
    - 300 RPM => 600+ Hz sample rate on output
      - Aim for 1000 Hz refresh/sample rate
  - Dual H bridge 
    - Current feedback
    - PWM directly driven by MCU
      - 10 bit PWM (1024 steps)
      - 1000 Hz * 1024 PWM = 1+ MHz base frequency
- DIY Optical/Magnetic hybrid encoder
  - 3D printed disc incorporating:
    - 10 position absolute optical encoder
    - 10 pairs of disc magnets for an AS5311 for absolute position in each optical inteval
- MCU in wheel with high speed serial connection
  - Probably not slip ring in first version.
    - Coiled usb cable
  - 4 pole XLR for connecting through "quick release"

## Pedals

- Mechanicals based solely on 3D printed parts
- Syringes for hydraulic/pneumatic springs?
  - Possibly pressure sensor?
    - https://www.aliexpress.com/item/33054432260.html
- Encoder/pot or LC?
  - Which is cheapest?
  - Non-linear response?
    - Calibration of encoder/pot


