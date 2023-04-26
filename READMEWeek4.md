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
