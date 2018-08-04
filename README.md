VerySimpleImageViewer.js
==========
[![MIT License][license-image]][license-url]

[license-image]: http://img.shields.io/badge/license-MIT-blue.svg?style=flat
[license-url]: LICENSE

### simple jquery plugin for display Images 
### Allows to zoom-in, zoom-out, and reset an image

### Version:
* 1.0.1

### Support:
* zoom-in
* zoom-out
* reset

### Demo
* See demo <a href="https://meshesha.github.io/verySimpleImageViewer/" target="_blank">here</a>.

###  usage:
 include necessary css files:
 ```
<link rel="stylesheet" href="./css/jquery.verySimpleImageViewer.css">
```
 include necessary js files:
 ```
<script type="text/javascript" src="./path/to/jquery.min.js"></script>
<script type="text/javascript" src="./js/jquery.verySimpleImageViewer.js"></script>
 ```
 html body :
 ```
 ...
   <div id="your_div_image_container"></div>
 ...
 ```
 add javascript:
 ```
<script type="text/javascript">
 var image_path = "images/img-01.jpg";
 $("#your_div_image_container").verySimpleImageViewer({
    imageSource: image_path, /*image path*/
    frame: ['100%', '100%'], /*width and height in percent or pixels*/
    maxZoom: '900%', /*max zoom in percent*/
    zoomFactor: '10%', /*zoom steps in percent*/
    saveZoomPos: true, /*true , false - enable or disable saving zoom position even after reload the page  */
    mouse: true,  /*true , false - enable or disable mouse usage*/
    keyboard: true, /*true , false - Enable or disable the use of keyboard shortcuts*/
    toolbar: true /*true , false - show or hide toolbar*/
 });
</script>
 ``` 
 keyboard shortcuts:
 ```
  "+" or "x" or "X" - zoom in
  "-" or "z" or "Z" - zoom out
  "c" or "C" - reset - center image
  "w" - move up
  "s" - move down
  "a" - move left
  "d" - move right
 ```
 
###  Changelog:
 v.1.0.1:
 - added saveZoomPos:(true/false) -  If true, this will keep the zoom position even after reloading the page (using web storage technology).
