---
title: "Writing Your First React Application"
author: ariffin
date: 2023-07-22 00:24:00 +0800
categories: [Blogging, React]
tags: [React]
---

# Writing Your First React Application in VS Code: An Approachable Guide 🚀

Hey, folks! 👋 Hope you're having a fantastic day! Today, we're going to explore the wild and wonderful world of React.js. Buckle up as we create our very first React application using the marvelously versatile Visual Studio Code (VS Code). 😄 If you're a newbie in this space, don't fret. This guide is meant to be as approachable and as newbie-friendly as possible.

Alright, let's dive in! 🏊

## Prerequisites 🛠️

Before we get started, there are a couple of things you need to have installed on your machine:

1. **Node.js and npm**: We'll be using Node.js as our runtime and npm (which comes with Node.js) as our package manager. Download the latest LTS (Long Term Support) version from [here](https://nodejs.org/).

2. **Visual Studio Code**: This will be our text editor of choice for this tutorial. Download it from [here](https://code.visualstudio.com/).

## Step 1: Setting Up The Project 🚧

First, we're going to create a new React application. Open your terminal or command prompt and navigate to the directory where you'd like to create your project. Enter the following command:

```bash
npx create-react-app my-first-react-app
```

Sit back and relax as `create-react-app` sets up a new React application for you, with all the bells and whistles already configured. Once it's done, navigate into your new project's directory:

```bash
cd my-first-react-app
```

## Step 2: Opening the Project in VS Code 📂
Once you're in your project's directory, launch VS Code and open the project. You can do this in one of two ways:

* Run `code .` in your terminal if you have added VS Code to your PATH.
* Or simply open VS Code, click on `File > Open...` and navigate to your project's directory.
There you go! You should now see your new React app opened in VS Code. You'll notice several directories and files. Don't worry, we'll get to those later. 😎

## Step 3: Let's Understand The File Structure 📚
At first glance, the file structure of a React app can feel a little overwhelming. But once you get the hang of it, you'll realize it's beautifully organized:

* `public/`: This directory contains the static files of your application, including `index.html` where the magic of React gets attached. 🎩
* `src/`: This is where your React components live, along with their CSS and tests. 🏠
* `package.json`: This file manages dependencies, scripts, and other metadata about your project. 📜

## Step 4: Your First React Component 🧩
For simplicity, let's create a new component within the `src/` directory. Create a new file, name it `Greeting.js`, and paste the following code:

```jsx
import React from 'react';

function Greeting() {
  return (
    <h1>Hello, World!</h1>
  );
}

export default Greeting;
```

In this file, we create a functional component (Greeting) that simply renders an h1 tag with the text 'Hello, World!'. 🌍

## Step 5: Rendering the Greeting Component 🎨
To render this component, open `src/App.js`, delete the existing code within the `App` component, and import the `Greeting` component:

```jsx
import React from 'react';
import './App.css';
import Greeting from './Greeting';

function App() {
  return (
    <div className="App">
      <Greeting />
    </div>
  );
}

export default App;
```

## Step 6: Running The App 🏃
To view your masterpiece, simply open your terminal and enter:

```bash 
npm start
```

This will start the development server and open your default browser at `http://localhost:3000`. You should see your glorious "Hello, World!" greeting staring back at you! 🎉

That's it! You've just built your first React app using Visual Studio Code. 🥳

React has a lot more to offer, like state management, lifecycle methods, hooks, and more. But as with anything new, baby steps. We'll get there! 👣

Remember, the key to mastering anything is consistency and practice. So keep tinkering, keep exploring, and above all, have fun! 🎈

See you in the next one, happy coding! 🚀