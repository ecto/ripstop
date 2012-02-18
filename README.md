#Ripstop

`-webkit-overflow-scrolling: touch` is awesome. Ripstop makes it more awesome.

### Before Ripstop

When pulling down or up when child is already at edge, 
the page will rip from browser chrome and reveal linen.

### After Ripstop

When pulling down or up when child is already at edge, 
the child will rip from the parent, revealing the parent.

##usage

Pull in Ripstop:

````html
<script src="/javascripts/ripstop.js"></script>
````

With pure JS:

````javascript
window.onload = function () {
  ripstop(
    document.getElementById('wrapper')
  );
}
````

With jQuery:

````javascript
$(document).ready(function(){
  $('#wrapper').ripstop();
});
````

Ripstop should be applied to a block wrapper element with one larger child.
The wrapper must have the following style:

````css
#wrapper {
  overflow: scroll;
  -webkit-overflow-scrolling: touch;
}
````

##license

(The MIT License)

Copyright (c) 2011 Cam Pedersen <cam@onswipe.com>

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the 'Software'), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED 'AS IS', WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.

