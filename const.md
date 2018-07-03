# const

Const is used to assign a constant value to the variable. And the value cannot be changed. Its fixed.

```
const a = 50;
a = 60; // shows error. You cannot change the value of const.
```

```
const LANGUAGES = ['Js', 'Ruby', 'Python', 'Go'];
LANGUAGES = "Javascript"; // shows error.
LANGUAGES.push('Java'); // Works fine.
console.log(LANGUAGES); // ['Js', 'Ruby', 'Python', 'Go', 'Java']
```

Consider in this way. Whenever you define a const variable, Javascript references the address of the value to the variable. In our example the **variable ‘LANGUAGES’ actually references to the memory allocated to the array**. So you **cannot change the variable to reference some other memory location later**. Throughout the program it only references to the array.
