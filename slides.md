---
theme: apple-basic
background: 'linear-gradient(135deg, #667eea 0%, #764ba2 100%)'
class: text-center
highlighter: shiki
lineNumbers: false
drawings:
  persist: false
transition: slide-left
title: JavaScript Code Golf for Everyone
colorSchema: dark
fonts:
  sans: 'Inter'
  mono: 'Fira Code'
layout: center
style: |
  section {
    display: flex !important;
    flex-direction: column;
    justify-content: center;
    align-items: center;
  }
---

# 🏌️‍♂️ JavaScript Code Golf  
## *Writing the Shortest Code Possible*
---
layout: center
---

# 🎯 What is Code Golf?

**Code Golf** is a programming challenge where the goal is to solve problems using the **fewest characters possible**.

Every character counts like a stroke in golf — the shorter your code, the better your score!

---
layout: center
transition: slide-left
class: text-center
---

# 📚 A Brief History of JavaScript

<div class="max-w-4xl mx-auto grid grid-cols-3 gap-6 mt-10 text-sm text-white/90">

<!-- 1995 -->
<div class="p-4 bg-blue-600/20 rounded-xl shadow animate-fade-in-up">
  <h3 class="text-base font-bold text-blue-300 mb-1">🚀 1995</h3>
  <p>Brendan Eich creates JavaScript at Netscape in just 10 days. First named <em>Mocha</em>.</p>
</div>

<!-- 1997 -->
<div class="p-4 bg-yellow-600/20 rounded-xl shadow animate-fade-in-up delay-100">
  <h3 class="text-base font-bold text-yellow-300 mb-1">📏 1997</h3>
  <p>Standardized as <strong>ECMAScript</strong> to reduce browser quirks.</p>
</div>

<!-- 2005 -->
<div class="p-4 bg-green-600/20 rounded-xl shadow animate-fade-in-up delay-200">
  <h3 class="text-base font-bold text-green-300 mb-1">🌐 2005</h3>
  <p><strong>Ajax</strong> & <strong>jQuery</strong> simplify dynamic web apps.</p>
</div>

<!-- 2009 -->
<div class="p-4 bg-purple-600/20 rounded-xl shadow animate-fade-in-up delay-300">
  <h3 class="text-base font-bold text-purple-300 mb-1">⚙️ 2009</h3>
  <p><strong>Node.js</strong> launches — JavaScript goes server-side.</p>
</div>

<!-- 2015 -->
<div class="p-4 bg-pink-600/20 rounded-xl shadow animate-fade-in-up delay-400">
  <h3 class="text-base font-bold text-pink-300 mb-1">🚀 2015</h3>
  <p><strong>ES6+</strong> brings modern syntax: arrow functions, classes, modules.</p>
</div>

<!-- Today -->
<div class="p-4 bg-cyan-600/20 rounded-xl shadow animate-fade-in-up delay-500">
  <h3 class="text-base font-bold text-cyan-300 mb-1">🌟 Today</h3>
  <p>JS powers web, servers, mobile, desktop, and even IoT.</p>
</div>

</div>
---
layout: center
---

# 🎪 Essential JavaScript Golf Features

<div class="max-w-5xl mx-auto">

<div class="grid grid-cols-2 gap-6 mt-8">

<div class="p-4 bg-blue-500/20 rounded-xl">
<h4 class="font-bold mb-3">🏹 Arrow Functions</h4>
<div class="font-mono text-sm bg-black/20 p-2 rounded">
function(x){return x*2}
<br>
<span class="text-green-400">x=>x*2</span>
</div>
</div>

<div class="p-4 bg-green-500/20 rounded-xl">
<h4 class="font-bold mb-3">❓ Ternary Operator</h4>
<div class="font-mono text-sm bg-black/20 p-2 rounded">
if(x>0)return "pos";else return "neg"
<br>
<span class="text-green-400">x>0?"pos":"neg"</span>
</div>
</div>

<div class="p-4 bg-purple-500/20 rounded-xl">
<h4 class="font-bold mb-3">📋 Array Methods</h4>
<div class="font-mono text-sm bg-black/20 p-2 rounded">
for(let i=0;i&lt;arr.length;i++)...
<br>
<span class="text-green-400">arr.map(x=>...)</span>
</div>
</div>

<div class="p-4 bg-red-500/20 rounded-xl">
<h4 class="font-bold mb-3">🔄 Template Literals</h4>
<div class="font-mono text-sm bg-black/20 p-2 rounded">
arr.join('')
<br>
<span class="text-green-400">arr.join``</span>
</div>
</div>

