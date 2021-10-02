Initialization
import board
import NeoPixel
pin = board.D18
PIXEL_NUM = 96
ORDER = neopixel.RGB
pixels = neopixel.NeoPixel(pin, PIXEL_NUM, auto_write=False, pixel_order=ORDER)

pixels.show() - shows the new colors on the pixels - needed wtih auto_write set to False
pixels.fill(color) - fill the pixels with color
pixels.brightness - change brightness (between 0 and 1.0)
pixels.deinit() - blank out the pixels