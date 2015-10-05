---
layout:     post
title:      Don't waste your engineers
date:       2015-10-05
summary:    Think about optimizing for engineering time rather than for computing resources.
categories:
---

![Don't waste your engineers](/images/2015-09-dont-waste-your-engineers.jpg)

Usually, when you talk about optimizing a system, you think about making it use less memory, less CPU, less bandwidth, less battery etc. But all these resources are getting exponentially cheaper, thanks to the natural evolution of the industry. Especially in the 80s or 90s, optimization was key to getting your software to even work. We all know the stories about all the hacks engineers had to pull to launch those side-scrolling games, for example.

But this is 2015. Optimizations are expensive in engineering time. And as the price of computing resources gets lower and lower, that time spent optimizing is less and less justifiable. Especially that engineer salaries haven’t gone down a bit.

Don’t get me wrong, if optimizations improve user experience, then in most cases that time is well spent. I’m just talking about optimizing for the sake of reducing resource usage, or making your program “fast”, just because.

When I worked at Google, I sometimes had to run huge map reduce tasks on lots of machines. They have cool stats on the jobs and they show you much money you spent with your task - but they express it in terms of engineering time, rather than dollars. Even though some of these tasks would take days to complete and used tons of resources, the statistic was super low each time (less than an engineer minute cost). If you think about it, even reading this blog post is vastly more expensive to your employer.

So I propose we start thinking about optimizations differently. It shouldn’t be just about computing resources. Programmers are a resource too. In fact they are the most expensive resource of the equation.

So when you design your code, you should almost always optimize for readability rather than time of execution. When you design your backend, you should optimize for maintainability, rather than high throughput. When you design a programming framework, you should optimize for quick starts and ease of debugging, rather than deep configuration.

And I dare say it, for projects where dynamic typing is OK, high-level languages with good community support, like [JavaScript, should be your default choice](http://blog.andreipolmolea.com/you-should-choose-javascript/).
