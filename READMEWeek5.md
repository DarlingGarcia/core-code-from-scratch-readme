## Time Coverter

```
Funcion number <- GetValidNumber (message)
	isInvalidNumber = Verdadero
	Mientras isInvalidNumber Hacer
		isDigit = Verdadero
		Escribir message
		Leer number
		Para i<-0 Hasta Longitud(number) -1 Hacer
			possibleDigit = Subcadena(number, i, i)
			Si ~(possibleDigit >= "0" & possibleDigit <= "9") Entonces
				isDigit = Falso
			Fin Si
		Fin Para
		
		Si ~isDigit Entonces
			Escribir 'ERROR: That is not a number; please try again';
            Escribir '';
		SiNo
			isInvalidNumber = Falso
		Fin Si
	Fin Mientras
Fin Funcion

Algoritmo TimeCoverter
	// 86400 is 24*60*60
	dayInSeconds = 86400
	
	// 3600 is 60*60
	hourInSeconds = 3600
	
	// 60 is 1*60
	minuteInSeconds = 60
	
	seconds = ConvertirANumero(GetValidNumber("Insert number of seconds"))
	
	days = trunc(seconds / dayInSeconds)
	seconds = seconds % dayInSeconds
	
	hours = trunc(seconds / hourInSeconds)
	seconds = seconds % hourInSeconds
	
	minutes = trunc(seconds / minuteInSeconds)
	seconds = seconds % minuteInSeconds
	
	result = "Days: " + ConvertirATexto(days) +", Hours: " + ConvertirATexto(hours) + ", Minutes: " + ConvertirATexto(minutes) + " and seconds: " + ConvertirATexto(seconds)
	Imprimir result
FinAlgoritmo

```
