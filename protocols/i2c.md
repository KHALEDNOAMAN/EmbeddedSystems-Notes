# I2C (Inter-Integrated Circuit)

I2C is a synchronous, multi-master, multi-slave, packet-switched, single-ended, serial bus.

## Pins
- **SDA**: Serial Data
- **SCL**: Serial Clock

*Both require pull-up resistors.*

## Addressing
- 7-bit or 10-bit addressing
- R/W bit appended to address

## Diagram
`	ext
SDA: ---\___/----------\___
SCL: ------\_/-\_...
`
"@

Upload-File -path "protocols/spi.md" -message "Add SPI notes" -contentStr @"
# SPI (Serial Peripheral Interface)

SPI is a synchronous serial communication interface specification used for short-distance communication, primarily in embedded systems.

## Pins
- **MOSI**: Master Out Slave In
- **MISO**: Master In Slave Out
- **SCLK**: Serial Clock
- **CS/SS**: Chip Select / Slave Select

## Modes
Determined by CPOL (Clock Polarity) and CPHA (Clock Phase).
- Mode 0: CPOL=0, CPHA=0
- Mode 1: CPOL=0, CPHA=1
- Mode 2: CPOL=1, CPHA=0
- Mode 3: CPOL=1, CPHA=1