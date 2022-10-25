# Google Web Fonts | A List for Developers
View list: https://619bfc86515892816bd8a83e--angry-brahmagupta-f007bf.netlify.app/

### Update 10/25/2022
Website has been rebuilt with simpler code to make website easier to setup with Github Pages (Reverted back to vanilla CSS). Additionally, new fonts have been added and UX/UI has been overhauled for a new design.

## Introduction
This simple webpage was created to store all of the google fonts that I have discovered throughout my web development journey and will serve as a iterative list of new fonts. It was also another way for me to practice new ideas and code schemes; therefore, I've added notes for the various practices i've learned and implemented in the list itself.


## Folder Architecture System
I started by designing a root folder heirarchy architecture that would fit my needs as a developer and serve as an improvement over my previous architecture.

To create this architecture I looked at various community architectures as well as other common systems used by larger teams and combined them, with a splash of my own taste, to create a system that fit my needs. Here is the basic format of the system I use:
```
v Root
|--v app                 //Contains styles and scripts | I prefer app, you could also use src.
|----> js                  //Javascript files
|----v scss                //SASS files and partials
|------v base                 //Contains global boilerplate code and defaults for main elements and primary styles.
|      |  _base.scss
|      |  _reset.scss
|      |  _type.scss
|      |  _animations.scss
|      |  _...
|------v layout                //Contains styles for main site sections, grid/flex, and other layout styles.
|      |  _header.scss
|      |  _footer.scss
|      |  _nav.scss
|      |  _flex.scss
|      |  _grid.scss
|      |  _...
|------v modules                 //Contains styles for smaller widgets and UI elements that make up the page.
|      |  _buttons.scss
|      |  _forms.scss
|      |  _media.scss
|      |  _cards.scss
|      |  _dropdown.scss
|      |  _...
|------v utils                 //Contains styles for use in SCSS applications across all styles.
|      |  _variables.scss
|      |  _functions.scss
|      |  _colors.scss
|      |  _mixins.scss
|      |  _breakpoints.scss
|      |  _...
|--> assets                   //Contains files for site such as images, fonts, video, etc.
|--> common                   //HTML pages and the like.
|--> dist                     //Contains css files compiled from scss.
```

## Top to Bottom: The Header
After setting up some scss files, I set out to design the header, or top nav bar, that would simply display the title of the page. I worked on the following:
* Styling the body to have an off white color and styling the header to have a white color.
* Setting globals for margin and padding to remove space around header.
* Set flex in _grid.scss for justify content and align content to align header in top bar.

## Top to Bottom: The Cards
Once the top header was done, I started designing the cards that make up each google font. I worked on the following:
* Setting a white background for the card as well as a box shadow to make it stand out.
* Margins to push it away from edges of the viewport and other cards.
* Padding to add "padding" within the card, increasing white space between the inner text.
* Using flex I set up a system of classes that align the 3 text elements horizontally and vertically.

## The Meat: Fonts
I then imported all of the google fonts within the _type.scss file and applied them via classes. This part was relatively simple compared to the rest. The font were broken into two sections: sans serif and serif.

## Wrapping It Up
To finish it off, I added simple css animations to the font cards, cards for importing the font, and a footer. To see all of these details, you can download the repository and view the page as an html document, otherwise the link at the top offers a barebones format for quick reading.
