# Fibonacci Series - Iterative Solution

* [Source code](https://github.com/Hyuk/JavaScript-Study/blob/master/javascript-algorithms/javascript-algorithms/fibonacci-series-iterative-solution/index.js) 

```javascript
function fib(n) {
  const result = [0, 1];

  for(let i = 2; i<=n; i++) {
    const a = result[i - 1];
    const b = result[i - 2];
    result.push(a + b);
  }
  return result[n];
}
```