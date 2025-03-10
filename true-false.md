# Truthy Values (Evaluate to true)
"Hello" → Non-empty string
42 → Any non-zero number
-1 → Negative numbers
[] → Empty array
{} → Empty object
Infinity → Positive infinity
-Infinity → Negative infinity
function() {} → Any function
new Date() → A valid date object
true → The Boolean value true


# Falsy Values (Evaluate to false)
"" → Empty string
0 → Zero
-0 → Negative zero
null → Null value
undefined → Undefined value
NaN → Not a Number
false → The Boolean value false
0n → BigInt zero
document.all → A special falsy value in browsers
null == undefined → Both are falsy in comparisons




# JavaScript Truthy and Falsy Values

## 📌 Understanding Truthy and Falsy Values in JavaScript

In JavaScript, values are either **truthy** (evaluate to `true`) or **falsy** (evaluate to `false`) in a Boolean context.

---

## ✅ **Truthy Values (Evaluate to `true`)**
The following values are **truthy** in JavaScript:

```javascript
if ("Hello") {
    console.log("Truthy: Non-empty string");
}

if (42) {
    console.log("Truthy: Number is not zero");
}

if (-1) {
    console.log("Truthy: Negative numbers count");
}

if ([]) {
    console.log("Truthy: Empty array");
}

if ({}) {
    console.log("Truthy: Empty object");
}

if (Infinity) {
    console.log("Truthy: Positive infinity");
}

if (-Infinity) {
    console.log("Truthy: Negative infinity");
}

if (function() {}) {
    console.log("Truthy: Function is always truthy");
}

if (new Date()) {
    console.log("Truthy: Date object is valid");
}

if (true) {
    console.log("Truthy: Boolean true is truthy");
}



if (false) {
    console.log("Falsy: Boolean false"); // ❌ No output
}

if ("") {
    console.log("Falsy: Empty string"); // ❌ No output
}

if (0) {
    console.log("Falsy: Zero"); // ❌ No output
}

if (-0) {
    console.log("Falsy: Negative zero"); // ❌ No output
}

if (null) {
    console.log("Falsy: Null value"); // ❌ No output
}

if (undefined) {
    console.log("Falsy: Undefined value"); // ❌ No output
}

if (NaN) {
    console.log("Falsy: NaN (Not a Number)"); // ❌ No output
}

if (0n) {
    console.log("Falsy: BigInt zero"); // ❌ No output
}

if (document.all) {
    console.log("Falsy: Special browser value"); // ❌ No output
}

if (null == undefined) {
    console.log("Falsy: Null and undefined are loosely equal");
}
