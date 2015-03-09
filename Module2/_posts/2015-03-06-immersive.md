---
module: 2
title: "Fonts & Layout"
category: immersive
layout: default
---

# First Hour

## Layout

- [learnlayout](http://learnlayout.com)

### The box model

- **Content** - The content of the box, where text and images appear
- **Padding** - Clears an area around the content. The padding is transparent
- **Border** - A border that goes around the padding and content
- **Margin** - Clears an area outside the border. The margin is transparent

### Some math is involved

Check out our [box](http://jsfiddle.net/ntsnre62/).

{% highlight css %}

.box {
    background-color: #cc0000;
	width: 100px;
	height: 100px;
	margin: 15px;
	padding: 15px;
    border: 5px dotted black;
}

{% endhighlight %}

The **width** of the box clearly states 100px. However, if you "inspect element" it shows as 140px. Why?

Answer: **padding** and **border** are added on top of the width value.

	  width + (2 * padding) + (2 * border) = total width
	------------------------------------------------------
	  100px +   (2 * 15px)  +   (2 * 5px)  = 140px

### Position
- Absolute
- Relative
- Fixed

### Alignment
- Centering
- Float left
- Text alignment


# Second Hour

## Typography

### Type for Dummies

**Fonts** are a universe in itself. Some designers spend their life doing mostly font design. There are several categories of fonts:

- Serif
- Sans-serif
- Slab
- Brush
- ...

## Webfonts

### Where to get them

#### Free:
Usually less weights (bold, italic, etc) and way less good options. Always check for international characters. Some staples like **Open Sans** are all over the web.

- [Google Fonts](http://www.google.com/fonts)
- [Fontsquirrel](http://www.fontsquirrel.com)

#### Paid:
More unique fonts, made by pros. Lots of weights. Can get very expensive.

- [Adobe Typekit](http://www.typekit.com) (subscription)
- [MyFonts](http://www.myfonts.com) (purchase license)

### How to choose fonts

- Pick two
- Don't be afraid to combine **serif** + **sans**
- Keep the *mood* consistent
- Only import the font weights you need

#### Read these:

- [Hoefler & Co](http://www.typography.com/techniques/)
- [The Webfont Combinator](http://font-combinator.com)
- [Typecast](http://typecast.com)

### How to apply them to your website

#### Import the fonts

##### Option A. Google Fonts

If you use Google Fonts, you will be provided with a simple way to choose which weights.

1. Choose one or more fonts
2. Click "Add to collection"
3. Go to tab "Use"
4. Select font weights
5. Copy **standard** website code (ex. `<link href='http://fonts.googleapis.com/css?family=Open+Sans' rel='stylesheet' type='text/css'>`)
6. Paste it on your HTML, *before* your main style sheet.

##### Option B. Host Locally

You can also download fonts from Google Fonts, or Fontsquirrel. That makes downloads faster and more guaranteed, but involve a bit more complicated, hands-on approach.

- Choose and download your fonts
- Go to Fontsquirrel > Webfont Generator
- Follow the instructions and download the "font kit"
- Unzip the file. Copy all fonts into a folder on your site (example: `assets/fonts`)
- Look for the style sheet files. You'll see something like:

{% highlight css %}

@font-face {
    font-family: 'open_sansbold';
    src: url('OpenSans-Bold-webfont.eot');
    src: url('OpenSans-Bold-webfont.eot?#iefix') format('embedded-opentype'),
         url('OpenSans-Bold-webfont.woff') format('woff'),
         url('OpenSans-Bold-webfont.ttf') format('truetype'),
         url('OpenSans-Bold-webfont.svg#open_sansbold') format('svg');
    font-weight: normal;
    font-style: normal;

}

{% endhighlight %}

- Add it to the top of your style sheet. You'll need to add one of these for each font weight. Make sure you pay attention to **path**.
- Change the appropriate path to the font file on your structure (`/assets/fonts` in our example)
- Change the **font-family** and **font-weight** values to match what each @font-face is referring to (in our example's case, it should be "Open Sans" and "bold")

#### Using the font

After you import the font, you can simply use it in your CSS:

{% highlight css %}

font-family: 'Open Sans';

{% endhighlight %}

### Licensing

Any .ttf font can be used as a web font. However, you must pay attention to licensing and make sure you only use fonts on the web which are licensed for such use.