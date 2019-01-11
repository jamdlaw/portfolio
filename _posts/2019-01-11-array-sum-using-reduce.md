---
layout: post
title: "Use The reduce() function to sum inventory"
categories: mics
---

I highly recommend taking a course call <a href="https://javascript30.com/">javascript30</a>, by Wes Bos. It is a free class and you will learn a lot of really good javascript stuff in bit size amounts. Below is a code snippet from that class, but modified to show how it can be used to quickly count inventory stored in an array. 

{% highlight javascript %}
	const data = ['Red Shirt', 'Red Shirt', 'Blue Shirt', 
				'Blue Shirt', 'Green Shirt', 'Black Shirt', 'Red Shirt',
				 'Pink Shirt', 'Green Shirt', 'Black Shirt', 'Red Shirt',
				 'Pink Shirt', 'Red Shirt', 'Blue Shirt', 'Orange Shirt'];
const inventorySum = data.reduce(function(obj, item) {
  if (!obj[item]) {
    obj[item] = 0;
  }
  obj[item]++;
  return obj;
}, {});
console.log(inventorySum);
{% endhighlight%}
 
