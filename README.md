# sample
Great question 🔥
These **array methods** are **SUPER IMPORTANT** for **React**, **JavaScript**, **exams**, and **interviews**.

I’ll explain **`map`, `filter`, `find`, `includes`**
➡️ **what they do, how they work, when to use, and examples** (very simple).

---

## 📦 Sample Array (We’ll use this everywhere)

```js
const numbers = [1, 2, 3, 4, 5]
const users = [
  { id: 1, name: 'Ram', active: true },
  { id: 2, name: 'Sita', active: false },
  { id: 3, name: 'Lakshman', active: true },
]
```

---

# 🔁 1. `map()` – Transform Each Item

### 👉 What it does:

* Loops through array
* **Returns a NEW array**
* Changes each element

### 👉 When to use:

* Modify data
* Display lists in React

---

### ✅ Example 1: Double Numbers

```js
const doubled = numbers.map(num => num * 2)
console.log(doubled)
```

**Output:**

```js
[2, 4, 6, 8, 10]
```

---

### ✅ Example 2: Get User Names (React usage)

```js
const names = users.map(user => user.name)
console.log(names)
```

**Output:**

```js
['Ram', 'Sita', 'Lakshman']
```

🟢 **React Example**

```jsx
{users.map(user => (
  <p key={user.id}>{user.name}</p>
))}
```

---

# 🔍 2. `filter()` – Select Some Items

### 👉 What it does:

* Loops through array
* Returns **only matching items**
* Returns a **NEW array**

### 👉 When to use:

* Search
* Remove items
* Show active users

---

### ✅ Example 1: Even Numbers

```js
const evens = numbers.filter(num => num % 2 === 0)
console.log(evens)
```

**Output:**

```js
[2, 4]
```

---

### ✅ Example 2: Active Users

```js
const activeUsers = users.filter(user => user.active)
console.log(activeUsers)
```

**Output:**

```js
[
  { id: 1, name: 'Ram', active: true },
  { id: 3, name: 'Lakshman', active: true }
]
```

---

# 🎯 3. `find()` – Get ONE Item

### 👉 What it does:

* Finds **first matching item**
* Returns **one object/value**
* If not found → `undefined`

### 👉 When to use:

* Get user by ID
* Edit form
* Details page

---

### ✅ Example: Find User by ID

```js
const user = users.find(user => user.id === 2)
console.log(user)
```

**Output:**

```js
{ id: 2, name: 'Sita', active: false }
```

⚠️ Difference:

* `filter()` → returns array
* `find()` → returns single object

---

# 🔎 4. `includes()` – Check if Value Exists

### 👉 What it does:

* Checks if value exists in array
* Returns `true` or `false`

### 👉 When to use:

* Validation
* Permissions
* Search

---

### ✅ Example 1: Number Exists?

```js
console.log(numbers.includes(3)) // true
console.log(numbers.includes(10)) // false
```

---

### ✅ Example 2: Role Check

```js
const roles = ['admin', 'user']

if (roles.includes('admin')) {
  console.log('Access granted')
}
```

---

# 🧠 Summary Table (VERY IMPORTANT)

| Method       | Returns             | Use                   |
| ------------ | ------------------- | --------------------- |
| `map()`      | New array           | Transform data        |
| `filter()`   | New array           | Select multiple items |
| `find()`     | Single value/object | Get one item          |
| `includes()` | Boolean             | Check existence       |

---

# ❌ Common Mistakes

❌ Using `map()` instead of `filter()`
❌ Expecting array from `find()`
❌ Forgetting `return` inside `{}`

---

# 📝 Exam Answer (Short & Perfect)

> `map()` is used to transform array elements.
> `filter()` is used to select elements based on condition.
> `find()` returns the first matching element.
> `includes()` checks whether a value exists in an array.

---

## 🔥 Want Next?

I can explain:
1️⃣ `reduce()` (most confusing but powerful)
2️⃣ Array methods in **real React project**
3️⃣ `map + filter` combined
4️⃣ Interview questions on array methods
5️⃣ Practice questions with answers

Just tell me 👇
