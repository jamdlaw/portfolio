---
layout: post
title: "Apply function in Javascript to extend arrays"
categories: javascript
---

The apply function is Javascript does basically the same thing as the call function. BUT it has one distinct advantage to us as everyday programmers. Unlike the *call* function which takes in a variable(s) as the parameter(s) to execute a function against. The *apply* function takes an array. 
This may sound like a small difference, but when you think about the fact that a lot of data is stored in arrays already this function has a huge advantage to us as everyday programmers. 
I thought that was the end of what I wanted to know about the function, but then I did some reading online and come to find out there is another HUGE advantage to the apply function that I did not realize at first. Credit to [www.w3schools.com]("https://www.w3schools.com/js/js_function_apply.asp") for explaining how you can extend the Math objects functionality and run them on arrays using *apply*. A quick example of this would be if we had a an array of scores 

```javascript
	let scores = [100, 22000, 5000, 300 ];
```

And we wanted to get the high score from this array we can do it in one line such as 

```javascript
	let highScore = Math.apply.max(null, scores);
```

So the full script would be 
```javascript
let scores = [100, 22000, 5000, 300 ];
let highScore = Math.max.apply(null, scores);
console.log(highScore);
```

As the blog post above has pointed out arrays do not have a *max* function so using apply to barrow the functionality found in Math.max is a powerful way to extend the functionality of other already existing data stored in arrays, let your imagination run wild. 


