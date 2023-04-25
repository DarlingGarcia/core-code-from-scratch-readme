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
