# Queue

* [Source code](https://github.com/Hyuk/JavaScript-Study/blob/master/javascript-algorithms/javascript-algorithms/queue/index.js) 

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
}

module.exports = Queue;
```