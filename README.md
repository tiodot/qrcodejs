# QRCode.js
QRCode.js is javascript library for making QRCode. QRCode.js supports Cross-browser with HTML5 Canvas and table tag in DOM.
QRCode.js has no dependencies.

min.js CDN:
```
https://static.meituan.net/bs/fin-mall/latest/qrcode.min.js
```

## Basic Usages
```
<div id="qrcode"></div>
<script type="text/javascript">
var qrCode = new QRCode("http://jindo.dev.naver.com/collie");
document.getElementById("qrcode").appendChild(qrCode.getCanvas())
</script>
```

or with some options

```
<div id="qrcode"></div>
<script type="text/javascript">
var qrcode = new QRCode(document.getElementById("qrcode"), {
	text: "http://jindo.dev.naver.com/collie",
	width: 128,
	height: 128,
	colorDark : "#000000",
	colorLight : "#ffffff",
	correctLevel : QRCode.CorrectLevel.H
});
</script>
```

and you can use some methods

```
qrcode.clear(); // clear the code.
qrcode.makeCode("http://naver.com"); // make another code.
```

## Browser Compatibility
IE6~10, Chrome, Firefox, Safari, Opera, Mobile Safari, Android, Windows Mobile, ETC.

## License
MIT License

## Contact
twitter @davidshimjs

[![Bitdeli Badge](https://d2weczhvl823v0.cloudfront.net/davidshimjs/qrcodejs/trend.png)](https://bitdeli.com/free "Bitdeli Badge")
