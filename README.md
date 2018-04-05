# dcon-nashville-prenote
Song lyrics for the drupalcon nashville prenote, using [slides.js](https://github.com/hakimel/reveal.js). For complete documentation, see the slides.js github page.

# How to use the presentation

You can run this presentation on your local machine. 

```
git clone --recursive https://github.com/ohthehugemanatee/dcon-nashville-prenote.git
cd dcon-nashville-prenote
php -S 0.0.0.0:8080
```

Then visit `http://localhost/index-local.html` in your browser.

## How to edit the presentation

Edit `presentation.md`.

* Write anything you like in markdown
* new (vertical) slides are separated by 3 linebreaks
* new (horizontal) slides are separated by a line with just `***` on it.
* On each slide, if you add a `Note:`, it will begin a speaker notes section until the end of the slide.
* You can add raw HTML without any special handling
* To add an image, put it in a subdirectory in this repo, and reference it in `![](img/my-image.jpg)<!-- .element height="300px" width="300px" -->`. Note this example also adds HTML element attributes for `width` and `height`.


