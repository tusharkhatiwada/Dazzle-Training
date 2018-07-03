# Spread attributes

Spread attributes help to spread the expression as the name suggests. In simple words, it converts a list of elements to an array and vice versa.

**Example without spread attributes:**

```
let SumElements = (arr) => {
 console.log(arr); // [10, 20, 40, 60, 90]
 let sum = 0;
 for (let element of arr) {
  sum += element;
 }
 console.log(sum); // 220.
}
SumElements([10, 20, 40, 60, 90]);
```

Above example is straightforward. We are declaring a function to accept array as parameter and returning its sum. Its simple.

**Now consider the same example with spread attributes**

```
let SumElements = (...arr) => {
 console.log(arr); // [10, 20, 40, 60, 90]
let sum = 0;
 for (let element of arr) {
  sum += element;
 }
 console.log(sum); // 220.
}
SumElements(10, 20, 40, 60, 90); // Note we are not passing array here. Instead we are passing the elements as arguments.
```

In the above example, the spread attribute converts the list of elements (i.e) the parameters to an array.

**Another Example:**

```
Math.max(10, 20, 60, 100, 50, 200); // returns 200.
```

Math.max is a simple method that returns the maximum element from given list. It doesn’t accept an array.

```
let arr = [10, 20, 60];
Math.max(arr); // Shows error. Doesn't accept an array.
```

So lets use our savior.

```
let arr = [10, 20, 60];
Math.max(...arr); // 60
```

In the above example, the spread attribute converts the array to list of elements.
