---
layout: post
title: JS 입문
subtitle: JavaScript
categories: Language
tags: [JS, Nomad Coder, web]
---



## Type of Variables


| Type | editable | etc |
| :------ |:--- | :--- |
| var | editable | . |
| let | editable | . |
| const | uneditable | . |

## Various form of data container
array(list) : classic array  
object : similar with class  
function : classic function


{% highlight javascript %}
let array1 = [0, 1, 2, "data"];
const object1 = {
    property1 : 3,
    property2 : "string",
    property3 : 1.5
};

function func1(a, b) {
    console.log(a);
    return a*b;
};

const object2 = {
    prop : function(a, b){
        return a+b;
    }
};
{% endhighlight %}

