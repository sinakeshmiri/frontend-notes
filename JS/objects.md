# objects in JS

```
let obj = {
	name: "sina" ,
	age: 20
};

//access it
console.log(obj.name);
console.log(obj['name']);

```

* add methods *

```
let obj = {
	name: "sina" ,
	age: 20,
	login: function(){
		console.log("hi");
	}
};

obj.login();




```

* this keyword *

contex of current object , calling it directly will show the golabal object which is window object

```
let obj = {
	name: "sina" ,
	age: 20,
	whoami: function(){
		console.log(this.name);
	}
	// you can also create methods like this
	howoldami(){
		console.log(this.name);
	}
};

obj.whoami();


```

* () => {} vs function(){} for this keyword *

if you create a method via an arrow function it wont initalize the `this` keyword
```
let obj = {
	name: "sina" ,
	age: 20 , 
	whoami: ()=>{
		console.log(this);
	}
};

obj.whoami();

//window {0: Window, window: Window, self: Window, document: document, name: '', location: Location, …}

```
* object arrays *
```
const books = [{
    name : "subtle art of not giving a fuck" , author : "mark manson"},{
    name : "unfuck your self" , author : "gary bishop"}
];

let library = {
    books : books
}

```

* math object *

```
console.log (Math.PI);

// round numbers :

let a = 1.01;

Math.round(a);
// 1
Math.random();
// outputs a random number between 0 and 1
Math.round(Math.random()*100);
// outputs a random number between 0 and 100

```
![image](https://user-images.githubusercontent.com/72389059/203903157-291fe03a-9ece-42c8-b0f0-745291d38aaa.png)

![image](https://user-images.githubusercontent.com/72389059/203904760-741f32f5-45bd-457c-936c-4f76b6e55a71.png)

