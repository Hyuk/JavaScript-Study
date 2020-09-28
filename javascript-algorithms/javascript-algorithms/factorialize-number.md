# Factorialize a Number

```javascript
function factorialize(num) {
  let factorialNum = 1;
  for (let i = 1; i <= num; i++){
    factorialNum *= i;
  }
  return factorialNum;
}

factorialize(5);
```