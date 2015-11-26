<h3>Check if SVG document is loaded, when embedded in html inside object tag</h3><br>
<b><mark>HTML:</mark></b>
<code>
<object id="svgholder" data="some.svg" type="image/svg+xml" width="100%" height="100%"></object>
</code>

<b><mark>JS/Jquery</mark></b>
<code>
var $svgholder =  body.find('object#svgholder'); /*some selector jquery*/
$svgholder[0].onload = function(){
				alert();
			}
</code>
<i>OR</i>
<code>
$svgholder.load("image/svg+xml", function() {
				alert();
			});
</code>
