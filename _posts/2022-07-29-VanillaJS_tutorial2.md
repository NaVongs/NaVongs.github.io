---
layout: post
title: JS 입문 2
subtitle: JavaScript
categories: Language
tags: [JS, Nomad Coder, web]
---



## Link JS with HTML


{% highlight javascript%}
const title = document.getElementById("title");

console.dir(title);

title.innerText = "New Text";
{% endhighlight %}

Object "Document" let JS be able to access HTML elements.  
**getElementByID, getElementByClassname, getElementByTagname.. etc**  

Nomad's Suggestion : **querySelector, querySelectorAll**

{% highlight javascript %}
const title = document.qeurySelector("div.class_name:first-child h1");
//Maybe I can erase 'div'

console.log(title);
title.innerText = "new_text";

{% endhighlight %}

We can use 'console' object to check condition of object: console.log, console.dir, etc...


## Event check

{% highlight javascript %}
function handleTitleClick(){
    console.log("title was clicked!");
    title.innerText = "title Clicked!";
    title.style.color = "red";
}


title.addEventListener("click", handleTitleClick);
{% endhighlight %}

We can 'listen' events of HTML: name of properties starts with 'on'. Name of events can be also found googling 'Web APIs'.