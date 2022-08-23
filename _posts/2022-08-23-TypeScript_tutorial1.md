---
layout: post
title: TypeScript
subtitle: TypeScript
categories: NomadCoders
tags: [JS, TS, Nomad Coder, Nodejs]
---

## TypeScript
To complement type explicity of JavaScript  
Compiled as JavaScript  
Required software : Nodejs  

## Type of TS
{% highlight TypeScript %}
const val : string = "hi";
const object : {
    args1 : string,
    args2 : number,
} = {
    args1 : "hi",
    args2 : 0,
}
type type_name = {
    args1 : string,
    args2? : number
}
const obj2 : type_name = {
    args1 : "hello",
}
function func1(para: string) : type_name {
    return {
        para,
    };
}
const func2 = (para: string) : type_name => ({para});

{% endhighlight %}

TS can give a value type explicity with the way above.  
TS uses value types of JS.  

| readyonly | make values read-only |
| tuple | give each element type explicity |
| any | take type explicity away (like JS) |