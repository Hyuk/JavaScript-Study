# Fibonacci Series - Recursive Solution

* [Source code](https://github.com/Hyuk/JavaScript-Study/blob/master/javascript-algorithms/javascript-algorithms/fibonacci-series-recursive-solution/index.js) 

```javascript
function fib(n) {
  if(n<2) {
    return n;
  }
  return fib(n-1) + fib(n-2);
}
```