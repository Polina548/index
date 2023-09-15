# index
lab1
<html>
<head>
<script>
function result(){
	var sum = 0;
	var N = Number(document.forms["frm"].elements["N"].value);
	var x = Number(document.forms["frm"].elements["x"].value);
	if(x>1){
		for(var n = 0; n <= N; n++){
			sum = sum + ((-1)**(n+1)/(2*n+1)*x**(2*n+1));
		}
		document.write(sum);
	} else{
		document.write("Введённое значение X не соответствует условию ")
	} }
</script>
</head>
<body>
	<form id="frm">
	<label>Введите первое число</label><br>
	<input type = "text" id = "N"><br>
	<label>Введите второе число</label><br>
	<input type = "text" id = "x"><br>
	<input type="button" onclick ="result()" value="Отправить">
</form>
</body>
</html>

