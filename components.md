# Empire Media UI Kit

---

**Example button**

<p align="left">
  <img width="160" height="60" src="https://res.cloudinary.com/mostmojo/image/upload/v1586952100/example-btn.png">
</p>

#### HTML

`<a class="win-link" href="#link" target="_blank"><p class="win-now">EXAMPLE</p></a>`

#### CSS

```
.win-now {
	padding: 1rem 4rem;
	background-image: linear-gradient(45deg, rgb(255, 249, 181), rgb(131, 116, 0));
	border: 4px solid rgb(191, 187, 138);
	border-radius: 4px;
	text-decoration: none;
	font-size: 1.4rem;
	color: black;
}

.win-now:hover {
	transform: translateY(2px);
	animation: all 0.4s ease;
	background-image: linear-gradient(45deg, rgb(239, 233, 171), rgb(82, 73, 0));
}
```

---

**Date in `mm-dd-yyyy` format**

#### HTML

Will output:
`<p>April 16, 2020</p>`

#### JavaScript

```
<script type="text/javascript">
	const monthNames = [
		'January',
		'February',
		'March',
		'April',
		'May',
		'June',
		'July',
		'August',
		'September',
		'October',
		'November',
		'December',
	];
	let dateObj = new Date();
	let month = monthNames[dateObj.getMonth()];
	let day = String(dateObj.getDate()).padStart(2, '0');
	let year = dateObj.getFullYear();
	let output = month + '\n' + day + ', ' + year;
	document.write(output);
</script>
```
