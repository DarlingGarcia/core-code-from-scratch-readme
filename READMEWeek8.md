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
