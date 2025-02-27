# CSS quick start

https://medium.com/marketkarma/58-bytes-of-css-to-look-great-nearly-everywhere-befbc1e08b96

```css
html {
  font-family: sans-serif;  
  font-size: 1.25em;
  max-width: 70ch;
  margin: auto;
  padding: 2ch;
  line-height: 1.75;
  background: #FFF;
  color: #222;
}

h1,h2,h3,h4,h5,h6 {
  margin: 3em 0 1em;
}

p,ul,ol,li {
  margin-bottom: 2em;
}

pre {
  overflow-x: auto;
}

@media print {
  color: unset
}
```


## font-family: sans-serif

Users achieve better reability with a sans serif font versus a serif font, for the most users, and most website contexts.


## font-size: 1.25em

Recent design trends and screen sizes tend toward bigger font sizes. Prefer "em" or "rem" over "px" because users can scale "em" more easily.


## color: #222

Foreground color is hex code #222222 which is dark gray. More users can read dark gray text better than pure black text, when the text is on a web page with a white background.


## background: #FFF

Background color is hex code #FFFFFF which is pure white. More users achieve better reability with the color combination of foreground dark gray on background pure white.


## margin: auto

Margin is automatic. This centers the page content.


## padding: 2ch

Padding is 2 characters on all four sides. If the display's width goes under the max-width set above, then this padding prevents edge-to-edge text on mobile.


## line-height: 1.75

Line height is 1.75 times normal. Line spacing between lines helps increase visual clarity. The line height is unitless because it is a multiplier, not a pixel count, not a font size, etc.


## max-width: 70ch

Maximum width is 70 characters. The "readable range" is usually 60-80 character widths, and CSS lets you express that directly with the "ch" unit which means "characters".


## pre { overflow-x: auto; }

Solve side-to-side scrolling of preformatted text, such as side-to-side scrolling when a page is showing source code blocks.


## @media print { color: unset }

When the user prints the page, then do not use color. For our CSS, this means that the user's printer will print pure black text, and not dark gray text.

