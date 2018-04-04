# dcon-nashville-prenote
Song lyrics for the drupalcon nashville prenote, using [slides.js](https://github.com/hakimel/reveal.js). For complete documentation, see the slides.js github page.

## How to run the slides

To run this locally, clone it and start a webserver in the directory:

```
git clone --recursive https://github.com/ohthehugemanatee/dcon-nashville-prenote.git
cd dcon-nashville-prenote
php -S 0.0.0.0:8080
```

Then visit `http://localhost:8080/index.html`.

### How to run the slides in multiplex mode

Multiplex mode is where one "master" presenter controls everyone watching a "client" version of the presentation. You can have a whole audience watch the client version on their own devices, changing slides when the speaker chooses.

The multiplex version of the presentation is in the `multiplex` branch. Check it out with `git checkout multiplex`.

Then you need two browsers: one watching the "client" version at `index.html`, and one watching the "master" version at `index-master.html`. You can do this from the same device by following the instructions above.

But if you *really* want to impress people, you should do it from different devices.

1. Set up a temporary public URL that points to your computer. A great way is to install the free `localtunnel` program, with: `npm install -g localtunnel`.

2. Start the local web server as above, with `php -S 0.0.0.0:8080`

3. Have localtunnel assign a URL for you, with: `lt --port 8080` . It will tell you the URL to your computer.

In one browser, access `index-master.html`. This browser will be the "master". On another device, preferably in a distant country, access `index.html`. This browser will be a client. Get a bunch of friends (you have those, right?) to access it, too. The more the merrier! "access" can be from `http://localhost:8080/` on your local computer, but everyone else must use the localtunnel URL.

You will notice that the client presentations do not have navigation arrows. Navigate the presentation with the master device, and watch the clients BEND TO YOUR WILL.

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


