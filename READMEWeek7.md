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

