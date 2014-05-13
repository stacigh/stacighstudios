Helppo (that's Finnish for Easy)
===

Hi. I'm a starter theme called `Helppo`, which is based off of `underscores`. I'm a theme meant for hacking so don't use me as a Parent Theme. Instead try turning me into the next, most awesome, WordPress theme out there. That's what I'm here for.

I may have started out as another `underscores` project but I'm also packaged with `H5BP` and `Unsemantic Grid System`. My CSS stylesheet is built with SCSS so you'll need to have at least a basic understanding of how to use SASS/Compass.

* A just right amount of lean, well-commented, modern, HTML5 templates.
* A helpful 404 template.
* A sample custom header implementation in `inc/custom-header.php` that can be activated by uncommenting one line in functions.php and adding the code snippet found in the comments of `inc/custom-header.php` to your `header.php` template.
* Custom template tags in `inc/template-tags.php` that keep your templates clean and neat and prevent code duplication.
* Some small tweaks in `inc/extras.php` that can improve your theming experience.
* A script at `js/navigation.js` that makes your menu a toggled dropdown on small screens (like your phone), ready for CSS artistry. It's enqueued in `functions.php`.
* Smartly organized starter CSS in `style.scss` that will help you to quickly get your design off the ground.
* Licensed under GPLv2 or later. :) Use it to make something cool.


Getting Started
---------------

Download `Helppo` from github. The first thing you want to do is copy the `Helppo` directory and change the name to something else - Like, say, `megatherium` - then you'll need to do a five-step find and replace on the name in all the templates.

* Search for: <code>&nbsp;helppo</code> (with a space before it) and replace with: <code>&nbsp;Megatherium</code> (with a space before it)
* Search for: `Helppo` and replace with: `Megatherium`
* Search for: `helppo` and replace with: `megatherium`

Then, update the stylesheet header in style.css and the links in footer.php with your own information. 


Optional IE7 Support
---------------
Still need to support IE7? (You poor soul!) In style.scss, you'll be presented with this variable: `$legacy_support_for_ie: false;`. All you have to do is set it to `true`. Bam. Instant IE7 support.


H5BP
---------------
Love the `HTML 5 Boiler Plate`? Yeah! So do I! And, as you see, in case you still need to support IE7, I got your back. Need to support less than IE7? Ouch, bro. I can't help you out of the box but feel free to fork and modify. 


Modernizr
---------------
Modernizer's great if you still have to support legacy browsers. But almost all HTML5/CSS3 features have been implemented by modern browsers. However, there are still a handful of CSS and HTML features that are unsupported by IE9. For this reason, I'm rollin' with a custom version of Modernizr that will add support for `text-shadow`, `transition` and the `placeholder` attribute. You know... in case you absolutely have to have fallbacks for these features. Need to support less than IE9? Download a custom build of `Modernizr` and overwrite the `modernizer.custom.js` file from `/js/vendor/`

Don't know how to use Modernizr? Video: http://css-tricks.com/video-screencasts/126-using-modernizr/


Unsemantic
---------------
I'm built on Unsemantic Grid System but I've been slimmed down quite a bit (by over 1500 lines of code). Here's what's missing out of the box: IE7 support, Prefix & Suffix and Push & Pull. If you don't need to support IE7 and don't use push/pull or prefix/suffix, you won't notice a difference. However, I've come pre-packaged with some options for you in case you can't live without prefix/suffix and push/pull Unsemantic features. 

* Don't need any of these extra features? No probs. Make sure `_layout-slim.scss` is imported (section 2.0 of style.scss)
* Need to use Prefix/Suffix (white space)? Import `_layout-p2.scss`
* Need to use everything, including IE7? Import `_layout.scss` and don't forget to set `$legacy_support_for_ie` to `true`.

I come packaged with Tablet and Mobile breakpoints. Defaults:
* Mobile Max Width: 767px
* Tablet Min Width: 768px
* Tablet Max Width: 1024px
* Desktop Min Width: 1025px
* Desktop Max Width: 1200px

But these can be easily changed in the style.scss file.


Normalize
---------------
Forked version from @kristerkari; for more information: https://github.com/kristerkari/normalize.scss

I come packaged with an SCSS version of Normalize for editing ease. Program your sitewide settings in the style.scss file -- Settings like font properties, heading sizes, colors and buttons can be customized up front without hunting through the entire series of stylesheets to change settings.


Underscores
---------------
All the best stuff from Underscores has been left intact! The CSS has been cleaned up a bit but it has been pretty much left untouched.


Did I miss something?
---------------
If you've noticed something I've missed or would like to contribute to this project, feel free to branch and send me a pull request! 
