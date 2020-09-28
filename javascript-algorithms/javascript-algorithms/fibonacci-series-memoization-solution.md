# Fibonacci Series - Memoization Solution

* [Source code](https://github.com/Hyuk/JavaScript-Study/blob/master/javascript-algorithms/javascript-algorithms/fibonacci-series-memoization-solution/index.js)

```javascript
function memoize(fn) {
  const cache = {};
  return function(...args) {
    if(cache[args]) {
      return cache[args];
    }
    const result = fn.apply(this, args);
    cache[args] = result;

    return result;
  };
}

function slowFib(n) {
  if(n<2) {
    return n;
  }
  return fib(n-1) + fib(n-2);
}

const fib = memoize(slowFib)

module.exports = fib;
```