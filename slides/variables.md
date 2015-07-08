###  <strong>Variables</strong>
***
	/* Syntax */
	@{variable name}: value;

	/* Example Declarations */
	@brand_color: orange;
	@text_color: #fff
	@link-color: #428bca;

	/* Usage */
	section{
		background-color: @brand-color;
	}
	.link:hover{
		color: @link-color;
	}
