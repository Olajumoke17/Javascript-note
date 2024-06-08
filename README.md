## String methods;
  **1. String length:** The length property returns the length of a string:
``` javascript
Example;
let text = ["ABCDEFGHIJKLMNOPQRSTUVWXYZ"];
 let length = text.length;
```
  **2. Javascript The charAt()**
 The charAt() method returns the character at a specified index (position) in a string:
```javascript
Example;
let text = "HELLO WORLD";
let char = text.charAt(0);
```
 **3. JavaScript String slice()**
 slice extracts a part of a string and returns the extracted part in a new string.
The method takes 2 parameters: start position, and end position (end not included).
```javascript
Example;
Slice out a portion of a string from position 7 to position 13:
let text = "Apple, Banana, Kiwi";
let part = text.slice(7, 13); 
```
 **4. JavaScript String toUpperCase()**
 A string is converted to upper case with toUpperCase():
```javascript
Example;
let text1 = "Hello World!";
let text2 = text1.toUpperCase();
```

**5. JavaScript String toLowerCase()**
 A string is converted to upper case with toLowerCase():
``` javascript
Example;
let text1 = "Hello World!";
let text2 = text1.toLowerCase();
```
**6. JavaScript String concat()**
 Concat() joins two or more strings:
```javascript
Example;
let text1 = "Hello";
let text2 = "World";
let text3 = text1.concat(" ", text2);
```
The concat() method can be used instead of the plus operator. These two lines do the same:
```javascript
Example;
text = "Hello" + " " + "World!";
text = "Hello".concat(" ", "World!");
```

**7. JavaScript String trim()**
 The trim() method removes whitespace from both sides of a string:
 ```javascript
Example;
let text1 = "      Hello World!      ";
let text2 = text1.trim();
```

**8. JavaScript String trimStart()**
The trimStart() method works like trim(), but removes whitespace only from the start of a string.
```javascript
Example;
let text1 = "     Hello World!     ";
let text2 = text1.trimStart();
```
**9. JavaScript String trimEnd()**
The trimEnd() method works like trim(), but removes whitespace only from the end of a string.
```javascript
Example
let text1 = "     Hello World!     ";
let text2 = text1.trimEnd();
```

**10. JavaScript String repeat()**
The repeat() method returns a string with a number of copies of a string.
The repeat() method returns a new string.
The repeat() method does not change the original string.
```javascript
Examples
Create copies of a text:
let text = "Hello world!";
let result = text.repeat(2);
```
## Array Methods
**1. JavaScript Array length**
The length property returns the length (size) of an array:
```javascript
Example
const fruits = ["Banana", "Orange", "Apple", "Mango"];
let size = fruits.length;
# JavaScript Array at()
```
```
Examples
Get the third element of fruits using at():
const fruits = ["Banana", "Orange", "Apple", "Mango"];
let fruit = fruits.at(2);
answer is apple
```
**2. JavaScript Array join()**
The join() method also joins all array elements into a string. It behaves just like toString(), but in addition you can specify the separator:
```javascript
Example
const fruits = ["Banana", "Orange", "Apple", "Mango"];
document.getElementById("demo").innerHTML = fruits.join(" * ");
Result:
Answer Banana * Orange * Apple * Mango
```
**3. JavaScript Array pop()**
The pop() method removes the last element from an array:
```javascript
Example
const fruits = ["Banana", "Orange", "Apple", "Mango"];
fruits.pop();
```
 **4. JavaScript Array push()**
The push() method adds a new element to an array (at the end):
```javascript
Example
const fruits = ["Banana", "Orange", "Apple", "Mango"];
fruits.push("Kiwi");
```
**5. JavaScript Array shift()**
The shift() method removes the first array element and "shifts" all other elements to a lower index.
```javascript
Example
const fruits = ["Banana", "Orange", "Apple", "Mango"];
fruits.shift();
```
**6. JavaScript Array unshift()**
The unshift() method adds a new element to an array (at the beginning), and "unshifts" older elements:
```javascript
Example
const fruits = ["Banana", "Orange", "Apple", "Mango"];
fruits.unshift("Lemon");
```

**7. JavaScript Array length**
The length property provides an easy way to append a new element to an array:
```javascript
Example
const fruits = ["Banana", "Orange", "Apple", "Mango"];
fruits[fruits.length] = "Kiwi";
```
**8. JavaScript Array delete()**
*Warning !*
Using delete() leaves undefined holes in the array.
Use pop() or shift() instead.
```javascript
Example
const fruits = ["Banana", "Orange", "Apple", "Mango"];
delete fruits[0];
```

**9. JavaScript Array concat()**
The concat() method creates a new array by merging (concatenating) existing arrays:
```javascript
Example (Merging Two Arrays)
const myGirls = ["Cecilie", "Lone"];
const myBoys = ["Emil", "Tobias", "Linus"];
const myChildren = myGirls.concat(myBoys);
```

## Javascript number methods
**1. The valueOf() Method**
valueOf() returns a number as a number.
```javascript
Example;
let x = 123;
x.valueOf();
(123).valueOf();
(100 + 23).valueOf();
```

 **2. The parseInt() Method**
parseInt() parses a string and returns a whole number. Spaces are allowed. Only the first number is returned:

**3.The Number.isInteger() Method**
The Number.isInteger() method returns true if the argument is an integer.
```javascript
Example
Number.isInteger(10);
Number.isInteger(10.5);
```

 **4. The toString() Method**
The toString() method returns a number as a string.
toString()
The .toString() method converts a numeric value into a string.
```javascript
 Example 1
let x = 10
let num = x.toString()
console.log(num)                // Output: '10'
```
```
All number methods can be used on any type of numbers (literals, variables, or expressions):
```
```
Example
let x = 123;
x.toString();
(123).toString();
(100 + 23).toString();
```
**5. JavaScript Number Format** Number()
The Number() method converts a string into a number.
```javascript
 Example 1
let x = '10'
let num = Number(x)
console.log(num)                 // Output: 10
console.log(num * 9)             // Output: 90
```


 **6. parseFloat()**
The .parseFloat() method parses a string value and returns the number with its decimal value.
```javascript
// Example 1
let x = '10.99'
let num = parseFloat(x)
console.log(num)                 
```

**7. toPrecision()** 
toPrecision() returns the numeric value with a specific length. It takes an argument that signifies the length. If given without a specific length, the method returns the number as it is.
```javascript
 Example 1
var num = 456.789;
```

**8. valueOf()**
The valueOf() method is used to return the primitive value of the Number object you’re calling it on. Primitive types in JavaScript are number, string, bigint, symbol, undefined, null, and boolean.
```javascript
let x = 45
let num = x.valueOf()
console.log(num)                 // Output: 45
console.log(typeof num);         // Output: Number
```

**9. toLocaleString()**
The toLocaleString() method uses a local language format to convert a number and returns it as a string. It takes two arguments, locales and options , which defines the language of which conversion you want to use, and the behavior of the function.
```javascript
Example;
obj.toLocaleString([locales[, options]])
let num = 226537.883;
//US English
console.log(num.toLocaleString('en-US'));     Output: 226,537.883
```

**10. isInteger()**
.isInteger() checks whether the given value is an integer and returns a boolean value.
```javascript
Example 1
let x = 10
let num = Number.isInteger(x)
console.log(num)                     // Output: true
```

**11. isFinite()**
.isFinite() checks whether the given value is finite and returns a boolean value.
```javascript
//Example 1
let x = 10
let num = Number.isFinite(x)
console.log(num)                     // Output: true
```