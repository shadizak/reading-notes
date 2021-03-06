


 
# Today's topics are interesting and enjoyable:

**>  1. Images in HTML**
**>  2. Color in HTML**
**>  3. Text in HTML**

> # 1. Images in Links:
 - How to add images to pages  
 - Choosing the right format
 - Optimizing images for the web

### There are many reasons why you might want to add an image to a web page: you might want to include a logo, photograph, illustration, diagram, or chart.

## HTML Images Syntax

In HTML, images are defined with the  `<img>`  tag.

The  `<img>`  tag is empty, it contains attributes only, and does not have a closing tag.

The  `src`  attribute specifies the URL (web address) of the image:

    <img src="_url_">
## The Alt Attribute

The  `alt`  attribute provides an alternate text for an image, if the user for some reason cannot view it (because of slow connection, an error in the src attribute, or if the user uses a screen reader).

The value of the  `alt`  attribute should describe the image:## The alt Attribute

The  `alt`  attribute provides an alternate text for an image, if the user for some reason cannot view it (because of slow connection, an error in the src attribute, or if the user uses a screen reader).

The value of the  `alt`  attribute should describe the image:

    <img src="img_chania.jpg"  alt="Flowers in Chania">
If a browser cannot find an image, it will display the value of the `alt` attribute.

###  Image Size - Width and Height

You can use the  `style`  attribute to specify the width and height of an image.

    <img src="img_girl.jpg"  alt="Girl in a jacket"  style="width:500px;height:600px;">
Alternatively, you can use the  `width`  and  `height`  attributes:

    <img src="img_girl.jpg"  alt="Girl in a jacket"  width="500"  height="600">
The `width` and `height` attributes always define the width and height of the image in pixels.

###  Width and Height, or Style?

The  `width`,  `height`, and  `style`  attributes are valid in HTML.

However, we suggest using the  `style`  attribute. It prevents styles sheets from changing the size of images:

    <!DOCTYPE html>  
    <html>  
    <head>  
    <style>  
    img  {  
    width:  100%;  
    }  
    </style>  
    </head>  
    <body>  
      
    <img src="html5.gif"  alt="HTML5 Icon"  width="128"  height="128">  
    <img src="html5.gif"  alt="HTML5 Icon"  style="width:128px;height:128px;">  
      
    </body>  
    </html>


   ## Three rules for CreatIng Images
   There are three rules to remember when you are creating images for your website which are summarized below. We go into greater detail on each topic over the next nine pages.

1. Save Images In the rIght format
Websites mainly use images in jpeg, gif, or png format. If you choose the wrong image format then your image might not look as sharp as it should and can make the web page slower to load.

2. Save Images at the rIght sIze
You should save the image at the same width and height it will appear on the website. If  
the image is smaller than the width or height that you have specified, the image can be distorted and stretched. If the image is larger than the width and height if you have specified, the image will take longer to display on the page.

3. Use the correct resolutIon
Computer screens are made up of dots known as pixels. Images used on the web are also made up of tiny dots. Resolution refers to the number of dots per inch, and most computer screens only show web pages at 72 pixels

per inch. So saving images at a higher resolution results in images that are larger than necessary and take longer to download.

> ## **Summary Images**

 - The <img> element is used to add images to a web page.
 - You must always specify a src attribute to indicate the source of an
   image and an alt attribute to describe the content of an image.
 - You should save images at the size you will be using them on the web
   page and in the appropriate format.
 - Photographs are best saved as JPEGs; illustrations or logos that use
   flat colors are better saved as GIFs.

> # 2. Color in Links:
- How to specify colors  
 - Color terminology and contrast
  - Background color
**Color can really bring your pages to life.**

**How to choose color for any element?**
HTML colors are specified with predefined color names, or with RGB, HEX, HSL, RGBA, or HSLA values.

## Color Values
**The following three `<div>` elements have their background color set with RGB, HEX, and HSL values:**

    <h1 style="background-color:rgb(255, 99, 71);">...</h1>  
    <h1 style="background-color:#ff6347;">...</h1>  
    <h1 style="background-color:hsl(9, 100%, 64%);">...</h1>
Result: 

![image info](./img/img6.png)

 1. ٌRGB Values
 These express colors in terms of how much red, green and blue are used to make it up. For example: rgb(100,100,90)

2. Hex Codes
These are six-digit codes that represent the amount of red, green and blue in a color, preceded by a pound or hash # sign. For example: #ee3e80

3. Color names
There are 147 predefined color names that are recognized  
by browsers. For example: DarkCyan.

## Background  Color
By -> `background-color`
CSS treats each HTML element as if it appears in a box, and the background-color property sets the color of the background for that box.

You can specify your choice of background color in the same three ways you can specify foreground colors: RGB values, hex codes, and color names (covered on the next page).

If you do not specify a background color, then the background is transparent.

By default, most browser windows have a white background, but browser users can set a background color for their windows, so if you want  
to be sure that the background is white you can use the background-color property on the <body> element.

## Understanding Color
Every color on a computer screen is created by mixing amounts of red, green, and blue. To find the color you want, you can use a color picker
Computer monitors are made up of thousands of tiny squares called pixels (if you look very closely at your monitor you should be able to see them).

When the screen is not turned on, it's black because it's not emitting any light. When it's on, each pixel can be a different color, creating a picture.

The color of every pixel on the screen is expressed in terms of a mix of red, green, and blue — just like on a television screen
![image info](./img/img7.png)

> # 3. Text in Links:

 - Size and typeface of text
 - Bold, italics, capitals, underlines
 - Spacing between lines, words, and letters

> **The properties that allow you to control the appearance of text can be
> split into two groups:**

 1. Those that directly affect the font and its appearance (including
    the typeface, whether it is regular, bold or italic, and the size of
    the text).
    
 2. Those that would have the same effect on text no matter what font
   you were using (including the color of text and the spacing between
    words and letters).


### 1. Specifying Typefaces

#### By Using > font-family
he font-family property allows you to specify the typeface that should be used for any text inside the element(s) to which a CSS rule applies.

The value of this property is the name of the typeface you want to use.

The people who are visiting your site need the typeface you have specified installed on their computer in order for it to be displayed.

You can specify a list of fonts separated by commas so that,  
if the user does not have your first choice of typeface installed, the browser can try to use an alternative font from the list.

It is also common to end with a generic font name for that type of font (which you saw on pages 269-270).

If a font name is made up of more than one word, it should be put in double quotes.

Designers suggest pages usually look better if they use no more than three typefaces on a page.

### 2. Size of Type 
### By Using :> font-size
The font-size property enables you to specify a size for the  font. There are several ways to specify the size of a font. The most common are:

1. Pixels

	Pixels are commonly used because they allow web designers very precise control over how much space their text takes up. The number of pixels is followed by the letters px.

2. Percentages

	The default size of text in browsers is 16px. So a size of 75% would be the equivalent of 12px, and 200% would be 32px.

	If you create a rule to make all text inside the <body> element to be 75% of the default size (to make it 12px), and then specify another rule that indicates the content of an element inside the <body> element should be 75% size, it will be 9px (75% of the 12px font size).

3. ems

	An em is equivalent to the width of a letter m.
	
![image info](./img/img8.png)

## 3. Bold

### By >> font-weight
The font-weight property allows you to create bold text. There are two values that this property commonly takes:
  **1. Normal**
This causes text to appear at a normal weight.
  **2. Bold**
This causes text to appear bold.

In this example, you can see that the element whose class attribute has a value of credits has been bolded.
![image info](./img/img9.png)

