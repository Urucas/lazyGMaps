lazyGMaps
==========

javascript to lazy load google maps api v3. Created to use in phonegap apps and avoid the initial overload of scripts.


Usage
=====
Instead of this
``` html
<script src="https://maps.googleapis.com/maps/api/js?v=3.exp&amp;sensor=false&amp;libraries=places"></script>
```
use this method to lazy load the google maps api only when needed
``` javascript
lazyGMaps({
  success: function() {
      // start creating your maps here
  },
  beforeLoad: function() {
    // is there something you wanna do before loading gmaps ?
    // maybe showing a dialog or spinner ?
  }
});
```
