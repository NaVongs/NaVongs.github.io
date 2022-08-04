---
layout: post
title: JS 입문 3
subtitle: JavaScript
categories: Language
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

But when form 'submit' something(it's default movement), it renew the browser. So we have to block it with "*argument*.preventDefault()".  

