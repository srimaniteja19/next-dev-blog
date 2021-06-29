---
title: "JavaScript Some and Every methods"
date: "June 29, 2021"
excerpt: "We will look at new JavaScript ES6 Array methods some and every"
cover_image: "/images/posts/img1.png"
---

Both some and every method is used to test whether or not elements are present in the array. <br>
In this article, we are going to look at the differences between **some** and **every** method

## some()

```javascript
const words = ["cat", "be", "danger", "dog", "log", "bag", "wag"];

words.some((word) => word.length === 3); //true
```

The some() method tests whether at least one element in the array passes the test implemented by the provided function. It returns a **Boolean value**.
<br>
In the above example, the word array contains certain words. Each word has a length greater than or equal to two. In the above some() method we are checking if any word has length three or not. It returns the Boolean value **true** if any of the lengths of the words is three, otherwise, it returns **false**.

---

## every()

```javascript
const words = ["dog", "dig", "log", "bag", "wag"];
words.every((word) => word.length === 3); //true
```

The every() method tests whether all elements in the array pass the test implemented by the provided function. It returns a Boolean value.
<br>
In the above example, the word array contains certain words. Each word has a length greater than or equal to two. In the above every() method we are checking if any word has length three or not. It returns the Boolean value **true** if any of the lengths of the words is three, otherwise, it returns **false**.

**Then what is the difference between some() and every()**

```javascript
const words = ["dog", "dig", "log", "ba", "wag"];
words.every((word) => word.length === 3); //false
```

In the above example, In the above every() method we are checking if any word has length three or not. It returned false because every() method tests whether all elements in the array pass the test implemented by the provided function. It returns a Boolean value. so it returned **false**

**Thank you for reading the article**
