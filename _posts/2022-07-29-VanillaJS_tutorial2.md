---
layout: post
title: JS 입문 2
subtitle: JavaScript
categories: NomadCoders
tags: [JS, Nomad Coder, Web]
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
    title.style.color = "red"; //changing CSS w/ JS
    
}


title.addEventListener("click", handleTitleClick);
{% endhighlight %}

We can 'listen' events of HTML: name of properties starts with 'on'. Name of events can be also found googling 'Web APIs'.

Anothe way to check event is using *oneventname* properties.
But handling branch with changing classname can make some problem: cause it loses previous name.

**Use CSS class to toggle**
{% highlight javascript %}
function handleTitleClick(){
    const clickedClass = "clicked";
    if(h1.classList.contains(clickedClass)){
        h1.classList.remove(clickedClass);
    }
    else{
        h1.classList.add(clickedClass);
    }
    
}


h1.addEventListener("click", handleTitleClick);
{% endhighlight %}

{% highlight CSS %}
h1{
    color: green;
}

.some{
    color:#ff00ff;
}

.clicked{
    color: #00aaaa;
    font-family: 'Courier New', Courier, monospace;
    transition: color 0.5s ease-in-out
}

{% endhighlight %}

*※When other settings are the same, CSS class below is applied.* 


