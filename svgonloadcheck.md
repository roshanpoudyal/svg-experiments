```HTML
<h3>Check if SVG document is loaded, when embedded in html inside object tag</h3><br>
<b><mark>HTML:</mark></b>

<object id="svgholder" data="some.svg" type="image/svg+xml" width="100%" height="100%"></object>

<b><mark>JS/Jquery</mark></b>
```
```javascript
var $svgholder =  body.find('object#svgholder'); /*some selector jquery*/
$svgholder[0].onload = function(){
				alert();
}
```
```HTML
<i>OR</i>
```
```javascript
$svgholder.load("image/svg+xml", function() {
				alert();
});
```
