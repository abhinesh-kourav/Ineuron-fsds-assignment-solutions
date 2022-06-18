## PYTHON BASIC ASSIGNMENT 14

1. What does RGBA stand for?<br>
Ans. RGBA color values are an extension of RGB color values with an alpha channel - which specifies the opacity for a color.<br>
RGBA - Red, Blue, Green, Alpha

2. From the Pillow module, how do you get the RGBA value of any images?<br>
Ans.
```
from PIL import Image
img = Image.open('5tz4x7.jpg')
pixels = img.convert('RGBA')
data = img.getdata()
lop = []
for pixel in data:
    lop.append(pixel)
print(lop)
```

3. What is a box tuple, and how does it work?<br>
Ans. <br>
It is a tuple of four integer coordinates that represent a rectangular region in an image. The four integers are, in order, as follows:<br>
Left : The x-coordinate of the leftmost edge of the box.<br>
Top : The y-coordinate of the top edge of the box.<br>
Right : The x-coordinate of one pixel to the right of the rightmost edge of the box. This integer must be greater than the left integer.<br>
Bottom : The y-coordinate of one pixel lower than the bottom edge of the box. This integer must be greater than the top integer.

4. Use your image and load in notebook then, How can you find out the width and height of an
Image object?
```
from PIL import Image

img = Image.open('5tz4x7.jpg')
width, height = img.size
print(width, height)
```

5. What method would you call to get Image object for a 100×100 image, excluding the lower-left
quarter of it?<br>
Ans.<br>
`img.crop((0, 50, 50, 50))`

6. After making changes to an Image object, how could you save it as an image file?<br>
Ans.<br>
`img.save('xyz.png')`

7. What module contains Pillow’s shape-drawing code?
Ans.<br>
ImageDraw

8. Image objects do not have drawing methods. What kind of object does? How do you get this kind
of object?<br>
Ans.<br>
ImageDraw objects have shape-drawing methods such as point(), line(), or rectangle(). They are returned by passing the Image object to the ImageDraw.Draw() function.