# Complete Interview Preparation Roadmap
## From Zero to Hero: Full Stack Developer Journey

---

## 📋 Table of Contents

### **Phase 1: Job Switch Sprint (2-3 Months)**
1. [Raw JavaScript Fundamentals](#chapter-1-raw-javascript-fundamentals)
2. [Pattern-Based DSA in JavaScript](#chapter-2-pattern-based-dsa-in-javascript)
3. [React.js Deep Dive](#chapter-3-reactjs-deep-dive)
4. [Next.js Mastery](#chapter-4-nextjs-mastery)
5. [Node.js & Backend Essentials](#chapter-5-nodejs--backend-essentials)
6. [System Design Basics](#chapter-6-system-design-basics-for-interviews)
7. [Behavioral Interview Prep](#chapter-7-behavioral-interview--resume-stories)
8. [GitHub Profile & Portfolio](#chapter-8-github-profile--portfolio-cleanup)

### **Phase 2: FAANG/Big Tech Preparation (6-9 Months)**
9. [Java Fundamentals & OOP](#chapter-9-java-fundamentals--oop)
10. [Spring Boot & Microservices](#chapter-10-spring-boot--microservices)
11. [Advanced DSA & Competitive Programming](#chapter-11-advanced-dsa--competitive-programming)
12. [Low Level Design (LLD)](#chapter-12-low-level-design-lld)
13. [Advanced System Design](#chapter-13-advanced-system-design)

### **Appendix**
- [Week-by-Week Schedule](#week-by-week-schedule)
- [Resources & Practice Platforms](#resources--practice-platforms)
- [Interview Checklist](#final-interview-checklist)

---

## 🎯 Your Context & Goals

### Who You Are
- **Name:** Pavan S J
- **Experience:** 4+ years as Full Stack Developer
- **Tech Stack:** Next.js, React.js, Node.js, GraphQL, REST APIs, MongoDB, AWS
- **Current Reality:** Can build projects with AI/Google support but cannot write code from scratch on paper/notepad
- **JavaScript Knowledge:** React + Hooks + basic Node, but NOT core raw JavaScript
- **DSA/LLD Experience:** Absolute zero

### What You're Targeting

**Phase 1 Goals (2-3 months):**
- Target Companies: Razorpay, Groww, Zepto, Juspay, Postman, Urban Company, Swiggy, Ola, PhonePe
- Target Roles: Full Stack Developer (React + Node) OR Frontend Engineer (React/Next.js)
- Salary Range: 16-25 LPA (realistic step-up from current position)

**Phase 2 Goals (6-9 months after Phase 1):**
- Target Companies: FAANG, Big4, Top Product Companies (Google, Amazon, Microsoft, Meta, Netflix, Uber, Airbnb)
- Target Roles: Senior Software Engineer, Staff Engineer
- Tech Stack Addition: Java + Spring Boot + Advanced DSA + LLD + System Design

### The Strategy
- **NO Java in Phase 1** — use JavaScript for everything (DSA, projects, interviews)
- **Pattern-based learning** — recognize problem types, apply templates
- **Honest positioning** — no lies about Spring Boot, focus on MERN strength
- **GitHub showcase** — make your profile interview-ready
- **Phase 1 → Job Switch → Phase 2** — checkpoint approach, not all-or-nothing

---

## ⏱️ Timeline Overview

### Phase 1: 10-12 Weeks Total

| Week | Focus Area | Hours/Week |
|------|------------|------------|
| 1-2 | Raw JavaScript Fundamentals | 20-25 |
| 3-10 | Pattern-Based DSA (Core Focus) | 25-30 |
| 3-10 | React/Next.js Deep Dive (Parallel) | 10-15 |
| 8-10 | Node.js Backend Strengthening | 10-15 |
| 9-10 | System Design Basics | 10-12 |
| 10-11 | Behavioral Prep + Resume Stories | 8-10 |
| 11-12 | GitHub Cleanup + Mock Interviews | 10-15 |

**Total Time Commitment:** 25-35 hours/week (including weekends)

### Phase 2: 24-36 Weeks (Post Job Switch)

| Month | Focus Area |
|-------|------------|
| 1-2 | Java Fundamentals + OOP |
| 2-3 | Spring Boot Basics + REST APIs |
| 3-4 | Advanced DSA in Java |
| 4-5 | Low Level Design (LLD) |
| 5-6 | Advanced System Design |
| 6+ | Mock Interviews + Company-specific prep |

---

# PHASE 1: JOB SWITCH SPRINT (2-3 MONTHS)

---


## Chapter 1: Raw JavaScript Fundamentals

**Duration:** 2 Weeks (Week 1-2)  
**Goal:** Build the foundation needed for DSA problem-solving in JavaScript  
**Daily Time:** 3-4 hours

### Why This Chapter Matters for You
You know React + Hooks, which means you already understand:
- Functions (components are functions)
- Arrays and objects (props, state)
- Callbacks (event handlers, useEffect)

**What you're missing:** Using these in raw problem-solving context without React framework. This chapter bridges that gap.

---

### Week 1: Core Building Blocks

#### Day 1-2: Variables, Data Types & Operators

**Topics to Cover:**
```javascript
// 1. Variable Declarations (let, const, var differences)
let count = 0;           // can reassign
const name = "Pavan";    // cannot reassign
var old = "avoid";       // function-scoped, avoid in modern JS

// 2. Primitive Data Types
let num = 42;                    // Number
let str = "Hello";               // String
let bool = true;                 // Boolean
let nothing = null;              // Null
let notDefined = undefined;      // Undefined
let id = Symbol("id");           // Symbol (rarely needed for DSA)
let bigNum = 123456789n;         // BigInt

// 3. Type Checking
console.log(typeof num);         // "number"
console.log(typeof str);         // "string"

// 4. Type Coercion (IMPORTANT for interviews)
console.log("5" + 3);            // "53" (string concatenation)
console.log("5" - 3);            // 2 (numeric operation)
console.log(true + 1);           // 2
console.log(false + 1);          // 1

// 5. Operators
// Arithmetic: +, -, *, /, %, **
// Comparison: ==, ===, !=, !==, <, >, <=, >=
// Logical: &&, ||, !
// Ternary: condition ? true : false

// 6. Important Gotchas
console.log(0.1 + 0.2 === 0.3);  // false (floating point issue)
console.log(NaN === NaN);         // false (NaN is not equal to itself)
console.log(null == undefined);   // true (loose equality)
console.log(null === undefined);  // false (strict equality)
```

**Practice Problems (Day 1-2):**
1. Write a function to swap two numbers without a temp variable
2. Check if a number is even/odd
3. Find the larger of two numbers
4. Convert Celsius to Fahrenheit
5. Calculate simple interest

---

#### Day 3-4: Strings & String Methods

**Topics to Cover:**
```javascript
// 1. String Creation
let str1 = "Hello";              // double quotes
let str2 = 'World';              // single quotes
let str3 = `Hello ${name}`;      // template literals (backticks)

// 2. String Properties
str1.length                      // 5

// 3. Essential String Methods (MUST KNOW FOR DSA)
str1.charAt(0)                   // "H"
str1.charCodeAt(0)               // 72 (ASCII code)
str1.indexOf("l")                // 2 (first occurrence)
str1.lastIndexOf("l")            // 3
str1.includes("ell")             // true
str1.substring(1, 4)             // "ell" (start, end - exclusive)
str1.slice(1, 4)                 // "ell" (works with negative indices)
str1.slice(-3)                   // "llo"
str1.toUpperCase()               // "HELLO"
str1.toLowerCase()               // "hello"
str1.trim()                      // removes whitespace from both ends
str1.split("")                   // ["H", "e", "l", "l", "o"]
str1.replace("l", "L")           // "HeLlo" (only first match)
str1.replaceAll("l", "L")        // "HeLLo"

// 4. String Concatenation
let full = str1 + " " + str2;    // "Hello World"
let full2 = `${str1} ${str2}`;   // "Hello World" (preferred)

// 5. String to Array and Back
let arr = str1.split("");        // ["H", "e", "l", "l", "o"]
let back = arr.join("");         // "Hello"

// 6. Important for DSA
// Strings are IMMUTABLE in JavaScript
str1[0] = "h";                   // Won't change the string
// To modify, convert to array, modify, then join back
```

**Practice Problems (Day 3-4):**
1. Reverse a string
2. Check if a string is a palindrome
3. Count vowels in a string
4. Check if two strings are anagrams
5. Find the first non-repeating character in a string
6. Convert "hello world" to "Hello World" (title case)

---

#### Day 5-7: Arrays & Array Methods

**Topics to Cover:**
```javascript
// 1. Array Creation
let arr1 = [1, 2, 3, 4, 5];
let arr2 = new Array(5);         // [empty × 5]
let arr3 = Array(5).fill(0);     // [0, 0, 0, 0, 0]

// 2. Accessing Elements
arr1[0]                          // 1
arr1[arr1.length - 1]            // 5 (last element)
arr1.at(-1)                      // 5 (modern way to get last element)

// 3. CRITICAL Array Methods for DSA

// Adding/Removing Elements
arr1.push(6)                     // adds to end, returns new length
arr1.pop()                       // removes from end, returns removed element
arr1.unshift(0)                  // adds to beginning, returns new length
arr1.shift()                     // removes from beginning, returns removed element

// Searching
arr1.indexOf(3)                  // 2 (first index, -1 if not found)
arr1.lastIndexOf(3)              // 2
arr1.includes(3)                 // true
arr1.find(x => x > 2)            // 3 (first element matching condition)
arr1.findIndex(x => x > 2)       // 2 (index of first match)

// Iteration Methods (MASTER THESE)
arr1.forEach((val, idx, arr) => {})      // no return value
arr1.map(x => x * 2)                     // [2, 4, 6, 8, 10]
arr1.filter(x => x % 2 === 0)            // [2, 4]
arr1.reduce((acc, val) => acc + val, 0)  // 15 (sum)
arr1.some(x => x > 3)                    // true (at least one matches)
arr1.every(x => x > 0)                   // true (all match)

// Slicing/Splicing
arr1.slice(1, 3)                 // [2, 3] (doesn't modify original)
arr1.splice(1, 2)                // removes 2 elements from index 1
arr1.splice(1, 0, 10, 20)        // inserts 10, 20 at index 1

// Sorting
arr1.sort()                      // sorts as strings! [1, 10, 2, 3]
arr1.sort((a, b) => a - b)       // ascending [1, 2, 3, 10]
arr1.sort((a, b) => b - a)       // descending [10, 3, 2, 1]

// Reversing
arr1.reverse()                   // modifies in place

// Joining
arr1.join(", ")                  // "1, 2, 3, 4, 5"

// Flattening
let nested = [1, [2, [3, 4]]];
nested.flat(2)                   // [1, 2, 3, 4]

// Creating ranges
Array.from({length: 5}, (_, i) => i)     // [0, 1, 2, 3, 4]
[...Array(5)].map((_, i) => i)           // [0, 1, 2, 3, 4]

// Copying arrays
let copy1 = [...arr1]            // spread operator
let copy2 = arr1.slice()         // slice without arguments
let copy3 = Array.from(arr1)     // Array.from
```

**Practice Problems (Day 5-7):**
1. Find the second largest element in an array
2. Remove duplicates from an array
3. Rotate an array by k positions
4. Find missing number in array [1, 2, 3, ..., n]
5. Move all zeros to the end
6. Find the intersection of two arrays
7. Merge two sorted arrays
8. Find pair with given sum (Two Sum - Easy)

---

### Week 2: Functions, Objects & Control Flow

#### Day 8-9: Functions

**Topics to Cover:**
```javascript
// 1. Function Declaration
function add(a, b) {
    return a + b;
}

// 2. Function Expression
const subtract = function(a, b) {
    return a - b;
};

// 3. Arrow Functions (MOST USED IN MODERN JS)
const multiply = (a, b) => a * b;              // implicit return
const divide = (a, b) => {                     // explicit return
    return a / b;
};
const square = x => x * x;                     // single param, no parens
const greet = () => console.log("Hello");      // no params

// 4. Default Parameters
function power(base, exp = 2) {
    return base ** exp;
}
power(5)        // 25
power(5, 3)     // 125

// 5. Rest Parameters
function sum(...numbers) {
    return numbers.reduce((acc, num) => acc + num, 0);
}
sum(1, 2, 3, 4, 5)  // 15

// 6. Scope & Closures (IMPORTANT)
function outer() {
    let count = 0;
    return function inner() {
        count++;
        return count;
    };
}
const counter = outer();
console.log(counter());  // 1
console.log(counter());  // 2

// 7. Recursion Basics
function factorial(n) {
    if (n <= 1) return 1;           // base case
    return n * factorial(n - 1);    // recursive case
}

// 8. Higher-Order Functions
// Functions that take functions as arguments or return functions
function applyOperation(arr, operation) {
    return arr.map(operation);
}
applyOperation([1, 2, 3], x => x * 2);  // [2, 4, 6]
```

**Practice Problems (Day 8-9):**
1. Write a function to check if a number is prime
2. Calculate Fibonacci using recursion
3. Implement a counter using closure
4. Write a function to flatten nested arrays
5. Implement a custom map function
6. Calculate power using recursion
7. Check if a string has balanced parentheses (recursion)

---

#### Day 10-11: Objects & Maps

**Topics to Cover:**
```javascript
// 1. Object Creation
let person = {
    name: "Pavan",
    age: 27,
    skills: ["React", "Node", "JS"]
};

// 2. Accessing Properties
person.name              // "Pavan" (dot notation)
person["age"]            // 27 (bracket notation)
let key = "skills";
person[key]              // ["React", "Node", "JS"]

// 3. Adding/Modifying Properties
person.city = "Bangalore";
person.age = 28;

// 4. Deleting Properties
delete person.age;

// 5. Checking Properties
"name" in person         // true
person.hasOwnProperty("name")  // true

// 6. Object Methods
Object.keys(person)      // ["name", "skills", "city"]
Object.values(person)    // ["Pavan", ["React", "Node", "JS"], "Bangalore"]
Object.entries(person)   // [["name", "Pavan"], ...]

// 7. Object Destructuring
let {name, skills} = person;
let {name: fullName} = person;  // rename

// 8. Spread Operator
let newPerson = {...person, age: 27};

// 9. Map (Better than Object for DSA)
let map = new Map();
map.set("key1", "value1");
map.set(1, "one");
map.get("key1")          // "value1"
map.has("key1")          // true
map.delete("key1")
map.size                 // 1
map.clear()

// Iterating Map
for (let [key, value] of map) {
    console.log(key, value);
}

// 10. Set (For unique values)
let set = new Set([1, 2, 3, 2, 1]);
console.log(set);        // Set {1, 2, 3}
set.add(4);
set.has(2);              // true
set.delete(2);
set.size;                // 3

// Converting between Set and Array
let arr = [...set];
let newSet = new Set(arr);
```

**Practice Problems (Day 10-11):**
1. Count frequency of each character in a string (use Map)
2. Find the first unique character in a string
3. Group anagrams together
4. Check if two objects are equal (deep comparison)
5. Find common elements in two arrays (use Set)
6. Remove duplicates maintaining order (use Set)
7. Implement a phone book (use Map)

---

#### Day 12-14: Control Flow & Loops

**Topics to Cover:**
```javascript
// 1. If-Else
if (condition) {
    // code
} else if (anotherCondition) {
    // code
} else {
    // code
}

// 2. Switch
switch (value) {
    case 1:
        console.log("One");
        break;
    case 2:
        console.log("Two");
        break;
    default:
        console.log("Other");
}

// 3. For Loop
for (let i = 0; i < 5; i++) {
    console.log(i);
}

// 4. While Loop
let i = 0;
while (i < 5) {
    console.log(i);
    i++;
}

// 5. Do-While Loop
let j = 0;
do {
    console.log(j);
    j++;
} while (j < 5);

// 6. For...of (Arrays, Strings, Sets, Maps)
for (let item of [1, 2, 3]) {
    console.log(item);
}

// 7. For...in (Objects)
for (let key in person) {
    console.log(key, person[key]);
}

// 8. Break & Continue
for (let i = 0; i < 10; i++) {
    if (i === 5) break;      // exit loop
    if (i % 2 === 0) continue;  // skip iteration
    console.log(i);
}

// 9. Nested Loops (VERY COMMON IN DSA)
for (let i = 0; i < 3; i++) {
    for (let j = 0; j < 3; j++) {
        console.log(i, j);
    }
}

// 10. Loop Patterns for DSA
// Pattern 1: Two pointers
let left = 0, right = arr.length - 1;
while (left < right) {
    // process
    left++;
    right--;
}

// Pattern 2: Sliding window
for (let i = 0; i < arr.length - k + 1; i++) {
    let sum = 0;
    for (let j = i; j < i + k; j++) {
        sum += arr[j];
    }
}
```

**Practice Problems (Day 12-14):**
1. Print patterns:
   ```
   *
   **
   ***
   ****
   *****
   ```
2. FizzBuzz (1 to 100, print Fizz for multiples of 3, Buzz for 5, FizzBuzz for both)
3. Find all prime numbers up to n (Sieve of Eratosthenes)
4. Print multiplication table
5. Reverse each word in a sentence
6. Find all divisors of a number
7. Check if array is sorted

---

### Week 2 Final Days: ES6+ Features

**Topics to Cover:**
```javascript
// 1. Destructuring
let [a, b, ...rest] = [1, 2, 3, 4, 5];  // a=1, b=2, rest=[3,4,5]
let {name, age} = person;

// 2. Spread Operator
let arr1 = [1, 2, 3];
let arr2 = [...arr1, 4, 5];     // [1, 2, 3, 4, 5]
let obj1 = {a: 1, b: 2};
let obj2 = {...obj1, c: 3};     // {a: 1, b: 2, c: 3}

// 3. Template Literals
let name = "Pavan";
let msg = `Hello ${name}!`;

// 4. Optional Chaining
let user = {profile: {name: "Pavan"}};
user?.profile?.name              // "Pavan"
user?.address?.city              // undefined (no error)

// 5. Nullish Coalescing
let value = null;
let result = value ?? "default";  // "default"
// Different from ||: 0 ?? "default" gives 0, not "default"

// 6. Array/Object Methods
// Already covered in previous sections

// 7. Math Object (USEFUL FOR DSA)
Math.max(1, 2, 3)                // 3
Math.min(1, 2, 3)                // 1
Math.floor(4.7)                  // 4
Math.ceil(4.3)                   // 5
Math.round(4.5)                  // 5
Math.abs(-5)                     // 5
Math.pow(2, 3)                   // 8
Math.sqrt(16)                    // 4
Math.random()                    // random between 0 and 1

// Random integer between min and max
function randomInt(min, max) {
    return Math.floor(Math.random() * (max - min + 1)) + min;
}
```

---

### End of Week 2: Mini Assessment

**Complete these problems on paper/notepad (no AI/Google):**

1. **String Manipulation:** Given a string, return it reversed with vowels capitalized
2. **Array Problem:** Find the missing number in [1, 2, ..., n] with one missing
3. **Object Problem:** Given array of objects `[{name: "A", age: 25}, {name: "B", age: 30}]`, return object with max age
4. **Frequency Counter:** Count frequency of each element in an array
5. **Two Pointer:** Check if a string is a palindrome (ignore spaces and case)
6. **Recursion:** Calculate sum of digits of a number recursively
7. **Map Usage:** Find first non-repeating character in a string
8. **Nested Loops:** Print all pairs from an array

**Pass Criteria:** Solve 6/8 problems within 90 minutes without help.  
**If you pass:** Move to Chapter 2 (DSA)  
**If not:** Spend 2 more days reviewing weak areas, then retry

---

### Week 2 Summary: What You Should Be Comfortable With

✅ Variables, data types, type coercion  
✅ All string methods (split, slice, substring, indexOf, includes, etc.)  
✅ All array methods (map, filter, reduce, sort, forEach, etc.)  
✅ Writing functions (arrow, regular, recursive)  
✅ Objects and Maps (CRUD operations)  
✅ Loops (for, while, for...of, nested loops)  
✅ Control flow (if-else, switch)  
✅ ES6+ syntax (destructuring, spread, template literals)  

**YOU ARE NOW READY FOR DSA!**

---


## Chapter 2: Pattern-Based DSA in JavaScript

**Duration:** 6-8 Weeks (Week 3-10)  
**Goal:** Master interview DSA patterns, not competitive programming  
**Daily Time:** 3-4 hours  
**Total Problems to Solve:** 150-200 (quality over quantity)

### The Pattern-Based Approach (Why This Works)

**Traditional DSA learning:** Learn every algorithm → try random problems → get stuck → give up  
**Pattern-based learning:** Learn problem patterns → recognize patterns → apply templates → solve faster

**You will learn 15 core patterns that cover 80% of interview questions.**

---

### Pattern Learning Framework

**For Each Pattern:**
1. **Understand the concept** (15-20 min theory)
2. **Learn the template code** (30 min, write it 3 times)
3. **Solve 8-12 problems** (Easy → Medium progression)
4. **Identify pattern triggers** (how to recognize this pattern in new problems)

---

### Week 3-4: Foundation Patterns



#### Pattern 1: Arrays & Hashing (3 days)

**When to use:** Counting, frequency, lookup, duplicates, grouping

**Core Techniques:**
```javascript
// Technique 1: Frequency Counter
function frequencyCounter(arr) {
    const freq = new Map();
    for (let num of arr) {
        freq.set(num, (freq.get(num) || 0) + 1);
    }
    return freq;
}

// Technique 2: Two Pass Method
function twoPass(arr) {
    // First pass: collect information
    const info = {};
    for (let item of arr) {
        // process
    }
    // Second pass: use information
    for (let item of arr) {
        // process with info
    }
}

// Technique 3: Array as Hash (when values are small integers)
function arrayAsHash(arr) {
    const hash = new Array(1001).fill(0);  // if values 0-1000
    for (let num of arr) {
        hash[num]++;
    }
}
```

**Must-Solve Problems:**
1. ✅ Two Sum (LeetCode 1) - CRITICAL
2. ✅ Contains Duplicate (LeetCode 217)
3. ✅ Valid Anagram (LeetCode 242)
4. ✅ Group Anagrams (LeetCode 49)
5. ✅ Top K Frequent Elements (LeetCode 347)
6. ✅ Product of Array Except Self (LeetCode 238)
7. ✅ Longest Consecutive Sequence (LeetCode 128)
8. First Missing Positive (LeetCode 41)
9. Subarray Sum Equals K (LeetCode 560)
10. 4Sum (LeetCode 18)

**Pattern Recognition Triggers:**
- "Find duplicates" → Use Set or Map
- "Count frequency" → Use Map
- "Group by property" → Use Map with arrays
- "Find pair/sum" → Use Set while iterating



#### Pattern 2: Two Pointers (3 days)

**When to use:** Sorted arrays, palindromes, pairs, reversing

**Core Template:**
```javascript
// Template 1: Opposite Direction (most common)
function twoPointersOpposite(arr) {
    let left = 0;
    let right = arr.length - 1;
    
    while (left < right) {
        // check condition
        if (condition) {
            // process
            left++;
            right--;
        } else if (anotherCondition) {
            left++;
        } else {
            right--;
        }
    }
}

// Template 2: Same Direction (slow-fast)
function twoPointersSame(arr) {
    let slow = 0;
    
    for (let fast = 0; fast < arr.length; fast++) {
        if (condition) {
            // process
            slow++;
        }
    }
    return slow;
}

// Template 3: Fast & Slow (Cycle Detection)
function fastSlowPointer(head) {
    let slow = head;
    let fast = head;
    
    while (fast && fast.next) {
        slow = slow.next;
        fast = fast.next.next;
        if (slow === fast) return true;  // cycle found
    }
    return false;
}
```

**Must-Solve Problems:**
1. ✅ Valid Palindrome (LeetCode 125)
2. ✅ Two Sum II - Sorted (LeetCode 167)
3. ✅ 3Sum (LeetCode 15) - CRITICAL
4. ✅ Container With Most Water (LeetCode 11)
5. ✅ Remove Duplicates from Sorted Array (LeetCode 26)
6. ✅ Move Zeroes (LeetCode 283)
7. Trapping Rain Water (LeetCode 42)
8. Sort Colors (LeetCode 75)
9. Linked List Cycle (LeetCode 141)
10. Remove Nth Node From End (LeetCode 19)

**Pattern Recognition Triggers:**
- "Sorted array" → Two pointers
- "Palindrome" → Two pointers from ends
- "Remove duplicates in place" → Slow-fast pointers
- "Find pair/triplet" → Two/three pointers
- "Detect cycle" → Fast-slow pointers



#### Pattern 3: Sliding Window (4 days)

**When to use:** Subarray/substring problems, contiguous elements, "window of size k"

**Core Template:**
```javascript
// Template 1: Fixed Window Size
function fixedWindow(arr, k) {
    let windowSum = 0;
    
    // Build first window
    for (let i = 0; i < k; i++) {
        windowSum += arr[i];
    }
    
    let maxSum = windowSum;
    
    // Slide the window
    for (let i = k; i < arr.length; i++) {
        windowSum += arr[i] - arr[i - k];  // add new, remove old
        maxSum = Math.max(maxSum, windowSum);
    }
    
    return maxSum;
}

// Template 2: Dynamic Window Size (most common in interviews)
function dynamicWindow(arr) {
    let left = 0;
    let result = 0;
    let windowState = {};  // track window state
    
    for (let right = 0; right < arr.length; right++) {
        // Expand window: add arr[right]
        // Update window state
        
        // Shrink window if invalid
        while (windowIsInvalid) {
            // Remove arr[left]
            // Update window state
            left++;
        }
        
        // Update result with valid window
        result = Math.max(result, right - left + 1);
    }
    
    return result;
}

// Template 3: At Most K pattern
function atMostK(arr, k) {
    let left = 0, count = 0;
    let map = new Map();
    
    for (let right = 0; right < arr.length; right++) {
        map.set(arr[right], (map.get(arr[right]) || 0) + 1);
        
        while (map.size > k) {
            map.set(arr[left], map.get(arr[left]) - 1);
            if (map.get(arr[left]) === 0) map.delete(arr[left]);
            left++;
        }
        
        count += right - left + 1;
    }
    return count;
}
```

**Must-Solve Problems:**
1. ✅ Max Sum Subarray of Size K (GFG)
2. ✅ Longest Substring Without Repeating Characters (LeetCode 3) - CRITICAL
3. ✅ Minimum Window Substring (LeetCode 76) - HARD but important
4. ✅ Longest Repeating Character Replacement (LeetCode 424)
5. ✅ Permutation in String (LeetCode 567)
6. ✅ Find All Anagrams in String (LeetCode 438)
7. Max Consecutive Ones III (LeetCode 1004)
8. Longest Substring with At Most K Distinct Characters (LeetCode 340)
9. Fruit Into Baskets (LeetCode 904)
10. Subarrays with K Different Integers (LeetCode 992)

**Pattern Recognition Triggers:**
- "Subarray/substring" → Sliding window
- "Contiguous elements" → Sliding window
- "Window of size K" → Fixed sliding window
- "Longest/shortest substring with condition" → Dynamic window
- "At most K distinct" → Shrinking window



#### Pattern 4: String Manipulation (2 days)

**When to use:** String problems, palindromes, pattern matching

**Core Techniques:**
```javascript
// Technique 1: Character Array Manipulation
function manipulateString(s) {
    const arr = s.split('');
    // modify array
    return arr.join('');
}

// Technique 2: Two Pointer on String
function isPalindrome(s) {
    let left = 0, right = s.length - 1;
    while (left < right) {
        if (s[left] !== s[right]) return false;
        left++;
        right--;
    }
    return true;
}

// Technique 3: Character Frequency
function anagram(s, t) {
    if (s.length !== t.length) return false;
    const freq = {};
    for (let char of s) freq[char] = (freq[char] || 0) + 1;
    for (let char of t) {
        if (!freq[char]) return false;
        freq[char]--;
    }
    return true;
}
```

**Must-Solve Problems:**
1. ✅ Reverse String (LeetCode 344)
2. ✅ Valid Palindrome (LeetCode 125)
3. ✅ Longest Palindromic Substring (LeetCode 5)
4. ✅ Longest Common Prefix (LeetCode 14)
5. Valid Parentheses (LeetCode 20)
6. Implement strStr() (LeetCode 28)
7. String to Integer (atoi) (LeetCode 8)
8. Zigzag Conversion (LeetCode 6)

---

### Week 5-6: Intermediate Patterns



#### Pattern 5: Stack (3 days)

**When to use:** Parentheses, next greater/smaller, monotonic sequences, DFS

**Core Template:**
```javascript
// Template 1: Basic Stack Operations
const stack = [];
stack.push(item);      // add
stack.pop();           // remove and return
stack[stack.length-1]; // peek

// Template 2: Matching Parentheses
function isValid(s) {
    const stack = [];
    const pairs = {')': '(', '}': '{', ']': '['};
    
    for (let char of s) {
        if (char === '(' || char === '{' || char === '[') {
            stack.push(char);
        } else {
            if (stack.length === 0 || stack.pop() !== pairs[char]) {
                return false;
            }
        }
    }
    return stack.length === 0;
}

// Template 3: Monotonic Stack (Next Greater Element)
function nextGreaterElement(nums) {
    const result = new Array(nums.length).fill(-1);
    const stack = [];  // store indices
    
    for (let i = 0; i < nums.length; i++) {
        while (stack.length > 0 && nums[i] > nums[stack[stack.length-1]]) {
            const idx = stack.pop();
            result[idx] = nums[i];
        }
        stack.push(i);
    }
    return result;
}

// Template 4: Min Stack
class MinStack {
    constructor() {
        this.stack = [];
        this.minStack = [];
    }
    
    push(val) {
        this.stack.push(val);
        const min = this.minStack.length === 0 ? val : 
                    Math.min(val, this.minStack[this.minStack.length-1]);
        this.minStack.push(min);
    }
    
    pop() {
        this.stack.pop();
        this.minStack.pop();
    }
    
    top() {
        return this.stack[this.stack.length-1];
    }
    
    getMin() {
        return this.minStack[this.minStack.length-1];
    }
}
```

**Must-Solve Problems:**
1. ✅ Valid Parentheses (LeetCode 20) - CRITICAL
2. ✅ Min Stack (LeetCode 155)
3. ✅ Evaluate Reverse Polish Notation (LeetCode 150)
4. ✅ Daily Temperatures (LeetCode 739)
5. ✅ Next Greater Element I (LeetCode 496)
6. ✅ Largest Rectangle in Histogram (LeetCode 84) - HARD
7. Simplify Path (LeetCode 71)
8. Remove K Digits (LeetCode 402)
9. Decode String (LeetCode 394)
10. Asteroid Collision (LeetCode 735)

**Pattern Recognition Triggers:**
- "Valid parentheses/brackets" → Stack
- "Next greater/smaller element" → Monotonic stack
- "Min/max in O(1)" → Min/Max stack
- "Evaluate expression" → Stack
- "Nested structure" → Stack



#### Pattern 6: Binary Search (4 days)

**When to use:** Sorted array, find element, search space reduction, "find minimum/maximum that satisfies"

**Core Template:**
```javascript
// Template 1: Classic Binary Search
function binarySearch(arr, target) {
    let left = 0, right = arr.length - 1;
    
    while (left <= right) {
        const mid = Math.floor(left + (right - left) / 2);
        
        if (arr[mid] === target) {
            return mid;
        } else if (arr[mid] < target) {
            left = mid + 1;
        } else {
            right = mid - 1;
        }
    }
    return -1;
}

// Template 2: Find First/Last Occurrence
function findFirst(arr, target) {
    let left = 0, right = arr.length - 1;
    let result = -1;
    
    while (left <= right) {
        const mid = Math.floor(left + (right - left) / 2);
        
        if (arr[mid] === target) {
            result = mid;
            right = mid - 1;  // continue searching left
        } else if (arr[mid] < target) {
            left = mid + 1;
        } else {
            right = mid - 1;
        }
    }
    return result;
}

// Template 3: Search Space Binary Search (ADVANCED)
function searchSpace(arr, condition) {
    let left = minPossibleAnswer;
    let right = maxPossibleAnswer;
    
    while (left < right) {
        const mid = Math.floor(left + (right - left) / 2);
        
        if (isPossible(mid)) {
            right = mid;  // try smaller
        } else {
            left = mid + 1;  // need larger
        }
    }
    return left;
}

// Template 4: Rotated Array Search
function searchRotated(nums, target) {
    let left = 0, right = nums.length - 1;
    
    while (left <= right) {
        const mid = Math.floor(left + (right - left) / 2);
        
        if (nums[mid] === target) return mid;
        
        // Determine which half is sorted
        if (nums[left] <= nums[mid]) {  // left half sorted
            if (target >= nums[left] && target < nums[mid]) {
                right = mid - 1;
            } else {
                left = mid + 1;
            }
        } else {  // right half sorted
            if (target > nums[mid] && target <= nums[right]) {
                left = mid + 1;
            } else {
                right = mid - 1;
            }
        }
    }
    return -1;
}
```

**Must-Solve Problems:**
1. ✅ Binary Search (LeetCode 704)
2. ✅ Search Insert Position (LeetCode 35)
3. ✅ Find First and Last Position (LeetCode 34)
4. ✅ Search in Rotated Sorted Array (LeetCode 33) - CRITICAL
5. ✅ Find Minimum in Rotated Sorted Array (LeetCode 153)
6. ✅ Koko Eating Bananas (LeetCode 875)
7. Find Peak Element (LeetCode 162)
8. Search a 2D Matrix (LeetCode 74)
9. Median of Two Sorted Arrays (LeetCode 4) - HARD
10. Aggressive Cows (GFG/Codeforces)

**Pattern Recognition Triggers:**
- "Sorted array" → Binary search
- "Find in O(log n)" → Binary search
- "Rotated sorted array" → Modified binary search
- "Find minimum/maximum that satisfies condition" → Binary search on answer
- "Allocate/distribute with constraints" → Binary search



#### Pattern 7: Linked Lists (3 days)

**When to use:** Linked list problems (obviously), in-place operations, cycle detection

**Core Operations:**
```javascript
// Node Definition
class ListNode {
    constructor(val = 0, next = null) {
        this.val = val;
        this.next = next;
    }
}

// Template 1: Reverse Linked List (MUST MEMORIZE)
function reverseList(head) {
    let prev = null;
    let curr = head;
    
    while (curr) {
        const next = curr.next;  // save next
        curr.next = prev;        // reverse link
        prev = curr;             // move prev
        curr = next;             // move curr
    }
    return prev;
}

// Template 2: Fast & Slow Pointers
function middleNode(head) {
    let slow = head;
    let fast = head;
    
    while (fast && fast.next) {
        slow = slow.next;
        fast = fast.next.next;
    }
    return slow;
}

// Template 3: Merge Two Lists
function mergeTwoLists(l1, l2) {
    const dummy = new ListNode(0);
    let current = dummy;
    
    while (l1 && l2) {
        if (l1.val < l2.val) {
            current.next = l1;
            l1 = l1.next;
        } else {
            current.next = l2;
            l2 = l2.next;
        }
        current = current.next;
    }
    
    current.next = l1 || l2;
    return dummy.next;
}

// Template 4: Remove Nodes
function removeElements(head, val) {
    const dummy = new ListNode(0);
    dummy.next = head;
    let current = dummy;
    
    while (current.next) {
        if (current.next.val === val) {
            current.next = current.next.next;
        } else {
            current = current.next;
        }
    }
    return dummy.next;
}
```

**Must-Solve Problems:**
1. ✅ Reverse Linked List (LeetCode 206) - CRITICAL, MUST MEMORIZE
2. ✅ Merge Two Sorted Lists (LeetCode 21)
3. ✅ Linked List Cycle (LeetCode 141)
4. ✅ Remove Nth Node From End (LeetCode 19)
5. ✅ Middle of Linked List (LeetCode 876)
6. ✅ Palindrome Linked List (LeetCode 234)
7. Intersection of Two Linked Lists (LeetCode 160)
8. Remove Duplicates from Sorted List (LeetCode 83)
9. Add Two Numbers (LeetCode 2)
10. Copy List with Random Pointer (LeetCode 138)

**Pattern Recognition Triggers:**
- "Reverse" → Iterative reversal template
- "Middle/cycle" → Fast-slow pointers
- "Merge" → Dummy node + two pointers
- "Remove nodes" → Dummy node
- "In-place" → Pointer manipulation

---

### Week 7-8: Advanced Patterns



#### Pattern 8: Trees (Binary Trees) (5 days)

**When to use:** Tree traversal, paths, depth, structure manipulation

**Core Templates:**
```javascript
// Tree Node Definition
class TreeNode {
    constructor(val = 0, left = null, right = null) {
        this.val = val;
        this.left = left;
        this.right = right;
    }
}

// Template 1: DFS Traversals (MUST MEMORIZE ALL THREE)
// Inorder: Left -> Root -> Right
function inorder(root) {
    if (!root) return [];
    return [...inorder(root.left), root.val, ...inorder(root.right)];
}

// Preorder: Root -> Left -> Right
function preorder(root) {
    if (!root) return [];
    return [root.val, ...preorder(root.left), ...preorder(root.right)];
}

// Postorder: Left -> Right -> Root
function postorder(root) {
    if (!root) return [];
    return [...postorder(root.left), ...postorder(root.right), root.val];
}

// Template 2: BFS (Level Order Traversal)
function levelOrder(root) {
    if (!root) return [];
    const result = [];
    const queue = [root];
    
    while (queue.length > 0) {
        const levelSize = queue.length;
        const level = [];
        
        for (let i = 0; i < levelSize; i++) {
            const node = queue.shift();
            level.push(node.val);
            if (node.left) queue.push(node.left);
            if (node.right) queue.push(node.right);
        }
        result.push(level);
    }
    return result;
}

// Template 3: Height/Depth
function maxDepth(root) {
    if (!root) return 0;
    return 1 + Math.max(maxDepth(root.left), maxDepth(root.right));
}

// Template 4: Path Sum
function hasPathSum(root, targetSum) {
    if (!root) return false;
    if (!root.left && !root.right) return root.val === targetSum;
    
    return hasPathSum(root.left, targetSum - root.val) ||
           hasPathSum(root.right, targetSum - root.val);
}

// Template 5: Validate BST
function isValidBST(root, min = -Infinity, max = Infinity) {
    if (!root) return true;
    if (root.val <= min || root.val >= max) return false;
    
    return isValidBST(root.left, min, root.val) &&
           isValidBST(root.right, root.val, max);
}
```

**Must-Solve Problems:**
1. ✅ Maximum Depth of Binary Tree (LeetCode 104)
2. ✅ Invert Binary Tree (LeetCode 226)
3. ✅ Symmetric Tree (LeetCode 101)
4. ✅ Binary Tree Level Order Traversal (LeetCode 102) - CRITICAL
5. ✅ Diameter of Binary Tree (LeetCode 543)
6. ✅ Path Sum (LeetCode 112)
7. ✅ Lowest Common Ancestor (LeetCode 236)
8. ✅ Validate Binary Search Tree (LeetCode 98)
9. Binary Tree Right Side View (LeetCode 199)
10. Construct Binary Tree from Preorder and Inorder (LeetCode 105)
11. Serialize and Deserialize Binary Tree (LeetCode 297)
12. Kth Smallest Element in BST (LeetCode 230)

**Pattern Recognition Triggers:**
- "Tree traversal" → DFS (inorder/preorder/postorder) or BFS
- "Level-wise" → BFS/Level order
- "Path sum/root to leaf" → DFS with sum tracking
- "BST" → Inorder gives sorted order
- "Lowest common ancestor" → Recursive search
- "Height/depth" → Recursive max depth



#### Pattern 9: Backtracking (4 days)

**When to use:** Generate all possibilities, permutations, combinations, subsets, constraint satisfaction

**Core Template:**
```javascript
// Template 1: Subsets/Combinations (Choose or Not Choose)
function subsets(nums) {
    const result = [];
    
    function backtrack(index, current) {
        // Base case
        if (index === nums.length) {
            result.push([...current]);
            return;
        }
        
        // Choose current element
        current.push(nums[index]);
        backtrack(index + 1, current);
        current.pop();  // backtrack
        
        // Don't choose current element
        backtrack(index + 1, current);
    }
    
    backtrack(0, []);
    return result;
}

// Template 2: Permutations
function permute(nums) {
    const result = [];
    
    function backtrack(current, remaining) {
        if (remaining.length === 0) {
            result.push([...current]);
            return;
        }
        
        for (let i = 0; i < remaining.length; i++) {
            current.push(remaining[i]);
            const newRemaining = [...remaining.slice(0, i), ...remaining.slice(i + 1)];
            backtrack(current, newRemaining);
            current.pop();  // backtrack
        }
    }
    
    backtrack([], nums);
    return result;
}

// Template 3: Combination Sum (can reuse elements)
function combinationSum(candidates, target) {
    const result = [];
    
    function backtrack(start, current, sum) {
        if (sum === target) {
            result.push([...current]);
            return;
        }
        if (sum > target) return;
        
        for (let i = start; i < candidates.length; i++) {
            current.push(candidates[i]);
            backtrack(i, current, sum + candidates[i]);  // i, not i+1 (can reuse)
            current.pop();
        }
    }
    
    backtrack(0, [], 0);
    return result;
}

// Template 4: N-Queens (Constraint Satisfaction)
function solveNQueens(n) {
    const result = [];
    const board = Array(n).fill(null).map(() => Array(n).fill('.'));
    
    function isValid(row, col) {
        // Check column
        for (let i = 0; i < row; i++) {
            if (board[i][col] === 'Q') return false;
        }
        // Check diagonal
        for (let i = row - 1, j = col - 1; i >= 0 && j >= 0; i--, j--) {
            if (board[i][j] === 'Q') return false;
        }
        for (let i = row - 1, j = col + 1; i >= 0 && j < n; i--, j++) {
            if (board[i][j] === 'Q') return false;
        }
        return true;
    }
    
    function backtrack(row) {
        if (row === n) {
            result.push(board.map(r => r.join('')));
            return;
        }
        
        for (let col = 0; col < n; col++) {
            if (isValid(row, col)) {
                board[row][col] = 'Q';
                backtrack(row + 1);
                board[row][col] = '.';  // backtrack
            }
        }
    }
    
    backtrack(0);
    return result;
}
```

**Must-Solve Problems:**
1. ✅ Subsets (LeetCode 78) - CRITICAL
2. ✅ Subsets II (LeetCode 90)
3. ✅ Permutations (LeetCode 46) - CRITICAL
4. ✅ Permutations II (LeetCode 47)
5. ✅ Combination Sum (LeetCode 39)
6. ✅ Combination Sum II (LeetCode 40)
7. ✅ Palindrome Partitioning (LeetCode 131)
8. Letter Combinations of Phone Number (LeetCode 17)
9. Generate Parentheses (LeetCode 22)
10. Word Search (LeetCode 79)
11. N-Queens (LeetCode 51)

**Pattern Recognition Triggers:**
- "Generate all" → Backtracking
- "Permutations/combinations" → Backtracking
- "Subsets" → Choose or not choose
- "Satisfy constraints" → Backtracking with validation
- "Partition" → Backtracking with substring/subarray



#### Pattern 10: Graphs (BFS/DFS) (4 days)

**When to use:** Graph traversal, connected components, shortest path, dependencies

**Core Templates:**
```javascript
// Graph Representation
// 1. Adjacency List (most common)
const graph = {
    0: [1, 2],
    1: [0, 3],
    2: [0, 3],
    3: [1, 2]
};

// 2. Edge List
const edges = [[0,1], [0,2], [1,3], [2,3]];

// Template 1: DFS (Recursive)
function dfs(node, graph, visited = new Set()) {
    if (visited.has(node)) return;
    
    visited.add(node);
    console.log(node);  // process node
    
    for (let neighbor of graph[node]) {
        dfs(neighbor, graph, visited);
    }
}

// Template 2: DFS (Iterative with Stack)
function dfsIterative(start, graph) {
    const visited = new Set();
    const stack = [start];
    
    while (stack.length > 0) {
        const node = stack.pop();
        
        if (visited.has(node)) continue;
        visited.add(node);
        console.log(node);  // process node
        
        for (let neighbor of graph[node]) {
            if (!visited.has(neighbor)) {
                stack.push(neighbor);
            }
        }
    }
}

// Template 3: BFS (Level-wise traversal)
function bfs(start, graph) {
    const visited = new Set([start]);
    const queue = [start];
    
    while (queue.length > 0) {
        const node = queue.shift();
        console.log(node);  // process node
        
        for (let neighbor of graph[node]) {
            if (!visited.has(neighbor)) {
                visited.add(neighbor);
                queue.push(neighbor);
            }
        }
    }
}

// Template 4: Number of Islands (2D Grid DFS)
function numIslands(grid) {
    let count = 0;
    
    function dfs(i, j) {
        if (i < 0 || i >= grid.length || j < 0 || j >= grid[0].length ||
            grid[i][j] === '0') {
            return;
        }
        
        grid[i][j] = '0';  // mark visited
        
        // Visit all 4 directions
        dfs(i + 1, j);
        dfs(i - 1, j);
        dfs(i, j + 1);
        dfs(i, j - 1);
    }
    
    for (let i = 0; i < grid.length; i++) {
        for (let j = 0; j < grid[0].length; j++) {
            if (grid[i][j] === '1') {
                count++;
                dfs(i, j);
            }
        }
    }
    
    return count;
}

// Template 5: Detect Cycle (Undirected Graph)
function hasCycle(graph, n) {
    const visited = new Set();
    
    function dfs(node, parent) {
        visited.add(node);
        
        for (let neighbor of graph[node]) {
            if (!visited.has(neighbor)) {
                if (dfs(neighbor, node)) return true;
            } else if (neighbor !== parent) {
                return true;  // cycle found
            }
        }
        return false;
    }
    
    for (let i = 0; i < n; i++) {
        if (!visited.has(i)) {
            if (dfs(i, -1)) return true;
        }
    }
    return false;
}

// Template 6: Topological Sort (Kahn's Algorithm - BFS)
function topologicalSort(n, edges) {
    const graph = Array(n).fill(0).map(() => []);
    const inDegree = Array(n).fill(0);
    
    // Build graph
    for (let [u, v] of edges) {
        graph[u].push(v);
        inDegree[v]++;
    }
    
    // Start with nodes having 0 in-degree
    const queue = [];
    for (let i = 0; i < n; i++) {
        if (inDegree[i] === 0) queue.push(i);
    }
    
    const result = [];
    while (queue.length > 0) {
        const node = queue.shift();
        result.push(node);
        
        for (let neighbor of graph[node]) {
            inDegree[neighbor]--;
            if (inDegree[neighbor] === 0) {
                queue.push(neighbor);
            }
        }
    }
    
    return result.length === n ? result : [];  // empty if cycle
}
```

**Must-Solve Problems:**
1. ✅ Number of Islands (LeetCode 200) - CRITICAL
2. ✅ Clone Graph (LeetCode 133)
3. ✅ Course Schedule (LeetCode 207) - CRITICAL (Cycle Detection)
4. ✅ Course Schedule II (LeetCode 210) - Topological Sort
5. ✅ Pacific Atlantic Water Flow (LeetCode 417)
6. ✅ Graph Valid Tree (LeetCode 261)
7. Surrounded Regions (LeetCode 130)
8. Word Ladder (LeetCode 127)
9. Reconstruct Itinerary (LeetCode 332)
10. Alien Dictionary (LeetCode 269) - HARD

**Pattern Recognition Triggers:**
- "Connected components" → DFS or BFS
- "2D grid traversal" → DFS/BFS on grid
- "Shortest path (unweighted)" → BFS
- "Cycle detection" → DFS with parent tracking
- "Topological order/dependencies" → Topological sort
- "All paths" → DFS with backtracking

---

### Week 9-10: Dynamic Programming & Final Patterns



#### Pattern 11: Dynamic Programming (DP) - Part 1 (5 days)

**When to use:** Optimization (min/max), counting ways, overlapping subproblems

**DP Approach:**
1. Identify if it's a DP problem (optimization, counting, overlapping subproblems)
2. Define the state (what does dp[i] represent?)
3. Write the recurrence relation
4. Identify base cases
5. Decide iteration order (bottom-up)

**Core Templates:**
```javascript
// Template 1: 1D DP (Fibonacci Pattern)
function climbStairs(n) {
    if (n <= 2) return n;
    
    const dp = new Array(n + 1);
    dp[1] = 1;
    dp[2] = 2;
    
    for (let i = 3; i <= n; i++) {
        dp[i] = dp[i-1] + dp[i-2];
    }
    
    return dp[n];
}

// Space Optimized
function climbStairsOptimized(n) {
    if (n <= 2) return n;
    let prev2 = 1, prev1 = 2;
    
    for (let i = 3; i <= n; i++) {
        const curr = prev1 + prev2;
        prev2 = prev1;
        prev1 = curr;
    }
    return prev1;
}

// Template 2: 0/1 Knapsack (Choose or Not Choose)
function knapsack(weights, values, capacity) {
    const n = weights.length;
    const dp = Array(n + 1).fill(0).map(() => Array(capacity + 1).fill(0));
    
    for (let i = 1; i <= n; i++) {
        for (let w = 0; w <= capacity; w++) {
            if (weights[i-1] <= w) {
                // Choose or not choose
                dp[i][w] = Math.max(
                    values[i-1] + dp[i-1][w - weights[i-1]],  // choose
                    dp[i-1][w]                                 // don't choose
                );
            } else {
                dp[i][w] = dp[i-1][w];  // can't choose
            }
        }
    }
    return dp[n][capacity];
}

// Template 3: Longest Common Subsequence (2D DP)
function lcs(text1, text2) {
    const m = text1.length, n = text2.length;
    const dp = Array(m + 1).fill(0).map(() => Array(n + 1).fill(0));
    
    for (let i = 1; i <= m; i++) {
        for (let j = 1; j <= n; j++) {
            if (text1[i-1] === text2[j-1]) {
                dp[i][j] = 1 + dp[i-1][j-1];
            } else {
                dp[i][j] = Math.max(dp[i-1][j], dp[i][j-1]);
            }
        }
    }
    return dp[m][n];
}

// Template 4: Unbounded Knapsack (Coin Change)
function coinChange(coins, amount) {
    const dp = Array(amount + 1).fill(Infinity);
    dp[0] = 0;
    
    for (let i = 1; i <= amount; i++) {
        for (let coin of coins) {
            if (i >= coin) {
                dp[i] = Math.min(dp[i], 1 + dp[i - coin]);
            }
        }
    }
    
    return dp[amount] === Infinity ? -1 : dp[amount];
}
```

**Must-Solve Problems (Week 9):**
1. ✅ Climbing Stairs (LeetCode 70) - START HERE
2. ✅ House Robber (LeetCode 198)
3. ✅ Coin Change (LeetCode 322) - CRITICAL
4. ✅ Longest Increasing Subsequence (LeetCode 300)
5. ✅ Word Break (LeetCode 139)
6. ✅ Combination Sum IV (LeetCode 377)
7. Maximum Product Subarray (LeetCode 152)
8. Decode Ways (LeetCode 91)
9. Unique Paths (LeetCode 62)
10. Jump Game (LeetCode 55)

**Pattern Recognition Triggers:**
- "Count ways to reach" → 1D DP (Fibonacci-like)
- "Minimum/maximum cost" → DP optimization
- "Subsequence/substring" → 2D DP
- "Unlimited use" → Unbounded knapsack
- "Limited use" → 0/1 knapsack



#### Pattern 12: Heaps/Priority Queue (3 days)

**When to use:** Kth largest/smallest, top K elements, merge K sorted, median finding

**Core Template:**
```javascript
// JavaScript doesn't have built-in heap, so we use tricks or implement

// MinHeap Implementation (for interviews, you might get away with sorting)
class MinHeap {
    constructor() {
        this.heap = [];
    }
    
    push(val) {
        this.heap.push(val);
        this.bubbleUp(this.heap.length - 1);
    }
    
    pop() {
        if (this.heap.length === 0) return null;
        if (this.heap.length === 1) return this.heap.pop();
        
        const min = this.heap[0];
        this.heap[0] = this.heap.pop();
        this.bubbleDown(0);
        return min;
    }
    
    peek() {
        return this.heap[0];
    }
    
    size() {
        return this.heap.length;
    }
    
    bubbleUp(idx) {
        while (idx > 0) {
            const parent = Math.floor((idx - 1) / 2);
            if (this.heap[idx] >= this.heap[parent]) break;
            [this.heap[idx], this.heap[parent]] = [this.heap[parent], this.heap[idx]];
            idx = parent;
        }
    }
    
    bubbleDown(idx) {
        while (true) {
            let smallest = idx;
            const left = 2 * idx + 1;
            const right = 2 * idx + 2;
            
            if (left < this.heap.length && this.heap[left] < this.heap[smallest]) {
                smallest = left;
            }
            if (right < this.heap.length && this.heap[right] < this.heap[smallest]) {
                smallest = right;
            }
            if (smallest === idx) break;
            
            [this.heap[idx], this.heap[smallest]] = [this.heap[smallest], this.heap[idx]];
            idx = smallest;
        }
    }
}

// Quick Select for Kth Largest (Alternative to Heap)
function quickSelect(nums, k) {
    k = nums.length - k;  // kth largest = (n-k)th smallest
    
    function partition(left, right) {
        const pivot = nums[right];
        let i = left;
        
        for (let j = left; j < right; j++) {
            if (nums[j] <= pivot) {
                [nums[i], nums[j]] = [nums[j], nums[i]];
                i++;
            }
        }
        [nums[i], nums[right]] = [nums[right], nums[i]];
        return i;
    }
    
    let left = 0, right = nums.length - 1;
    while (left <= right) {
        const pivotIdx = partition(left, right);
        if (pivotIdx === k) return nums[k];
        else if (pivotIdx < k) left = pivotIdx + 1;
        else right = pivotIdx - 1;
    }
}

// Top K Frequent Elements (Using Map + Bucket Sort)
function topKFrequent(nums, k) {
    const freq = new Map();
    for (let num of nums) {
        freq.set(num, (freq.get(num) || 0) + 1);
    }
    
    // Bucket sort: index = frequency
    const buckets = Array(nums.length + 1).fill(null).map(() => []);
    for (let [num, count] of freq) {
        buckets[count].push(num);
    }
    
    const result = [];
    for (let i = buckets.length - 1; i >= 0 && result.length < k; i--) {
        result.push(...buckets[i]);
    }
    
    return result.slice(0, k);
}
```

**Must-Solve Problems:**
1. ✅ Kth Largest Element (LeetCode 215) - CRITICAL
2. ✅ Top K Frequent Elements (LeetCode 347)
3. ✅ Find Median from Data Stream (LeetCode 295) - HARD but asked often
4. ✅ Merge K Sorted Lists (LeetCode 23)
5. K Closest Points to Origin (LeetCode 973)
6. Task Scheduler (LeetCode 621)
7. Reorganize String (LeetCode 767)
8. Kth Smallest Element in Sorted Matrix (LeetCode 378)

**Pattern Recognition Triggers:**
- "Kth largest/smallest" → Heap or QuickSelect
- "Top K elements" → Heap
- "Merge K sorted" → Min heap
- "Median" → Two heaps (max heap + min heap)
- "Schedule/frequency" → Max heap



#### Pattern 13: Greedy Algorithms (2 days)

**When to use:** Local optimal leads to global optimal, scheduling, intervals

**Core Templates:**
```javascript
// Template 1: Interval Scheduling (Merge Intervals)
function merge(intervals) {
    if (intervals.length === 0) return [];
    
    // Sort by start time
    intervals.sort((a, b) => a[0] - b[0]);
    
    const result = [intervals[0]];
    
    for (let i = 1; i < intervals.length; i++) {
        const last = result[result.length - 1];
        const curr = intervals[i];
        
        if (curr[0] <= last[1]) {
            // Overlap: merge
            last[1] = Math.max(last[1], curr[1]);
        } else {
            // No overlap: add new interval
            result.push(curr);
        }
    }
    
    return result;
}

// Template 2: Jump Game
function canJump(nums) {
    let maxReach = 0;
    
    for (let i = 0; i < nums.length; i++) {
        if (i > maxReach) return false;  // can't reach here
        maxReach = Math.max(maxReach, i + nums[i]);
        if (maxReach >= nums.length - 1) return true;
    }
    
    return true;
}

// Template 3: Activity Selection
function maxMeetings(start, end) {
    const meetings = start.map((s, i) => [s, end[i]]);
    meetings.sort((a, b) => a[1] - b[1]);  // sort by end time
    
    let count = 1;
    let lastEnd = meetings[0][1];
    
    for (let i = 1; i < meetings.length; i++) {
        if (meetings[i][0] > lastEnd) {
            count++;
            lastEnd = meetings[i][1];
        }
    }
    
    return count;
}
```

**Must-Solve Problems:**
1. ✅ Jump Game (LeetCode 55)
2. ✅ Jump Game II (LeetCode 45)
3. ✅ Merge Intervals (LeetCode 56) - CRITICAL
4. ✅ Insert Interval (LeetCode 57)
5. Non-overlapping Intervals (LeetCode 435)
6. Meeting Rooms II (LeetCode 253)
7. Gas Station (LeetCode 134)
8. Partition Labels (LeetCode 763)

---

#### Pattern 14: Bit Manipulation (1-2 days)

**When to use:** Space optimization, XOR tricks, single number problems

**Core Operations:**
```javascript
// Basic Operations
n & 1           // Check if odd (last bit is 1)
n & (n-1)       // Remove rightmost set bit
n | (1 << i)    // Set ith bit
n & ~(1 << i)   // Clear ith bit
n ^ (1 << i)    // Toggle ith bit
n >> 1          // Divide by 2
n << 1          // Multiply by 2
n & -n          // Get rightmost set bit

// XOR Properties (IMPORTANT)
a ^ a = 0
a ^ 0 = a
a ^ b ^ a = b  // XOR is commutative and associative

// Count Set Bits
function countBits(n) {
    let count = 0;
    while (n > 0) {
        n &= (n - 1);  // remove rightmost set bit
        count++;
    }
    return count;
}

// Single Number (XOR all)
function singleNumber(nums) {
    let result = 0;
    for (let num of nums) {
        result ^= num;
    }
    return result;
}
```

**Must-Solve Problems:**
1. ✅ Single Number (LeetCode 136)
2. ✅ Number of 1 Bits (LeetCode 191)
3. ✅ Counting Bits (LeetCode 338)
4. Single Number II (LeetCode 137)
5. Reverse Bits (LeetCode 190)
6. Power of Two (LeetCode 231)
7. Sum of Two Integers (LeetCode 371)

---

#### Pattern 15: Math & Geometry (1-2 days)

**Quick Topics:**
```javascript
// GCD (Euclidean Algorithm)
function gcd(a, b) {
    while (b !== 0) {
        [a, b] = [b, a % b];
    }
    return a;
}

// LCM
function lcm(a, b) {
    return (a * b) / gcd(a, b);
}

// Prime Check
function isPrime(n) {
    if (n <= 1) return false;
    if (n <= 3) return true;
    if (n % 2 === 0 || n % 3 === 0) return false;
    
    for (let i = 5; i * i <= n; i += 6) {
        if (n % i === 0 || n % (i + 2) === 0) return false;
    }
    return true;
}

// Fast Power (a^b mod m)
function power(a, b, m) {
    let result = 1;
    a %= m;
    
    while (b > 0) {
        if (b & 1) result = (result * a) % m;
        a = (a * a) % m;
        b >>= 1;
    }
    return result;
}
```

**Must-Solve Problems:**
1. Happy Number (LeetCode 202)
2. Plus One (LeetCode 66)
3. Pow(x, n) (LeetCode 50)
4. Sqrt(x) (LeetCode 69)
5. Rotate Image (LeetCode 48)
6. Spiral Matrix (LeetCode 54)

---

### Week 10: Revision & Mock Interviews

**Days 1-3: Pattern Revision**
- Revisit all pattern templates
- Solve 1-2 problems from each pattern
- Focus on patterns you struggled with

**Days 4-5: Mixed Problem Solving**
- Solve 5 random medium problems daily
- Time yourself: 30-40 min per problem
- Practice identifying patterns quickly

**Days 6-7: Mock Interviews**
- Use Pramp, Interviewing.io, or LeetCode mock
- 2 problems in 45 minutes
- Practice explaining your approach
- Write clean, working code on first attempt

---

### DSA Summary: What You Must Know Cold

**Code Templates to Memorize (Write 10 times each):**
1. ✅ Binary search (classic)
2. ✅ Two pointers (opposite direction)
3. ✅ Sliding window (dynamic size)
4. ✅ Reverse linked list
5. ✅ Merge two sorted lists
6. ✅ DFS (recursive and iterative)
7. ✅ BFS (level order)
8. ✅ Tree traversals (inorder, preorder, postorder)
9. ✅ Backtracking (subsets, permutations)
10. ✅ 1D DP (Fibonacci pattern)

**Pattern Recognition Speed Test (Practice this):**
Read problem → Identify pattern → 30 seconds max

**150-200 Problems Breakdown:**
- Easy: 40-50 problems
- Medium: 100-130 problems
- Hard: 10-20 problems (only common ones)

**LeetCode Premium Worth It?**
Yes, if targeting specific companies (has company-tagged questions)

---


## Chapter 3: React.js Deep Dive

**Duration:** Running parallel with DSA (Week 3-10)  
**Goal:** Go beyond hooks, master React internals and interview topics  
**Weekly Time:** 10-15 hours (2 hours/day, 5 days)

### Why This Chapter Matters for You
You already know React + Hooks from building projects. This chapter fills the gaps interviewers test:
- React lifecycle and rendering behavior
- Performance optimization
- Advanced patterns
- State management approaches
- Testing concepts

---

### Week 1-2: Core Concepts Beyond Basics

#### React Fundamentals Review

**JSX & Virtual DOM:**
```javascript
// JSX is syntactic sugar for React.createElement
<div className="container">Hello</div>
// Compiles to:
React.createElement('div', {className: 'container'}, 'Hello')

// Virtual DOM: React's in-memory representation
// Reconciliation: Process of comparing old and new virtual DOM
// Diffing: Algorithm to find minimal changes needed
```

**Component Types:**
```javascript
// Functional Components (What you use)
function MyComponent(props) {
    return <div>{props.name}</div>;
}

// Class Components (Legacy, but asked in interviews)
class MyComponent extends React.Component {
    render() {
        return <div>{this.props.name}</div>;
    }
}
```

**Props & State:**
```javascript
// Props: Data passed from parent (immutable in child)
function Parent() {
    return <Child name="Pavan" age={27} />;
}

// State: Internal component data (mutable)
function Counter() {
    const [count, setCount] = useState(0);
    return <button onClick={() => setCount(count + 1)}>{count}</button>;
}

// Props Drilling Problem (leads to Context API)
<GrandParent>
  <Parent>
    <Child data={data} /> {/* data passed through multiple levels */}
  </Parent>
</GrandParent>
```



#### All React Hooks (Master These)

**1. useState:**
```javascript
const [state, setState] = useState(initialValue);

// Functional update (when new state depends on old)
setCount(prevCount => prevCount + 1);

// Lazy initialization (expensive computation)
const [state, setState] = useState(() => {
    return expensiveComputation();
});
```

**2. useEffect:**
```javascript
// Runs after every render
useEffect(() => {
    // side effect code
});

// Runs once on mount (empty dependency array)
useEffect(() => {
    // setup code
    return () => {
        // cleanup code
    };
}, []);

// Runs when dependencies change
useEffect(() => {
    // effect code
}, [dep1, dep2]);

// Common use cases:
// - Fetching data
// - Subscriptions
// - DOM manipulation
// - Event listeners
```

**3. useContext:**
```javascript
// Create context
const ThemeContext = React.createContext('light');

// Provider
function App() {
    return (
        <ThemeContext.Provider value="dark">
            <Child />
        </ThemeContext.Provider>
    );
}

// Consumer
function Child() {
    const theme = useContext(ThemeContext);
    return <div>{theme}</div>;
}
```

**4. useReducer:**
```javascript
// For complex state logic
const initialState = {count: 0};

function reducer(state, action) {
    switch (action.type) {
        case 'increment':
            return {count: state.count + 1};
        case 'decrement':
            return {count: state.count - 1};
        default:
            return state;
    }
}

function Counter() {
    const [state, dispatch] = useReducer(reducer, initialState);
    return (
        <>
            Count: {state.count}
            <button onClick={() => dispatch({type: 'increment'})}>+</button>
        </>
    );
}
```

**5. useRef:**
```javascript
// Two use cases:
// 1. Access DOM elements
function TextInput() {
    const inputRef = useRef(null);
    
    const focusInput = () => {
        inputRef.current.focus();
    };
    
    return <input ref={inputRef} />;
}

// 2. Store mutable value (doesn't trigger re-render)
function Timer() {
    const intervalRef = useRef(null);
    
    useEffect(() => {
        intervalRef.current = setInterval(() => {
            console.log('tick');
        }, 1000);
        
        return () => clearInterval(intervalRef.current);
    }, []);
}
```

**6. useMemo:**
```javascript
// Memoize expensive computation
function ExpensiveComponent({data}) {
    const processedData = useMemo(() => {
        return data.map(item => {
            // expensive operation
            return processItem(item);
        });
    }, [data]);  // recompute only when data changes
    
    return <div>{processedData}</div>;
}
```

**7. useCallback:**
```javascript
// Memoize function reference
function Parent() {
    const [count, setCount] = useState(0);
    
    // Without useCallback, new function created on every render
    const handleClick = useCallback(() => {
        console.log('clicked');
    }, []);  // function reference stays same
    
    return <Child onClick={handleClick} />;
}

// Child won't re-render if onClick reference doesn't change
const Child = React.memo(({onClick}) => {
    return <button onClick={onClick}>Click</button>;
});
```

**8. useLayoutEffect:**
```javascript
// Runs synchronously after DOM mutations, before paint
// Use for DOM measurements
useLayoutEffect(() => {
    const rect = divRef.current.getBoundingClientRect();
    setPosition(rect.top);
}, []);
```

**9. Custom Hooks:**
```javascript
// Reusable logic
function useFetch(url) {
    const [data, setData] = useState(null);
    const [loading, setLoading] = useState(true);
    const [error, setError] = useState(null);
    
    useEffect(() => {
        fetch(url)
            .then(res => res.json())
            .then(data => {
                setData(data);
                setLoading(false);
            })
            .catch(err => {
                setError(err);
                setLoading(false);
            });
    }, [url]);
    
    return {data, loading, error};
}

// Usage
function MyComponent() {
    const {data, loading, error} = useFetch('/api/users');
    
    if (loading) return <div>Loading...</div>;
    if (error) return <div>Error: {error.message}</div>;
    return <div>{data}</div>;
}
```



### Week 3-4: Performance Optimization

#### React.memo
```javascript
// Prevents re-render if props haven't changed
const ExpensiveChild = React.memo(function Child({data}) {
    console.log('rendering child');
    return <div>{data}</div>;
});

// Custom comparison
const Child = React.memo(
    ({data}) => <div>{data.name}</div>,
    (prevProps, nextProps) => {
        return prevProps.data.id === nextProps.data.id;
    }
);
```

#### Code Splitting & Lazy Loading
```javascript
// Lazy load components
const LazyComponent = React.lazy(() => import('./LazyComponent'));

function App() {
    return (
        <Suspense fallback={<div>Loading...</div>}>
            <LazyComponent />
        </Suspense>
    );
}

// Route-based code splitting
const Home = lazy(() => import('./routes/Home'));
const About = lazy(() => import('./routes/About'));
```

#### Performance Anti-patterns to Avoid
```javascript
// ❌ Bad: Creating function in render
function Parent() {
    return <Child onClick={() => console.log('click')} />;
}

// ✅ Good: Use useCallback
function Parent() {
    const handleClick = useCallback(() => console.log('click'), []);
    return <Child onClick={handleClick} />;
}

// ❌ Bad: Creating object in render
function Parent() {
    return <Child style={{color: 'red'}} />;
}

// ✅ Good: Define outside or useMemo
const style = {color: 'red'};
function Parent() {
    return <Child style={style} />;
}

// ❌ Bad: Inline complex computation
function Component({data}) {
    return <div>{data.map(item => expensiveCalc(item))}</div>;
}

// ✅ Good: Use useMemo
function Component({data}) {
    const processed = useMemo(() => 
        data.map(item => expensiveCalc(item)), [data]
    );
    return <div>{processed}</div>;
}
```

#### React DevTools Profiler
- Learn to identify slow renders
- Use Profiler tab to measure component performance
- Identify unnecessary re-renders



### Week 5-6: Advanced Patterns & State Management

#### Component Patterns

**1. Higher-Order Component (HOC):**
```javascript
// Wraps component to add functionality
function withAuth(Component) {
    return function AuthenticatedComponent(props) {
        const {isAuthenticated} = useAuth();
        
        if (!isAuthenticated) {
            return <Redirect to="/login" />;
        }
        
        return <Component {...props} />;
    };
}

// Usage
const ProtectedPage = withAuth(MyPage);
```

**2. Render Props:**
```javascript
// Component accepts function as child
function Mouse({render}) {
    const [position, setPosition] = useState({x: 0, y: 0});
    
    useEffect(() => {
        const handleMove = (e) => {
            setPosition({x: e.clientX, y: e.clientY});
        };
        window.addEventListener('mousemove', handleMove);
        return () => window.removeEventListener('mousemove', handleMove);
    }, []);
    
    return render(position);
}

// Usage
<Mouse render={({x, y}) => <h1>Mouse at {x}, {y}</h1>} />
```

**3. Compound Components:**
```javascript
// Components that work together
const TabsContext = React.createContext();

function Tabs({children, defaultTab}) {
    const [activeTab, setActiveTab] = useState(defaultTab);
    
    return (
        <TabsContext.Provider value={{activeTab, setActiveTab}}>
            {children}
        </TabsContext.Provider>
    );
}

function TabList({children}) {
    return <div className="tab-list">{children}</div>;
}

function Tab({id, children}) {
    const {activeTab, setActiveTab} = useContext(TabsContext);
    return (
        <button 
            className={activeTab === id ? 'active' : ''}
            onClick={() => setActiveTab(id)}
        >
            {children}
        </button>
    );
}

function TabPanel({id, children}) {
    const {activeTab} = useContext(TabsContext);
    return activeTab === id ? <div>{children}</div> : null;
}

// Usage
<Tabs defaultTab="home">
    <TabList>
        <Tab id="home">Home</Tab>
        <Tab id="profile">Profile</Tab>
    </TabList>
    <TabPanel id="home">Home Content</TabPanel>
    <TabPanel id="profile">Profile Content</TabPanel>
</Tabs>
```

#### State Management Options

**1. useState + Context (Simple Apps):**
```javascript
const AppContext = React.createContext();

function AppProvider({children}) {
    const [user, setUser] = useState(null);
    const [theme, setTheme] = useState('light');
    
    return (
        <AppContext.Provider value={{user, setUser, theme, setTheme}}>
            {children}
        </AppContext.Provider>
    );
}
```

**2. useReducer + Context (Medium Apps):**
```javascript
const AppContext = React.createContext();

const initialState = {
    user: null,
    theme: 'light',
    notifications: []
};

function reducer(state, action) {
    switch (action.type) {
        case 'SET_USER':
            return {...state, user: action.payload};
        case 'TOGGLE_THEME':
            return {...state, theme: state.theme === 'light' ? 'dark' : 'light'};
        default:
            return state;
    }
}

function AppProvider({children}) {
    const [state, dispatch] = useReducer(reducer, initialState);
    
    return (
        <AppContext.Provider value={{state, dispatch}}>
            {children}
        </AppContext.Provider>
    );
}
```

**3. Redux (Large Apps) - Know the Concepts:**
```javascript
// Action
const increment = () => ({type: 'INCREMENT'});

// Reducer
function counterReducer(state = {count: 0}, action) {
    switch (action.type) {
        case 'INCREMENT':
            return {count: state.count + 1};
        default:
            return state;
    }
}

// Store
import {createStore} from 'redux';
const store = createStore(counterReducer);

// Component
import {useSelector, useDispatch} from 'react-redux';

function Counter() {
    const count = useSelector(state => state.count);
    const dispatch = useDispatch();
    
    return (
        <div>
            {count}
            <button onClick={() => dispatch(increment())}>+</button>
        </div>
    );
}
```

**4. Zustand (Modern, Simple):**
```javascript
import create from 'zustand';

const useStore = create(set => ({
    count: 0,
    increment: () => set(state => ({count: state.count + 1})),
    decrement: () => set(state => ({count: state.count - 1}))
}));

function Counter() {
    const {count, increment} = useStore();
    return <button onClick={increment}>{count}</button>;
}
```

**Know when to use what:**
- Local state: useState
- Shared state (2-3 components): Props/Context
- Complex state logic: useReducer
- Global state (many components): Context + useReducer OR Redux/Zustand



### Week 7: Forms, Routing & Testing Basics

#### Forms in React

**1. Controlled Components:**
```javascript
function LoginForm() {
    const [email, setEmail] = useState('');
    const [password, setPassword] = useState('');
    
    const handleSubmit = (e) => {
        e.preventDefault();
        console.log({email, password});
    };
    
    return (
        <form onSubmit={handleSubmit}>
            <input 
                type="email"
                value={email}
                onChange={(e) => setEmail(e.target.value)}
            />
            <input 
                type="password"
                value={password}
                onChange={(e) => setPassword(e.target.value)}
            />
            <button type="submit">Login</button>
        </form>
    );
}
```

**2. Form Libraries (Know these exist):**
- React Hook Form (modern, performant)
- Formik (popular, more features)

#### React Router

**Basic Concepts:**
```javascript
import {BrowserRouter, Routes, Route, Link, useNavigate, useParams} from 'react-router-dom';

function App() {
    return (
        <BrowserRouter>
            <nav>
                <Link to="/">Home</Link>
                <Link to="/about">About</Link>
                <Link to="/users/123">User</Link>
            </nav>
            
            <Routes>
                <Route path="/" element={<Home />} />
                <Route path="/about" element={<About />} />
                <Route path="/users/:id" element={<User />} />
                <Route path="*" element={<NotFound />} />
            </Routes>
        </BrowserRouter>
    );
}

// Access params
function User() {
    const {id} = useParams();
    return <div>User ID: {id}</div>;
}

// Programmatic navigation
function Login() {
    const navigate = useNavigate();
    
    const handleLogin = () => {
        // ... login logic
        navigate('/dashboard');
    };
    
    return <button onClick={handleLogin}>Login</button>;
}

// Protected routes
function ProtectedRoute({children}) {
    const {isAuthenticated} = useAuth();
    return isAuthenticated ? children : <Navigate to="/login" />;
}

<Route path="/dashboard" element={
    <ProtectedRoute>
        <Dashboard />
    </ProtectedRoute>
} />
```

#### Testing Basics (Theory Level)

**Types of Tests:**
1. **Unit Tests:** Test individual components in isolation
2. **Integration Tests:** Test how components work together
3. **E2E Tests:** Test entire user flows

**Testing Library Overview:**
```javascript
import {render, screen, fireEvent} from '@testing-library/react';
import Counter from './Counter';

test('increments counter', () => {
    render(<Counter />);
    
    const button = screen.getByText('+');
    const count = screen.getByText('0');
    
    fireEvent.click(button);
    
    expect(screen.getByText('1')).toBeInTheDocument();
});
```

**Know these concepts:**
- Jest (test runner)
- React Testing Library (component testing)
- Testing best practices (test behavior, not implementation)



### React Interview Questions (Must Know)

**Conceptual Questions:**
1. What is Virtual DOM? How does React's reconciliation work?
2. What's the difference between controlled and uncontrolled components?
3. What are keys in React? Why are they important?
4. Explain React component lifecycle (class vs hooks)
5. What's the difference between useEffect and useLayoutEffect?
6. When would you use useReducer instead of useState?
7. How does Context API work? What are its limitations?
8. Explain React Fiber architecture (high-level)
9. What are the rules of hooks?
10. How do you optimize React app performance?

**Coding Questions (Practice These):**
1. Build a counter with increment/decrement
2. Create a todo list with add/delete/toggle
3. Implement a search filter for a list
4. Build an infinite scroll component
5. Create a custom hook for API fetching
6. Implement debounced search
7. Build a form with validation
8. Create tabs component
9. Implement modal/popup
10. Build autocomplete component

**State Management Questions:**
1. When would you use Redux vs Context API?
2. Explain Redux flow (Action → Reducer → Store)
3. What is Redux Toolkit?
4. How do you handle async actions in Redux? (Redux Thunk/Saga)
5. What are selectors in Redux?

---

## Chapter 4: Next.js Mastery

**Duration:** Parallel with DSA (Week 5-8)  
**Goal:** Master Next.js for full-stack interviews  
**Weekly Time:** 8-10 hours

### Why Next.js Matters
Next.js is heavily used in modern companies. Knowing it makes you more valuable.

---

### Core Next.js Concepts

#### 1. File-based Routing

**Pages Router (v12, still common):**
```
pages/
├── index.js                 → /
├── about.js                 → /about
├── blog/
│   ├── index.js            → /blog
│   └── [slug].js           → /blog/:slug
└── api/
    └── users.js            → /api/users
```

**App Router (v13+, modern):**
```
app/
├── page.js                  → /
├── layout.js               → Root layout
├── about/
│   └── page.js             → /about
├── blog/
│   ├── page.js             → /blog
│   └── [slug]/
│       └── page.js         → /blog/:slug
└── api/
    └── users/
        └── route.js        → /api/users
```



#### 2. Rendering Strategies (CRITICAL - MEMORIZE)

**SSR (Server-Side Rendering):**
```javascript
// Pages Router
export async function getServerSideProps(context) {
    const res = await fetch('https://api.example.com/data');
    const data = await res.json();
    
    return {
        props: {data}  // passed to component as props
    };
}

function Page({data}) {
    return <div>{data}</div>;
}

// App Router
async function Page() {
    const res = await fetch('https://api.example.com/data', {
        cache: 'no-store'  // SSR behavior
    });
    const data = await res.json();
    
    return <div>{data}</div>;
}
```

**SSG (Static Site Generation):**
```javascript
// Pages Router
export async function getStaticProps() {
    const res = await fetch('https://api.example.com/data');
    const data = await res.json();
    
    return {
        props: {data},
        revalidate: 60  // ISR: regenerate every 60 seconds
    };
}

// For dynamic routes
export async function getStaticPaths() {
    const posts = await fetchPosts();
    const paths = posts.map(post => ({
        params: {slug: post.slug}
    }));
    
    return {
        paths,
        fallback: 'blocking'  // or false, true
    };
}

// App Router (default is SSG)
async function Page() {
    const res = await fetch('https://api.example.com/data', {
        cache: 'force-cache'  // SSG behavior (default)
    });
    const data = await res.json();
    
    return <div>{data}</div>;
}
```

**ISR (Incremental Static Regeneration):**
```javascript
// Regenerate static page after certain time
export async function getStaticProps() {
    const data = await fetchData();
    
    return {
        props: {data},
        revalidate: 10  // regenerate every 10 seconds
    };
}
```

**CSR (Client-Side Rendering):**
```javascript
// Use useEffect to fetch on client
'use client'  // App Router directive

function Page() {
    const [data, setData] = useState(null);
    
    useEffect(() => {
        fetch('/api/data')
            .then(res => res.json())
            .then(setData);
    }, []);
    
    if (!data) return <div>Loading...</div>;
    return <div>{data}</div>;
}
```

**When to use what:**
- **SSR:** Data changes frequently, need fresh data every request (dashboards, user-specific)
- **SSG:** Content rarely changes, SEO important (blog, marketing pages)
- **ISR:** Static but occasionally updated (product pages, news)
- **CSR:** Client-specific data, no SEO needed (logged-in dashboards)



#### 3. API Routes

**Pages Router:**
```javascript
// pages/api/users.js
export default async function handler(req, res) {
    if (req.method === 'GET') {
        const users = await fetchUsers();
        res.status(200).json(users);
    } else if (req.method === 'POST') {
        const user = await createUser(req.body);
        res.status(201).json(user);
    } else {
        res.status(405).json({message: 'Method not allowed'});
    }
}

// Dynamic route: pages/api/users/[id].js
export default async function handler(req, res) {
    const {id} = req.query;
    const user = await fetchUser(id);
    res.status(200).json(user);
}
```

**App Router:**
```javascript
// app/api/users/route.js
import {NextResponse} from 'next/server';

export async function GET(request) {
    const users = await fetchUsers();
    return NextResponse.json(users);
}

export async function POST(request) {
    const body = await request.json();
    const user = await createUser(body);
    return NextResponse.json(user, {status: 201});
}

// app/api/users/[id]/route.js
export async function GET(request, {params}) {
    const {id} = params;
    const user = await fetchUser(id);
    return NextResponse.json(user);
}
```

#### 4. Image Optimization

```javascript
import Image from 'next/image';

function Profile() {
    return (
        <Image
            src="/profile.jpg"
            alt="Profile"
            width={500}
            height={500}
            priority  // Load eagerly for above-fold images
            placeholder="blur"  // Show blur while loading
        />
    );
}
```

#### 5. Middleware

```javascript
// middleware.js (root level)
import {NextResponse} from 'next/server';

export function middleware(request) {
    const token = request.cookies.get('token');
    
    if (!token) {
        return NextResponse.redirect(new URL('/login', request.url));
    }
    
    return NextResponse.next();
}

export const config = {
    matcher: ['/dashboard/:path*', '/profile/:path*']  // Apply to these routes
};
```

#### 6. Environment Variables

```bash
# .env.local
DATABASE_URL=postgresql://...
NEXT_PUBLIC_API_URL=https://api.example.com  # Available in browser
SECRET_KEY=abc123  # Server-only
```

```javascript
// Usage
const dbUrl = process.env.DATABASE_URL;  // Server-only
const apiUrl = process.env.NEXT_PUBLIC_API_URL;  // Client + Server
```

#### 7. Layout & Metadata

**App Router:**
```javascript
// app/layout.js
export const metadata = {
    title: 'My App',
    description: 'App description'
};

export default function RootLayout({children}) {
    return (
        <html lang="en">
            <body>
                <header>Header</header>
                {children}
                <footer>Footer</footer>
            </body>
        </html>
    );
}

// app/blog/layout.js (nested layout)
export default function BlogLayout({children}) {
    return (
        <div className="blog-layout">
            <aside>Sidebar</aside>
            <main>{children}</main>
        </div>
    );
}
```

#### 8. Server & Client Components (App Router)

```javascript
// Server Component (default)
async function ServerComponent() {
    const data = await fetch('...');  // Can use async
    // Cannot use hooks, event handlers
    return <div>{data}</div>;
}

// Client Component (add 'use client')
'use client'

function ClientComponent() {
    const [count, setCount] = useState(0);  // Can use hooks
    // Can handle events
    return <button onClick={() => setCount(count + 1)}>{count}</button>;
}
```

**Rules:**
- Server components by default in App Router
- Add `'use client'` for interactivity/hooks
- Server components can import client components, not vice versa



### Next.js Interview Questions

**Core Concepts:**
1. What's the difference between SSR, SSG, and CSR?
2. Explain ISR (Incremental Static Regeneration)
3. When would you use getStaticProps vs getServerSideProps?
4. What's the difference between Pages Router and App Router?
5. How does Next.js Image component optimize images?
6. What are Server Components? When to use them?
7. Explain Next.js middleware use cases
8. How does routing work in Next.js?
9. What's the purpose of next.config.js?
10. How do you handle authentication in Next.js?

**Performance Questions:**
1. How do you optimize a Next.js app?
2. What's code splitting in Next.js?
3. How does Next.js handle caching?
4. Explain static optimization
5. What are the trade-offs between different rendering methods?

---

## Chapter 5: Node.js & Backend Essentials

**Duration:** Parallel with DSA (Week 7-9)  
**Goal:** Strengthen backend knowledge for full-stack role  
**Weekly Time:** 10-12 hours

---

### Express.js Fundamentals

#### Basic Setup
```javascript
const express = require('express');
const app = express();

// Middleware
app.use(express.json());  // Parse JSON bodies
app.use(express.urlencoded({extended: true}));  // Parse URL-encoded

// Routes
app.get('/', (req, res) => {
    res.send('Hello World');
});

app.get('/api/users', (req, res) => {
    res.json({users: []});
});

app.post('/api/users', (req, res) => {
    const user = req.body;
    // Save user
    res.status(201).json(user);
});

// Start server
const PORT = process.env.PORT || 3000;
app.listen(PORT, () => {
    console.log(`Server running on port ${PORT}`);
});
```

#### Middleware Pattern
```javascript
// Custom middleware
const logger = (req, res, next) => {
    console.log(`${req.method} ${req.url}`);
    next();  // Pass to next middleware
};

app.use(logger);

// Error handling middleware
app.use((err, req, res, next) => {
    console.error(err.stack);
    res.status(500).json({error: 'Something went wrong'});
});

// Auth middleware
const auth = (req, res, next) => {
    const token = req.headers.authorization;
    if (!token) {
        return res.status(401).json({error: 'Unauthorized'});
    }
    // Verify token
    req.user = verifyToken(token);
    next();
};

app.get('/api/protected', auth, (req, res) => {
    res.json({message: 'Protected data', user: req.user});
});
```

#### RESTful API Design
```javascript
// User routes
app.get('/api/users', getAllUsers);           // Get all
app.get('/api/users/:id', getUserById);       // Get one
app.post('/api/users', createUser);           // Create
app.put('/api/users/:id', updateUser);        // Update (full)
app.patch('/api/users/:id', partialUpdate);   // Update (partial)
app.delete('/api/users/:id', deleteUser);     // Delete

// Route parameters
app.get('/api/users/:id', (req, res) => {
    const {id} = req.params;
    // fetch user by id
});

// Query parameters
app.get('/api/users', (req, res) => {
    const {page, limit} = req.query;  // /api/users?page=1&limit=10
    // paginated results
});
```



### Database Integration

#### MongoDB with Mongoose
```javascript
const mongoose = require('mongoose');

// Connect
mongoose.connect('mongodb://localhost:27017/myapp', {
    useNewUrlParser: true,
    useUnifiedTopology: true
});

// Schema
const userSchema = new mongoose.Schema({
    name: {type: String, required: true},
    email: {type: String, required: true, unique: true},
    age: Number,
    createdAt: {type: Date, default: Date.now}
});

// Model
const User = mongoose.model('User', userSchema);

// CRUD Operations
async function createUser(data) {
    const user = new User(data);
    await user.save();
    return user;
}

async function getUsers() {
    return await User.find();
}

async function getUserById(id) {
    return await User.findById(id);
}

async function updateUser(id, data) {
    return await User.findByIdAndUpdate(id, data, {new: true});
}

async function deleteUser(id) {
    return await User.findByIdAndDelete(id);
}

// Query operators
User.find({age: {$gte: 18}});  // age >= 18
User.find({name: {$in: ['Alice', 'Bob']}});  // name in list
User.find({email: {$regex: /gmail/}});  // email contains 'gmail'
```

#### PostgreSQL with node-postgres
```javascript
const {Pool} = require('pg');

const pool = new Pool({
    host: 'localhost',
    port: 5432,
    database: 'myapp',
    user: 'postgres',
    password: 'password'
});

// Query
async function getUsers() {
    const result = await pool.query('SELECT * FROM users');
    return result.rows;
}

async function createUser(name, email) {
    const result = await pool.query(
        'INSERT INTO users (name, email) VALUES ($1, $2) RETURNING *',
        [name, email]
    );
    return result.rows[0];
}

// Prepared statements prevent SQL injection
async function getUserById(id) {
    const result = await pool.query(
        'SELECT * FROM users WHERE id = $1',
        [id]
    );
    return result.rows[0];
}
```

### Authentication & Security

#### JWT Authentication
```javascript
const jwt = require('jsonwebtoken');
const bcrypt = require('bcrypt');

// Register
async function register(req, res) {
    const {email, password} = req.body;
    
    // Hash password
    const hashedPassword = await bcrypt.hash(password, 10);
    
    // Save user
    const user = await User.create({email, password: hashedPassword});
    
    res.status(201).json({message: 'User created'});
}

// Login
async function login(req, res) {
    const {email, password} = req.body;
    
    // Find user
    const user = await User.findOne({email});
    if (!user) {
        return res.status(401).json({error: 'Invalid credentials'});
    }
    
    // Verify password
    const isValid = await bcrypt.compare(password, user.password);
    if (!isValid) {
        return res.status(401).json({error: 'Invalid credentials'});
    }
    
    // Generate token
    const token = jwt.sign(
        {userId: user._id, email: user.email},
        process.env.JWT_SECRET,
        {expiresIn: '7d'}
    );
    
    res.json({token});
}

// Auth middleware
function authMiddleware(req, res, next) {
    const token = req.headers.authorization?.split(' ')[1];  // Bearer token
    
    if (!token) {
        return res.status(401).json({error: 'No token provided'});
    }
    
    try {
        const decoded = jwt.verify(token, process.env.JWT_SECRET);
        req.user = decoded;
        next();
    } catch (err) {
        res.status(401).json({error: 'Invalid token'});
    }
}
```

#### Security Best Practices
```javascript
// 1. Use helmet for security headers
const helmet = require('helmet');
app.use(helmet());

// 2. Enable CORS properly
const cors = require('cors');
app.use(cors({
    origin: 'https://yourdomain.com',
    credentials: true
}));

// 3. Rate limiting
const rateLimit = require('express-rate-limit');
const limiter = rateLimit({
    windowMs: 15 * 60 * 1000,  // 15 minutes
    max: 100  // limit each IP to 100 requests per windowMs
});
app.use('/api/', limiter);

// 4. Input validation
const {body, validationResult} = require('express-validator');

app.post('/api/users',
    body('email').isEmail(),
    body('password').isLength({min: 6}),
    (req, res) => {
        const errors = validationResult(req);
        if (!errors.isEmpty()) {
            return res.status(400).json({errors: errors.array()});
        }
        // Process request
    }
);

// 5. Sanitize user input (prevent XSS)
const mongoSanitize = require('express-mongo-sanitize');
app.use(mongoSanitize());
```



### Error Handling & Logging

```javascript
// Custom error class
class AppError extends Error {
    constructor(message, statusCode) {
        super(message);
        this.statusCode = statusCode;
        this.isOperational = true;
    }
}

// Async error wrapper
const asyncHandler = (fn) => {
    return (req, res, next) => {
        Promise.resolve(fn(req, res, next)).catch(next);
    };
};

// Usage
app.get('/api/users/:id', asyncHandler(async (req, res) => {
    const user = await User.findById(req.params.id);
    if (!user) {
        throw new AppError('User not found', 404);
    }
    res.json(user);
}));

// Global error handler
app.use((err, req, res, next) => {
    err.statusCode = err.statusCode || 500;
    err.message = err.message || 'Internal Server Error';
    
    // Log error
    console.error(err);
    
    // Send response
    res.status(err.statusCode).json({
        error: err.message,
        ...(process.env.NODE_ENV === 'development' && {stack: err.stack})
    });
});

// Logging with Winston
const winston = require('winston');

const logger = winston.createLogger({
    level: 'info',
    format: winston.format.json(),
    transports: [
        new winston.transports.File({filename: 'error.log', level: 'error'}),
        new winston.transports.File({filename: 'combined.log'})
    ]
});

if (process.env.NODE_ENV !== 'production') {
    logger.add(new winston.transports.Console());
}

// Use logger
logger.info('User logged in', {userId: user.id});
logger.error('Database connection failed', {error: err.message});
```

### File Upload

```javascript
const multer = require('multer');
const path = require('path');

// Configure storage
const storage = multer.diskStorage({
    destination: (req, file, cb) => {
        cb(null, 'uploads/');
    },
    filename: (req, file, cb) => {
        const uniqueName = Date.now() + '-' + Math.round(Math.random() * 1E9);
        cb(null, uniqueName + path.extname(file.originalname));
    }
});

// File filter
const fileFilter = (req, file, cb) => {
    const allowedTypes = ['image/jpeg', 'image/png', 'image/gif'];
    if (allowedTypes.includes(file.mimetype)) {
        cb(null, true);
    } else {
        cb(new Error('Invalid file type'), false);
    }
};

const upload = multer({
    storage,
    fileFilter,
    limits: {fileSize: 5 * 1024 * 1024}  // 5MB max
});

// Single file upload
app.post('/api/upload', upload.single('image'), (req, res) => {
    res.json({
        filename: req.file.filename,
        path: req.file.path
    });
});

// Multiple files
app.post('/api/upload-multiple', upload.array('images', 10), (req, res) => {
    res.json({files: req.files});
});
```

### Node.js Interview Questions

**Core Concepts:**
1. What is Node.js? How is it different from browser JavaScript?
2. Explain the Event Loop
3. What's the difference between sync and async code?
4. What are callbacks, promises, and async/await?
5. Explain streams in Node.js
6. What's the purpose of package.json?
7. Difference between require() and import?
8. What is middleware in Express?
9. How do you handle errors in Express?
10. Explain CORS and why it's needed

**Database Questions:**
1. SQL vs NoSQL - when to use what?
2. What are database indexes?
3. Explain ACID properties
4. What's SQL injection? How to prevent?
5. What are database transactions?

**Security Questions:**
1. How do you secure a REST API?
2. What is JWT? How does it work?
3. Explain authentication vs authorization
4. How do you store passwords securely?
5. What's XSS and CSRF? How to prevent?

**Performance Questions:**
1. How do you optimize Node.js performance?
2. What's caching? Types of caching?
3. Explain clustering in Node.js
4. How do you handle memory leaks?
5. What are worker threads?

---


## Chapter 6: System Design Basics for Interviews

**Duration:** 2 Weeks (Week 9-10)  
**Goal:** Understand core system design concepts for mid-level interviews  
**Daily Time:** 1-2 hours  

### Important Note
You don't need to design Netflix or Uber for Phase 1. You need to understand:
- Basic architectural concepts
- Common patterns
- How to think through scaling problems
- Vocabulary to discuss design trade-offs

---

### The System Design Interview Framework

**Standard Approach (Memorize This):**
1. **Clarify Requirements (5 min)**
   - Functional requirements (what features?)
   - Non-functional requirements (scale, performance, availability?)
   - Constraints (users, data size, traffic?)

2. **High-Level Design (10 min)**
   - Draw basic architecture
   - Identify main components
   - Show data flow

3. **Deep Dive (20 min)**
   - Discuss specific components
   - Address bottlenecks
   - Explain trade-offs

4. **Wrap Up (5 min)**
   - Identify potential issues
   - Discuss monitoring, scaling
   - Answer questions

---

### Core Concepts (Master These)

#### 1. Client-Server Architecture
```
Client (Browser/Mobile)
    ↓
Load Balancer
    ↓
Application Servers (Multiple)
    ↓
Database
```

**Key Points:**
- Client sends requests
- Server processes and responds
- Stateless servers (no session data on server)
- Load balancer distributes traffic



#### 2. Scalability

**Vertical Scaling (Scale Up):**
- Add more CPU, RAM, storage to existing server
- Pros: Simple, no code changes
- Cons: Limited, expensive, single point of failure

**Horizontal Scaling (Scale Out):**
- Add more servers
- Pros: Better fault tolerance, cost-effective
- Cons: Complexity, need load balancer

**When discussing scalability:**
- Current load: 100 requests/sec
- Expected load: 10,000 requests/sec
- How to handle: Add servers, caching, database optimization

#### 3. Load Balancing

**What:** Distributes traffic across multiple servers

**Algorithms:**
- Round Robin: Requests distributed equally
- Least Connections: Send to server with fewest connections
- IP Hash: Same client → same server (session affinity)

**Benefits:**
- No single point of failure
- Better resource utilization
- Can add/remove servers dynamically

```
         Load Balancer
         /     |     \
    Server1  Server2  Server3
```

#### 4. Caching

**What:** Store frequently accessed data in fast memory

**Levels:**
- Browser cache (client-side)
- CDN cache (edge locations)
- Application cache (Redis, Memcached)
- Database cache (query cache)

**Cache Strategies:**
```javascript
// 1. Cache-Aside (Lazy Loading)
async function getData(key) {
    // Check cache first
    let data = await cache.get(key);
    if (data) return data;
    
    // If not in cache, get from DB
    data = await db.get(key);
    
    // Store in cache
    await cache.set(key, data, TTL);
    return data;
}

// 2. Write-Through
async function saveData(key, data) {
    // Write to cache and DB
    await cache.set(key, data);
    await db.set(key, data);
}

// 3. Write-Behind
async function saveData(key, data) {
    // Write to cache immediately
    await cache.set(key, data);
    // Write to DB asynchronously (queue)
    queue.push({key, data});
}
```

**Cache Eviction:**
- LRU (Least Recently Used) - most common
- LFU (Least Frequently Used)
- FIFO (First In First Out)
- TTL (Time To Live)

**When to use:**
- Read-heavy workloads
- Expensive computations
- Frequently accessed data

#### 5. Database Design

**SQL vs NoSQL:**

**SQL (PostgreSQL, MySQL):**
- Structured data
- ACID transactions
- Complex queries, joins
- Use when: Banking, e-commerce, structured data

**NoSQL (MongoDB, Cassandra):**
- Flexible schema
- Horizontal scaling
- Fast reads/writes
- Use when: Social media, real-time analytics, unstructured data

**Database Scaling:**

**1. Indexing:**
```sql
-- Speed up queries
CREATE INDEX idx_user_email ON users(email);

-- Trade-off: Faster reads, slower writes
```

**2. Replication:**
```
     Master DB (writes)
     /          \
Replica 1    Replica 2  (reads)
```
- Master handles writes
- Replicas handle reads
- Eventual consistency

**3. Sharding (Horizontal Partitioning):**
```
Users 1-1M    → Shard 1
Users 1M-2M   → Shard 2
Users 2M-3M   → Shard 3
```
- Split data across multiple databases
- Shard by user ID, geography, etc.
- Complex: Cross-shard queries difficult

**4. Connection Pooling:**
- Reuse database connections
- Avoid overhead of creating new connections
- Critical for performance



#### 6. API Design

**REST Principles:**
- Stateless
- Resource-based URLs
- Standard HTTP methods (GET, POST, PUT, DELETE)
- Use HTTP status codes correctly

**Good API Design:**
```javascript
// ✅ Good
GET    /api/users           // Get all users
GET    /api/users/123       // Get user 123
POST   /api/users           // Create user
PUT    /api/users/123       // Update user 123
DELETE /api/users/123       // Delete user 123

// Pagination
GET /api/users?page=1&limit=20

// Filtering
GET /api/users?role=admin&status=active

// Sorting
GET /api/users?sort=createdAt&order=desc

// ❌ Bad
GET /api/getUsers
POST /api/user/delete/123
GET /api/users/getAllActiveUsers
```

**Rate Limiting:**
```javascript
// Prevent abuse
const rateLimit = {
    free: '100 requests/hour',
    pro: '1000 requests/hour',
    enterprise: 'unlimited'
};

// Response headers
X-RateLimit-Limit: 100
X-RateLimit-Remaining: 75
X-RateLimit-Reset: 1640000000
```

**Pagination:**
```javascript
// Offset-based (simple)
GET /api/posts?page=2&limit=20

// Cursor-based (better for real-time data)
GET /api/posts?cursor=abc123&limit=20

// Response
{
    data: [...],
    pagination: {
        nextCursor: "xyz789",
        hasMore: true
    }
}
```

#### 7. Message Queues

**What:** Asynchronous communication between services

**Use Cases:**
- Email sending
- Image processing
- Video transcoding
- Notifications

**Example (RabbitMQ/SQS concept):**
```
User uploads video
    ↓
API Server → Queue → Worker 1 (compress)
                  → Worker 2 (generate thumbnail)
                  → Worker 3 (extract metadata)
```

**Benefits:**
- Decouple services
- Handle traffic spikes
- Retry failed jobs
- Process in background

#### 8. CDN (Content Delivery Network)

**What:** Distributed servers that cache static content near users

**How it works:**
```
User in India
    ↓
CDN Edge Server (Mumbai) → Origin Server (US)
    ↓
Fast delivery (cached)
```

**Use for:**
- Images, videos
- CSS, JavaScript files
- Static HTML pages

**Benefits:**
- Faster load times
- Reduced server load
- Better user experience

#### 9. Microservices vs Monolith

**Monolith:**
```
Single Application
├── User Service
├── Product Service
├── Order Service
└── Payment Service
```

**Pros:** Simple, easy to develop/deploy  
**Cons:** Hard to scale, deploy all or nothing

**Microservices:**
```
User Service    → User DB
Product Service → Product DB
Order Service   → Order DB
Payment Service → Payment DB
```

**Pros:** Independent scaling, deploy separately  
**Cons:** Complex, network latency, distributed transactions

**For Phase 1 interviews:** Understand both, mention trade-offs



### CAP Theorem (Important for Distributed Systems)

**CAP:** You can have at most 2 of 3:
- **C**onsistency: All nodes see same data at same time
- **A**vailability: Every request gets a response
- **P**artition Tolerance: System works despite network failures

**Real-world examples:**
- **CP (Consistency + Partition):** Banking systems - need consistency
- **AP (Availability + Partition):** Social media - need availability
- **CA (Consistency + Availability):** Single-node DB - no partition tolerance needed

**In interviews:**
"Given CAP theorem, I'd prioritize [X and Y] because [reason based on requirements]"

---

### Sample System Design Problems (Phase 1 Level)

#### Problem 1: URL Shortener (like bit.ly)

**Requirements:**
- Shorten long URLs
- Redirect short → long
- Track click counts
- 1 million URLs/day

**High-Level Design:**
```
User
  ↓
Load Balancer
  ↓
App Servers (Generate short URL, hash function)
  ↓
Cache (Redis) - Popular URLs
  ↓
Database (URL mappings)
```

**Key Points:**
- Hash function to generate short code (base62 encoding)
- Cache popular URLs
- Database: id, short_code, long_url, clicks, created_at
- Scale: Sharding by short_code

#### Problem 2: Design a Rate Limiter

**Requirements:**
- Limit users to N requests per time window
- Return 429 if exceeded

**Algorithms:**
1. **Fixed Window:** Count requests per minute
2. **Sliding Window:** More accurate, uses timestamps
3. **Token Bucket:** Replenish tokens at fixed rate

**Implementation (Token Bucket):**
```javascript
class RateLimiter {
    constructor(capacity, refillRate) {
        this.capacity = capacity;
        this.tokens = capacity;
        this.refillRate = refillRate;
        this.lastRefill = Date.now();
    }
    
    allowRequest() {
        this.refillTokens();
        
        if (this.tokens > 0) {
            this.tokens--;
            return true;
        }
        return false;
    }
    
    refillTokens() {
        const now = Date.now();
        const elapsed = (now - this.lastRefill) / 1000;
        const tokensToAdd = elapsed * this.refillRate;
        
        this.tokens = Math.min(this.capacity, this.tokens + tokensToAdd);
        this.lastRefill = now;
    }
}
```

#### Problem 3: Design a Notification System

**Requirements:**
- Send email, SMS, push notifications
- 1M notifications/day

**High-Level Design:**
```
API Server
  ↓
Message Queue
  ↓
Worker 1 (Email)
Worker 2 (SMS)
Worker 3 (Push)
  ↓
Notification DB (track status)
```

**Key Points:**
- Use queue for async processing
- Retry failed notifications
- Priority queue for urgent notifications
- Template system for messages
- Track delivery status

#### Problem 4: Design a File Storage System (like Dropbox)

**Requirements:**
- Upload/download files
- Sync across devices
- Version history

**High-Level Design:**
```
Client
  ↓
API Server
  ↓
Metadata DB (file info, versions)
  ↓
Object Storage (S3) - Actual files
  ↓
CDN (for downloads)
```

**Key Points:**
- Chunk large files (easier upload/sync)
- Deduplication (same file uploaded twice)
- Metadata: file_id, name, size, chunks, version
- Sync: Poll or WebSocket for changes



### System Design Interview Checklist

**Always discuss:**
1. ✅ Requirements (functional + non-functional)
2. ✅ Scale estimates (users, requests/sec, data size)
3. ✅ Database choice (SQL vs NoSQL) with reasoning
4. ✅ Caching strategy
5. ✅ API design
6. ✅ How to scale (load balancer, horizontal scaling)
7. ✅ Potential bottlenecks
8. ✅ Trade-offs made

**Common follow-up questions:**
- "How would you handle 10x traffic?"
- "What if the database becomes slow?"
- "How do you ensure data consistency?"
- "What monitoring would you add?"

---

## Chapter 7: Behavioral Interview & Resume Stories

**Duration:** 1 Week (Week 11)  
**Goal:** Prepare compelling stories and master behavioral questions  
**Daily Time:** 1-2 hours

### Why This Matters
Technical skills get you to the interview. Stories get you the offer.

---

### STAR Method (Memorize This)

Every story should have:
- **S**ituation: Context, background (1-2 sentences)
- **T**ask: Challenge or goal (1 sentence)
- **A**ction: What YOU did (3-4 sentences, most important)
- **R**esult: Outcome, metrics, learning (1-2 sentences)

**Example:**
> **S:** "In my previous role, our e-commerce checkout had a 40% abandonment rate."
> 
> **T:** "I was tasked with improving the conversion rate within 2 months."
> 
> **A:** "I analyzed user behavior using Google Analytics and found users were confused by the multi-step form. I redesigned it into a single-page checkout, implemented auto-save for form data, and added progress indicators. I also optimized the payment gateway integration to reduce load time from 3s to 1s."
> 
> **R:** "Within 6 weeks, we reduced abandonment to 22%, increasing monthly revenue by ₹8 lakhs. The solution was rolled out across all our products."



### Prepare 8 Core Stories from Your Experience

Look at your resume projects and extract stories for these categories:

#### 1. Technical Challenge
**Question:** "Tell me about a difficult technical problem you solved."

**Your story template:**
- Project: [Pick from your resume]
- Challenge: What was complex? (Performance, scale, integration, bug)
- Your solution: Technical approach, technologies used
- Result: Metrics, impact

**Example topics from your experience:**
- Optimizing GraphQL queries
- Migrating from REST to GraphQL
- Implementing real-time features with WebSocket
- Solving performance issues in React app
- Database optimization

#### 2. Project You're Proud Of
**Question:** "Tell me about a project you're most proud of."

**Focus on:**
- Scope and impact
- Your specific contributions
- Technologies used
- Challenges overcome
- Business value delivered

**Pick your best project:** ERP system, OTT platform, or e-commerce

#### 3. Working with Team
**Question:** "Describe a time you worked in a team."

**Story structure:**
- Team size, your role
- How you collaborated
- Challenges in coordination
- How you resolved conflicts
- Outcome

**From your experience:**
- Working with designers on UI/UX
- Collaborating with backend team on APIs
- Code reviews and knowledge sharing
- Mentoring junior developers (if applicable)

#### 4. Handling Conflict/Disagreement
**Question:** "Tell me about a disagreement with a teammate."

**Important:**
- Show maturity
- Focus on resolution, not blame
- Emphasize learning

**Example template:**
> "During the [project], I disagreed with the senior developer about [technical decision]. I believed [your approach] was better because [reason]. Instead of arguing, I prepared a document comparing both approaches with pros/cons and performance data. We discussed it in a team meeting, and ultimately we went with a hybrid approach that combined the best of both. This taught me the value of data-driven discussions."

#### 5. Failure/Mistake
**Question:** "Tell me about a time you failed."

**Structure:**
- What went wrong (be honest but brief)
- What you learned (focus here)
- How you improved
- How you'd handle it differently now

**Good examples:**
- Deployed bug to production → learned importance of testing
- Missed a deadline → learned to communicate early
- Made wrong architecture choice → learned to research more

**DON'T say:** "I've never failed" or blame others



#### 6. Taking Initiative/Going Beyond
**Question:** "Tell me about a time you went above and beyond."

**From your experience:**
- Implemented feature not originally planned
- Improved codebase (refactoring, documentation)
- Helped other teams
- Learned new technology to solve problem

#### 7. Meeting Tight Deadline
**Question:** "Describe a time you worked under pressure."

**Structure:**
- Tight deadline/pressure situation
- How you prioritized
- How you managed time
- Delivered on time or communicated delay
- Result

#### 8. Learning New Technology
**Question:** "Tell me about a time you learned something new quickly."

**Your examples:**
- Learning GraphQL for project
- Picking up Next.js
- Learning AWS services
- Mastering a new library/framework

---

### Common Behavioral Questions (Prepare Answers)

**Leadership/Initiative:**
1. Tell me about a time you led a project
2. Describe a situation where you took initiative
3. How do you handle responsibility?

**Problem Solving:**
1. Tell me about a complex problem you solved
2. Describe a time you had to debug a difficult issue
3. How do you approach unknown problems?

**Communication:**
1. Describe a time you had to explain something technical to non-technical person
2. How do you handle feedback?
3. Tell me about a presentation you gave

**Adaptability:**
1. Tell me about a time priorities changed suddenly
2. How do you handle changing requirements?
3. Describe a time you had to learn quickly

**Conflict Resolution:**
1. Tell me about a disagreement with a coworker
2. How do you handle conflicting opinions?
3. Describe a time you received critical feedback

**Culture Fit:**
1. Why do you want to work here?
2. Where do you see yourself in 5 years?
3. What motivates you?
4. What's your ideal work environment?

---

### Questions to Ask Interviewer (Always Prepare 3-5)

**About Role:**
- What does a typical day look like?
- What would be my first project/task?
- What are the biggest challenges facing the team?
- How is success measured in this role?

**About Team:**
- Can you tell me about the team structure?
- What's the tech stack?
- How does the team collaborate?
- What's the code review process?

**About Company:**
- What are the company's goals for this year?
- How does the company support professional development?
- What's the deployment process?
- What's the on-call/support structure?

**Growth:**
- What are opportunities for growth?
- Does the company support learning (courses, conferences)?
- How are promotions decided?

**DON'T ask about:**
- Salary (wait for HR/offer stage)
- Work-life balance (comes across wrong)
- When will I get promoted

---

### Resume Story Preparation Exercise

**Week 11 Task:**
1. **Day 1-2:** Write 8 STAR stories (one for each category above)
2. **Day 3:** Practice telling them out loud (2-3 min each)
3. **Day 4:** Record yourself, identify filler words ("um", "like", "actually")
4. **Day 5:** Mock behavioral interview with friend/family
5. **Day 6-7:** Refine stories based on feedback

**Story Length:**
- Keep each story 2-3 minutes
- Focus 60% on Action (what YOU did)
- Quantify results when possible (%, time, money saved)

---


## Chapter 8: GitHub Profile & Portfolio Cleanup

**Duration:** 1 Week (Week 12)  
**Goal:** Make your GitHub interview-ready  
**Daily Time:** 2-3 hours

### Why GitHub Matters
Recruiters and interviewers WILL check your GitHub. A polished profile = professional impression.

---

### GitHub Profile Optimization

#### 1. Profile README (Create this first)
```markdown
# Hi, I'm Pavan S J 👋

## Full Stack Developer | React | Next.js | Node.js

🔭 I'm currently working on scalable web applications using the MERN stack

🌱 I'm learning System Design and Data Structures

💼 4+ years of experience building production applications

🛠️ Tech Stack:
- **Frontend:** React.js, Next.js, TypeScript, Redux, Tailwind CSS
- **Backend:** Node.js, Express.js, GraphQL, REST APIs
- **Database:** MongoDB, PostgreSQL, Redis
- **Cloud:** AWS (EC2, S3, Lambda), Docker
- **Tools:** Git, GitHub Actions, Jest, React Testing Library

📫 How to reach me: [LinkedIn](https://linkedin.com/in/yourprofile) | [Email](mailto:your@email.com)

---

### 📊 GitHub Stats

![Your GitHub stats](https://github-readme-stats.vercel.app/api?username=yourusername&show_icons=true&theme=radical)

### 🚀 Featured Projects

[![Repo 1](https://github-readme-stats.vercel.app/api/pin/?username=yourusername&repo=repo1)](https://github.com/yourusername/repo1)
[![Repo 2](https://github-readme-stats.vercel.app/api/pin/?username=yourusername&repo=repo2)](https://github.com/yourusername/repo2)
```

**Create at:** `https://github.com/yourusername/yourusername/blob/main/README.md`

#### 2. Pin 6 Best Repositories
Choose projects that show:
- Different technologies
- Clean code
- Real-world use cases
- Recent activity

**Good mix:**
1. Full-stack project (MERN/PERN)
2. React component library
3. Node.js backend API
4. Next.js project
5. DSA solutions (LeetCode/CodeForces)
6. Open source contribution (if any)



### Project README Template

**Every pinned project MUST have a good README:**

```markdown
# Project Name

Brief description (1-2 sentences)

![Demo Screenshot](screenshot.png)

## 🌟 Features

- Feature 1
- Feature 2
- Feature 3
- Feature 4

## 🚀 Tech Stack

**Frontend:** React.js, Redux, Tailwind CSS
**Backend:** Node.js, Express.js, MongoDB
**Other:** JWT, Socket.io, AWS S3

## 📦 Installation

```bash
# Clone the repository
git clone https://github.com/yourusername/project.git

# Install dependencies
cd project
npm install

# Set up environment variables
cp .env.example .env

# Run the application
npm run dev
```

## 🔧 Environment Variables

```
DATABASE_URL=your_database_url
JWT_SECRET=your_jwt_secret
AWS_ACCESS_KEY=your_aws_key
```

## 📸 Screenshots

![Screenshot 1](screenshots/1.png)
![Screenshot 2](screenshots/2.png)

## 🎯 Key Highlights

- Implemented real-time chat using Socket.io
- Optimized database queries, reduced response time by 60%
- Deployed on AWS with CI/CD pipeline

## 🧪 Running Tests

```bash
npm test
```

## 📝 API Documentation

### Authentication
- `POST /api/auth/register` - Register new user
- `POST /api/auth/login` - Login user

### Users
- `GET /api/users` - Get all users (auth required)
- `GET /api/users/:id` - Get user by ID

## 🤝 Contributing

Contributions are welcome! Please open an issue first.

## 📄 License

MIT License

## 👤 Author

**Pavan S J**
- GitHub: [@yourusername](https://github.com/yourusername)
- LinkedIn: [Your Profile](https://linkedin.com/in/yourprofile)

---

⭐️ If you found this project helpful, please give it a star!
```

---

### Code Quality Checklist

**Before publishing any project:**

1. **✅ Remove sensitive data**
   - No API keys, passwords, tokens in code
   - Use `.env.example` instead of `.env`
   - Add `.env` to `.gitignore`

2. **✅ Clean commit history**
   - Meaningful commit messages
   - Not "asdfasd" or "final final v3"
   - Use conventional commits: `feat:`, `fix:`, `docs:`

3. **✅ Code formatting**
   - Consistent indentation
   - No commented-out code
   - Remove console.logs (or use proper logging)
   - Add ESLint/Prettier

4. **✅ Documentation**
   - README with clear instructions
   - Comments for complex logic
   - API documentation

5. **✅ Project structure**
   - Organized folders
   - Clear naming conventions
   - Separate concerns

**Example structure:**
```
project/
├── client/
│   ├── src/
│   │   ├── components/
│   │   ├── pages/
│   │   ├── utils/
│   │   └── App.js
│   └── package.json
├── server/
│   ├── controllers/
│   ├── models/
│   ├── routes/
│   ├── middleware/
│   └── server.js
├── .gitignore
├── README.md
└── package.json
```



### Projects to Build (If You Don't Have Good Ones)

**Choose 2-3 from this list and build them during Week 12:**

#### 1. Task Management App (Full Stack)
- **Features:** CRUD tasks, categories, deadlines, search, filter
- **Tech:** React + Node + MongoDB
- **Highlights:** Drag-drop, real-time updates, auth
- **Time:** 3-4 days

#### 2. E-commerce Product Page
- **Features:** Product listing, cart, checkout, payment integration
- **Tech:** Next.js + Stripe + MongoDB
- **Highlights:** SSR/SSG, image optimization, payment flow
- **Time:** 4-5 days

#### 3. Real-time Chat Application
- **Features:** Private messages, group chat, online status
- **Tech:** React + Node + Socket.io + MongoDB
- **Highlights:** WebSocket, real-time, message history
- **Time:** 3-4 days

#### 4. Blog Platform with CMS
- **Features:** Create/edit posts, markdown support, comments, search
- **Tech:** Next.js + MDX + PostgreSQL
- **Highlights:** SSG for posts, full-text search
- **Time:** 4-5 days

#### 5. URL Shortener
- **Features:** Shorten URLs, custom slugs, analytics, QR codes
- **Tech:** Node + Express + Redis + PostgreSQL
- **Highlights:** Caching, analytics, API design
- **Time:** 2-3 days

**Building tips:**
- Focus on core features first
- Deploy to Vercel/Netlify/Railway
- Add live demo link in README
- Write clean, commented code
- Include screenshots

---

### GitHub Activity

**Make your profile active:**

1. **Daily commits (during prep period):**
   - Push DSA solutions daily
   - Work on projects
   - Contribute to docs
   
2. **Contribution graph:**
   - Aim for 3-5 commits per week minimum
   - Consistent activity > random bursts

3. **Activity to showcase:**
   - Issues opened/resolved
   - Pull requests
   - Code reviews (if contributing to open source)

**DON'T:**
- Fake commits (empty commits just for green squares)
- Copy-paste projects without understanding
- Leave half-finished projects public

---

### Week 12 Action Plan

**Day 1-2: Cleanup**
- Create profile README
- Pin 6 repositories
- Add README to all pinned repos
- Remove sensitive data
- Clean commit history

**Day 3-5: Build Project**
- Choose one project from list
- Build with clean code
- Write comprehensive README
- Add screenshots
- Deploy to production

**Day 6-7: Polish**
- Test all projects locally
- Verify all README instructions work
- Add GitHub stats to profile
- Update LinkedIn with GitHub link
- Get feedback from peers

---

### Portfolio Website (Optional but Recommended)

**Simple portfolio using:**
- Next.js + Tailwind CSS
- Deploy on Vercel (free)

**Sections:**
1. Hero (Name, title, CTA)
2. About (Brief intro)
3. Skills (Tech stack)
4. Projects (3-5 best projects with links)
5. Experience (from resume)
6. Contact (Email, LinkedIn, GitHub)

**Keep it simple:**
- Clean design
- Fast loading
- Mobile responsive
- No fancy animations that distract

**Domain (optional):**
- `yourname.dev` or `yourname.com`
- ₹800-1000/year
- Professional touch

---

### LinkedIn Optimization (Quick)

1. **Profile photo:** Professional headshot
2. **Headline:** "Full Stack Developer | MERN Stack | React | Node.js | Next.js"
3. **About:** 3-4 paragraphs about you, tech stack, what you're looking for
4. **Experience:** Match your resume
5. **Skills:** Add top 10 skills, get endorsements
6. **Projects:** Add projects with links
7. **Activity:** Share tech articles, comment on posts (1-2x per week)

---

## END OF PHASE 1

**You are now ready to apply and interview!**

At this point you have:
- ✅ Solid JavaScript fundamentals
- ✅ 150+ DSA problems solved with patterns
- ✅ Deep React, Next.js, Node.js knowledge
- ✅ Basic system design understanding
- ✅ Prepared behavioral stories
- ✅ Professional GitHub profile

**Target Companies for Phase 1:**
- Razorpay, Groww, Zepto, Juspay
- Urban Company, Swiggy, Ola, PhonePe
- Postman, Browserstack, Hasura
- Good startups (Series B/C)
- Product companies (non-FAANG)

**Expected Outcome:**
- 16-25 LPA range
- Full Stack or Frontend Engineer role
- Better work environment
- Growth opportunity

---

# PHASE 2: FAANG/BIG TECH PREPARATION (6-9 MONTHS)

**Start Phase 2 AFTER you switch jobs. Use your new job as:**
- Stable income
- Real-world experience
- Networking opportunities
- Learning from senior engineers

**Phase 2 Goal:** FAANG/Big4 level preparation

---


## Chapter 9: Java Fundamentals & OOP

**Duration:** 8 Weeks (Month 1-2)  
**Goal:** Master Java from scratch for enterprise development  
**Daily Time:** 2-3 hours

### Why Java for Phase 2
- FAANG companies use Java heavily (backend services)
- Enterprise standard
- Strong typing helps with large codebases
- Spring Boot dominance in microservices

---

### Week 1-2: Java Basics

#### Setup & First Program
```java
// HelloWorld.java
public class HelloWorld {
    public static void main(String[] args) {
        System.out.println("Hello, World!");
    }
}

// Compile: javac HelloWorld.java
// Run: java HelloWorld
```

#### Data Types & Variables
```java
// Primitive types
byte age = 27;              // 8-bit (-128 to 127)
short year = 2024;          // 16-bit
int population = 1000000;   // 32-bit (most common)
long distance = 10000000L;  // 64-bit (note L suffix)
float price = 99.99f;       // 32-bit (note f suffix)
double salary = 50000.50;   // 64-bit (default for decimals)
char grade = 'A';           // 16-bit Unicode
boolean isActive = true;    // true or false

// Reference types
String name = "Pavan";
Integer num = 10;           // Wrapper class

// Type casting
int x = 10;
double y = x;               // Implicit (widening)
int z = (int) 9.99;         // Explicit (narrowing) → 9
```

#### Operators & Control Flow
```java
// Operators (same as JavaScript mostly)
int sum = 5 + 3;
int diff = 5 - 3;
boolean isEqual = (5 == 5);
boolean isGreater = (5 > 3);

// Control flow
if (age >= 18) {
    System.out.println("Adult");
} else {
    System.out.println("Minor");
}

// Switch (Java 14+ supports enhanced switch)
switch (day) {
    case "Monday":
        System.out.println("Start of week");
        break;
    case "Friday":
        System.out.println("TGIF");
        break;
    default:
        System.out.println("Another day");
}

// Loops
for (int i = 0; i < 5; i++) {
    System.out.println(i);
}

int j = 0;
while (j < 5) {
    System.out.println(j);
    j++;
}

// Enhanced for loop
int[] numbers = {1, 2, 3, 4, 5};
for (int num : numbers) {
    System.out.println(num);
}
```

#### Arrays
```java
// Declaration and initialization
int[] arr1 = new int[5];              // [0, 0, 0, 0, 0]
int[] arr2 = {1, 2, 3, 4, 5};         // Direct initialization
String[] names = new String[3];

// Access
arr2[0] = 10;
int first = arr2[0];
int length = arr2.length;             // Note: length is property, not method

// Multi-dimensional arrays
int[][] matrix = new int[3][3];
int[][] grid = {
    {1, 2, 3},
    {4, 5, 6},
    {7, 8, 9}
};

// Array utilities
import java.util.Arrays;

int[] nums = {5, 2, 8, 1, 9};
Arrays.sort(nums);                    // Sorts in place
String str = Arrays.toString(nums);   // "[1, 2, 5, 8, 9]"
int[] copy = Arrays.copyOf(nums, nums.length);
```



### Week 3-4: Object-Oriented Programming (CRITICAL)

#### Classes & Objects
```java
public class Person {
    // Instance variables (fields)
    private String name;
    private int age;
    
    // Constructor
    public Person(String name, int age) {
        this.name = name;
        this.age = age;
    }
    
    // Default constructor
    public Person() {
        this.name = "Unknown";
        this.age = 0;
    }
    
    // Getter
    public String getName() {
        return name;
    }
    
    // Setter
    public void setName(String name) {
        this.name = name;
    }
    
    // Method
    public void introduce() {
        System.out.println("Hi, I'm " + name + " and I'm " + age);
    }
    
    // Static method (belongs to class, not instance)
    public static void printInfo() {
        System.out.println("Person class");
    }
}

// Usage
Person p1 = new Person("Pavan", 27);
p1.introduce();
Person.printInfo();
```

#### The Four Pillars of OOP

**1. Encapsulation:**
```java
public class BankAccount {
    private double balance;  // Private: can't access directly
    
    public BankAccount(double initial) {
        this.balance = initial;
    }
    
    // Controlled access through methods
    public void deposit(double amount) {
        if (amount > 0) {
            balance += amount;
        }
    }
    
    public boolean withdraw(double amount) {
        if (amount > 0 && amount <= balance) {
            balance -= amount;
            return true;
        }
        return false;
    }
    
    public double getBalance() {
        return balance;
    }
}
```

**2. Inheritance:**
```java
// Parent class
public class Animal {
    protected String name;  // Protected: accessible in subclasses
    
    public Animal(String name) {
        this.name = name;
    }
    
    public void eat() {
        System.out.println(name + " is eating");
    }
}

// Child class
public class Dog extends Animal {
    private String breed;
    
    public Dog(String name, String breed) {
        super(name);  // Call parent constructor
        this.breed = breed;
    }
    
    // Method overriding
    @Override
    public void eat() {
        System.out.println(name + " the dog is eating");
    }
    
    // New method
    public void bark() {
        System.out.println("Woof!");
    }
}

// Usage
Dog myDog = new Dog("Max", "Golden Retriever");
myDog.eat();   // Uses overridden method
myDog.bark();
```

**3. Polymorphism:**
```java
// Compile-time polymorphism (Method Overloading)
public class Calculator {
    public int add(int a, int b) {
        return a + b;
    }
    
    public double add(double a, double b) {
        return a + b;
    }
    
    public int add(int a, int b, int c) {
        return a + b + c;
    }
}

// Runtime polymorphism (Method Overriding)
Animal animal1 = new Animal("Generic");
Animal animal2 = new Dog("Buddy", "Labrador");

animal1.eat();  // "Generic is eating"
animal2.eat();  // "Buddy the dog is eating" (calls Dog's version)
```

**4. Abstraction:**
```java
// Abstract class (can't instantiate)
public abstract class Shape {
    protected String color;
    
    public Shape(String color) {
        this.color = color;
    }
    
    // Abstract method (must be implemented by subclass)
    public abstract double area();
    
    // Concrete method
    public void displayColor() {
        System.out.println("Color: " + color);
    }
}

public class Circle extends Shape {
    private double radius;
    
    public Circle(String color, double radius) {
        super(color);
        this.radius = radius;
    }
    
    @Override
    public double area() {
        return Math.PI * radius * radius;
    }
}

// Interface (100% abstract)
public interface Drawable {
    void draw();  // public abstract by default
    
    // Default method (Java 8+)
    default void display() {
        System.out.println("Displaying...");
    }
    
    // Static method
    static void info() {
        System.out.println("Drawable interface");
    }
}

public class Rectangle implements Drawable {
    @Override
    public void draw() {
        System.out.println("Drawing rectangle");
    }
}
```



### Week 5-6: Java Collections Framework (MASTER THIS)

#### List Interface
```java
import java.util.*;

// ArrayList (Dynamic array, most common)
List<String> list = new ArrayList<>();
list.add("Apple");
list.add("Banana");
list.add(1, "Orange");           // Insert at index
list.get(0);                     // "Apple"
list.set(0, "Mango");            // Update
list.remove(0);                  // Remove by index
list.remove("Banana");           // Remove by value
list.size();                     // 2
list.contains("Orange");         // true
list.clear();                    // Remove all

// LinkedList (Good for insertions/deletions)
List<Integer> linkedList = new LinkedList<>();
linkedList.add(1);
linkedList.addFirst(0);
linkedList.addLast(2);

// Vector (Thread-safe, but slower - legacy)
List<String> vector = new Vector<>();
```

#### Set Interface (No duplicates)
```java
// HashSet (Unordered, fastest)
Set<String> hashSet = new HashSet<>();
hashSet.add("Java");
hashSet.add("Python");
hashSet.add("Java");             // Ignored (duplicate)
hashSet.size();                  // 2
hashSet.contains("Java");        // true
hashSet.remove("Python");

// LinkedHashSet (Maintains insertion order)
Set<String> linkedHashSet = new LinkedHashSet<>();

// TreeSet (Sorted order)
Set<Integer> treeSet = new TreeSet<>();
treeSet.add(5);
treeSet.add(1);
treeSet.add(3);
// Stored as: [1, 3, 5]
```

#### Map Interface (Key-Value pairs)
```java
// HashMap (Unordered, fastest, most common)
Map<String, Integer> map = new HashMap<>();
map.put("Pavan", 27);
map.put("John", 30);
map.get("Pavan");                // 27
map.getOrDefault("Alice", 0);    // 0
map.containsKey("John");         // true
map.containsValue(27);           // true
map.remove("John");
map.size();                      // 1

// Iterate over map
for (Map.Entry<String, Integer> entry : map.entrySet()) {
    String key = entry.getKey();
    Integer value = entry.getValue();
}

// Or
for (String key : map.keySet()) {
    Integer value = map.get(key);
}

// LinkedHashMap (Maintains insertion order)
Map<String, Integer> linkedMap = new LinkedHashMap<>();

// TreeMap (Sorted by keys)
Map<String, Integer> treeMap = new TreeMap<>();
```

#### Queue Interface
```java
// LinkedList as Queue
Queue<String> queue = new LinkedList<>();
queue.offer("First");            // Add to end
queue.offer("Second");
queue.peek();                    // "First" (don't remove)
queue.poll();                    // "First" (remove and return)

// PriorityQueue (Min-heap by default)
Queue<Integer> pq = new PriorityQueue<>();
pq.offer(5);
pq.offer(1);
pq.offer(3);
pq.poll();                       // 1 (smallest)

// Max-heap
Queue<Integer> maxHeap = new PriorityQueue<>((a, b) -> b - a);
maxHeap.offer(5);
maxHeap.offer(1);
maxHeap.offer(3);
maxHeap.poll();                  // 5 (largest)

// Deque (Double-ended queue)
Deque<String> deque = new ArrayDeque<>();
deque.addFirst("A");
deque.addLast("B");
deque.removeFirst();
deque.removeLast();
```

#### Stack (Legacy, use Deque instead)
```java
Stack<Integer> stack = new Stack<>();
stack.push(1);
stack.push(2);
stack.peek();                    // 2
stack.pop();                     // 2

// Better: Use Deque as Stack
Deque<Integer> stack2 = new ArrayDeque<>();
stack2.push(1);
stack2.push(2);
stack2.peek();
stack2.pop();
```

#### Collections Utility Methods
```java
List<Integer> list = new ArrayList<>(Arrays.asList(5, 2, 8, 1, 9));

Collections.sort(list);                    // [1, 2, 5, 8, 9]
Collections.reverse(list);                 // [9, 8, 5, 2, 1]
Collections.shuffle(list);                 // Random order
int max = Collections.max(list);
int min = Collections.min(list);
int freq = Collections.frequency(list, 5);

// Binary search (list must be sorted)
Collections.sort(list);
int index = Collections.binarySearch(list, 5);
```



### Week 7-8: Advanced Java Concepts

#### Generics
```java
// Generic class
public class Box<T> {
    private T value;
    
    public void set(T value) {
        this.value = value;
    }
    
    public T get() {
        return value;
    }
}

Box<Integer> intBox = new Box<>();
intBox.set(10);
int value = intBox.get();

// Generic method
public static <T> void printArray(T[] array) {
    for (T element : array) {
        System.out.println(element);
    }
}

// Bounded generics
public class NumberBox<T extends Number> {
    private T value;
    // T must be Number or its subclass
}
```

#### Exception Handling
```java
// Try-catch
try {
    int result = 10 / 0;  // ArithmeticException
} catch (ArithmeticException e) {
    System.out.println("Error: " + e.getMessage());
} finally {
    System.out.println("Always executes");
}

// Multiple catch
try {
    // code
} catch (IOException e) {
    // handle IOException
} catch (SQLException e) {
    // handle SQLException
} catch (Exception e) {
    // handle any other exception
}

// Try-with-resources (auto-close)
try (BufferedReader br = new BufferedReader(new FileReader("file.txt"))) {
    String line = br.readLine();
} catch (IOException e) {
    e.printStackTrace();
}

// Custom exception
public class InvalidAgeException extends Exception {
    public InvalidAgeException(String message) {
        super(message);
    }
}

public void setAge(int age) throws InvalidAgeException {
    if (age < 0) {
        throw new InvalidAgeException("Age cannot be negative");
    }
    this.age = age;
}
```

#### Streams & Lambda (Java 8+)
```java
import java.util.stream.*;

List<Integer> numbers = Arrays.asList(1, 2, 3, 4, 5, 6, 7, 8, 9, 10);

// Filter
List<Integer> evens = numbers.stream()
    .filter(n -> n % 2 == 0)
    .collect(Collectors.toList());

// Map
List<Integer> squares = numbers.stream()
    .map(n -> n * n)
    .collect(Collectors.toList());

// Reduce
int sum = numbers.stream()
    .reduce(0, (a, b) -> a + b);

// Chaining
List<Integer> result = numbers.stream()
    .filter(n -> n % 2 == 0)
    .map(n -> n * 2)
    .sorted()
    .collect(Collectors.toList());

// Other operations
numbers.stream().distinct();           // Remove duplicates
numbers.stream().limit(5);             // First 5 elements
numbers.stream().skip(5);              // Skip first 5
numbers.stream().anyMatch(n -> n > 5); // true
numbers.stream().allMatch(n -> n > 0); // true
numbers.stream().count();              // 10
```

#### Multithreading Basics
```java
// Method 1: Extend Thread
class MyThread extends Thread {
    public void run() {
        System.out.println("Thread running");
    }
}

MyThread t1 = new MyThread();
t1.start();

// Method 2: Implement Runnable (better)
class MyRunnable implements Runnable {
    public void run() {
        System.out.println("Thread running");
    }
}

Thread t2 = new Thread(new MyRunnable());
t2.start();

// Method 3: Lambda
Thread t3 = new Thread(() -> {
    System.out.println("Thread running");
});
t3.start();

// Synchronized method (thread-safe)
public synchronized void increment() {
    count++;
}

// ExecutorService (Thread pool)
ExecutorService executor = Executors.newFixedThreadPool(5);
executor.submit(() -> {
    System.out.println("Task executed");
});
executor.shutdown();
```

#### File I/O
```java
import java.io.*;
import java.nio.file.*;

// Read file
try {
    List<String> lines = Files.readAllLines(Paths.get("file.txt"));
    for (String line : lines) {
        System.out.println(line);
    }
} catch (IOException e) {
    e.printStackTrace();
}

// Write file
try {
    Files.write(
        Paths.get("output.txt"),
        "Hello World".getBytes()
    );
} catch (IOException e) {
    e.printStackTrace();
}

// BufferedReader (for large files)
try (BufferedReader br = new BufferedReader(new FileReader("file.txt"))) {
    String line;
    while ((line = br.readLine()) != null) {
        System.out.println(line);
    }
} catch (IOException e) {
    e.printStackTrace();
}
```

---

## Chapter 10: Spring Boot & Microservices

**Duration:** 8 Weeks (Month 3-4)  
**Goal:** Master Spring Boot for enterprise backend development  
**Daily Time:** 2-3 hours

### Why Spring Boot
- Industry standard for Java backend
- Microservices architecture
- Used by most large companies
- High demand skill

---

### Week 1-2: Spring Boot Basics

#### Project Setup
```java
// Using Spring Initializr (start.spring.io)
// Dependencies: Spring Web, Spring Data JPA, H2 Database, Lombok

// Application.java (Main class)
@SpringBootApplication
public class Application {
    public static void main(String[] args) {
        SpringApplication.run(Application.class, args);
    }
}
```

#### REST Controller
```java
@RestController
@RequestMapping("/api/users")
public class UserController {
    
    @Autowired
    private UserService userService;
    
    // GET all users
    @GetMapping
    public List<User> getAllUsers() {
        return userService.findAll();
    }
    
    // GET user by ID
    @GetMapping("/{id}")
    public ResponseEntity<User> getUserById(@PathVariable Long id) {
        return userService.findById(id)
            .map(ResponseEntity::ok)
            .orElse(ResponseEntity.notFound().build());
    }
    
    // POST create user
    @PostMapping
    public ResponseEntity<User> createUser(@RequestBody User user) {
        User savedUser = userService.save(user);
        return ResponseEntity.status(HttpStatus.CREATED).body(savedUser);
    }
    
    // PUT update user
    @PutMapping("/{id}")
    public ResponseEntity<User> updateUser(
        @PathVariable Long id,
        @RequestBody User user
    ) {
        return userService.update(id, user)
            .map(ResponseEntity::ok)
            .orElse(ResponseEntity.notFound().build());
    }
    
    // DELETE user
    @DeleteMapping("/{id}")
    public ResponseEntity<Void> deleteUser(@PathVariable Long id) {
        if (userService.deleteById(id)) {
            return ResponseEntity.noContent().build();
        }
        return ResponseEntity.notFound().build();
    }
}
```



#### Entity & Repository
```java
// User Entity
@Entity
@Table(name = "users")
@Data  // Lombok: generates getters, setters, toString, etc.
@NoArgsConstructor
@AllArgsConstructor
public class User {
    @Id
    @GeneratedValue(strategy = GenerationType.IDENTITY)
    private Long id;
    
    @Column(nullable = false)
    private String name;
    
    @Column(unique = true, nullable = false)
    private String email;
    
    private int age;
    
    @CreatedDate
    private LocalDateTime createdAt;
    
    @LastModifiedDate
    private LocalDateTime updatedAt;
}

// Repository Interface
public interface UserRepository extends JpaRepository<User, Long> {
    // Custom queries
    Optional<User> findByEmail(String email);
    List<User> findByAgeGreaterThan(int age);
    
    @Query("SELECT u FROM User u WHERE u.name LIKE %:name%")
    List<User> searchByName(@Param("name") String name);
}
```

#### Service Layer
```java
@Service
public class UserService {
    
    @Autowired
    private UserRepository userRepository;
    
    public List<User> findAll() {
        return userRepository.findAll();
    }
    
    public Optional<User> findById(Long id) {
        return userRepository.findById(id);
    }
    
    public User save(User user) {
        return userRepository.save(user);
    }
    
    public Optional<User> update(Long id, User userDetails) {
        return userRepository.findById(id)
            .map(user -> {
                user.setName(userDetails.getName());
                user.setEmail(userDetails.getEmail());
                user.setAge(userDetails.getAge());
                return userRepository.save(user);
            });
    }
    
    public boolean deleteById(Long id) {
        if (userRepository.existsById(id)) {
            userRepository.deleteById(id);
            return true;
        }
        return false;
    }
}
```

### Week 3-4: Advanced Spring Boot

#### Exception Handling
```java
// Custom Exception
public class ResourceNotFoundException extends RuntimeException {
    public ResourceNotFoundException(String message) {
        super(message);
    }
}

// Global Exception Handler
@RestControllerAdvice
public class GlobalExceptionHandler {
    
    @ExceptionHandler(ResourceNotFoundException.class)
    public ResponseEntity<ErrorResponse> handleResourceNotFound(
        ResourceNotFoundException ex
    ) {
        ErrorResponse error = new ErrorResponse(
            HttpStatus.NOT_FOUND.value(),
            ex.getMessage(),
            System.currentTimeMillis()
        );
        return ResponseEntity.status(HttpStatus.NOT_FOUND).body(error);
    }
    
    @ExceptionHandler(Exception.class)
    public ResponseEntity<ErrorResponse> handleGlobalException(
        Exception ex
    ) {
        ErrorResponse error = new ErrorResponse(
            HttpStatus.INTERNAL_SERVER_ERROR.value(),
            ex.getMessage(),
            System.currentTimeMillis()
        );
        return ResponseEntity.status(HttpStatus.INTERNAL_SERVER_ERROR)
            .body(error);
    }
}
```

#### Validation
```java
import javax.validation.constraints.*;

@Entity
public class User {
    @NotBlank(message = "Name is required")
    @Size(min = 2, max = 50, message = "Name must be between 2 and 50 characters")
    private String name;
    
    @Email(message = "Invalid email format")
    @NotBlank(message = "Email is required")
    private String email;
    
    @Min(value = 18, message = "Age must be at least 18")
    @Max(value = 100, message = "Age must be less than 100")
    private int age;
}

// Controller
@PostMapping
public ResponseEntity<User> createUser(@Valid @RequestBody User user) {
    // If validation fails, throws MethodArgumentNotValidException
    return ResponseEntity.ok(userService.save(user));
}
```

#### Security (JWT Authentication)
```java
// Security Configuration
@Configuration
@EnableWebSecurity
public class SecurityConfig extends WebSecurityConfigurerAdapter {
    
    @Override
    protected void configure(HttpSecurity http) throws Exception {
        http
            .csrf().disable()
            .authorizeRequests()
            .antMatchers("/api/auth/**").permitAll()
            .anyRequest().authenticated()
            .and()
            .sessionManagement()
            .sessionCreationPolicy(SessionCreationPolicy.STATELESS);
        
        http.addFilterBefore(
            jwtAuthenticationFilter,
            UsernamePasswordAuthenticationFilter.class
        );
    }
}

// JWT Utility
@Component
public class JwtUtil {
    @Value("${jwt.secret}")
    private String secret;
    
    public String generateToken(String username) {
        return Jwts.builder()
            .setSubject(username)
            .setIssuedAt(new Date())
            .setExpiration(new Date(System.currentTimeMillis() + 86400000)) // 1 day
            .signWith(SignatureAlgorithm.HS512, secret)
            .compact();
    }
    
    public String extractUsername(String token) {
        return Jwts.parser()
            .setSigningKey(secret)
            .parseClaimsJws(token)
            .getBody()
            .getSubject();
    }
    
    public boolean validateToken(String token) {
        try {
            Jwts.parser().setSigningKey(secret).parseClaimsJws(token);
            return true;
        } catch (Exception e) {
            return false;
        }
    }
}
```

### Week 5-6: Microservices Architecture

#### Key Concepts
- **Service Discovery:** Eureka
- **API Gateway:** Spring Cloud Gateway
- **Load Balancing:** Ribbon
- **Circuit Breaker:** Resilience4j
- **Config Management:** Spring Cloud Config
- **Distributed Tracing:** Zipkin

#### Sample Microservices Setup
```
API Gateway → User Service → User DB
           → Product Service → Product DB
           → Order Service → Order DB
```

#### Service Communication
```java
// Using RestTemplate
@Service
public class OrderService {
    
    @Autowired
    private RestTemplate restTemplate;
    
    public Order createOrder(OrderRequest request) {
        // Call Product Service
        Product product = restTemplate.getForObject(
            "http://product-service/api/products/" + request.getProductId(),
            Product.class
        );
        
        // Call User Service
        User user = restTemplate.getForObject(
            "http://user-service/api/users/" + request.getUserId(),
            User.class
        );
        
        // Create order
        Order order = new Order(user, product, request.getQuantity());
        return orderRepository.save(order);
    }
}

// Using WebClient (Reactive)
@Service
public class OrderService {
    
    @Autowired
    private WebClient.Builder webClientBuilder;
    
    public Mono<Order> createOrder(OrderRequest request) {
        return webClientBuilder.build()
            .get()
            .uri("http://product-service/api/products/" + request.getProductId())
            .retrieve()
            .bodyToMono(Product.class)
            .flatMap(product -> {
                // Create order logic
                return Mono.just(new Order());
            });
    }
}
```

---


## Chapter 11: Advanced DSA & Competitive Programming

**Duration:** 8-12 Weeks (Month 3-5)  
**Goal:** Master advanced algorithms and problem-solving  
**Daily Time:** 3-4 hours

### Advanced DSA Topics

#### 1. Advanced Dynamic Programming
- Matrix Chain Multiplication
- Edit Distance
- Partition problems
- Egg Drop Problem
- Palindrome Partitioning
- Longest Palindromic Subsequence
- Wildcard Pattern Matching
- Burst Balloons

#### 2. Advanced Graph Algorithms
- Dijkstra's Algorithm (Shortest Path)
- Bellman-Ford Algorithm
- Floyd-Warshall Algorithm
- Minimum Spanning Tree (Kruskal's, Prim's)
- Strongly Connected Components (Tarjan's)
- Topological Sort variations
- Network Flow (Max Flow - Min Cut)

#### 3. Advanced Tree Algorithms
- Segment Trees
- Fenwick Tree (Binary Indexed Tree)
- Trie variations
- Suffix Trees/Arrays
- LCA (Lowest Common Ancestor)
- Tree DP problems

#### 4. String Algorithms
- KMP Pattern Matching
- Rabin-Karp Algorithm
- Z-Algorithm
- Manacher's Algorithm (Longest Palindrome)

#### 5. Mathematical Algorithms
- Modular Arithmetic
- Fast Exponentiation
- Sieve variations
- Number Theory basics
- Combinatorics

**Target: 300+ total problems by end of Phase 2**

---

## Chapter 12: Low Level Design (LLD)

**Duration:** 6-8 Weeks (Month 5-6)  
**Goal:** Master object-oriented design for interviews  
**Daily Time:** 2-3 hours

### SOLID Principles (MUST KNOW)

**S - Single Responsibility Principle:**
Each class should have one responsibility

**O - Open/Closed Principle:**
Open for extension, closed for modification

**L - Liskov Substitution Principle:**
Subtypes must be substitutable for base types

**I - Interface Segregation Principle:**
Many specific interfaces > one general interface

**D - Dependency Inversion Principle:**
Depend on abstractions, not concretions

### Design Patterns (Top 10 for Interviews)

**1. Singleton:**
```java
public class Database {
    private static Database instance;
    
    private Database() {}
    
    public static synchronized Database getInstance() {
        if (instance == null) {
            instance = new Database();
        }
        return instance;
    }
}
```

**2. Factory:**
```java
public interface Vehicle {
    void drive();
}

public class VehicleFactory {
    public static Vehicle createVehicle(String type) {
        if (type.equals("car")) return new Car();
        if (type.equals("bike")) return new Bike();
        return null;
    }
}
```

**3. Observer:**
```java
public interface Observer {
    void update(String message);
}

public class Subject {
    private List<Observer> observers = new ArrayList<>();
    
    public void attach(Observer observer) {
        observers.add(observer);
    }
    
    public void notifyObservers(String message) {
        for (Observer observer : observers) {
            observer.update(message);
        }
    }
}
```

**4. Strategy:**
**5. Decorator:**
**6. Adapter:**
**7. Builder:**
**8. Prototype:**
**9. Command:**
**10. State:**

### Classic LLD Problems

**1. Design Parking Lot:**
- Classes: ParkingLot, Floor, Slot, Vehicle, Ticket
- Requirements: Multiple floors, different vehicle types, payment

**2. Design Library Management System:**
- Classes: Library, Book, Member, Librarian, Transaction
- Requirements: Issue/return books, search, fines

**3. Design Chess Game:**
- Classes: Board, Piece, Player, Move, Game
- Requirements: Valid moves, check/checkmate

**4. Design Splitwise:**
- Classes: User, Expense, Group, Split
- Requirements: Equal/unequal/percentage splits

**5. Design Elevator System:**
- Classes: Elevator, Floor, Request, Controller
- Requirements: Multiple elevators, optimization

**6. Design Tic-Tac-Toe:**
**7. Design Snake & Ladder:**
**8. Design ATM:**
**9. Design Movie Ticket Booking:**
**10. Design Hotel Booking System:**

---


## Chapter 13: Advanced System Design

**Duration:** 8-10 Weeks (Month 7-9)  
**Goal:** Design large-scale distributed systems  
**Daily Time:** 2-3 hours

### Advanced Concepts

#### 1. Database Sharding Strategies
- Range-based sharding
- Hash-based sharding
- Directory-based sharding
- Consistent Hashing

#### 2. Distributed Caching
- Cache invalidation strategies
- Cache warming
- Write-through vs Write-back
- Distributed cache (Redis Cluster)

#### 3. Message Queues Deep Dive
- RabbitMQ vs Kafka
- Pub-Sub vs Point-to-Point
- Message ordering guarantees
- Dead letter queues

#### 4. Distributed Transactions
- Two-Phase Commit (2PC)
- Saga Pattern
- Event Sourcing
- CQRS (Command Query Responsibility Segregation)

#### 5. Service Mesh
- Istio
- Linkerd
- Service discovery
- Circuit breaking
- Rate limiting

#### 6. Observability
- Logging (ELK Stack)
- Metrics (Prometheus, Grafana)
- Tracing (Jaeger, Zipkin)
- APM tools

### Classic System Design Problems (FAANG Level)

**1. Design WhatsApp/Messenger:**
- Requirements: 1 billion users, real-time messaging, media sharing
- Key components: WebSocket servers, message queue, media storage
- Challenges: Message ordering, online status, delivery receipts

**2. Design Instagram/Photo Sharing:**
- Requirements: Upload photos, feed, followers, likes
- Key components: CDN, image processing, news feed service
- Challenges: Feed generation, image optimization, scalability

**3. Design Uber/Ride-sharing:**
- Requirements: Match drivers and riders, real-time location, pricing
- Key components: Location service, matching service, payment
- Challenges: Geospatial indexing, surge pricing, ETA calculation

**4. Design Netflix/Video Streaming:**
- Requirements: Video upload, encoding, streaming, recommendations
- Key components: CDN, video processing pipeline, recommendation engine
- Challenges: Adaptive bitrate, content delivery, scale

**5. Design Twitter:**
- Requirements: Post tweets, follow users, timeline, trending
- Key components: Timeline service, fanout service, trending service
- Challenges: Timeline generation, celebrity problem, real-time updates

**6. Design YouTube:**
**7. Design Facebook News Feed:**
**8. Design Amazon/E-commerce:**
**9. Design Dropbox/Google Drive:**
**10. Design Zoom/Video Conferencing:**
**11. Design TinyURL:**
**12. Design Rate Limiter:**
**13. Design Typeahead/Autocomplete:**
**14. Design Web Crawler:**
**15. Design Design API Rate Limiter:**

### System Design Interview Template

**1. Requirements Clarification (5-10 min):**
- Functional requirements
- Non-functional requirements (scale, latency, availability)
- Constraints

**2. Capacity Estimation (5 min):**
- DAU (Daily Active Users)
- Requests per second
- Storage requirements
- Bandwidth

**3. API Design (5 min):**
- Define main APIs
- Request/response format

**4. High-Level Design (10-15 min):**
- Draw architecture diagram
- Identify main components
- Show data flow

**5. Deep Dive (20 min):**
- Database schema
- Scaling strategy
- Caching strategy
- Load balancing
- Potential bottlenecks
- Trade-offs

**6. Wrap-up (5 min):**
- Monitoring & alerting
- Security considerations
- Future improvements

---


## Week-by-Week Schedule

### Phase 1 Detailed Schedule (12 Weeks)

#### Week 1-2: JavaScript Fundamentals
- **Mon-Wed:** Variables, data types, strings, arrays (3 hours/day)
- **Thu-Fri:** Functions, objects, loops (3 hours/day)
- **Sat-Sun:** Practice problems, mini assessment (4 hours/day)

#### Week 3: Arrays & Hashing + React Review
- **Mon-Wed:** DSA patterns (2 hours) + React hooks deep dive (1.5 hours)
- **Thu-Fri:** Practice problems (2 hours) + React performance (1.5 hours)
- **Sat-Sun:** Solve 10-12 problems + Build React component (5 hours)

#### Week 4: Two Pointers + Sliding Window + Next.js Basics
- **Mon-Wed:** Two pointers problems (2 hours) + Next.js routing (1 hour)
- **Thu-Fri:** Sliding window problems (2 hours) + Next.js SSR/SSG (1 hour)
- **Sat-Sun:** Mixed problems + Next.js project setup (5 hours)

#### Week 5-6: Stack + Binary Search + Node.js
- **Mon-Wed:** Stack patterns (2 hours) + Express basics (1.5 hours)
- **Thu-Fri:** Binary search problems (2 hours) + MongoDB/PostgreSQL (1.5 hours)
- **Sat-Sun:** Mixed problems + Build REST API (5 hours)

#### Week 7: Linked Lists + Trees + Security
- **Mon-Wed:** Linked list problems (2 hours) + Authentication (1 hour)
- **Thu-Fri:** Tree problems (2 hours) + API security (1 hour)
- **Sat-Sun:** Mixed problems + Add auth to project (4 hours)

#### Week 8: Backtracking + Graphs
- **Mon-Wed:** Backtracking patterns (2 hours) + Project work (1 hour)
- **Thu-Fri:** Graph problems (2 hours) + Project work (1 hour)
- **Sat-Sun:** Mixed problems (5 hours)

#### Week 9: Dynamic Programming + System Design
- **Mon-Wed:** DP patterns (2 hours) + System design basics (1 hour)
- **Thu-Fri:** DP problems (2 hours) + Sample designs (1 hour)
- **Sat-Sun:** Mixed problems + Practice design questions (4 hours)

#### Week 10: Heaps + Final DSA Review + System Design
- **Mon-Wed:** Heap problems (2 hours) + System design practice (1 hour)
- **Thu-Fri:** Greedy + Bit manipulation (2 hours) + Design practice (1 hour)
- **Sat-Sun:** Revision + Mock interviews (5 hours)

#### Week 11: Behavioral Prep + Resume Polish
- **Mon-Tue:** Write STAR stories (2 hours/day)
- **Wed-Thu:** Practice stories aloud (2 hours/day)
- **Fri:** Mock behavioral interview (2 hours)
- **Sat-Sun:** GitHub cleanup + Resume updates (4 hours/day)

#### Week 12: Final Prep + Applications
- **Mon-Tue:** Build/polish portfolio project (4 hours/day)
- **Wed-Thu:** Mock technical interviews (3 hours/day)
- **Fri:** Profile optimization (LinkedIn, GitHub) (3 hours)
- **Sat-Sun:** Start applying to companies (4 hours/day)

---

### Phase 2 Detailed Schedule (9 Months)

#### Month 1-2: Java Fundamentals
- **Week 1-2:** Java basics, syntax, control flow (2-3 hours/day)
- **Week 3-4:** OOP concepts, inheritance, polymorphism (2-3 hours/day)
- **Week 5-6:** Collections framework, generics (2-3 hours/day)
- **Week 7-8:** Streams, multithreading, file I/O (2-3 hours/day)

#### Month 3-4: Spring Boot
- **Week 1-2:** Spring Boot basics, REST APIs (2-3 hours/day)
- **Week 3-4:** JPA, security, validation (2-3 hours/day)
- **Week 5-6:** Microservices concepts (2-3 hours/day)
- **Week 7-8:** Build full microservices project (3-4 hours/day)

#### Month 5: Advanced DSA
- **Week 1-2:** Advanced DP, graph algorithms (3 hours/day)
- **Week 3-4:** String algorithms, mathematical algorithms (3 hours/day)
- Target: 250+ total problems by end of month

#### Month 6: Low Level Design
- **Week 1:** SOLID principles, design patterns (2 hours/day)
- **Week 2-3:** Practice 5 LLD problems (2-3 hours/day)
- **Week 4:** Mock LLD interviews (2 hours/day)

#### Month 7-9: Advanced System Design
- **Week 1-4:** Study advanced concepts (distributed systems, etc.)
- **Week 5-8:** Practice 10+ system design problems
- **Week 9-12:** Mock system design interviews, company-specific prep

---


## Resources & Practice Platforms

### DSA Practice Platforms

**Primary (Use these):**
- **LeetCode:** Best for interview prep, company-tagged questions
  - Start with Easy, move to Medium
  - Premium worth it for company questions
  - Target: 200+ problems in Phase 1, 350+ total in Phase 2

- **GeeksforGeeks:** Good explanations, Indian company focus
  - Practice DSA sheets
  - Company-specific practice

**Secondary (Optional):**
- **HackerRank:** Skills certification
- **CodeForces:** Competitive programming (Phase 2)
- **AtCoder:** Competitive programming (Phase 2)
- **InterviewBit:** Structured learning path

### DSA Resources

**Books:**
- "Cracking the Coding Interview" by Gayle Laakmann McDowell (MUST READ)
- "Elements of Programming Interviews" (Java version for Phase 2)

**YouTube Channels:**
- **NeetCode:** Pattern-based explanations (HIGHLY RECOMMENDED)
- **Striver (take U forward):** Indian perspective, great explanations
- **Abdul Bari:** Algorithm concepts
- **Aditya Verma:** DP, backtracking patterns
- **freeCodeCamp:** Full courses

**Websites:**
- **NeetCode.io:** 150 problem list with pattern grouping
- **LeetCode Discuss:** Learn from others' solutions
- **AlgoExpert:** Paid, but good explanations

### System Design Resources

**Books:**
- "Designing Data-Intensive Applications" by Martin Kleppmann (BIBLE)
- "System Design Interview" by Alex Xu (Vol 1 & 2) (MUST READ)

**YouTube Channels:**
- **Gaurav Sen:** Excellent system design explanations
- **Tech Dummies:** Detailed system design
- **sudoCODE:** System design interviews
- **Success in Tech:** Real interview experiences

**Websites:**
- **System Design Primer (GitHub):** Comprehensive guide
- **Grokking the System Design Interview:** Paid course, worth it
- **ByteByteGo:** Newsletter + courses by Alex Xu

### Web Development Resources

**React/Next.js:**
- Official documentation (best resource)
- **Web Dev Simplified (YouTube):** Clear explanations
- **Traversy Media (YouTube):** Project-based learning
- **freeCodeCamp:** Full courses

**Node.js/Backend:**
- Official Node.js documentation
- **Hussein Nasser (YouTube):** Backend concepts
- **Academind (YouTube):** Full-stack courses

**Java/Spring Boot:**
- Official Spring documentation
- **Amigoscode (YouTube):** Spring Boot tutorials
- **Java Brains (YouTube):** Spring concepts
- Baeldung.com: Spring tutorials

### Mock Interview Platforms

**Highly Recommended:**
- **Pramp:** Free peer interviews
- **Interviewing.io:** Anonymous interviews with engineers
- **LeetCode Mock:** Timed mock interviews

**Paid (worth it if budget allows):**
- **InterviewKickstart:** Structured program
- **AlgoExpert:** Interview prep platform
- **Exponent:** PM + SDE interviews

### Company Preparation

**Research:**
- **Glassdoor:** Interview experiences, salaries
- **LeetCode Discuss:** Company-specific questions
- **Blind:** Anonymous company discussions
- **levels.fyi:** Salary information

**For Indian Companies:**
- **GeeksforGeeks:** Company-specific questions
- **InterviewBit:** Indian company focus

---

## Final Interview Checklist

### 1 Week Before Interview

**Technical:**
- [ ] Revise all DSA pattern templates
- [ ] Solve 3-5 medium problems daily
- [ ] Review system design concepts
- [ ] Practice explaining solutions out loud

**Behavioral:**
- [ ] Review STAR stories
- [ ] Practice with friend/mirror
- [ ] Prepare questions to ask interviewer
- [ ] Research the company

**Logistics:**
- [ ] Test internet connection (for remote)
- [ ] Prepare workspace (quiet, well-lit)
- [ ] Test webcam and microphone
- [ ] Have water, paper, pen ready

### Day Before Interview

- [ ] Light revision (don't cram)
- [ ] Review your resume thoroughly
- [ ] Prepare stories for each resume point
- [ ] Get good sleep (8 hours)
- [ ] Lay out professional clothes

### Interview Day

**Before Interview:**
- [ ] Eat a good meal
- [ ] Use bathroom
- [ ] Log in 10 minutes early
- [ ] Have paper and pen ready
- [ ] Close all distractions

**During Interview:**
- [ ] Think out loud
- [ ] Ask clarifying questions
- [ ] Start with brute force, then optimize
- [ ] Test your code with examples
- [ ] Handle edge cases
- [ ] Stay calm if stuck

**After Interview:**
- [ ] Send thank you email within 24 hours
- [ ] Note down questions asked (for future)
- [ ] Reflect on what went well/poorly

---


## Common Mistakes to Avoid

### Technical Interview Mistakes

1. **❌ Jumping straight to code**
   - ✅ First understand problem, ask questions, discuss approach

2. **❌ Silent coding**
   - ✅ Think out loud, explain your reasoning

3. **❌ Not considering edge cases**
   - ✅ Empty arrays, null values, negative numbers, large inputs

4. **❌ Ignoring time/space complexity**
   - ✅ Always analyze and mention Big O

5. **❌ Giving up too quickly**
   - ✅ Work through the problem, ask for hints if truly stuck

6. **❌ Not testing code**
   - ✅ Walk through code with example inputs

7. **❌ Arguing with interviewer**
   - ✅ Listen to hints, adapt your approach

### Behavioral Interview Mistakes

1. **❌ Rambling, no structure**
   - ✅ Use STAR method, keep it concise (2-3 min)

2. **❌ Blaming others**
   - ✅ Focus on what YOU did, show ownership

3. **❌ No specific examples**
   - ✅ Use real stories with metrics/results

4. **❌ Saying "I don't know"**
   - ✅ "I haven't faced that, but here's how I'd approach it"

5. **❌ Not asking questions**
   - ✅ Always have 3-5 thoughtful questions prepared

### General Mistakes

1. **❌ Inconsistency in resume and interview**
   - ✅ Know your resume inside out

2. **❌ Appearing disinterested**
   - ✅ Show enthusiasm for the role

3. **❌ Bad internet/unprofessional setup**
   - ✅ Test everything beforehand

4. **❌ Not following up**
   - ✅ Send thank you email

---

## Salary Negotiation Tips (For After Offer)

### Do Your Research
- Use levels.fyi, Glassdoor, Blind
- Know the market rate for your YOE and location
- Consider total compensation (base + bonus + stocks + benefits)

### Negotiation Strategy
1. **Never give first number:** "What's the budget for this role?"
2. **Don't accept immediately:** "Thanks! Can I have 2-3 days to review?"
3. **Negotiate everything:** Base salary, signing bonus, stocks, WFH, learning budget
4. **Have competing offers:** Leverage for better package
5. **Be professional:** Negotiate firmly but politely

### What to Say
- "Based on my research and experience, I was expecting ₹X"
- "Is there flexibility in the base salary?"
- "Can we increase the signing bonus?"
- "I have another offer at ₹Y, can you match?"

### Red Flags to Watch For
- Lowball offer with no negotiation room
- Vague about compensation structure
- Pressuring you to accept quickly
- No clarity on growth path

---

## Mental Health & Burnout Prevention

### During Preparation

**Schedule breaks:**
- 1 day off per week (complete detox)
- 10-minute break every hour
- 1 hour break after 3 hours of study

**Physical health:**
- Exercise 30 min daily (walk/gym/yoga)
- Proper sleep (7-8 hours)
- Healthy meals, stay hydrated

**Mental well-being:**
- Don't compare with others
- Track progress, celebrate small wins
- Talk to friends/family
- It's okay to have bad days

### During Job Search

- Apply to 5-10 companies per week (not 50)
- Rejections are normal (even at senior level)
- Each interview is practice
- Take breaks between interviews

### Remember

> "This is a marathon, not a sprint. Consistent effort beats sporadic bursts."

> "Your worth is not defined by interview outcomes. You're already capable."

---


## Final Words

### Your Journey Map

**Where you are now:**
- 4+ years experience in MERN stack
- Built production applications
- Strong project-level skills
- But gaps in fundamentals (DSA, core JS, system design)

**Phase 1 Goal (2-3 months):**
- Fill the gaps
- Get interview-ready
- Land a better job (16-25 LPA)
- Companies like Razorpay, Groww, Zepto, Postman
- Role: Full Stack or Frontend Engineer

**Phase 2 Goal (6-9 months after job switch):**
- Deep expertise in Java + Spring Boot
- Advanced DSA mastery
- Low-level and high-level design
- FAANG/Big Tech ready
- Companies: Google, Amazon, Microsoft, Meta, Netflix
- Role: Senior SDE, Staff Engineer

### Success Criteria

**Phase 1 Success:**
- ✅ Solved 150+ DSA problems
- ✅ Can explain all resume projects in detail
- ✅ Professional GitHub profile
- ✅ Understand system design basics
- ✅ Confident in behavioral interviews
- ✅ Got job offer with 40-60% salary increase

**Phase 2 Success:**
- ✅ Solved 350+ DSA problems
- ✅ Built Spring Boot microservices
- ✅ Can design complex systems
- ✅ Solved 10+ LLD problems
- ✅ Strong competitive programming skills
- ✅ Got offer from top tech company

### What If You Fail Interviews?

**It's normal.** Even experienced engineers fail interviews.

**What to do:**
1. **Ask for feedback:** Politely request areas to improve
2. **Analyze:** What went wrong? DSA? System design? Behavioral?
3. **Improve:** Focus on weak areas for 2-3 weeks
4. **Reapply:** Wait 6 months for same company, or apply elsewhere
5. **Keep learning:** Every interview is practice

### Motivation

You've already proven you can build real applications. You've worked in production environments. You've delivered value to companies.

**What's missing is not talent—it's practice in interview-specific skills.**

This roadmap gives you the exact path. All you need to do is:
- Show up every day
- Put in the work
- Stay consistent
- Don't give up

### 90-Day Commitment (Phase 1)

For the next 90 days:
- **I will code every single day**
- **I will solve at least 2 DSA problems daily**
- **I will not compare myself to others**
- **I will track my progress**
- **I will not give up**

### Support System

**Join communities:**
- LeetCode Discord
- Reddit: r/cscareerquestions, r/developersIndia
- Twitter: Follow #100DaysOfCode
- Find an accountability partner

**Need help?**
- LeetCode discussion forums
- GeeksforGeeks comment sections
- Stack Overflow
- Discord coding communities

---

## Document Change Log

**Version 1.0 (Current):**
- Complete Phase 1 roadmap (12 weeks)
- Complete Phase 2 roadmap (9 months)
- All chapters with code examples
- Resources and practice platforms
- Weekly schedules
- Interview checklists

**How to use this document:**
1. Print or bookmark this document
2. Read relevant chapter before starting each week
3. Follow the weekly schedule
4. Check off completed topics
5. Track problems solved in a spreadsheet
6. Revisit concepts when needed

---

## Quick Reference: Must-Know Lists

### DSA Must-Know (Write 10 times each)
1. Binary search template
2. Two pointers template
3. Sliding window template
4. DFS traversal (tree + graph)
5. BFS traversal
6. Backtracking template
7. DP patterns (1D, 2D, knapsack)
8. Reverse linked list
9. Merge two sorted lists
10. Inorder/preorder/postorder traversal

### React Must-Know
1. All hooks (useState, useEffect, useContext, useReducer, useRef, useMemo, useCallback)
2. Component lifecycle
3. Context API
4. Performance optimization (React.memo, useMemo, useCallback)
5. Error boundaries
6. React Router
7. Forms (controlled components)
8. State management patterns

### System Design Must-Know
1. Load balancing
2. Caching (types, strategies)
3. Database scaling (sharding, replication)
4. CAP theorem
5. Microservices vs Monolith
6. API design best practices
7. Message queues
8. CDN

### Behavioral Must-Have Stories
1. Technical challenge
2. Project you're proud of
3. Working with team
4. Handling conflict
5. Failure/mistake
6. Taking initiative
7. Meeting tight deadline
8. Learning new technology

---

## Congratulations!

You now have a complete roadmap from where you are to where you want to be.

**The roadmap is clear. The resources are here. The only variable is YOU.**

Start today. Start small. But start.

Week 1, Day 1 starts tomorrow. Open Chapter 1, spend 2-3 hours on JavaScript basics, solve 5 practice problems.

That's it. Just show up tomorrow and do the work.

Then show up the day after. And the day after that.

90 days from now, you'll be a completely different engineer.

9 months from now, you'll be working at a company you dreamed of.

**You've got this. Now go build your future.**

---

**End of Document**

**Total Pages:** ~85-90 pages  
**Total Time Investment Phase 1:** 12 weeks × 25-30 hours = 300-360 hours  
**Total Time Investment Phase 2:** 9 months × 15-20 hours/week = 540-720 hours  
**Total Problems Target:** 350+ DSA problems  

**Created for:** Pavan S J  
**Date:** December 2024  
**Purpose:** Complete interview preparation roadmap from mid-level to FAANG  

**Good luck! 🚀**

