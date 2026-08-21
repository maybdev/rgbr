# rgbr
🟥🟩🟦 A mini JS library that demos a subpixel effect on a HTML canvas.

***

### ⛳ Variables
**`rgbr.width`** *(default 256)*  
The number of available pixels horizontally.  
*⚠️ Changing this variable will not change the canvas width ⚠️*

**`rgbr.height`** *(default 256)*  
The number of available pixels vertically.  
*⚠️ Changing this variable will not change the canvas height ⚠️*

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

***

```html
<script src="https://maybdev.github.io/rgbr/rgbr.js"></script>

<script>
  rgbr.clear(255,255,255);
</script>
```
