<!--  Roadmap Of This Milestone-->

recap javascript

1. template string
2. arrow function
3. spread operator
4. array method
   1. map
   2. filter
   3. find
   4. forEach
5. json
6. data fetching
7. data

what i will learn from this module

1. component
2. how component works
3. jsx
4. how jsx works
5. how to pass data by using props
6. conditional rendering
7. hook state
   1. useState
   2. useEffict
   3. data fetching and event handle
   4. state management

<!-- 35-1 Six JavaScript Fundamentals That You Need To Know -->

1. variable
   1. let
   2. const
2. conditon
   1. if/else
   2. else if
   3. logical operator (AND , OR , NOT)
3. Array and Array method (push,pop,shift,unshift,slice,splice)
4. object (access valeu from object updata and change value in object )
5. loop (for , for of , for in , while , do while)
6. function (arguments)

<!-- 35-2 Template String, Arrow Function, Spread Operator -->

1. template string (``) : use data dynamically (${}) multiple line string
2. arrow function (=>) : it can implicite return when it is a single line function and it has no own this and we can not get arguments in arrow function and can use rest operator to get rest of the arguments
3. spread operator (...) : to use this one i can copy an array or object and if i want i can add new element with existing element

<!-- 35-3 Array Methods Map Filter Find ForEach -->

map: this method return data and create new array but main array will not upgrade it will still be same .

const result = products.map(product => console.log(product.brand))

forEach: this method do not return any thing . it just do some work . it will be used for do some work when we no need to get from it .

filter: this method return a new array when conditionally matched.

find : this method return only one single item if conditionally matched . it will return first matched element .

<!-- 35-4 Array And Object Destructuring -->

array destructuring : this technique is like access the element by a variable . it follow index number

const friends = ["Hero Alom","Hena","Bapparaj","Kabila"]

const [hero,hena,Bapparaj,Kabila] = friends;

object destructuring : this is like access the element of object like a variable . but it follow object key name .

const person = {
name: "Shaon",
age : 24,
nationality: "Bangladeshi"
}

const {name,age,nationality}= person
console.log(name,age,nationality)

<!-- 35-5 JSON, Fetch, Keys, Values, Array Add Or Remove Using Dots -->

json : when i have a normal object or data that need to send to server first i have to convert it to json format for that i have to use stringify() method

const person = {
name: "Shaon",
age : 24,
nationality: "Bangladeshi"
}

const jsonData = JSON.stringify(person)
console.log(jsonData)

if i want to use json data as normal object that i have to convert it to a normal object for that i have to use parse() method .

const jsonParse = JSON.parse(jsonData)
console.log(jsonParse)

fetch is used for client to server request

fetch("url")
.then(respose => respose.json())
.then(data => console.log)
fetch .then .then this method called chaining method
here when we used fethc then i will get a response . after response if data is available then i will get json format data after that if json data is available then i will get data as data variable.

<!-- how to get object keys ?  -->

const keys = Object.keys(objName);

<!-- how to get object values ?  -->

const values = Object.values(objName);

<!-- spread operator to copy array as new array  -->

const products = [
{ brand: "Apple", model: "iPhone 13 Pro", color: "Silver", price: 50000 },
{ brand: "Samsung", model: "S26 Ultra", color: "Black", price: 50000 },
{ brand: "Xaomi", model: "Xaomi Note 15 Pro", color: "White", price: 25000 },
{ brand: "OnePlus", model: "OnePlus 8 Pro", color: "Purple", price: 30000 },
];
const newProduct = {
brand: "Walton",
model: "Walton Phone",
color: "blue",
price: 15000,
};

const allProduct = [...products, newProduct];
console.log(allProduct)

<!-- truthy and falsy value -->
<!-- falsy -->

1. 0
2. -1
3. ""
4. null
5. false
6. undefined
7. big int

other then this all value is truthy

const value = null;
if (value) {
console.log("Truthy");
} else {
console.log("Falsy");
}

<!-- ternary operator  -->

const result = name === "Shaon" ? true:false;
console.log(result)


<!-- multiple condition in ternary operator  -->

 