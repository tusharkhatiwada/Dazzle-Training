# Arrow Function

Functions in ES6 have changed a bit. I mean the syntax.

```
// Old Syntax
function oldOne() {
 console.log("Hello World..!");
}
```

```
// New Syntax
var newOne = () => {
 console.log("Hello World..!");
}
```

The new syntax may be confusing a little bit. But I will try to explain the syntax.

There are two parts of the syntax.

**var newOne = ()**

**=> {}**

The first part is just declaring a variable and assigning the function (i.e) () to it. It just says the variable is actually a function.

Then the second part is declaring the body part of the function. The arrow part with the curly braces defines the body part.

Another example with parameters.

```
let NewOneWithParameters = (a, b) => {
 console.log(a+b); // 30
}
NewOneWithParameters(10, 20);
```

I don’t think I need to give explanation for this. Its straightforward.

# Default Parameters:

If you are familiar with other programming languages like Ruby, Python then default parameters isn’t new to you.

Default parameters are parameters which are given by default while declaring a function. But it’s value can be changed when calling the function.

Example

```
let Func = (a, b = 10) => {
 return a + b;
}
Func(20); // 20 + 10 = 30
```

In the above example, we are passing only one parameter. The function makes use of the default parameter and executes the function.

Consider another example:

```
Func(20, 50); // 20 + 50 = 70
```

In the above example, the function takes two parameters and the second parameter replaces the default parameter.

Consider another example:

```
let NotWorkingFunction = (a = 10, b) => {
 return a + b;
}
NotWorkingFunction(20); // NAN. Not gonna work.
```

When you are calling the function with parameters they get assigned in the order. (i.e) the first value gets assigned to the first parameter and the second value gets assign to the second parameter and so on..

In the above example, the value 20 gets assigned to parameter ‘a’ and ‘b’ is not having any value. So we are not getting any output.

But,

```
NotWorkingFunction(20, 30); // 50;
```

Works fine.
