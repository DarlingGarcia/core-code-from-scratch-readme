## String: substr()

```
function firstWord(word){
  word = word.trim()
  foundIndex = word.indexOf(' ')
  return word.substr(0, foundIndex)
}
```
