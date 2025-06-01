# 2667. Create Hello World Function

### 🔗 LeetCode Link

[LeetCode Problem #2667 – Create Hello World Function](https://leetcode.com/problems/create-hello-world-function/)

---

## 🧠 Problem Description

Write a function `createHelloWorld`. It should return a **new function** that always returns `"Hello World"` regardless of any arguments passed to it.

---

## 🧪 Examples

### Example 1:

```js
const f = createHelloWorld();
f(); // "Hello World"
```

### Example 2:

```js
const f = createHelloWorld();
f({}, null, 42); // "Hello World"
```

---

## ✅ Constraints

* The returned function may receive **any number and type of arguments**.
* It must always return `"Hello World"`.

---

## 💡 Solution

```js
const createHelloWorld = () => {
    return function(...args) {
        return "Hello World";
    };
};
```