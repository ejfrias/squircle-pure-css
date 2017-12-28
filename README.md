# squircle-pure-css
A pure CSS implementation of squircle shape

This will only work on a square shaped element (i.e. with equal height and width like 100x100)

```css
.squircle {
	background-color: #1abc9c;
	border: 0;
	border-radius: 20%;
	outline: none;
	padding: 10px;
	color: #ffffff;
	position: relative;
	width: 100px;
	height: 100px;
}

.squircle::before {
	content: ' ';
	border-radius: 2% / 50%;
	background-color: #1abc9c;
	position: absolute;
	top: 17%;
	bottom: 17%;
	right: -1.5%;
	left: -1.5%;
	z-index: -1;
}

.squircle::after {
	content: ' ';
	border-radius: 50% / 2%;
	background-color: #1abc9c;
	position: absolute;
	top: -1.5%;
	bottom: -1.5%;
	right: 17%;
	left: 17%;
	z-index: -1;
}
```
