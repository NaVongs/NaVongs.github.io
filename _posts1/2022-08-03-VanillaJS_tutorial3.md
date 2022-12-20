---
layout: post
title: JS 입문 3
subtitle: JavaScript
categories: NomadCoders
tags: [JS, Nomad Coder, Web]
---

## Button, Input blank, Hyperlink
**HTML elements**
{% highlight HTML %}
<button> </button>  
<input />  
<a href=""></a>

<form> </form>
{% endhighlight %}

"Button" can be operated listening *click* event.  
"Input" can get input value: stored in *value* property.  
"Form" let JS use functions of browser.  

But when form 'submit'(it's default movement) something, it reload the page. So we have to block it with "*argument*.preventDefault()".  

CSS can hide some HTML elements using class:
{% highlight CSS %}
.hidden{
    display: none;
}
{% endhighlight %}

and show another elements with adding and unsealing(removing hidden class).  
String merge can be done in the way as:
{% highlight Javascript %}
    *classname*.innerText = `Hello ${*stringname*}`;
{% endhighlight %}



## Storage ##
API "localStorage" let browser be able to store some values. It store data although a page is reloaded. It can be used to save ID lists.  

{% highlight javascript %}
function onLoginSubmit(event) {
    event.preventDefault();
    loginForm.classList.add(HIDDEN_CLASS);
    const username = loginInput.value;
    localStorage.setItem(USERNAME_KEY, username);
    showGreetings(username);
}

function onLogoutSubmit_diy(event){
    event.preventDefault();
    localStorage.removeItem(USERNAME_KEY);
    loginForm.classList.remove(HIDDEN_CLASS);
    greeting.classList.add(HIDDEN_CLASS);
    loginForm.addEventListener("submit", onLoginSubmit);
    logoutForm.classList.add(HIDDEN_CLASS);
}
{% endhighlight %}

*I tried adding a logout button by removing ID from localStorage: It works.*

