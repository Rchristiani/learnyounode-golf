## FILTERED LS (Exercise 5 of 13)
```js
a=process.argv;require('fs')
  .readdir(a[2],(_,f)=>f.map(f=>RegExp('.'+a[3]).test(f)&&console.log(f)))
```
