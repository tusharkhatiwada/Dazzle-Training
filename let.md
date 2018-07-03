# var

var has either global scope or scope inside functions

```
for(var i = 0; i<10; i++) {
  console.log(i)
}
console.log(i)
```

```
function(){
  for(var i = 0; i<10; i++) {
    console.log(i)
  }
  console.log(i)
}
```

```
function printing(){
  for(var i = 0; i<10; i++) {
    console.log(i)
  }
}
printing()
console.log(i)
```

# let

let is similar to var but let has scope. let is only accessible in the block level it is defined.

```
for(let i = 0; i<10; i++) {
  console.log(i)
}
console.log(i)
```

```
if (true) {
 let a = 40;
 console.log(a); //40
}
console.log(a); // undefined
```

In the above example variable ‘a’ is defined inside If statement and so it’s not accessible outside the function.

Another example:

```
let a = 50;
let b = 100;
if (true) {
 let a = 60;
 var c = 10;
 console.log(a/c); // 6
 console.log(b/c); // 10
}
console.log(c); // 10
console.log(a); // 50
```
