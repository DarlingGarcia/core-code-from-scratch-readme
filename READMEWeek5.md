## Time Converter

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
## Compare Distances

```
Funcion result <- compareDistances()
	positiveSum = 0
	negativeSum = 0
	Para i = 1 Hasta 5 Con Paso 1 Hacer
		Escribir "Write a number"
		Leer number
		Si number > 0 Entonces
			positiveSum = positiveSum + number
			
		SiNo
			negativeSum = negativeSum + number
		Fin Si
	Fin Para
	Si positiveSum > abs(negativeSum) Entonces
		result = Verdadero
	SiNo
		result = Falso	
	Fin Si
Fin Funcion


Algoritmo CompareDistancesExample
	Imprimir compareDistances()
FinAlgoritmo
```

## Sum Of Pairs

```
Funcion result <- SumOfPairs()
	result = 0
	Repetir
		Imprimir "Write a number between 1 to 100"
		Leer number
		Si number % 2 == 0 &  number > 0 & number < 101 Entonces
			result = result + number
		Fin Si
	Mientras Que number > 0 & number < 101
	Imprimir "Invalid Number"
Fin Funcion

Algoritmo SumOfPairsExample
	Imprimir SumOfPairs
FinAlgoritmo
```
## Mid Point

```
Funcion result <- MidPoint(number1, number2)
	Si number1 == number2 Entonces
		result = 0
	SiNo
		Si (number1 > 0 & number2 > 0) | (number1 < 0 & number2 < 0) Entonces
			result = (number1 + number2) / 2
		SiNo
			Si number1 > number2 Entonces
				result =(number1 + number2) / 2
			SiNo
				result =(number2 + number1) / 2
			Fin Si
		Fin Si
	Fin Si
	
Fin Funcion

Algoritmo MidPointExample
	Imprimir MidPoint(40, -80)
FinAlgoritmo
```
## Cashier

```
Funcion  Cashier()
	balance = 1000
	Repetir
		Imprimir "Select an option:"
		Imprimir "a. to deposit."
		Imprimir "b. withdraw."
		Imprimir "c. go out."
		Leer option
		Si option == "a" Entonces
			Imprimir "How much do you want to deposit?:"
			Leer amount
			balance = balance + amount
		Fin Si
		
		Si option == "b" Entonces
			Imprimir "How much do you want to withdraw?:"
			Leer amount
			balance = balance - amount
		Fin Si
		
		Si option <> "a" & option <> "b" & option <> "c" Entonces
			Imprimir "Invalid option"
		Fin Si
		Imprimir ""
	Mientras Que option <> "c"
	Imprimir balance
Fin Funcion


Algoritmo CashierExample
	Cashier()
FinAlgoritmo
```
