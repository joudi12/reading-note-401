# summery
# React Introduction
![image2](https://blog.paradisetechsoft.com/content/images/2019/08/image_2019_08_29T07_08_07_366Z.png)


React is a JavaScript library that aims to simplify development of visual interfaces.

Developed at Facebook and released to the world in 2013, it drives some of the most widely used code in the world, powering Facebook and Instagram among many, many other software companies.

Its primary goal is to make it easy to reason about an interface and its state in any point in time, by dividing the UI into a collection of components.

React is used to build single-page web applications, among with many other libraries and frameworks that were available before React came into life.


## JSX
![image](https://res.cloudinary.com/practicaldev/image/fetch/s--jaFWlQCW--/c_imagga_scale,f_auto,fl_progressive,h_420,q_auto,w_1000/https://dev-to-uploads.s3.amazonaws.com/i/bqc1gncxdhau0zfuxqmp.png)

Instead of artificially separating technologies by putting markup and logic in separate files, React separates concerns with loosely coupled units called “components” that contain both. We will come back to components in a further section.






JSX is an extension to JavaScript which allows you to declaratively create custom UI components. JSX has important benefits:

* Easy, declarative markup.
* Colocated with your component.
* Separate by concern, (e.g., UI vs state logic, vs side-effects) not by technology (e.g., HTML, CSS, JavaScript).
* Abstract away DOM differences.
* Abstract away from underlying tech so you can target many different platforms with React. (e.g., ReactNative, VR, Netflix Gibbon, Canvas/WebGL, email, ...)



##### Example:

```
const name = 'Josh Perez';
const element = <h1>Hello, {name}</h1>;

ReactDOM.render(
  element,
  document.getElementById('root')
);
```
We declare a variable called name and then use it inside JSX by wrapping it in curly braces. You can put any valid JavaScript expression inside the curly braces in JSX. 

______________________________________________________________________

## Rendering Elements

Elements are the smallest building blocks of React apps, and they describes what you want to see on the screen. Unlike browser DOM elements, React elements are plain objects, and are cheap to create. React DOM takes care of updating the DOM to match the React elements.

Example:

```
const element = <h1>Hello, world</h1>;
```

To render an element into the DOM, first give it san id, usually it will be called 'root'. Applications built with just React usually have a single root DOM node. If you are integrating React into an existing app, you may have as many isolated root DOM nodes as you like.


To render a React element into a root DOM node, pass both to ReactDOM.render():

```html
<div id="root"></div>
```

```javascript
const element = <h1>Hello, world</h1>;
ReactDOM.render(element, document.getElementById('root'));
```
______________________________________

## Components and Props

Components let you split the UI into independent, reusable pieces, and think about each piece in isolation.

Conceptually, components are like JavaScript functions. They accept arbitrary inputs (called “props”) and return React elements describing what should appear on the screen.

**Function and Class Components**

```javascript
function Welcome(props) {
  return <h1>Hello, {props.name}</h1>;
}
```

##### Rendering a Component

For example, this code renders “Hello, Sara” on the page:

```javascript
function Welcome(props) {
  return <h1>Hello, {props.name}</h1>;
}

const element = <Welcome name="Sara" />;
ReactDOM.render(
  element,
  document.getElementById('root')
);
```




1. We call ReactDOM.render() with the < Welcome name="Sara" /> element.
1. React calls the Welcome component with {name: 'Sara'} as the props.
1. Our Welcome component returns a < h1>Hello, Sara< /h1> element as the result.
1. React DOM efficiently updates the DOM to match < h1>Hello, Sara< /h1>.

_____________________________________________












