# 📑 Study Notes: ES6 Features in JavaScript (Part I)

### 🌟 Why ES6 Matters

- Released in **2015**, also called **ECMAScript 2015**.
- Solved long-standing problems with `var`.
- Improved **readability, maintainability, and scalability** of JavaScript.
- Introduced new syntax and features → cleaner, more powerful code.

---

### 🔑 Key Features Covered

#### 1️⃣ `let` & `const`

- **Problem with `var`**
    - Function-scoped, not block-scoped.
    - Variables can "leak" outside blocks.
    
```js
function testVar() {
   if (true) {
		var name = "Alice";
	}
	console.log(name); // 😲 Accessible outside block 
}
```
    
- **Solution: `let` and `const`**
    - `let` → block-scoped, can be reassigned.
    - `const` → block-scoped, **cannot be reassigned**.
    
```js
{
	let greeting = "hello";
	console.log(greeting); // "hello" 
} 
console.log(greeting); // ReferenceError  
const PI = 3.14; 
PI = 3.14159; // ❌ TypeError
```

⚠️ Note: `const` prevents **reassignment**, but objects/arrays declared with `const` can still be **mutated**.

---

#### 2️⃣ Arrow Functions

- Shorter syntax for writing functions.
- Automatically bind `this` (no need for `.bind()`).

```js
let numbers = [1, 2, 3];
let doubled = numbers.map(n => n * 2); 
console.log(doubled); // [2, 4, 6]
```

- Example conversion:

```js
// Traditional 
function greet(name) {
   return "Hello, " + name;
}  // Arrow 
const greet = name => `Hello, ${name}`;

```
---

#### 3️⃣ Template Literals

- Use **backticks** (`` ` ``).
- Allow **string interpolation** with `${}`.
- Support **multi-line strings** easily.

```js
let user = "John"; 
let age = 30;
console.log(`Hi, I’m ${user} and I’m ${age} years old.`);
```
💡 Example:

```js
let city = "Chennai"; 
let temp = 32;
console.log(`The temperature in ${city} is ${temp}°C.`);
```

---

#### 4️⃣ Destructuring

- Extract values from **arrays** or **objects** into variables directly.

```js
const user = { name: "Alice", age: 22 }; 
const { name, age } = user; 
console.log(name); // "Alice"
 console.log(age);  // 22
```

- With arrays:

```js
const [a, b] = [10, 20]; 
console.log(a, b); // 10 20
```

---

### 💡 Bonus Tips

- `const` does **not** mean immutable object.

```js
const person = { name: "Sam" }; 
person.name = "Sara"; // ✅ Allowed (object mutated)
```

---

### 📌 Summary / Key Takeaways

- Use `let` (reassignable, block-scoped) and `const` (non-reassignable, block-scoped).
- Use **arrow functions** for concise syntax & better `this` handling.
- Use **template literals** for string interpolation & multi-line strings.
- Use **destructuring** for quick data extraction from arrays/objects.
- ES6 makes code **cleaner, safer, and easier to read**.

---

# 📝 Cheat Sheet: ES6 Features (Part I)

- **`let` vs `const` vs `var`**
    
    - `var` → function-scoped ❌ (avoid)
    - `let` → block-scoped, reassignable
    - `const` → block-scoped, not reassignable (but objects/arrays mutable)
    
- **Arrow Functions**
    
```js
const greet = name => `Hello, ${name}`;
```
    
    - Short syntax, auto `this` binding.
    
- **Template Literals**
    
```js
`My name is ${user}, I’m ${age} years old.` 
```
    - String interpolation + multi-line support.
        
- **Destructuring**
    
```js
const {name, age} = user; 
const [a, b] = [10, 20];
```
    

✅ Use ES6 for **cleaner, modern, bug-free JS**.