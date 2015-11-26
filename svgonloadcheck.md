<h3>Check if SVG document is loaded, when embedded in html inside object tag</h3><br>
<b><mark>HTML:</mark></b>
```HTML
<object id="svgholder" data="some.svg" type="image/svg+xml" width="100%" height="100%"></object>
```
<b><mark>JS/Jquery</mark></b>
```jquery
var $svgholder =  body.find('object#svgholder'); /*some selector jquery*/
$svgholder[0].onload = function(){
				alert();
}
```
<i>OR</i>
```jquery
$svgholder.load("image/svg+xml", function() {
				alert();
});
```
