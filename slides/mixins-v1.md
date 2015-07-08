###  <strong>Cont...</strong>
***
<div class="row">
<div class="column-half">
<pre>
<code>
//Mixin Example2
\#id-mixin{
	padding: 10px 20px;
	line-height: 14px;
}
.hover-mixin(){
	border-bottom: dotted 2px orange;
}
.nav-link{
	font-size: 16px;
	.hover-mixin;
	\#id-mixin;
}
.sidebar-link{
	font-size: 24px;
	background-color: black;
	.hover-mixin;
}
</code>
</pre>
</div>
<div class="column-half">
<pre>
<code>
//Compiled CSS
\#id-mixin{
	padding: 10px 20px;
	line-height: 14px;
}
// No mixin output for .hover-mixin
.nav-link{
	font-size: 16px;
	border-bottom: dotted 2px orange;
	padding: 10px 20px;
	line-height: 14px;
}
.sidebar-link{
	font-size: 24px;
	background-color: black;
	border-bottom: dotted 2px orange;
}
</code>
</pre>
</div>
</div>
<small>Any CSS Class, ID, and Element definition can be mixed in</small>
