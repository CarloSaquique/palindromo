# palindromo

indique si la cadena ingresada es un palíndromo.
function texto()
{
	var palabra=prompt("Ingrese una palabra para saber si es un palíndromo:").toLowerCase();
 
	palabra=palabra.replace(/ /g, "");
 
	for (var i=0;i<palabra.length;i++){
		if(palabra[i]!=palabra[palabra.length-i-1]){
			return false;
		}
	}
	return true;
}
 
if(texto())
{
	alert("Si es palíndromo.");
}else{
	alert("No es palíndromo.")
}
