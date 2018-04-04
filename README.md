# dcon-nashville-prenote
Song lyrics for the drupalcon nashville prenote, using [slides.js](https://github.com/hakimel/reveal.js). For complete documentation, see the slides.js github page.

## How to run the slides

To run this locally, clone it and start a webserver in the directory:

```
git clone --recursive https://github.com/ohthehugemanatee/dcon-nashville-prenote.git
cd dcon-nashville-prenote
php -S 0.0.0.0:8080
```

Then visit `http://localhost/`.

## How to use the presentation

* Arrow keys advance the slides.
* Press `s` to open the Speaker notes
* Press `esc` or `o` to open the presentation Overview.
* Press `f` to go Fullscreen

## How to edit the presentation

Edit `presentation.md`.

* Write anything you like in markdown
* new (horizontal) slides are separated by 3 linebreaks
* new (vertical) slides are separated by 4 linebreaks.
* On each slide, if you add a `Note:`, it will begin a speaker notes section until the end of the slide.
* You can add raw HTML without any special handling
* To add an image, put it in a subdirectory in this repo, and reference it in `![](img/my-image.jpg)<!-- .element height="300px" width="300px" -->`. Note this example also adds HTML element attributes for `width` and `height`.


