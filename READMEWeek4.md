## Average Sales And Commission

```
Algoritmo AvgSalesAndCommission
	Imprimir "Write the total number of sales to insert: "
	Leer sales
	suma = 0
	
	Para i = 1 Hasta sales Con Paso 1 Hacer
		Imprimir "Write the value of the sale number: " + ConvertirATexto(i)
		Leer amount
		suma = suma + amount
	Fin Para
	
	Imprimir "The average sales is: " + ConvertirATexto(suma / sales)
	Si sales <= 5 Entonces
		Imprimir "The commision received is: " + ConvertirATexto(suma * 0.10)
	SiNo
		Imprimir "The commision received is: " + ConvertirATexto(suma * 0.15)
	Fin Si
FinAlgoritmo
```

## Even or odd

```
Algoritmo EvenOrOdd
	Repetir	
		Imprimir "Write a number between 1 and 50 "
		Leer number
		Si number >= 1 & number <= 50 Entonces
			// iterator value will 1 if number is odd; otherwise, it will be 2
			iteratorValue = 1
			Si number % 2 == 0 Entonces
				iteratorValue = 2
			Fin Si
			
			Para iterator = iteratorValue Hasta number Con Paso 2 Hacer
				Imprimir iterator
			Fin Para
		SiNo
			Imprimir "Invalid number"
		Fin Si
	Mientras Que ~(number >= 1 & number <= 50)
FinAlgoritmo
```
## Predefined Functions

![image](https://user-images.githubusercontent.com/128996495/234453541-5cfe211b-f975-4bda-874c-ae563b1c73d0.png)

```
Algoritmo PredefinedFunctions
	Imprimir "Absolute Value"
	Imprimir "Absolute value of -20: " + ConvertirATexto(abs(-20))
	Imprimir	""
	
	Imprimir "Truncate"
	Imprimir "Truncated value of 3.59: " + ConvertirATexto(trunc(3.59))
	Imprimir	""
	
	Imprimir "Rounding Function"
	Imprimir "Rounded value of 7.5: " + ConvertirATexto(redon(7.5))
	Imprimir	""
	
	Imprimir "Random Function"
	Imprimir "Random value between 0 and 15: " + ConvertirATexto(azar(15))
	Imprimir	""
	
	Imprimir "Length Function"
	Imprimir "Legth of the string What Happen: " + ConvertirATexto(Longitud("What Happen"))
	Imprimir	""
	
	Imprimir "Uppercase Function"
	Imprimir "String pseint converted to uppercase: " + Mayusculas("pseint")
	Imprimir	""
	
	Imprimir "Lowercase Function"
	Imprimir "String JAVASCRIPT converted to lowercase: " + Minusculas("JAVASCRIPT")
	Imprimir	""
	
	Imprimir "Substring Function"
	Imprimir "Substring of Programming: " + Subcadena("Programming", 0, 3)
	Imprimir	""
FinAlgoritmo
```

## Full Name

```
Funcion result <- Capitalize ( word )
	result = Mayusculas(Subcadena(word,0,0)) + Minusculas(Subcadena(word,1, Longitud(word) -1))
Fin Funcion

Algoritmo FullName
	Imprimir "Write a name: "
	Leer name
	Imprimir "Write a last name"
	Leer lastName
	Imprimir Capitalize(name) + " " + Capitalize(lastName)
FinAlgoritmo
```

## Throw Dice

```
Algoritmo ThrowDice
	Definir die1, die2 Como Entero
	Para i = 1 Hasta 10 Con Paso 1 Hacer
		die1 = Aleatorio(1,6)
		die2 = Aleatorio(1,6)
		Si die1 == die2 Entonces
			Imprimir die1, " ", die2, " the dice are the same"
		SiNo
			Imprimir die1, " ", die2
		Fin Si
	Fin Para
FinAlgoritmo
```

## Distance to zero

```
Algoritmo DistanceToZero
	greatestNumber = 0
	Para i = 1 Hasta 5 Con Paso 1 Hacer
		Imprimir "Write a number"
		Leer number
		number = abs(number)
		Si greatestNumber < number Entonces
			greatestNumber = number
		Fin Si
	Fin Para
	Imprimir trunc(greatestNumber)
FinAlgoritmo
```

##  Toss Coin

```
Algoritmo TossCoin
	Imprimir "Enter the name of the first player"
	Leer player1
	Imprimir "Enter the amount to play"
	Leer amount1
	Imprimir "Enter the name of the second player"
	Leer player2
	Imprimir "Enter the amount to play"
	Leer amount2
	
	result = ""
	Si amount1 <= 0 | amount2 <= 0 Entonces
		Si amount1 <= 0 & amount2 <= 0 Entonces
			result = "game canceled"
		SiNo
			Si amount1 <= 0 Entonces
				result = "player wins: " + Mayusculas(player2) + " amount won: 0"
			SiNo
				result = "player wins: " + Mayusculas(player1) + " amount won: 0"
			Fin Si	
		Fin Si
		
	SiNo
		Si Aleatorio(1,2) == 1 Entonces
			result = "player wins: " + Mayusculas(player1) + " amount won: " + ConvertirATexto(amount1)
		SiNo
			result = "player wins: " + Mayusculas(player2) + " amount won: " + ConvertirATexto(amount2)
		Fin Si
	Fin Si
	
	Imprimir result
FinAlgoritmo
```
