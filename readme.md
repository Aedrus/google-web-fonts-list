# Google Web Fonts - A List
This simple webpage was created to store all of the google fonts that I have used throughout my web development journey and will be updated with new ones. It was also another way for me to practice new ideas and code schemes; therefore, I've added in notes for the various practices i've learned and implemented in this readme.


# Folder Architecture System
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
