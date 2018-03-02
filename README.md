# Tiny CSS Modal

A featherweight (479 byte) css-only modal library based on this codepen https://codepen.io/timothylong/pen/HhAer by Timothy Long (Thanks Tim!)

Check it out here: https://void--.github.io/tiny-css-modal/

## Why?

All other modal libraries were too big or too ugly or too fancy. Can't we have a little css snippet that pops open the damn modal?

## How?

To use simply

`npm install tiny-css-modal`

add a link to the minified css

`<link rel="stylesheet" href="node_modules/tiny-css-modal/tiny-css-modal.min.css">`

add the following markup to any page where you want a modal:

```
<div id="tcm-open-modal" class="tcm-wrapper">
  <div class="tcm-content">
    <a href="#tcm-close-modal" title="Close" class="tcm-close-button">Close</a>
    <!-- Your content goes here -->
  </div>
</div>
```

and finally, add a link somewhere on the page to open the modal:

`<a href="#tcm-open-modal"><!-- Your text here --></a>`

If you can't get your jollies without using javascript you can trigger the modal by setting `location.hash` to `tcm-open-modal` and close it by setting `location.hash` to anything else.