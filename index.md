<!DOCTYPE html>
<html>

<head>
	<meta charset="utf-8">
	<title>岩龙挺的个人网站</title>
</head>

<body>

	<p>局部变量计数。</p>
	<button type="button" onclick="myFunction()">计数!</button>
	<p id="demo">0</p>
	<script>
		var add = (function () {
			var counter = 0;
			return function () { return counter += 1; }
		})();
		function te() {
			let a = 0;
			return function () { return ++a };
		}
		let test = te();

		console.log('%c [ test ]', 'font-size:13px; background:pink; color:#bf2c9f;', test)
		function myFunction() {
			document.getElementById("demo").innerHTML = test();
		}
	</script>

</body>

</html>
