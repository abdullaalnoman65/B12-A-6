## 1. What is the difference between var, let, and const?

- **var** → Function scoped, redeclare ও reassign করা যায় (পুরোনো JS)  
- **let** → Block scoped, redeclare করা যায় না কিন্তু reassign করা যায়  
- **const** → Block scoped, redeclare বা reassign কোনোটাই করা যায় না  


## 2. What is the difference between map(), forEach(), and filter()?

- forEach() → শুধু loop চালায়, কিছু return করে না
- map() → প্রতিটা element নিয়ে নতুন array return করে
- filter() → condition অনুযায়ী নতুন array বানায়



## 3. What are arrow functions in ES6?

Arrow functions provide a shorter and cleaner syntax for writing functions.  
They also bind `this` lexically, meaning they inherit `this` from the surrounding scope.


Benefits:
- Shorter syntax
- Lexical `this` binding
- Suitable for callbacks and functional programming

---

## 4. How does destructuring assignment work in ES6?

Destructuring allows extracting values from arrays or objects directly into variables.

```js
const numbers = [10, 20, 30];
const [x, y, z] = numbers;
console.log(x, y, z); 
const user = { name: "Noman", age: 22 };
const { name, age } = user;
console.log(name, age); 
```

---

## 5. Explain template literals in ES6. How are they different from string concatenation?

Template literals are defined using backticks (`` ` ``).  
They allow embedding variables and expressions inside a string using `${}` and support multi-line strings.

```js
const name = "Noman";
const age = 22;
const text1 = "My name is " + name + " and I am " + age + " years old.";
const text2 = `My name is ${name} and I am ${age} years old.`;
console.log(text1);
console.log(text2);
```