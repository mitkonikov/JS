# JS
Repository for all Javascripts that I've created

# Slide.it.js
Slide IT - Simple, light-weight javascript library for sliders

Here's how to implement it

### HTML
```html
<div id="sit-section">
	<div class="sit-slide sit-inactive" id="sit-slide-0"> SLIDE #1 </div>
	<div class="sit-slide sit-inactive" id="sit-slide-1"> SLIDE #2 </div>
	<div class="sit-slide sit-inactive" id="sit-slide-2"> SLIDE #3 </div>
</div>
```

! => Don't forget to get the library with the `<script>` tag

### Javascript
```javascript
$(document).slideIt();
```

To slide between slides, use the slideIt API
```javascript
$.fn.slideIt.NOW(slide1, slide2)
// ex:
$.fn.slideIt.NOW(0, 1)
// from slide 0 to slide 1
```

### (OPTIONAL) Settings
When initializing the library you can pass settings to it!
These below are the default settings
```javascript
$(document).slideIt({
	scaleDown: true,
    scaleDownFactor: 0.9,       // 0 - 1 (float range)
    scaleDownDuration: 200,     // NEEDS WORK
    translateFactor: false,     // in px
    slideWidth: 15.75,          // in em
    mainDuration: 500,
    fadeInDelay: 200,
    fadeInOut: true,
    easing: "linear"
});
```

### Dependencies
This library is depended upon jquery

### Misc
Thanks to [fullpage.js](https://raw.githubusercontent.com/alvarotrigo/fullPage.js) for the inspiration and the syntax scheme

##### Reporting problems
Please report the issues here on the GitHub page, not privatly on my email