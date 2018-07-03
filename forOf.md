# For of loop

for..of is very similar to for..in with slight modification.

for..of iterates through list of elements (i.e) like Array and returns the elements (not their index) one by one.

```
let arr = [2,3,4,1];
for (let value of arr) {
 console.log(value);
}
Output:
2
3
4
1
```

Note that the variable ‘value’ outputs each element in the array not the index.

**Another Example**

```
let string = "Javascript";
for (let char of string) {
 console.log(char);
}
Output:
J
a
v
a
s
c
r
i
p
t
```

Yes. It works for string too.
