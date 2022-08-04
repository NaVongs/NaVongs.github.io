---
layout: post
title: JS 입문 3
subtitle: JavaScript
categories: CloneCoding
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
API "localStorage" let browser be able to store some values. It store data although a page is reloaded.