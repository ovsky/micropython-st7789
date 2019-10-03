## MicroPython-ST7789
Simple port of popular Adafruit ST7789 display driver from CircuitPython to pure MicroPython. Can be also used as driver for cheap and good value for money chinese LCDs from Aliexpress. 

For the best performance it's highly recomended to compile scripts to .mpy before use.

Usage:
```python
from machine import Pin, SPI
import st7789

display = st7789.ST7789(SPI(1), dc=Pin(12), cs=Pin(15), rst=Pin(16))
display.fill(0x7521)
display.pixel(64, 64, 0)
```
