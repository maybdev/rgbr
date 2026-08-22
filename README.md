# rgbr
🟥🟩🟦 A mini JS library that demos a subpixel effect on a HTML canvas.

***

### 🎯 Functions
**`rgbr.pixel(x,y,r,g,b)`**  
Changes the pixel at the position **x,y** to the color **(r,g,b)**.

**`rgbr.rect(x,y,w,h,r,g,b)`**  
Changes all pixels inside a rectangle, sized **w,h** at the position **x,y** to the color **(r,g,b)**. Width and height must be positive.  
*⚠️ This is faster than `rgbr.pixel()` at making a solid rectangle ⚠️*

**`rgbr.clear(r,g,b)`**  
Fills the canvas with the color **(r,g,b)**.  
*⚠️ This is the equivalent of `rgbr.rect(0,0,rgbr.width(),rgbr.height(),r,g,b)` ⚠️*

**`rgbr.black()`**  
Fills the canvas with black.  
*⚠️ This is faster than `rgbr.clear(0,0,0)` ⚠️*

### ⛳ Function/Variable

**`rgbr.width(w)`**
* **If no argument is given**
  - Returns the logical width *(canvas width / 3)*
* **If an argument is given**
  - Changes the logical width to **w** *(may reset the canvas contents)*

*⚠️ Will break if **w** is not an integer ⚠️*

**`rgbr.height(h)`**
* **If no argument is given**
  - Returns the logical height *(canvas height / 3)*
* **If an argument is given**
  - Changes the logical height to **h** *(may reset the canvas contents)*

*⚠️ Will break if **h** is not an integer ⚠️*

### 🌑 Internal Variables

*`rgbr.s`*  
The canvas drawing context.

*`rgbr.c`*  
The canvas element.

*`rgbr.c.width`*  
The canvas width.

*`rgbr.c.height`*  
The canvas height.

***

```html
<script src="https://maybdev.github.io/rgbr/rgbr.js"></script>

<script>
  rgbr.clear(255,255,255);
</script>
```
