---
title: "Working with CSS in Your React Application"
author: ariffin
date: 2023-07-27 00:05:00 +0800
categories: [Blogging, React]
tags: [React]
---

# Working with CSS in Your React Application: Let’s Jazz Up That App.css! 🎨

Hello, code whisperers! 😊 You've ventured into the territory of React. Congrats! 🎉 But if you've found that your React app is looking a bit, well, vanilla, it's time to spruce things up a bit with CSS. Don't worry; I'm here to guide you through it.

I'm going to use the default App.css file that comes bundled in when you create a new React project. You might have deleted it or ignored it up until now, but today it's time to show it some love. Ready? Let's dive in! 🏊‍♂️

## 1. Setting the Stage with App.css 💻

To kick things off, locate the App.css file in your project directory. If you can't find it, no worries; you can always create a new CSS file and import it in your App.js file. It's usually in the 'src' directory and should look a little something like this:

```css
.App {
  text-align: center;
}

.App-logo {
  height: 40vmin;
  pointer-events: none;
}
```

The ".App" and ".App-logo" are class selectors. They're used to style HTML elements with the corresponding class.

## 2. Add Your Styles 🎨
You're the artist here! 🖌️ Get creative! Want to change the background color of your app? Easy peasy! Let's give it a background color of light blue because why not? It's summer! 🌞

```css
.App {
  text-align: center;
  background-color: lightblue;
}
```

Maybe you're more adventurous and want to spin the React logo (which is generally the App-logo class)? Just add some animation! 🎡

```css
.App-logo {
  animation: App-logo-spin infinite 20s linear;
  height: 40vmin;
  pointer-events: none;
}

@keyframes App-logo-spin {
  from {
    transform: rotate(0deg);
  }
  to {
    transform: rotate(360deg);
  }
}
```

And voilà! Your logo now spins continuously. Neat, huh? 😎

## 3. Apply Your Styles to Components ✨
Now that you have some flashy styles defined, let's get them into our components! Here's a refresher on how you might have your App.js set up:

```jsx
import React from 'react';
import './App.css';

function App() {
  return (
    <div className="App">
      <header className="App-header">
        <img src={logo} className="App-logo" alt="logo" />
        <p>
          Edit <code>src/App.js</code> and save to reload.
        </p>
        <a
          className="App-link"
          href="https://reactjs.org"
          target="_blank"
          rel="noopener noreferrer"
        >
          Learn React
        </a>
      </header>
    </div>
  );
}

export default App;
```

To apply your CSS styles, you just need to make sure your component has the corresponding class name. That's what "className" is doing here. It's the React way of saying "class". See, React isn't too bad! 😉

Just make sure that you've imported your App.css at the top of your App.js file with `import './App.css';`.

## 4. Transform App.css into a CSS Module and Import it 🚀
Are you ready to level up? 🏋️‍♀️ Let's take this a step further and turn our App.css into a CSS module. By doing this, we can scope our CSS to the components where it is imported. This way, we can avoid naming collisions and keep our CSS tidy. Ready? Let's dive in! 🏊‍♂️

First, rename your `App.css` file to `App.module.css`. This tells Create React App to treat this CSS file as a CSS module.

Your App.module.css file will look like this:

```css
.App {
  text-align: center;
  background-color: lightblue;
}

.App-logo {
  animation: App-logo-spin infinite 20s linear;
  height: 40vmin;
  pointer-events: none;
}

@keyframes App-logo-spin {
  from {
    transform: rotate(0deg);
  }
  to {
    transform: rotate(360deg);
  }
}
```

Nothing changed here, right? Well, the magic happens in your `App.js` file. Update the import statement to match the new filename, and import it as `styles`:

```jsx
import React from 'react';
import styles from './App.module.css';
```

Now, rather than using strings for class names, we use the `styles` object:

```jsx
function App() {
  return (
    <div className={styles.App}>
      <header className={styles['App-header']}>
        <img src={logo} className={styles['App-logo']} alt="logo" />
        <p>
          Edit <code>src/App.js</code> and save to reload.
        </p>
        <a
          className={styles['App-link']}
          href="https://reactjs.org"
          target="_blank"
          rel="noopener noreferrer"
        >
          Learn React
        </a>
      </header>
    </div>
  );
}

export default App;
```

Et voilà! 🎉 You've just transformed your App.css into a CSS module. Now your styles are scoped to your component, which means you can reuse class names in other components without worry. It's like having your own little CSS namespace! 😊

### 5. Celebrate! 🎊
And that's all folks! You've jazzed up your React application using your trusty sidekick, CSS. Now your app has that little extra something to make it shine. 🌟

Remember, CSS is just like any other part of coding. It can seem complicated and sometimes even frustrating, but with practice, you'll get the hang of it. Don't give up, and keep experimenting! 💪😀

Thanks for tuning in, and happy coding! 🚀