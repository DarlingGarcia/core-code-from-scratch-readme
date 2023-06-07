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

