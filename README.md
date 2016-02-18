# kookboekapp1
 <html>
	<head>
		<title>KookboekApp</title>
		<meta http-equiv='Content-Type' content='text/html; charset=utf-8'/>
	</head>
	<body> 
		<form onsubmit="maakRecept(); return false;">
			<fieldset>
				<legend>Vul waarden in voor het recept:
				</legend>
				<table>
				<tr>
					<td>Ingrediënt 1:</td>
					<td><input type="text" id="i1" /></td>
				</tr>
				<tr>
					<td>Ingrediënt 2:</td>
					<td><input type="text" id="i2" /></td>
				</tr>
				<tr>
					<td>Bewerking:</td>
					<td><input type="text" id="b" /></td>
				</tr>
				<tr>
					<td>Duur:</td>
					<td><input type="text" id="d" /></td>
				</tr>
				</table>
			</fieldset>
			<br/>
			<input type="submit" value="Maak recept" />
		</form>
		<p id="r"></p> Dit is de kookboekapp van Tim

		<script>
		function maakRecept() {
			
		var ingrediënt1 = document.getElementById("i1").value ;
		var ingrediënt2 = document.getElementById("i2").value ;
		var bewerking = document.getElementById("b").value ;
		var duur = document.getElementById("d").value ;
		var recept = ("Doe " + ingrediënt1 + " en " + ingrediënt2 + " samen en " + bewerking + " dit voor " + duur);
		
		document.getElementById("r").innerHTML = recept ;
		}
		</script>
	</body>
</html>
