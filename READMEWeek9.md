## "this" is a problem

```
function NameMe(first, last) {
    this.firstName = first;
    this.lastName = last;
    this.name = this.firstName + ' ' + this.lastName;
}
```

## Thinkful - List and Loop Drills: Lists of lists

```
function processData(data){
 const values = data.map(function(numbers, index) {
    const result = numbers[0] - numbers[1];
    return result;
  });

  let result = 1;
  values.forEach(function(value) {
    result = result * value;
  });

  return result;
}
```

## Stop gninnipS My sdroW!
```
function spinWords(string){
  let arr = string.split(" ")
  
  arr = arr.map((word) => {
    if(word.length >= 5){
      word = word.split('')
      word = word.reverse().join('')
    }
    return word
  })
  return arr.join(" ")
}
```

## "this" is an other problem
```
function NamedOne(first, last) {
// -- SHOULD be changed --
    Object.defineProperty(this, 'firstName', {
      set: function(newFirstName){
        first = newFirstName
        this.fullName = newFirstName + ' ' + this.lastName
      },
      get: function(){return first}
    })
  
   Object.defineProperty(this, 'lastName', {
      set: function(newLastName){
        last = newLastName
        this.fullName = this.firstName + ' ' + newLastName
      },
      get: function(){return last}
    })
  
     Object.defineProperty(this, 'fullName', {
      set: function(newFullName){
        const splitValue = newFullName.split(" ")
        if(splitValue.length > 1){
          first = splitValue[0]
          last = splitValue[1]
        }
      },
      get: function(){return this.firstName + ' ' + this.lastName}
    })  
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

## Convert string to camel case
```
function toCamelCase(myStr){
  if(myStr.length === 0){
    return ''
  }
let result =  myStr.replaceAll(/_|-/g, " ")
let arr = result.split(' ')
console.log(arr)
  
for (let i = 1; i < arr.length; i++){
  let palabra = arr[i]
  palabra = palabra.charAt(0).toUpperCase() + palabra.slice(1)
  arr[i] = palabra
}
  console.log(arr)
  return arr.join('')
}
```


## Moving Zeros To The End
```
function moveZeros(arr) {
  const zeros = arr.map((e, i) => e === 0 ? i : '').filter(x => typeof x == 'number')
  const copyArr = [...arr]
  for(let i = 0; i < zeros.length; i++){
    copyArr.splice(zeros[i] - i, 1)
  }
  
  for(let i = 0; i < zeros.length; i++){
    copyArr.push(0)
  }
  return copyArr
}
```


## Easy mathematical callback
```
function processArray(arr, callback) {
    return arr.map(cualquierCosa => callback(cualquierCosa))
}
```


## Valid Parentheses
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
    // en el momento que haya dos '(' consecutivos, ya deja de ser valido
    if(counter < 0){
      return false
    }
  }
  return counter == 0
}
```


## The Hashtag Generator
```
function generateHashtag (str) {
  str = str.trim()
  if(str.length === 0){
    return false
  }
  
  str = str.split(/\s+/)
  
  str = str.map((palabra) => palabra[0].toUpperCase() + palabra.slice(1))
  
  const result = "#" + str.join("")
  if(result.length > 140){
    return false
  }
  return result
}
```


## String incrementer
```
function findLasNumberIndex(string){
  let foundArr = string.match(/[a-z][0-9]+/gi)
  if(!foundArr){
    return 0
  }
  return string.indexOf(foundArr[foundArr.length - 1]) + 1
}

function incrementString (string) {
  let indexStarting = -1
  let regex = /[0-9]/g
  
  // si es solo un numero como '1'
  if(!isNaN(Number(string)) && string.length === 1){
    return String(Number(string) + 1)
  }
  
  // if it does not contain a number
  if(!regex.test(string)){
    return string + '1'
  }
  
  // get index of last numbers
  indexStarting = findLasNumberIndex(string)
  let alpha = string.slice(0, indexStarting)
  let numeric = string.slice(indexStarting)
  
  let leadingZero = 0
  
  for(let i = 0; i < numeric.length; i++){
    if(numeric[i] == '0'){
      leadingZero += 1
    }else{
      break
    }
  }
  
  let number = Number(numeric) + 1
  let arrNumber = String(number).split('')
  
  // if it just zeroes
  if(leadingZero === numeric.length){
    leadingZero = leadingZero -1
  }
  
  // si el numero era 99 o 999 y pasa aser 100 o 1000
  if(String(number)[String(number).length -1] == 0){
    leadingZero = leadingZero -1
  }
  for(let i = 0; i < leadingZero; i++){
    arrNumber.unshift(0)
  }

  return alpha + arrNumber.join('')
}
```
