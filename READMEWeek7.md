## String: substr()

```
function firstWord(word){
  word = word.trim()
  foundIndex = word.indexOf(' ')
  return word.substr(0, foundIndex)
}
```

## String: replace()

```
function normalize(date){
  return date.replaceAll('-', '/')
}
```

## Increment

```
let x = 3;
x++;
x = x * 2;
x--;

The solution is 7
```

## Fahrenheit

```
function toFahrenheit(celsius){
  return (celsius * 9/5) + 32
}
```

## Boolean

```
function nand(bool1, bool2){
  return !(bool1 && bool2)
}
```

## Objects

```
function animal(obj){
  return "This " + obj.color + " " + obj.name + " has " + obj.legs + " legs."
}
```

## Return to sanity

```
function mystery() {
  var results = {sanity: 'Hello'};
  return results;
}
```

## Object syntax debug

```
var rooms = {
  first: {
    description: 'This is the first room',
    items: {
      chair: 'The old chair looks comfortable',
      lamp: 'This lamp looks ancient'
    }
  },
  second: {
    description: 'This is the second room',
    items: {
      couch: 'This couch looks like it would hurt your back',
      table: 'On the table there is an unopened bottle of water'
    }
  }
}
```

## Count strings in objects

```
function strCount(arr){
  let count = 0
  if(!Array.isArray(arr)){
    arr = Object.values(arr)
  }
  
  for(let i = 0; i < arr.length; i++){
    if(typeof arr[i] === "string"){
      ++count
    } else if(typeof arr[i] === "object" && arr[i] !== null){
      count += strCount(arr[i])
    }
  }
  return count
}
```

## Extending JavaScript Objects: Get First & Last Array Element
```
// Write your code here...
Array.prototype.first = function (){
  return this[0]
}

Array.prototype.last = function(){
  return this[this.length -1]
}
```

##  Object Oriented Piracy

```
function Ship(draft,crew) {
 this.draft = draft;
 this.crew = crew;
 this.isWorthIt = () => {
   if(this.draft - (this.crew * 1.5) > 20){
     return true
   }else{
     return false
   }
 }
}
```

## Convert a String to a Number

```
const stringToNumber = function(str){
  return Number(str);
}
```

## Convert number to reversed array of digits

```
function digitize(n) {
  //convert to a string
  let myString = String(n)
  
  //convert string to an array of numbers
  let arr = myString.split("").map((elem) => Number(elem))
      
  //call array.reverse()
  arr = arr.reverse()
  
  //return arr
  return arr
}
```

## Truthy and Falsy

```
const truthy = [1,2,3,4,"2"];
const falsy = [0,false,null,undefined,""];
```

## Training JS #4: Basic data types--Array

```
function getLength(arr){
  //return length of arr
  return arr.length
}
function getFirst(arr){
  //return the first element of arr
  return arr[0]
}
function getLast(arr){
  //return the last element of arr
  return arr[arr.length - 1]
}
function pushElement(arr){
  var el=1;
  //push el to arr
  arr.push(el)
  return arr
}
function popElement(arr){
  //pop an element from arr
  arr.pop()
  return arr
}
```
