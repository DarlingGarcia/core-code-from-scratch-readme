## Which comes first, cereal or milk?
```
Algoritmo CerealWithMilkRecipe
	Escribir "Do you want your cereal with strawberries?"
	Leer cerealWithStrawberries
	Escribir "Grab a 12 oz bowl"
	Escribir "Pour milk into the bowl"
	Escribir "Add the cereal of your preference"
	Si cerealWithStrawberries == "yes" Entonces
		Escribir "Add strawberries"
		Escribir "Enjoy your bowl of cereal"
	SiNo
		Escribir "Enjoy your bowl of cereal"
	Fin Si
	
FinAlgoritmo
```
![image](https://user-images.githubusercontent.com/128996495/231322623-bfd4bc97-92a6-4630-81f9-cf673b740724.png)

### Flowchart

![image](https://user-images.githubusercontent.com/128996495/231326406-6f726492-009c-48e7-b3af-36c871032238.png)

## Logic Problem

The teacher asks his 5 students if they studied mathematics yesterday.

Alice: "Nobody studied math yesterday".
Bob: "1 person studied math yesterday".
Charlie: "2 people studied math yesterday".
Dan: "3 people studied mathematics yesterday".
Eva: "4 people studied mathematics yesterday".

The teacher knows that only those who studied would be telling the truth and those who didn't would be lying. Who is telling the truth?

If Alice is telling the truth, then she can't say that she studied since this is a contradiction.

Two statements cannot be true at the same time. For instance, "1 person studied..." and "2 people studied..." cannot possibly be true at the same time.

Therefore, the remaining solution is what Bob is telling. As he can be telling the truth, the only person that studied.

## Print My Name
```
Algoritmo myName
	Imprimir "Darling Garcia"
FinAlgoritmo
```
![image](https://user-images.githubusercontent.com/128996495/231911779-520f5ce3-199b-4251-a125-37cdafe87b22.png)

## Print My Name and Age
```
Algoritmo myNameAndAge
	Imprimir "Darling Garcia"
	Imprimir 34
FinAlgoritmo
```
![image](https://user-images.githubusercontent.com/128996495/231912223-90a0b5cb-fc9e-482e-90ef-89712ab9794f.png)

## Algorithm Game

![image](https://user-images.githubusercontent.com/128996495/231914436-34206f09-915a-4728-8e09-49ce32b66682.png)

## Mod
```
Algoritmo EvenOrOdd
	Imprimir "Insert a number"
	number = 0
	Leer number
	result = number % 2
	Imprimir result
FinAlgoritmo
```
![image](https://user-images.githubusercontent.com/128996495/231916848-f2c338f3-da15-4f4e-aa36-c32bd750e478.png)

![image](https://user-images.githubusercontent.com/128996495/231916910-7ed17a6f-a8d7-4770-94e3-c5c3f4d29ce1.png)


## Register Form
```
Algoritmo UserForm
	Imprimir "======================="
	Imprimir "User Form"
	Imprimir "First Name"
	firstName = ""
	Leer firstName
	Imprimir "Last Name"
	lastName = ""
	Leer lastName
	Imprimir "Age"
	age = ""
	Leer age
	Imprimir "Email"
	email = ""
	Leer email
	Imprimir "Address"
	address = ""
	Leer address
	
	Imprimir "======================="
	Imprimir "User Data"
	Imprimir "First Name: " + firstName
	Imprimir "Last Name: " + lastName
	Imprimir "Age: " + age
	Imprimir "Email: " + email
	Imprimir "Address: " + address
	FinAlgoritmo
```
![image](https://user-images.githubusercontent.com/128996495/231924321-05046aa0-c6aa-499c-955b-7898cab626da.png)

## Truth Tables

1. T & T = T ✅
2. T & F = F ✅
3. F & T = T ❌
4. F & F = F ✅
5. T | T = T ✅
6. T | F = F ❌
7. F | T = T ✅
8. F | F = F ✅
9. ~T = T ❌
10. ~F = T ✅
11. (T & F) | (~F) = T ✅
12. (T | F ) & (F | F) = T ❌
13. ~((T | F ) & (F | F)) & F = T ❌
14. ~((T | F ) & (F | F)) & T = F ❌

## Boolean Results

```
Algoritmo BooleanResults
	// The value for a is obtained by checking if 5 is equal to 3
	// Result: False
	a <- 5 == 3
	
	// The value for b is obtained by checking if 4 is not equal to 3
	// Result: True
	b <- 4 <> 3
	
	// The value for c is obtained by checking if 7 is greater than 7
	// Result: False
	c <- 7 > 7
	
	// The value for d is obtained by checking if 4 is less than 4
	// Result: False
	d <- 4 < 4
	
	// The value for e is obtained by checking if 100 is less than or equal to 90
	// Result: False
	e <- 100 <= 90
	
	// The value for f is obtained by checking if 40 is greater than or equal to 40
	// Result: True
	f <- 40 >= 40
FinAlgoritmo
```

## Identify odd and even numbers

```
Algoritmo OddAndEvenNumbers
	Imprimir "Insert a number: "
	Leer numero
	Si numero % 2 == 0 Entonces
		Imprimir "Number " + ConvertirATexto(numero) + " is even" 
	SiNo
		Imprimir "Number " + ConvertirATexto(numero) + " is odd" 
	Fin Si
FinAlgoritmo
```