<div class="p-4 bg-yellow-500/20 rounded-xl">
<h4 class="font-bold mb-3">📦 Spread Operator</h4>
<div class="font-mono text-sm bg-black/20 p-2 rounded">
str.split('')
<br>
<span class="text-green-400">[...str]</span>
</div>
</div>

<div class="p-4 bg-cyan-500/20 rounded-xl">
<h4 class="font-bold mb-3">🔢 Type Tricks</h4>
<div class="font-mono text-sm bg-black/20 p-2 rounded">
parseInt(x) || x===0
<br>
<span class="text-green-400">+x</span>
</div>
</div>

</div>

</div>

---
layout: center
---

# 🎭 JavaScript's "Weird" Behaviors

Don't worry if these look strange - they're JavaScript's quirks that golfers exploit:

<div class="grid grid-cols-2 gap-8 mt-8">

<div class="p-6 bg-blue-500/20 rounded-xl">
<h3 class="text-xl font-bold mb-4">🔢 Number Tricks</h3>
<div class="text-left text-sm space-y-2 font-mono">
<div>+true → 1</div>
<div>+false → 0</div>
<div>+"5" → 5</div>
<div>!!"text" → true</div>
</div>
<p class="text-xs opacity-60 mt-2">Converting things to numbers</p>
</div>

<div class="p-6 bg-green-500/20 rounded-xl">
<h3 class="text-xl font-bold mb-4">📝 String Tricks</h3>
<div class="text-left text-sm space-y-2 font-mono">
<div>[] + [] → ""</div>
<div>5 + "" → "5"</div>
<div>'5' - '2' → 3</div>
<div>'5' + '2' → "52"</div>
</div>
<p class="text-xs opacity-60 mt-2">Converting things to strings</p>
</div>

</div>

<div class="mt-8 p-4 bg-yellow-500/20 rounded-lg">
<strong>🧠 Don't Memorize These!</strong> Just know that JavaScript is very flexible about converting between numbers, text, and true/false values.
</div>

---
layout: center
---

# 📚 Example 1: Basic Function Shortening

<div class="max-w-4xl mx-auto">

## 💼 Production Code
```js
function addNumbers(firstNumber, secondNumber) {
    return firstNumber + secondNumber;
}
```
<div class="text-sm opacity-60 mt-2">📏 91 characters</div>
<div class="mt-8 mb-4">

</div>

## 🏌️‍♂️ Golfed Code
```js
(a,b)=>a+b
```
<div class="text-sm opacity-60 mt-2">⚡ 10 characters</div>

</div>

<div class="mt-8 p-4 bg-purple-500/20 rounded-lg">
<strong>🎯 Golf Trick:</strong> Arrow functions eliminate `function` keyword and braces
</div>

---
layout: center
---

# 🔄 Example 2: Removing Variable Declarations

<div class="max-w-4xl mx-auto">

## 💼 Production Code
```js
function calculateSquare(number) {
    let result = number * number;
    return result;
}
```
<div class="text-sm opacity-60 mt-2">📏 92 characters</div>
<div class="mt-8 mb-4">

</div>

## 🏌️‍♂️ Golfed Code
```js
n=>n*n
```
<div class="text-sm opacity-60 mt-2">⚡ 6 characters</div>

</div>

<div class="mt-8 p-4 bg-purple-500/20 rounded-lg">
<strong>🎯 Golf Tricks:</strong> Single letters + direct calculation
</div>

---
layout: center
---

# 🔢 Example 3: The Ternary Operator Magic

<div class="max-w-4xl mx-auto">

## 💼 Production Code
```js
function checkAge(age) {
    if (age >= 18) {
        return "adult";
    } else {
        return "minor";
    }
}
```
<div class="text-sm opacity-60 mt-2">📏 120 characters</div>
<div class="mt-8 mb-4">

</div>

## 🏌️‍♂️ Golfed Code
```js
a=>a>=18?"adult":"minor"
```
<div class="text-sm opacity-60 mt-2">⚡ 24 characters</div>

</div>

<div class="mt-8 p-4 bg-purple-500/20 rounded-lg">
<strong>🎯 Golf Trick:</strong> Ternary operator replaces entire if/else blocks
</div>

---
layout: center
---

# 🔁 Example 4: Array Processing Shortcuts

<div class="max-w-4xl mx-auto">

## 💼 Production Code
```js
function doubleAllNumbers(numbers) {
    let doubled = [];
    for (let i = 0; i < numbers.length; i++) {
        doubled.push(numbers[i] * 2);
    }
    return doubled;
}
```
<div class="text-sm opacity-60 mt-2">📏 177 characters</div>
<div class="mt-8 mb-4">

