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
## Simple calculator with Switch

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
	Segun operation Hacer
		"+":
			Escribir "Processing: " + ConvertirATexto(number1) + " + " + ConvertirATexto(number2)
			Escribir "Result: " + ConvertirATexto(number1 + number2)
		"-":
			Escribir "Processing: " + ConvertirATexto(number1) + " - " + ConvertirATexto(number2)
			Escribir "Result: " + ConvertirATexto(number1 - number2)
		"*":
			Escribir "Processing: " + ConvertirATexto(number1) + " * " + ConvertirATexto(number2)
			Escribir "Result: " + ConvertirATexto(number1 * number2)
		"/":
			Escribir "Processing: " + ConvertirATexto(number1) + " / " + ConvertirATexto(number2)
			Escribir "Result: " + ConvertirATexto(number1 / number2)
		De Otro Modo:
			Escribir "That operation is invalid"
	Fin Segun
FinAlgoritmo
```

## Multi Option Program

```
Algoritmo MultiOptionProgram
	Imprimir "========Choose an option========"
	Imprimir "1. Sum two numbers"
	Imprimir "2. Print the day of the week given the day number"
	Imprimir "3. Print the length of a given text"
	Leer option 
	
	Segun option Hacer
		1:
			Imprimir "Option #1 Sum two numbers"
			Imprimir "Insert the first number"
			Leer number1
			Imprimir "Insert the second number"
			Leer number2
			Imprimir "Result: " + ConvertirATexto(number1 + number2)
		2:
			Imprimir "Option #2 Print the day of the week given the day number"
			Imprimir "Insert a day number (1 - 7)"
			Leer number
			Segun number Hacer
				"1":
					Imprimir "Monday"
				"2":
					Imprimir "Tuesday"
				"3":
					Imprimir "Wednesday"
				"4":
					Imprimir "Thursday"
				"5":
					Imprimir "Friday"
				"6":
					Imprimir "Saturday"
				"7":
					Imprimir "Sunday"
				De Otro Modo:
					Imprimir "That is not a day number"
			Fin Segun
		3:
			Imprimir "Option #3 Print the length of a given text"
			Imprimir "Insert a text"
			Leer text
			Imprimir "Result: " + ConvertirATexto(Longitud(text))
		De Otro Modo:
			Imprimir "Option not available"
	Fin Segun
FinAlgoritmo
```

## Multiplication Tables

```
Algoritmo MultiplicationTables
	Imprimir "=============Multiplication Tables================="
	Imprimir "Enter a number"
	Leer number 
	counter <- 1
	Mientras counter <= 10 Hacer
		Imprimir number + " * " + ConvertirATexto(counter) + " = " + ConvertirATexto(ConvertirANumero(number) * counter)
		counter <- counter + 1
	Fin Mientras
FinAlgoritmo
```
