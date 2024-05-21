## **ES6-note**
---
### **1.變量聲明**
- let 和 const
- let 用於聲明變量，有塊級作用域（block scope）。
- const 用於聲明常量，也有塊級作用域，且值不能重新賦值。

```javascript
let a = 10;
const b = 20;
a = 30; // 合法
// b = 40; // 非法，會拋出錯誤
```

### **3. 箭頭函數**
簡化函數的語法，並且不綁定自己的 this。

```javascript
// 傳統函數
function add(x, y) {
    return x + y;
}

// 箭頭函數
const add = (x, y) => x + y;
```
### **4. 模板字面量**
使用反引號（`）定義字符串，支持嵌入表達式和多行字符串。
```js
const name = 'John';
const greeting = `Hello, ${name}!`; // Hello, John!
```
### **5. 解構賦值**
從數組或對象中提取值，並賦值給變量。

**數組解構**
```js
const arr = [1, 2, 3];
const [a, b, c] = arr;
```
```js
const obj = { name: 'John', age: 30 };
const { name, age } = obj;
```
### **6. 擴展運算符和剩餘運算符**
**擴展運算符**
```js
const arr1 = [1, 2, 3];
const arr2 = [...arr1, 4, 5]; // [1, 2, 3, 4, 5]
```
**剩餘運算符**
```js
function sum(...args) {
    return args.reduce((acc, val) => acc + val, 0);
}
```