</div>

## 🏌️‍♂️ Golfed Code
```js
a=>a.map(x=>x*2)
```
<div class="text-sm opacity-60 mt-2">⚡ 16 characters</div>

</div>

<div class="mt-8 p-4 bg-purple-500/20 rounded-lg">
<strong>🎯 Golf Trick:</strong> Array methods replace entire for loops
</div>

---
layout: center
---

# 📝 Example 5: String Manipulation Tricks

<div class="max-w-4xl mx-auto">

## 💼 Production Code
```js
function reverseString(inputString) {
    return inputString.split('').reverse().join('');
}
```
<div class="text-sm opacity-60 mt-2">📏 94 characters</div>
<div class="mt-8 mb-4">

</div>

## 🏌️‍♂️ Golfed Code
```js
s=>[...s].reverse().join``
```
<div class="text-sm opacity-60 mt-2">⚡ 26 characters</div>

</div>

<div class="mt-8 p-4 bg-purple-500/20 rounded-lg">
<strong>🎯 Golf Tricks:</strong> Spread operator + template literals
</div>

---
layout: center
---

# 🎲 Example 6: Mathematical Calculations

<div class="max-w-4xl mx-auto">

## 💼 Production Code
```js
function calculateFactorial(number) {
    if (number <= 1) {
        return 1;
    } else {
        return number * calculateFactorial(number - 1);
    }
}
```
<div class="text-sm opacity-60 mt-2">📏 161 characters</div>
<div class="mt-8 mb-4">

</div>

## 🏌️‍♂️ Golfed Code
```js
f=n=>n<2?1:n*f(n-1)
```
<div class="text-sm opacity-60 mt-2">⚡ 19 characters</div>

</div>

<div class="mt-8 p-4 bg-purple-500/20 rounded-lg">
<strong>🎯 Golf Tricks:</strong> Compact comparison + recursion
</div>

---
layout: center
---

# 🔍 Example 7: Finding Items in Arrays

<div class="max-w-4xl mx-auto">

## 💼 Production Code
```js
function findMaximumValue(numbers) {
    let maximum = numbers[0];
    for (let i = 1; i < numbers.length; i++) {
        if (numbers[i] > maximum) {
            maximum = numbers[i];
        }
    }
    return maximum;
}
```
<div class="text-sm opacity-60 mt-2">📏 229 characters</div>
<div class="mt-8 mb-4">

</div>

## 🏌️‍♂️ Golfed Code
```js
a=>Math.max(...a)
```
<div class="text-sm opacity-60 mt-2">⚡ 17 characters</div>

</div>

<div class="mt-8 p-4 bg-purple-500/20 rounded-lg">
<strong>🎯 Golf Tricks:</strong> Built-in functions + spread operator
</div>

---
layout: center
---

# 🎯 Example 8: Conditional Logic Chains

<div class="max-w-4xl mx-auto">

## 💼 Production Code
```js
function getGrade(score) {
    if (score >= 90) {
        return 'A';
    } else if (score >= 80) {
        return 'B';
    } else if (score >= 70) {
        return 'C';
    } else {
        return 'F';
    }
}
```
<div class="text-sm opacity-60 mt-2">📏 220 characters</div>
<div class="mt-4 mb-2">

</div>

## 🏌️‍♂️ Golfed Code
```js
s=>s>89?'A':s>79?'B':s>69?'C':'F'
```
<div class="text-sm opacity-60 mt-2">⚡ 33 characters</div>

</div>

<div class="mt-8 p-4 bg-purple-500/20 rounded-lg">
<strong>🎯 Golf Trick:</strong> Chained ternary operators
</div>

---
layout: center
---

# 🚀 Example 9: Advanced Array Creation

<div class="max-w-4xl mx-auto">

## 💼 Production Code
```js
function createNumberSequence(length) {
    let sequence = [];
    for (let i = 1; i <= length; i++) {
        sequence.push(i);
    }
    return sequence;
}
```
<div class="text-sm opacity-60 mt-2">📏 163 characters</div>
<div class="mt-8 mb-4">

</div>

## 🏌️‍♂️ Golfed Code
```js
n=>[...Array(n)].map((_,i)=>i+1)
```
<div class="text-sm opacity-60 mt-2">⚡ 32 characters</div>

</div>

<div class="mt-8 p-4 bg-purple-500/20 rounded-lg">
<strong>🎯 Golf Tricks:</strong> Array constructor + map with index
</div>

