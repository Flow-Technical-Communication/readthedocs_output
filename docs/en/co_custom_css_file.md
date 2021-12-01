# What is a CSS file?

The .css file defines the layout \(fonts, font size, background color, …\) of the webhelp, for example:

```
body {
	font-family: 'Montserrat,Arial,Helvetica,sans-serif';
}

.wh_logo img {
	max-width: 200px;
	padding: 0 20px 0 0;
	max-height: 75px;
}

main .uicontrol {
	color: #07AA51;
}

.title .uicontrol {
	font-weight: inherit;
}
```

**Attention:** The .css file is referenced in the template description file. When changing the name of the .css file, remember to adjust the code in the template description file.

This file is the final CSS to be applied, so it will override all other existing CSS files.

