###  <strong>Nested Rules</strong>
***
<div class="row">
<div class="column-half">
<pre>
<code>
// LESS Nesting
.grand-parent{
	background-color: pink
	.parent{
		color: black
		.child{
			font-size: 24px;
		}
	}
}

</code>
</pre>
</div>
<div class="column-half">
<pre>
<code>
// Pure CSS
.grand-parent{
	background-color: pink;
}
.grand-parent .parent{
	color: black;
}
.grand-parent .parent .child{
	font-size: 24px;
}

</code>
</pre>
</div>
</div>

<small>It is a good practice to limit nesting to maximum of 3 levels</small>
