 
# Today we are going to talk about texts and CSS in HTML

## Text

1. Headings and paragraphs
2. Bold, italic, emphasis
3. Structural and semantic markup
 
 
 ### Headings
 
HTML has six "levels" of headings:
<h1> is used for main headings <h2> is used for subheadings
If there are further sections under the subheadings then the <h3> element is used, and so on...
Browsers display the contents of headings at different sizes. The contents of an <h1> element is the largest, and the contents of an <h6> element is the smallest. The exact size at which each browser shows the headings can vary slightly. Users can also adjust the size of text in their browser. You will see how to control the size of text, its color, and the fonts used when we come to look at CSS.
 
_For Example_
 
```
html>
    <body>
         <h1>This is a Main Heading</h1>
         <h2>This is a Level 2 Heading</h2>
         <h3>This is a Level 3 Heading</h3>
         <h4>This is a Level 4 Heading</h4>
         <h5>This is a Level 5 Heading</h5>
         <h6>This is a Level 6 Heading</h6>
         
    </body>
</html>
```
### Paragraphs 
To create a paragraph, surround the words that make up the paragraph with an opening <p> tag and closing </p> tag.
By default, a browser will show each paragraph on a new line with some space between it and any subsequent paragraphs.
 _For Example_
 
```
    <p>Shadi</p>
    <p>Zaqout</p>
 ```
### Bold & iTalic 

1. ``` <b> ```
By enclosing words in the tags <b> and </b> we can make characters appear bold.
The <b> element also represents a section of text that would be presented in a visually different way (for example key words in a paragraph) although the use of the <b> element does not imply any additional meaning.

2. ``` <i>  ```  
By enclosing words in the tags <i> and </i> we can make characters appear italic.
The <i> element also represents a section of text that would be said in a different way from surrounding content — such as technical terms, names of ships, foreign words, thoughts, or other terms that would usually be italicized.
 
 ``` </i> ``` 
  
### Superscript and Subscript
1. ``` <sup> ```
The <sup> element is used
to contain characters that should be superscript such
as the suffixes of dates or mathematical concepts like raising a number to a power such as 22.

2. ``` <sub> ```
The <sub> element is used to contain characters that should be subscript. It is commonly used with foot notes or chemical formulas such as H20.

### Horizontal rules and Line breaks
There are two tags that can be used to control the layout of your page.
1. Horizontal Rule ``` <hr> ```

To create a break between themes — such as a change of topic in a book or a new scene
in a play — you can add a horizontal rule between sections using the <hr /> tag.
There are a few elements that do not have any words between an opening and closing tag. They are known as empty elements and they are written differently.
An empty element usually
has only one tag. Before the closing angled bracket of an empty element there will often be a space and a forward slash character. Some web page authors miss this out but it is a good habit to get into.

2. Line break ``` <br> -- ``` inserts a end of line where it appear
As you have already seen, the browser will automatically show each new paragraph or heading on a new line. But if you wanted to add a line break inside the middle of a paragraph you can use the line break tag <br />.


NOTE: Neither have a closing tag or associated text, their use is fairly straightforward.

### Strong & Emphasis
The <strong> and <em> tags are used for emphasizing parts of a text. The <strong> tag should be used to indicate strong importance, seriousness, or urgency, like to indicate key phrases in a text for someone skimming it. The <em> tag should be used to represent stress emphasis, like when you'd read the emphasized text in a different tone of voice. Both tags can be used together, where it makes sense.
 
 _Example code_
 
 ```
<!DOCTYPE html>
<html>
<head>
    <meta charset="utf-8">
    <title>HTML:The strong and em tags</title>
</head>
<body>
      <p>Where recognition of the inherent dignity and of the <strong>equal and inalienable rights</strong> of <em>all members of the human family</em> is the foundation of <strong><em>freedom, justice and peace in the world</em></strong>.</p>
 
 </body>
</html>
 ```
 ### Quotation
 There are two elements commonly used for marking up quotations:
 
 1. ``` <blockquote> ```
 
