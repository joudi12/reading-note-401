# summery 
## Thinking in React
![image](https://nithuan.files.wordpress.com/2019/03/3231e-1angcizj763gjua05kajf1w.png)
### One of the many great parts of React is how it makes you think about apps as you build them. In this document, we’ll walk you through the thought process of building a searchable product data table using React
1. Step 1: Break The UI Into A Component Hierarchy
2. Step 2: Build A Static Version in React
3. Step 3: Identify The Minimal (but complete) Representation Of UI State
4. Step 4: Identify Where Your State Should Live
5. Step 5: Add Inverse Data Flow



### Lists and Keys
#### First, let’s review how you transform lists in JavaScript.

#### Given the code below, we use the map() function to take an array of numbers and double their values. We assign the new array returned by map() to the variable doubled and log it:
```
const numbers = [1, 2, 3, 4, 5];
const doubled = numbers.map((number) => number * 2);
console.log(doubled);
This code logs [2, 4, 6, 8, 10] to the console.
```
#### In React, transforming arrays into lists of elements is nearly identical.
### Forms
#### Controlled Components
#### In HTML, form elements such as <input>, <textarea>, and <select> typically maintain their own state and update it based on user input. In React, mutable state is typically kept in the state property of components, and only updated with setState().

#### We can combine the two by making the React state be the “single source of truth”. Then the React component that renders a form also controls what happens in that form on subsequent user input. An input form element whose value is controlled by React in this way is called a “controlled component”.





