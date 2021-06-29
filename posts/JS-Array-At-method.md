---
title: "JavaScript Array.at method"
date: "June 29, 2021"
excerpt: "We will look at new JavaScript ES6 Array method Array.at"
cover_image: "/images/posts/img1.png"
---

## The Old way of accessing elements in an array

The usual way to access an element from an array is like this

```javascript
let arr = [1, 2, 3, 4, 5];
let num = arr[1];
num; //2
```

With this method, we cannot access the elements with the negative Index like

```javascript
let arr = [1, 2, 3, 4, 5];
let num = arr[-1];
num; //undefined
```

If we try with a negative index like arr[-1] or arr[-2] it returns undefined that's where `Array.prototype.at()` method comes in.

# `Array.prototype.at()`

The at() method takes an integer value and returns the item at that index, allowing for positive and negative integers.

### Example

```javascript
let arr = [1, 2, 3, 4, 5];
let num = arr.at[-1];
num; //5
```

Before we can access the last element of the array using `arr[arr.length-1]`. But with this `array.at()` method we can access elements with a negative index easily.

```
        //0,1,2,3,4 => positive index
let arr =[1,2,3,4,5]
       //-5,-4,-3,-2,-1  => negative index
```

But there is no browser support yet for this method

![image.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1614256509760/JVq4z3p-h.png)

**Reference [MDN article](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/at) **
