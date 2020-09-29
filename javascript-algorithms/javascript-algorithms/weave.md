# Weave

* [Source code](https://github.com/Hyuk/JavaScript-Study/blob/master/javascript-algorithms/javascript-algorithms/weave/index.js) 

* queue.js
```javascript
class Queue {
  constructor() {
    this.data = [];
  }

  add(record) {
    this.data.unshift(record);
  }

  remove() {
    return this.data.pop();
  }

  peek() {
    return this.data[this.data.length - 1];
  }
}

module.exports = Queue;
```

* weave.js
```javascript
const Queue = require('./queue');

function weave(sourceOne, sourceTwo) {
  const q = new Queue();
  while(sourceOne.peek() || sourceTwo.peek()) {
    if (sourceOne.peek()) {
      q.add(sourceOne.remove())
    }
    if(sourceTwo.peek()) {
      q.add(sourceTwo.remove())
    }
  }
  return q;
}

module.exports = weave;
```