---
layout: center
class: text-center
---

# Golf Examples

<div class="mt-4 grid grid-cols-1 gap-3 max-w-2xl mx-auto text-left text-sm">

<!-- FizzBuzz -->
<div class="p-2 bg-red-500/10 border border-red-500/30 rounded-md">
<h3 class="text-base font-semibold text-red-400 mb-1">🔥 FizzBuzz (63 chars)</h3>
<p class="text-xs bg-black/10 p-2 rounded font-mono whitespace-pre-wrap break-words leading-tight">
```js
for(i=0;i++<100;console.log(i%5?f||i:f+"Buzz"))f=i%3?"":"Fizz";
```
</p>
</div>

<!-- Prime Check -->
<div class="p-2 bg-blue-500/10 border border-blue-500/30 rounded-md">
<h3 class="text-base font-semibold text-blue-300 mb-1">🌟 Prime Check (46 chars)</h3>
<p class="text-xs bg-black/10 p-2 rounded font-mono whitespace-pre-wrap break-words leading-tight">
```js
n=>n>1&&![...Array(n)].some((_,i)=>i>1&&n%i<1)
```
</p>
</div>

<!-- Fibonacci -->
<div class="p-2 bg-green-500/10 border border-green-500/30 rounded-md">
<h3 class="text-base font-semibold text-green-300 mb-1">🎨 Fibonacci (24 chars)</h3>
<p class="text-xs bg-black/10 p-2 rounded font-mono whitespace-pre-wrap break-words leading-tight">
```js
f=n=>n<2?n:f(n-1)+f(n-2)
```
</p>
</div>

</div>

<div class="mt-4 text-xs bg-yellow-500/10 border border-yellow-500/30 px-3 py-2 rounded text-center">
<strong>🤯 Did you know?</strong> Some golfers build entire games in under <strong>1024 chars</strong>!
</div>

---
layout: center
class: text-center
background: 'linear-gradient(to bottom, #0f172a, #1e293b)'
---

# 🎯 Code Golfing vs 🕵️ Obfuscation

<div class="grid grid-cols-2 gap-6 text-sm max-w-5xl mx-auto text-left mt-8">

<div class="bg-emerald-800/40 border border-emerald-500 p-6 rounded-2xl shadow-lg text-white space-y-3">
  <h2 class="text-xl font-bold text-emerald-300 mb-2">🏌️ Code Golfing</h2>
  <ul class="list-disc list-inside leading-relaxed space-y-1">
    <li><strong>Goal:</strong> Write the <strong>shortest code</strong> possible</li>
    <li>Used in <strong>fun challenges & contests</strong></li>
    <li>Focuses on <strong>brevity, not readability</strong></li>
    <li><strong>Example:</strong> <code>f=n⇒n&lt;2?n:f(n-1)+f(n-2)</code></li>
  </ul>
</div>

<div class="bg-rose-800/40 border border-rose-500 p-6 rounded-2xl shadow-lg text-white space-y-3">
  <h2 class="text-xl font-bold text-rose-300 mb-2">🕵️ Obfuscation</h2>
  <ul class="list-disc list-inside leading-relaxed space-y-1">
    <li><strong>Goal:</strong> Make code <strong>hard to understand</strong></li>
    <li>Often used to <strong>hide intent or logic</strong></li>
    <li>May involve <strong>encryption or misleading names</strong></li>
    <li><strong>Example:</strong><br>
    <code class="block mt-1 text-xs">var _0x1a3b=["\x63\x6F\x6E\x73\x6F\x6C\x65"];<br>console[_0x1a3b[0]]("hi")</code></li>
  </ul>
</div>

</div>

---
layout: center
class: text-center
background: 'linear-gradient(to bottom, #0f172a, #1e293b)'
---

# 🕵️ Obfuscation

<div class="mx-auto text-left bg-rose-800/40 border border-rose-500 p-6 rounded-2xl shadow-lg text-white text-sm space-y-3">
<pre class="text-xs mt-1 overflow-x-auto p-2 bg-black/40 rounded-lg"><code>а='',б=!а+а,в=!б+а,г=а+{},д=б[а++],е=б[ж=а],
з=++ж+а,и=г[ж+з],б[и+=г[а]+(б.в+г)[а]+в[з]+д+е+б[ж]+и+д+г[а]+е][и](в[а]+в[ж]+б[з]+е+д+"('взломано')")()</code></pre>
</div>

---
theme: default
class: text-center
---

<h1 class="text-6xl font-semibold">Any Questions ❓</h1>
