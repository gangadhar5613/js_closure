## Hoisting Exercises

1. If the code is `valid` what will be the output and if `invalid` what will be the error. Write the error message.

```js
console.log(animal);
var animal = "monkey";
// Output or Error Message
//undefined;
```


```js
console.log(animal);
let animal = "monkey";
// cannot access animal before initialization;
```

```js
console.log(animal);
const animal = "monkey";
// cannot access animal before initialization;
```

```js
function sayHello(msg) {
  alert(msg);
}
sayHello("Hey Everyone");
// It will alert "Hey Everyone"
```

```js
sayHello("Hey Everyone");
function sayHello(msg) {
  alert(msg);
}
// It will alert "Hey Everyone";
```

```js
sayHello("Hey Everyone");
var sayHello = msg => {
  alert(msg);
};
//  error as SayHello function is  not a function;
```

```js
sayHello("Hey Everyone");
let sayHello = msg => {
  alert(msg);
};
// error as sayHello is not a function;
```