The <blockquote> element is used for longer quotes that take up an entire paragraph. Note how the <p> element is still used inside the <blockquote> element.
Browsers tend to indent the contents of the <blockquote> element, however you should not use this element just to indent a piece of text — rather you should achieve this effect using CSS.
 
 2. ``` <q> ```
 
 The <q> element is used for shorter quotes that sit within
a paragraph. Browsers are supposed to put quotes around the <q> element, however Internet Explorer does not — therefore many people avoid using the <q> element.
Both elements may use the cite attribute to indicate where the quote is from. Its value should be a URL that will have more information about the source of the quotation.
 
### The Abbreviation element

``` <abbr> ```
The `<abbr>` tag defines an abbreviation or an acronym, like "HTML", "CSS", "Mr.", "Dr.", "ASAP", "ATM".
 
_Example Code_ 

```
<!DOCTYPE html>
<html>
<body>

<h1>The abbr element</h1>

<p>The <abbr title="Cascading Style Sheets">CSS</abbr> was founded in Read 02 :) .</p>

</body>
</html>
```
### auTHor deTails
``` <address> ```
he <address> element has quite a specific use: to contain contact details for the author of the page.
It can contain a physical address, but it does not have to. For example, it may also contain a phone number or email address.
Browsers often display the content of the <address> element in italics.
You may also be interested in something called the hCard microformat for adding physical address information to your markup.

 ``` <address>
<p><a href="mailto:homer@example.org">
homer@example.org</a></p>
<p>742 Evergreen Terrace, Springfield.</p>
</address> 
```
## Example Text
his is a very simple HTML page that demonstrates text markup.
```
<html>
  <head>
<title>Text</title> </head>
<body>
<h1>The Story in the Book</h1>
<h2>Chapter 1</h2>
<p>Molly had been staring out of her window for about
an hour now. On her desk, lying between the copies of <i>Nature</i>, <i>New Scientist</i>, and all the other scientific journals her work had appeared in, was a well thumbed copy of <cite>On The Road</cite>. It had been Molly's favorite book since college, and the longer she spent in these four walls the more she felt she needed to be free.</p>
<p>She had spent the last ten years in this room, sitting under a poster with an Oscar Wilde quote proclaiming that <q>Work is the refuge of
people who have nothing better to do</q>. Although many considered her pioneering work, unraveling the secrets of the llama <abbr title="Deoxyribonucleic acid">DNA</abbr>, to be an outstanding achievement, Molly <em>did</em> think she had something better to do.</p>
  </body>
</html>
```

## IntroducIng CSS
  _into_

In this section, we will look at how to make your web pages more attractive, controlling the design of them using CSS.

**Content table**

1. Introduce you to how CSS works
2. Teach you how to write CSS rules
3. Show you how CSS rules apply to HTML pages


**What is CSS?**

CSS allows you to create rules that specify how the content of an element should appear. For example, you can specify that the background of the page is cream, all paragraphs should appear in gray using the Arial typeface, or that all level one headings should be in a blue, italic, Times typeface.

**Why CSS?**
CSS allows you to create rules that control the way that each individual box (and the contents of that box) is presented.


CSS works by associating rules with HTML elements. These rules govern how the content of specified elements should be displayed. A CSS rule contains two parts: a selector and a declaration.

```
p {
    font-family: Arial;
}
```

![CSS Rule](https://mdn.mozillademos.org/files/9461/css-declaration-small.png)

This rule indicates that all "p" elements should be shown in the Arial typeface.

Selectors indicate which element the rule applies to. The same rule can apply to more than one element if you separate the element names with commas.

Declarations indicate how the elements referred to in the selector should be styled. Declarations are split into two parts (a property and a value), and are separated by a colon.


**How to write CSS**
First you need to find the selector you want to apply **CSS** on it like paragraph or anything else like bellow
```
p, h1, h2, li {
    color: #cccccc;
    font-weight: 700; // 700 will give you a Bold text
}
```


 ## How to apply CSS in your page

There are three way to implement your CSS with
1. Inline CSS
2. Add style tag into head and put your css on it
3. External CSS file the link it to you page

 
 
