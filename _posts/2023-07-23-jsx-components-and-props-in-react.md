---
title: "JSX, Components, and Props in React"
author: ariffin
date: 2023-07-23 23:50:00 +0800
categories: [Blogging, React]
tags: [React]
---

# Spicing Up Your UI with JSX, Components, and Props in React! 😎
Hello, fellow coders! 👋 Get ready, as we're about to dive deep into the magical world of React.js, a place where JSX, components, and props are the superheroes saving the day. It's like the Avengers, but for web development. 🦸‍♂️💻

## So, What's the Deal with JSX? 🤔
JSX, or JavaScript XML, is a syntax extension for JavaScript. It allows us to write HTML in our React code. It's like chocolate and peanut butter—two great tastes that taste great together! 🍫🥜

Think about it this way: In a typical HTML file, you might have a `div` like this:

```html
<div>Hello, World!</div>
```
With JSX, you can write that same `div` in your JavaScript files. So, it looks like this:

```jsx
const element = <div>Hello, World!</div>;
```
Crazy cool, right? 😲

## Getting Comfy with Components 🛋
Next on our list are components. In React, everything is a component. You can think of a component as a self-contained piece of code that manages some part of the UI.

It's like building with LEGO blocks 🧱. Each block (component) has a specific role, and when you put them together, you create an impressive structure (your app).

Here's a simple example of a functional component in React:

```jsx
function Welcome(props) {
  return <h1>Hello, {props.name}</h1>;
}
```

In this example, `Welcome` is a functional component that takes an argument, `props`, and returns a React element. If we wanted to use this `Welcome` component, we would write something like this in our JSX:

```jsx
<Welcome name="Tony Stark" />
```

Which would render "Hello, Tony Stark" on the screen. Who knew we could have Iron Man on our web page with just a few lines of code? 🤩

## Now, Let's Get Our Hands Dirty 👐💻
So, we've chatted a fair bit about JSX, components, and props in React. But as we all know, when it comes to coding, seeing is believing—and doing is understanding. So, let's walk through a simple React program that combines all these elements. Prepare yourself for some real React action! 🎬

```jsx
// Importing the necessary React library and CSS
import React from 'react';
import './App.css';

// Creating a functional component named `Welcome`
function Welcome(props) {
  return <h1>Hello, {props.name}</h1>;
}

// Creating another functional component named `App`
function App() {
  return (
    <div className="App">
      <Welcome name="Tony Stark" />
      <Welcome name="Steve Rogers" />
      <Welcome name="Natasha Romanoff" />
    </div>
  );
}

// Exporting the App component as default
export default App;
```

Let me break this down for you! 🕵️‍♂️💡

In this program, we're creating an `App` component that returns a `div` containing multiple `Welcome` components. Each `Welcome` component receives a `name` prop and renders a message welcoming that name. So, our app is essentially throwing a welcome party for the Avengers. Yeah, you heard that right! 🎉

The `App` component is exported as default from this `App.js` file. Think of `App` as the master of ceremonies at our welcome party, telling every other component where to go and what to do. It’s like the Nick Fury of our Avengers team, leading the way! 🕶️🌐

And voila! You've just created your first small React application! 🥳

## Wrapping Up 🎁
There you have it, folks! We've explored the ins and outs of React.js, from understanding JSX, components, and props, to applying them in a practical React program. Now, you're all set to step into the React world and build some awesome web applications.

Remember, like any superpower, mastering React takes practice. So, keep building, keep experimenting, and keep having fun. You're on your way to becoming a web development superhero! 🦸‍♀️💻🎉

In the wise words of Tony Stark, "Sometimes you gotta run before you can walk." So, take your newfound knowledge and run with it! 🚀

Happy coding! 😄
