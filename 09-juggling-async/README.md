## JUGGLING ASYNC (Exercise 9 of 13)
```js
c=[],j=0,m='map';process.argv.slice(2)[m]((u,i)=>{
c[i]='';require('http').get(u,r=>
  r.on('data',r=>c[i]+=r).on('end',_=>j++&&j==3&&c[m](r=>console.log(r)))
)})
```
