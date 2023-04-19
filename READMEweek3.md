## Simple Calculator

```
Algoritmo SimpleCalculator
	Escribir "Insert the first number"
	Leer string1
	number1 = ConvertirANumero(string1)
	
	Escribir "Insert the second number"
	Leer string2
	number2 = ConvertirANumero(string2)
	
	Escribir "Choose one of the allowed operations (+, -, *, /)"
	Leer operation
	result = 0
	
	Si operation == "+" | operation == "-" | operation == "*" | operation == "/" Entonces
		Si operation == "+" Entonces
			Escribir "Processing: " + ConvertirATexto(number1) + " + " + ConvertirATexto(number2)
			result = number1 + number2
		Fin Si
		
		Si operation == "-" Entonces
			Escribir "Processing: " + ConvertirATexto(number1) + " - " + ConvertirATexto(number2)
			result = number1 - number2
		Fin Si
		
		Si operation == "*" Entonces
			Escribir "Processing: " + ConvertirATexto(number1) + " * " + ConvertirATexto(number2)
			result = number1 * number2
		Fin Si
		
		Si operation == "/" Entonces
			Escribir "Processing: " + ConvertirATexto(number1) + " / " + ConvertirATexto(number2)
			result = number1 / number2
		Fin Si
		
		Escribir "Result: " + ConvertirATexto(result)
	SiNo
		Escribir "That operation is invalid"
	Fin Si
	
FinAlgoritmo

```
![image](https://user-images.githubusercontent.com/128996495/232847057-a38b4f63-9b34-40f3-bcd9-6adee9008733.png)

## Special Number

```
Algoritmo specialNumber
	Leer n
	Si n == 100 Entonces
		Imprimir 'This is a special number'
	SiNo
		Si n < 1000 & n % 10 == 0 Entonces
			Imprimir 'This number is almost special'
		SiNo
			Imprimir 'Just a regular number'
		FinSi
	FinSi
FinAlgoritmo
```
