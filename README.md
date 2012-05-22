jquery-keynav
=============

This is a [jQuery](http://www.jquery.com) plugin to enable keyboard navigation in feed-like content (j-k navigation).

* j goes down, k goes up
* user can press and hold the key to navigate further
* you can add new nodes to the keyboard navigation as you load them
* node size changes are handled gracefully


Installation
------------

### Prequisites
  * [jQuery](http://www.jquery.com/) - 1.6.0 or better

### Required files
Copy `jquery.keynav.js` to your javascript folder.

Usage
-----
### Standard call with default settings:

    $('.feeditems').keynav();

Where $('.feeditems') are all the items you want the user to navigate within.

If you're implementing infinite scroll, it's safe to reinvocate every time after you've loaded new feed items:

    $('.feeditems').keynav();

### Options
	
	$('.feeditems').keynav({
        speed: 150, //scroll animation speed
        scrolltreshold: 60, //don't animate scrolling if item is fewer than *scrolltreshold* pixels tall
        keynext: 74, // key code for next item
        keyprev: 75 // key code for previous item
	});