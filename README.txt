readme.txt file

# Main CSS

https://latex.vercel.app/
https://github.com/vincentdoerig/latex-css/

## License

The Academicons font is licensed under the SIL OFL 1.1:
http://scripts.sil.org/OFL
Academicons CSS, LESS, and SASS files are licensed under the MIT License:
http://opensource.org/licenses/mit-license.html
The Academicons documentation is licensed under the CC BY 3.0 License:
http://creativecommons.org/licenses/by/3.0/

https://jpswalsh.github.io/academicons/
https://github.com/jpswalsh/academicons


Font Awesome Free License
-------------------------

Font Awesome Free is free, open source, and GPL friendly. You can use it for
commercial projects, open source projects, or really almost whatever you want.
Full Font Awesome Free license: https://fontawesome.com/license/free.

# Icons: CC BY 4.0 License (https://creativecommons.org/licenses/by/4.0/)
In the Font Awesome Free download, the CC BY 4.0 license applies to all icons
packaged as SVG and JS file types.

# Fonts: SIL OFL 1.1 License (https://scripts.sil.org/OFL)
In the Font Awesome Free download, the SIL OFL license applies to all icons
packaged as web and desktop font files.

# Code: MIT License (https://opensource.org/licenses/MIT)
In the Font Awesome Free download, the MIT license applies to all non-font and
non-icon files.

# Attribution
Attribution is required by MIT, SIL OFL, and CC BY licenses. Downloaded Font
Awesome Free files already contain embedded comments with sufficient
attribution, so you shouldn't need to do anything additional when using these
files normally.

We've kept attribution comments terse, so we ask that you do not actively work
to remove them from files, especially code. They're a great way for folks to
learn about Font Awesome.

# Brand Icons
All brand icons are trademarks of their respective owners. The use of these
trademarks does not indicate endorsement of the trademark holder by Font
Awesome, nor vice versa. **Please do not use brand logos for any purpose except
to represent the company, product, or service to which they refer.**



-----

for publist.

convert .bib to yaml using `pybtex` installed via `pip install pybtex`

```
pybtex-convert papers.bib papers.html
```

-----

# If i want to upgrading the TOC
If i want upgrade the toc generator 

# Table of Contents
Automatically generate a table of contents from the headings on the page

**[Demo](https://cferdinandi.github.io/table-of-contents/)**

[Getting Started](#getting-started) | [Options & Settings](#options-and-settings) | [Browser Compatibility](#browser-compatibility) | [License](#license)


## Getting Started

### 1. Include Table of Contents on your site.

```html
<script src="/assets/js/table-of-contents.js"></script>
```

### 2. Add the markup to your HTML.

Include an empty element on the page that will hold your table of contents, and give it a unique selector. You also need to wrap the content that you want to generate your table of contents from in an element with a unique selector.

You can use any selectors you want. The example below uses data attributes.

```html
<div data-toc></div>

<div data-content>
	<h2>Cat O'Nine Tails</h2>
	<p>...</p>

	<h3 id="the-brig">The Brig</h3>
	<p>...</p>

	<h4>Privateer</h4>
	<p>...</p>

	<h2>Ahoy</h2>
	<p>...</p>
</div>
```

*__Note:__ headings without an ID will have one automatically generated based on the heading content.*

### 3. Initialize Table of Contents

In the footer of your page, after the content, initialize Table of Contents by passing in two arguments: the table of contents element selector, and content selector.

```html
<script>
	tableOfContents('[data-toc]', '[data-content]');
</script>
```



## Options and Settings

You can pass options into `tableOfContents()` as an optional third argument when initializing it to customize how the script works.

```javascript
tableOfContents('[data-content]', '[data-toc]', {
	levels: 'h2, h3, h4, h5, h6', // The heading levels to generate a table of contents from
	heading: 'Table of Contents', // The heading text for the table of contents list
	headingLevel: 'h2', // The level to use for the heading for the table of contents list
	listType: 'ul' // The list type to use for the table of contents
});
```



## Browser Compatibility

Table of Contents works in all modern browsers, and IE 9 and above.



## License

The code is available under the [MIT License](LICENSE.md).

