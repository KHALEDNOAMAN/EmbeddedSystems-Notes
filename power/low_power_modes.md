# Low Power Modes

- **Sleep**: CPU stops, peripherals run. Wakes fast on interrupt.
- **Stop/Deep Sleep**: Main clocks stop. SRAM retained. Wake via EXTI or RTC.
- **Standby**: Vcore off. SRAM lost (except backup domain). Wakes via reset/wakeup pin.