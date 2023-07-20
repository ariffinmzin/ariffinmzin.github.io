---
title: "JavaScript Equality"
author: ariffin
date: 2023-07-20 23:15:00 +0800
categories: [Blogging, JavaScript]
tags: [javascript]
---

# 😃 JavaScript Equality Showdown: `==` vs `===` and `!=` vs `!==`

Hey there, coding buddies! 🖐️ Today, I want to dish out all the deets about a JavaScript topic that's been on my radar: the crazy cool difference between `==` and `===`, and `!=` and `!==`. At first, they looked like twins to me, but when I started to get my hands dirty, their unique quirks became super clear. Let's dive right in! 🏊‍♀️

## My Meet-cute with the Loose Equality Operator: `==`

First up is the `==` operator, the loosey-goosey equality operator. 😜 It's all about comparison but it first transforms the values to a common type - type coercion, in fancy terms. 🎩

Check this out:

```javascript
console.log(1 == "1"); // Outputs: true
```

Yeah, one is a number and the other is a string, but JavaScript doesn't sweat the small stuff. It converts the string to a number before the comparison and voila, both sides are equal! 🤷‍♂️

## Bumping Into the Strict Equality Operator: `===`
Next on the menu, `===`, the no-nonsense equality operator. This guy only says `true` if the operands are of the same type and contain the same value. No more, no less.

Here's what happened when I put it to the test:

```javascript
console.log(1 === "1"); // Outputs: false
```

Even though `"1"` looked the same, it was a string and not a number, and that made all the difference. 🕵️‍♂️

## The Unpredictable Loose Inequality Operator: `!=`
Moving on to `!=`, the loose inequality operator. It's a fun one! It says `false` if the operands become equal after some of that handy type coercion.

Take a look:

```javascript
console.log(1 != "1"); // Outputs: false
```
Type coercion steps up again, making the string a number and leaving both sides of the equation as equals. 🧮

## Meeting the Strict Inequality Operator: `!==`
Finally, `!==`, the operator that means serious business. It returns `true` if the operands are different types or if they're the same type but have different values.

And...action! 🎬

```javascript
console.log(1 !== "1"); // Outputs: true
```

No surprises here! `1` and `"1"` are different types, so `!==` gives a thumbs up. 👍

## Which One Am I Taking to the Dance?
While I've had fun with both loose and strict operators, I've found it's generally cooler to go with `===` and `!==` in JavaScript. They're like that reliable friend who's always there - no sudden surprises. 😌

But hey, `==` and `!=` have also had my back when I wanted type coercion on purpose. 🎭

I guess it's all about understanding these cool tools and using them the right way for what I want to achieve. So, whenever I'm about to drop a `==`, `===`, `!=`, or `!==`, I take a sec to think about which one is right for the situation. 🤔

That's a wrap for today! Stay tuned as I keep exploring the wild world of JavaScript, where the aim is to code smarter, not harder! Keep coding and keep smiling, my friends! 😄