# How to compare two JSON have the same properties without order?
  
  var obj1 = { name: "Person 1", age:5 };
  var obj2 = { age:5, name: "Person 1" };

In javascript, an object is collection of various data items that can be of different types like numbers, strings, boolean, and objects itself. 

In the above two statement examples, two different objects will be created with the names of 'obj1' and 'obj2'. 

Both the objects are storing different data items, one number (age) and one string (name).

Each data item is given an identifying name as 'name' and 'age'. But they are represented in different order in comparison to one object to another.

For instance, both objects have a name, which is called the key. In obj1, name is the key, and 'Person 1' is the value stored in it. In the second object, key is name and value is the same.

Even though the order of the keys are not same, we can compare the values of the 'name' key using a dot notation, which refers to the value.

Example code:

var obj1 = { name: "Person 1", age:5 };
var obj2 = { age:5, name: "Person 1" };

if (obj1.name===obj2.name) {
  console.log ("same name in both the objects");
}
