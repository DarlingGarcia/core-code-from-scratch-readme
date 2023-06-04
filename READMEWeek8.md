## Training JS #7: if..else and ternary operator!
```
function saleHotdogs(n){
  return n >= 5 && n < 10 ? n * 95 : n >= 10 ? n * 90 : n < 5 ? n * 100 : 0
}
```

## Training JS #8: Conditional statement--switch
```
function howManydays(month){
  var days;
  switch(month){
      case 4:
        days = 30
        break;
      
      case 6:
        days = 30
        break;
      
      case 9:
        days = 30
        break;
      
      case 11:
        days = 30
        break;
      
      case 2:
        days = 28
        break;
      
      default:
        days = 31
  }
  return days;
}
```

## Basic Calculator
```
function calculate(num1, operation, num2) {
 switch(operation){
     case '+':
      return num1 + num2
     
     case '-':
      return num1 - num2
     
     case '*':
      return num1 * num2
     
     case '/':
      return num2 === 0 ? null : num1 / num2
     
      case 'm':
      return num2 === 0 ? null : num1 % num2
     
     default:
      return null
 }
}
```

## Even or odd

```
function evenOrOdd(number) {
  return number % 2 === 0 ? 'Even' : 'Odd'
}
```

## A wolf in sheep's clothing

```
function warnTheSheep(queue) {
  const revArr = queue.reverse()
  if(revArr[0] === "wolf"){
    return "Pls go away and stop eating my sheep"
  }
  return `Oi! Sheep number ${revArr.indexOf('wolf')}! You are about to be eaten by a wolf!`
}
```

## Decode the morse code

```
decodeMorse = function(morseCode){
  let input = morseCode
  input = input.trim()
  let arr = input.split("   ")
  arr = arr.map((morseWord) => {    
    morseWord = morseWord.split(' ')
    morseWord = morseWord.map((morseChar) => MORSE_CODE[morseChar])
    return morseWord.join("")
  })
  return arr.join(" ")
}
```

## Who likes it?

```
function likes(names) {
  let resultado = ""
  
  if(names.length === 0){
    resultado = "no one likes this"
  }
                     
  if(names.length === 1){
    resultado = names[0] + " likes this"
  }
  
  if(names.length === 2){
    resultado = names[0] + " and " + names[1] +" like this"
  }
  
  if(names.length === 3){
    resultado = names[0] + ", " + names[1] + " and " + names[2] + " like this"
  }
  
  if(names.length > 3){
    resultado = names[0] + ", " + names[1] + " and " + (names.length - 2) + " others like this"
  }
  return resultado
}
```

## Bit Counting

```
var countBits = function(n) {
  let contador = 0
  
  while(n > 0){
    if(n % 2 === 1){
      contador = contador + 1
    }
    n = Math.trunc(n/2)
  }
  
  return contador
}
```

## Your order, please

```
function order(words){
  let oracion = ''
  
  let array = words.split(" ")
  
  for(let iterador = 1; iterador <= array.length; iterador++){

    for(let iteradaorAnidado = 0; iteradaorAnidado < array.length; iteradaorAnidado++){
        let word = array[iteradaorAnidado]
        console.log(word)
          if(word.includes(iterador)){
            oracion += word + " "
          }
    }
  }
  
  return oracion.trim()
}
```

## Counting duplicates

```
function duplicateCount(text){
  
  let resultado = {}
  let regex = /[a-z]/i
  
  for(let iterador = 0; iterador < text.length; iterador++){
    let caracter = text.charAt(iterador)
    
    if(regex.test(caracter)){
      caracter = caracter.toLowerCase()
    }

    
    if(resultado[caracter]){
      resultado[caracter] = resultado[caracter] + 1
      
    }else{
      resultado[caracter] =  1 
    }
  }

  let valores = Object.values(resultado)
  
  valores = valores.filter( (numeroDeVeces) => numeroDeVeces >= 2)
  
  return valores.length
}
```

## Encrypt this

```
var encryptThis = function(text) {
  // Implement me! :)
  function encrypt(word){
    word = word.split('')
    
    word[0] = word[0].charCodeAt()
    
    let temp = word[1]
    word[1] = word[word.length - 1]
    word[word.length - 1 ] = temp
    
    return word.join("")
  }
  text = text.split(' ')
  if(text < 2){
    return encrypt(text[0])
  }
  text = text.map(encrypt)
  return text.join(" ")
}
```

## Valid parentheses

```
function validParentheses(parens) {
  let counter = 0
  if(parens[0] === ')'){
    return false
  }
  for(let parenthese of parens){
    if(parenthese == '('){
      counter += 1
    }else{
      counter -= 1
    }
    if(counter < 0){
      return false
    }
  }
  return counter == 0
}
```
