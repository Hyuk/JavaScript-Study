# General Matrix Sprial

* [Source code](https://github.com/Hyuk/JavaScript-Study/blob/master/javascript-algorithms/javascript-algorithms/matrix.md) 

```javascript
// input
matrix(2)

// ouput
[[1, 2],
[4, 3]]

// input
matrix(3)

// ouput
[[1, 2, 3],
[8, 9, 4],
[7, 6, 5]]

// input
matrix(4)

// ouput
[[1, 2, 3, 4],
[12, 13, 14, 5],
[11, 16, 15, 6],
[10, 9, 8, 7]]
```

* Must Know
```javascript
const a = [];
a[3] = 'test';
[null,null,null,'test'];
```

* Solution
```javascript
function matrix(n) {
  const results = [];

  for(let i = 0; i < n; i++) {
     results.push([]);
  }

  let counter = 1;
  let startColumn = 0;
  let endColumn = n - 1;
  let startRow = 0;
  let endRow = n - 1;
  
  while(startColumn <= endColumn && startRow <= endRow) {
    // top row
    for(i = startColumn; i <= endColumn; i++) {
      result[startRow][i] = counter;
      counter++;
    }
    startRow++;
    for(i = startRow; i<= endRow; i++) {
      result[i][endColumn] = counter;
      counter++;
    }
    endColumn--;
    for(i = endColumn; i>=startColumn; i--) {
      result[endRow][i] = counter;
      counter++
    }
    endRow--;
    for(i = endRow; i>=startRow; i--) {
      result[i][startColumn] = counter;
      counter++
    }
    startCoumn++;
  }
  
  return results;
}

matrix(n);
```