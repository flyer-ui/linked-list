 <div>
  <a href="https://www.npmjs.com/package/small-linked-list">
    <img src="https://img.shields.io/npm/v/small-linked-list.svg">
  </a>
  <a href="LICENSE">
    <img src="https://img.shields.io/badge/License-MIT-yellow.svg">
  </a>
</div>

## small-linked-list
A simple linked list.

### installation
```
npm i small-linked-list
```

### Usage
``` JS
const linkedList = require('../out/index').default;

const test = new linkedList.default();
test.append('lang').append('demo').append('key');
console.log(JSON.stringify(test.getHead()));
test.insert(2,"test");
console.log(JSON.stringify(test.getHead()));
test.removeAt(2);
console.log(JSON.stringify(test.getHead()));

// {"next":{"next":{"next":null,"element":"key"},"element":"demo"},"element":"lang"}
// {"next":{"next":{"next":{"next":null,"element":"key"},"element":"test"},"element":"demo"},"element":"lang"}
// {"next":{"next":{"next":null,"element":"key"},"element":"demo"},"element":"lang"}
```

### API


Name | Parameters | Description
---------|----------|---------
 append | element:any | Append elements to the linked list of instances
 insert | (position:number,element:any) | Specify a position of the insertion element
 removeAt | (position:number) | Remove an element from the specified location
 isEmpty | - | Determine if the linked list is empty
 size | - | Get the size of the linked list
 indexOf | element:any | Find the corresponding index based on the incoming elment
 

### LICENSE
MIT @ Zheng peng fei