# rgbr
🟥🟩🟦 A mini JS library that demos a subpixel effect on a HTML canvas.

***

### ⛳ Variables
**`rgbr.width`**  
The number of available pixels horizontally.

**`rgbr.height`**  
The number of available pixels vertically.

### 🎯 Functions
**`rgbr.pixel(x,y,r,g,b)`**  
Changes the pixel at the position **x,y** to the color **(r,g,b)**.

**`rgbr.rect(x,y,w,h,r,g,b)`**  
Fills all pixels inside a rectangle, sized **w,h** at the position **x,y** to the color **(r,g,b)**. Width and height must be positive.  
*⚠️ This is faster than `rgbr.pixel()` at making a solid rectangle ⚠️*

**`rgbr.clear(r,g,b)`**  
Fills the canvas with the color **(r,g,b)**.  
*⚠️ This is the equivalent of `rgbr.rect(0,0,rgbr.width,rgbr.height,r,g,b)` ⚠️*

**`rgbr.black()`**  
Fills the canvas with black.  
*⚠️ This is faster than `rgbr.clear(0,0,0)` ⚠️*
