# Understanding TypeScript Types: A Gentle Introduction


If you are new to Typescript, you may have come across the word "types" quite often. Don’t worry, it’s not as scary as it sounds. 

In this article, I will explain what TypeScript is, what types are, why they matter, and examples of them in TypeScript.
By the end, you will have a basic understanding of how types work in TypeScript. 


>Note that this is a gentle introduction to types. If you want something complex, visit the [Typescript documentation](https://www.typescriptlang.org/docs/).
>You don’t need a previous knowledge of Typescript or Javascript to read this article.

## What is Typescript
To understand Typescript, think of TypeScript like adding labels to your boxes to remind you what's inside them. For example, if you have a box labeled "numbers only," you can't accidentally put a string (text) inside. This helps you stay organized and avoid mistakes.

TypeScript is an improved version of JavaScript, one of the popular languages for building web applications and websites.
It improves Javascript by addding an extra feature called types to help make codes and writing Javascript clearer and prevent errors.


## What are "Types" in TypeScript?
Imagine you have different items like shoes, books, and bottles. You wouldn’t want to mix them all together, right? You will organize them into separate groups. That’s what **types** do in TypeScript. 

Types act like labels that help organize information (data) in your program. They tell you and the computer what kind of data you are working with.

In simple terms, a type tells the computer what something is, so it knows how to handle it properly. For example, is it a number? A word (text)? Or a true/false statement? 


## Why does Types matter?
Types matter because they help you avoid mistakes when writing code. Imagine trying to add two numbers together like 7 + 10, but instead of using a number, you accidentally use a word like 7 + "hello". That’s a mistake that could break your program.
TypeScript will stop you and say,**“Hey, something is not right here!”**

Here is why types are important:
- TypeScript warns you if you try to do something that doesn’t make sense (like adding a word to a number).
- Types make your code easier to read and understand for both you and others.
- Types help ensure that your program behaves the way you expect it to.

>If you make a mistake, TypeScript will give you a warning before you even run the program.


## Common types in Typescript
Let’s look at some of the most common types in TypeScript. These are like the most basic “boxes” you will use to store data. Here are the most common types you will use in TypeScript:
Don’t worry if this feels like a lot, you will get used to it as you practice.

### Number
This type is used for numbers. It can be whole numbers like 1, 2, 3, or decimal numbers like 3.15.

**Example:**
```
let age: number = 29; 
```


**Explanation:**
- Here, age is a number, and we are telling TypeScript that it will always be a number.

### String
This type is used for text or words, like "hello" or "Nancy."

**Example:**
```
let name: string = "Nancy";
```
**Explanation:**
- In this example, name is a string, and we have assigned it the text “Nancy.”

### Boolean
This type is used for true or false values. It is useful when you want to know if something is either  true or false, yes or no,

**Example:**
```
let isHappy: boolean = true;
```
**Explanation**
- isHappy is a boolean type, and we have said that it is true.

## More complex Types in Typescript
Once you are comfortable with basic types like numbers, strings, and booleans, you can explore more complex types that allow you to handle multiple pieces of data at once.
Here are a some complex Types:

### Array
An array is like a list where you can store multiple values of the same type. For example, a list of numbers:

**Example:**
```
let scores: number[] = [11, 20, 40];
```
**Explanation:**
- This is a list (array) of numbers: 11, 20, and 40. Arrays are stored inside square brackets []  Like seen in the previous example.


### Object
An object is a collection of related information, where each piece of data is labeled. Imagine you want to store a person’s name and age:

**Example:**
```
let person: { name: string, age: number } = { name: "Nancy", age: 28 };
```
**Explanation:**
- In this case, the person has a name (which is a string) and an age (which is a number).

### Simple Example: Adding Two Numbers
Imagine we want to add two numbers together and display the result. You can use TypeScript to make sure you are really working with numbers. Here is how it looks:

```
let num1: number = 7;
let num2: number = 10;
let result: number = num1 + num2;

console.log(result); // Output: 17
```
**Explanation:**
- You tell TypeScript that both num1 and num2 are numbers.
- You also tell it that result will be a number.
- When you run the program, it adds num1 and num2 together and prints 17 on the screen.

#### If you try to add a number to a string (text), TypeScript will stop you, Like so:
```
let num1: number = 7;
let num2: string = "Nancy"; // TypeScript will show an error here.
let result: number = num1 + num2; // This will cause an error because you can't add a number and a word.
```
>This warning helps you fix the mistake before your program breaks.

## Conclusion
Understanding types in TypeScript is important because it help you avoid common mistakes, make your code clearer, and ensure your programs work as expected. 
It can be overwhelming at first but as you continue to learn TypeScript, types will become easier to use. You doing great!

