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
