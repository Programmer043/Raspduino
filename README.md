# Raspduino

This is a simple adapter that allows the use of Arduino UNO compatible shields to be used with a Raspberry Pi Pico.

The pinout is following:

GPIO0-13 - Arduino 0-13
GPIO14-15 - Arduino SDA/SCL (top left near reset)
GPIO16-17 - Extra UART header
GPIO16-19 - Extra SPI header
GPIO20 - Arduino A4 (SDA)
GPIO21 - Arduino A5 (SCL)
GPIO22 - Arduino A3
GPIO26-28 - Arduino A0-A2

NOTE: GPIO20-22 doesn't support analog in, so Arduino A3-A5 won't work as analog input. This is a hardware limitation of the Raspberry Pi Pico and can't be solved.

ADC_REF - Arduino AREF
3V3 OUT - Arduino 3V3
3V3_EN - N/C
VBUS (USB Power input) - Arduino 5V
VSYS - N/C
GND - Arduino GND

Arduino Vin - N/C

RUN - Arduino Reset and onboard switch

SWCLK - N/C
SWDIO - N/C
SWGND - N/C
