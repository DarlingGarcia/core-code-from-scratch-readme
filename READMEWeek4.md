## Even or odd

```
Algoritmo EvenOrOdd
	keepRunning = Verdadero
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
			// If it gets here, then keepRunning should be false to get out of the outer loop
			keepRunning = Falso
		SiNo
			Imprimir "Invalid number"
		Fin Si
	Mientras Que keepRunning
FinAlgoritmo
```
