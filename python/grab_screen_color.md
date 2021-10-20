```python
from mss import mss
import numpy


pixel_pos = { "left": 1234, "top": 123, "width": 1, "height": 1}

sct = mss()

pixel_rgb = numpy.array(sct.grab(pixel_pos))[0][0]
pixel_hex = '#%02x%02x%02x' % (pixelrgb[0], pixelrgb[1], pixelrgb[2])

  

print(pixel_rgb)
print(pixel_hex)

```