# Entry 1: Deciding on a tool, and a project idea
##### 11/14/26

# Introduction
After playing around with my tool, `math.js`, I was able to create a working calculator that takes in large equations, and outputs large values. It also can handle multiplication, division, addition, subtraction, exponents, and parentheses. The main purpose of this is to make a math learning game which I believe that it will help more people be qualified to get into government jobs, big tech, education, and more. It will help solve problems in order to reduce or stop waste. People will get smarter, get jobs, and pass their exams. However some people love math way too much and compete with others on who can do math better, and faster. On the other hand it will give people opportunities to get jobs in finance, banking, quant, but also creates lots of competition in that area.

I decided to use Math.js because it is one of the most popular, easy to use math libraries in Javascript. One of its most useful features is Expression Parser, which allows me to evaluate math strings, define custom functions, and compute symbolic expressions.

Compared to regular JavaScript, Math.js provides an extensive math library with support for complex, large numbers, fractions, matrices, and much more it has to offer. What makes this library different from the built-in Javascript math library is that it's limited to basic operations, while math.js expands the language, and the kinds of projects you can build.

# Development, and Challenges
The first thing I worked on was creating a calculator. To code it, I used the `input`, and `output` which created a text, and output box which the user could input their equation, and get a value back.

Code:
```js
<input id="input" oninput="out.value = eval(value.replace(/(\d)\(/g, '$1*(').replace(/\^/g, '**'))"> 
<h1><output id="out">Welcome to my Calculator</output></h1>
```

One important function I learned was `.replace()`, which replaced exponents `^` into `**` and inserted a multiplication sign in front of parentheses, converting implicit multiplication into explicit multiplication. This solved two problems I faced during development. The first problem was that exponents weren't working because JavaScript uses double asterisks (`**`) for exponentiation instead of the caret symbol (`^`). The second problem was that JavaScript doesn't automatically recognize implicit multiplication, such as `3(5)`, so I had to insert a multiplication sign in front of parentheses to make it work properly.

# Engineering Design Process
Currently, I am in Stage 7 of the Engineering Design Process because I'm trying to make `Math.js`, and `KaTeX` work together to make beautiful math, and equations that the user can input or solve.

Moving forward, I plan on creating a math learning game using Math.js to evaluate math equations, and paired with KaTeX to display clean math notation instead of just plain text.

I also want to implement randomized math equations, which will allow players to infinitely get random math problems based on the level they choose that they want to solve.

# Skills
One skill I have developed is learning on my own. I improved this skill by reading the [Math.js Documentation](https://mathjs.org/docs/index.html), and looking at [Mozilla](https://developer.mozilla.org) docs. For example, I have learned to somewhat use .replace, and math.evaluate to evaluate the expressions. and another skill I have developed is Problem Solving. I used this skill while trying to fix my calculators implicit multiplication, and exponentiation. by reading the Mozilla docs.

* Sources: [Math.js Download](https://mathjs.org/download.html), [Math.js Documentation](https://mathjs.org/docs/index.html), [Math.js Examples](https://mathjs.org/examples/index.html), [Mozilla Replace Function](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String/replace), [KaTeX](https://katex.org/), [KaTex Docs](https://katex.org/docs/api).

[Next](entry02.md)

[Home](../README.md)
