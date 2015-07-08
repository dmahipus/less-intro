###  <strong>Parametric Mixins</strong>
***
<div class="row">
<div class="column-half">
<pre>
<code>
//Parametric Mixin Example
.circle(@size, @color){
	width: @size;
	height: @size;
	background-color: @color;
	-webkit-border-radius: (@size/2);
       -moz-border-radius: (@size/2);
		    border-radius: (@size/2);
}
.circle-small{
	.circle(24px, tomato);
}
.circle-large{
	.circle(300px, orange);
}
</code>
</pre>
</div>
<div class="column-half">
<pre>
<code>
//Compiled CSS
.circle-small{
	width: 24px;
	height: 24px;
	background-color: tomato;
	-webkit-border-radius: 12px;
       -moz-border-radius: 12px;
		    border-radius: 12px;
}
.circle-large{
	width: 300px;
	height: 300px;
	background-color: orange;
	-webkit-border-radius: 150px;
       -moz-border-radius: 150px;
		    border-radius: 150px;
}
</code>
</pre>
</div>
</div>
