1- What are JavaScript Data Types?

ans- javascripts provides different data types to hold different types of values ..there are two types of data types in java script..
a)- Primitive Data types:-
string,
number,
boolean,
undefined,
null.
b)- Non-Primitive Data Types:-
Array,
objects


2- primitive and non primitive data types?

ans- primitive data type:- The predefined data types provided by JavaScript language are known as primitive data types. Primitive data types are also known as in-built data types.

non-primitive data types:-The data types that are derived from primitive data types of the JavaScript language are known as non-primitive data types. It is also known as derived data types or reference data types.


3- What is the use of isNaN function?
isNaN() method  returns true if a value is NaN.
the isNaN() method converts the value to a number before testing it..


4- What are undeclared and undefined variables?
Undeclared-->> it occurs when a variable which hasn't been declared using var, let or const is being tried to access ..

Undefined-->> it occurs when a variable has been declared using var, let or const but isn't given a value..


 5- Why JavaScript is called dynamically typed language?
JavaScript is a dynamic type language, means you don't need to specify type of the variable because it is dynamically used by JavaScript engine. You need to use var here to specify the data type. It can hold any type of values such as numbers, strings.. 
 eg- 
    var a = 40; // holding number
    var b= "bob"; // holding string..


 6- What is the differene between var and let?
    var-->>  var is function scope..
    let-->>  let is block scope..


 7- What is 'this' keyword in JavaScript?
    this-->> In JavaScript, the this keyword refers to an object.


 8-Explain the difference between "==" and "==="?
    ==>> it check only value
    ===>> it check the both value and data type..


 9- What is the significance of, and reason for, wrapping the entire content of a JavaScript source file in a function block?

ans-->> he main purpose of wrapping the entire content are:
    To avoid usage of global space.
    To avoid overriding of existing variables.
    To avoid namespace collision.
    To control visibility of member function.
    When code is wrapped inside a functional block, it reduces the collision with other libraries..



10- Discuss possible ways to write a function isInteger(x) that determines if x is an integer.
ans-->    function isInteger(x){
var is_number = typeof x == "number";
var is_not_a_float = String(x).indexOf('.') == -1;
return is_number && is_not_a_float;
}


11- Write a simple function (less than 160 characters) that returns a boolean indicating whether or not a string is a palindrome.

function isPal(str){
        let string = str.split("").reverse().join("");//split-->> divide the string in array format...
        return str.toLowerCase() === string.toLowerCase();

}
console.log(isPal("dad")); //true
console.log(isPalindrome("A car, a man, a maraca")); //true


12--What is a “closure” in JavaScript? Provide an example.
closure-->> a clsoure is an inner function that has access to the  out side function variable..
there have 3 scope--
1-local scope
2- out function variable
3- global scope

eg--

function show(){
    var j = ("it is a ou side function variable");
    console.log(j);
    function innerfun(){
        var k =("it is a inner function variable");
        console.log(k);
        console.log(j);
    }
    innerfunc();
}
show();


13-- How do you add an element at the begining of an array? How do you add one at the end?

const fruits = ["banana","grapesh","kiwi"];
fruits.unShift("watermelon");
console.log(fruits);

const fruits = ["litchi","mango","pineapple"];
fruits.push("orange");
console.log(fruits);


15-->> What is the value of typeof undefined == typeof NULL?
var myVar=null;

if(myVar === null){
    //I am null;
}

if (typeof myVar === 'undefined'){
    //myVar is undefined
}


16-- What is functional programming?
ans-->>Functional programming is a programming paradigm in which we try to bind everything in pure mathematical functions style. It is a declarative type of programming style..



17==>>What are the pros and cons of functional programming vs object-oriented programming?
ans->>> FP Pros and Cons---
+ Using clean and transparent functions leads to reliable results without side effects that deliver and return exactly what you expect.

+ It uses a more declarative style that focuses more on what needs to be done and less on how to do it, with an emphasis on efficiency and optimization.

– It is a relatively new paradigm and sometimes it is not so easy to find documentation or information compared to Object-oriented Programming.

– Sometimes it may not become illegible due to a very large number of functions compared to Object-oriented Programming.


--->>OOP Pros and Cons---

+ Objects and methods are very clear and understandable.

+ Use an imperative style, in which the code is read like a simple set of instructions, just like a computer would read it.

– May lead to unspecified and unexpected results in the sense that a parallel code that would have access to a common resource could do so in a way that produces unspecified results.

– Its methods can have side effects and may put an impact on processors.


18-->
What are two-way data binding and one-way data flow, and how are they different?

one-way data binding-->> in one-way binding the flow is one-directional..
 this means that the flow of code is from JS file to HTMl file..

 two-way data binding-->>
 -->>In a two-way binding, the flow is two-directional.
 -->>This means that the flow of code is from JS file to Html file as well as from Html file to JS  file.



19-- What is asynchronous programming, and why is it important in JavaScript?
==>Asynchronous programming makes it possible to express waiting for long-running actions without freezing the program during these actions. JavaScript environments typically implement this style of programming using callbacks, functions that are called when the actions complete
