# core-code-from-scratch-readme

## Pizza Recipe

### Ingredients
1. Water
2. Flour
3. Yeast
4. Tomato sauce
5. Salt
6. Pepperoni slices
7. Butter
8. Grated Mozarella cheese

### Steps
1. Mix dry ingredients (Flour, yeast and salt)
2. Add 1 and 1/2 cup of water
3. Mix the dough with water. After that, mix it with 1 spoon of butter
4. Knead the dough for 20 minutes and roll out the dough with a rolling pin
5. Add the tomato sauce, cheese and pepperoni slices onto dough
6. Put in a round perforated tray and bake the pizza in the oven (at 400°C)
7. Wait for 20 minutes
8. Cut the pizza with round pizza cutter
9. Serve the pizza

##  Hot N Cold

### Celsius to Fahrenheit
1. Multiply the temperature in Celsius by 9/5.
2. Add 32 to the result from step one
3. What you end up with is the temperature in Fahrenheit

### Fahrenheit to Celsius
1. Subtract 32 from the temperature in Fahrenheit
2. Multiply the result from step one by 5/9.
3. What you end up with is the temperature in Celsius

## Some Geometry

### Volume of a pyramid
1. Multiply 1/3 by base length
2. Multiply the result from step 1 by the product of the base width and the height
3. Print the result from step 2

### Volume of a cube
1. Raise any of its sides to the power of three.
2. Print the result of the step one.

### Volume of a sphere
1. Raise the sphere radius to the power of three.
2. Multiply the result from the step one by the product of PI(π) and 4/3
3. Print the result you get from step 2.

## Numbers

1. Get a number as an input
2. Check if the input is divisible by 2 with no decimal point
3. If the input is Even, then print "The numer is Even"
4. If the number is Odd, then print "The number is Odd"
5. End


![image](https://user-images.githubusercontent.com/128996495/229263249-dc9611b3-44b1-40ce-8ff0-bf78c0a15558.png)

## How old are you

1. Ask what year, month, and the day the user was born in.
2. Save the info in "birth_year," "birth_month", and "birth_day" variables respectively
3. Subtract "birth_year" from the current year. For instance, 2023-2001
4. Save the result in a variable called "year_result"
5. If today's date is behind "birth_month" and "birth_day," then subtract 1 to "year_result"
6. Print "year_result"

## Treasure

We are in a room with three chests. We know that at least one has a treasure in it. Each chest has a message, but all the messages are lies.

We're going to get the truth from each lie. Then, remove the illogical conclusions.

Left chest: The middle chest has a treasure / Truth: The middle chest doesn't have a treasure, so chest A and chest C have a treasure in them.

Middle chest: All these chests have treasures in them / Truth: All of these chests don't have a treasure, yet we know that at least one chest has a treasure in it.

Right chest: Only one of these chests has treasures / Truth: Only one of these chest doesn't have a treasure, so two chests have treasure in them.

The left and right chest tell us the same logical conclusion. However, the middle chest contradicts what we know about them.
Therefore, we can conclude that chest A and chest C have a treasure in them.

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

## Week 2 Logic Problem

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

## Week 2 Print My Name
```
Algoritmo myName
	Imprimir "Darling Garcia"
FinAlgoritmo
```
![image](https://user-images.githubusercontent.com/128996495/231911779-520f5ce3-199b-4251-a125-37cdafe87b22.png)

## Week 2 Print My Name and Age
```
Algoritmo myNameAndAge
	Imprimir "Darling Garcia"
	Imprimir 34
FinAlgoritmo
```
![image](https://user-images.githubusercontent.com/128996495/231912223-90a0b5cb-fc9e-482e-90ef-89712ab9794f.png)

## Week 2 Algorithm Game

![image](https://user-images.githubusercontent.com/128996495/231914436-34206f09-915a-4728-8e09-49ce32b66682.png)

## Week 2 Mod
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


## Week 2 Register Form
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

## Week 2 Boolean Results

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

## Week 2 Identify odd and even numbers

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
