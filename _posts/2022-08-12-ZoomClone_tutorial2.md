---
layout: post
title: Zoom 클론코딩
subtitle: Nodejs
categories: NomadCoders
tags: [JS, Nomad Coder, Nodejs]
---


## Socket.io

{% highlight javascript %}
//app.js
function func(arg){
    console.log(arg);
};
socket.emit("my_msg", argument, func);

//server.js
const elem = "in server";

socket.on("my_msg", (msg, done) => {
    //msg is argument
    done(elem);
});
{% endhighlight %}

Using emit and on, frontend can send function to backend, then backend calling function to be activated in frontend, can send backend data to frontend.


