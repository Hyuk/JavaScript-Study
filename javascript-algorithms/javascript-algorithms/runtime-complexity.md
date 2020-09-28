# Runtiem Complexity
* Constant Time - 1 - No matter how many elements we're working with, the algorithm/operation/whatever will always take the same amount of time

* Logarithmic Time - Log(n) - You have this if doubling the number of elements you are iterating over doesn't double the amount of work. Always assume that searching operations are log(n)

* Linear Time - n - Iterating through all elements in a collection of data. If you see a for loop spanning from '0' to 'array.length', you probably have 'n', or linear runtime 
  * String Reverse
  ```javascript
  // abc -> cba
  // abcdefghijklmnopqrstuvwxyz -> zyxwvutsrqponmlkjihgfedcba
  ```
  * [Fibonacci Series - Iterative Solution](https://github.com/Hyuk/JavaScript-Study/blob/master/javascript-algorithms/javascript-algorithms/fibonacci-series-iterative-solution.md)

* Quasilinear Time - n * Log(n) - You have this if doubling the number of elements you are iterating over doesn't double the amount of work. Always assume that any sorting operation is n * log(n)

* Quadratic Time - n ^ 2 - Every element in a collection has to be compared to every other element. 'The handshake problem'
  * Steps Algorithm
  ```javascript
  // steps = 2 
  // # -
  // # #
  // steps = 3
  // # - -
  // # # -
  // # # #
  // steps = 4
  // # - - -
  // # # - -
  // # # # -
  // # # # #
  ```
* Exponential Time - 2 ^ n - If you add a *single* element to a collection, the processing power required doubles
  * [Fibonacci Series - Recursive Solution](https://github.com/Hyuk/JavaScript-Study/blob/master/javascript-algorithms/javascript-algorithms/fibonacci-series-recursive-solution.md)
  
* Big 'O' Notation
  * O(n) - Linear
  * O(1) - Constant
  * O(n^2) - Quadratic

* Identifying Runtime Complexity
  * Iterating with a simple for loop through a single collection? -> Probably O(n)
  * Iterating through half a collection? -> Still O(n). There are no constants in runtime.
  * Iterating through two *different* collections with separate for loops? -> O(n + m)
  * Two nested for loops iterating over the same collection -> O(n^2)
  * Two nested for loops iterating over different collections? O(n*m)
  * Sorting? -> O(n * log(n))
  * Searching a sorted array? -> O(log(n))