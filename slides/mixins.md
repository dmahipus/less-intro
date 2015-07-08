###  <strong>Mixins</strong>
***
<div class="row">
<div class="column-half">
<pre>
<code>
//Mixin Example
.bordered{
	border-top: dashed 1px red;
	background-color: yellow;
}
.box1{
	color: green;
	.bordered;
}
.box2{
	color: blue;
	.bordered;
}
</code>
</pre>
</div>
<div class="column-half">
<pre>
<code>
//Compiled CSS
.bordered{
	border-top: dashed 1px red;
	background-color: yellow;
}
.box1{
	color: green;
	border-top: dashed 1px red;
	background-color: yellow;
}
.box2{
	color: blue;
	border-top: dashed 1px red;
	background-color: yellow;
}
</code>
</pre>
</div>
</div>

<small>It is a good practice to limit nesting to maximum of 3 levels</small>
