# JavaScript class declaration

ES6 introduced a new syntax for creating a class as shown in this example.

```
class Polygon {
   constructor(height, width) {
      this.h = height;
      this.w = width;
   }
   test() {
      console.log("The height of the polygon: ", this.h)
      console.log("The width of the polygon: ",this. w)
   }
}

//creating an instance  
var polyObj = new Polygon(10,20);
polyObj.test();
```

The Example given above declares a class ‘Polygon’. The class’s constructor takes two arguments - height and width respectively. The **this** keyword refers to the current instance of the class. In other words, the constructor above initializes two variables h and w with the parameter values passed to the constructor. The test () function in the class, prints the values of the height and width.

To make the script functional, an object of the class Polygon is created. The object is referred to by the polyObj variable. The function is then called via this object.

The following output is displayed on successful execution of the above code.

```
The height of the polygon:  10
The width of the polygon:  20
```
