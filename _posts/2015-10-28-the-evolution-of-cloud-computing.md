---
layout:     post
title:      The evolution of cloud computing
date:       2015-10-28
summary:    In the 2000's the world changed from bare metal to virtual instances. What is the next big paradigm shift in the cloud computing industry?
categories:
social_image: /images/2015-10-two-clouds.jpg
---

<p align="center">
<img src="/images/2015-10-two-clouds.jpg">
</p>

The basic concepts of cloud computing originated in the 50s when ["IBM and the Seven Dwarfs"](https://en.wikipedia.org/wiki/BUNCH) really started taking off their mainframe business. They were mainly used for batch processes, to support back of house operations like customer billing and they required significant technical expertise to deploy and operate them.

Later on, with the development of Unix and later Linux, large computer rooms, called at the time "Data Centers", started becoming popular. Inexpensive networking equipment allowed companies to deploy terminals in several locations across a building, while maintaining a central location for the actual data and computing resources. But these were generally isolated from the rest of the world and so their use cases were relatively limited.

Fast forward to the dot com boom era, data center demand exploded as companies needed systems that operated non-stop and were always connected to the internet. Renting them was based on square feet of space, as opposed to bandwidth or power necessary. So some companies quickly caught on and started cramming as many cheap servers as they could in every corner possible. There are some funny stories to be told about correlating motherboard temperature readings with ongoing fire, but I'll leave that for another day. :-)

<p align="center">
<img src="/images/2015-10-google-rack.jpg">
</p>

Needless to say, in 1997-2000, there was a lot to set up if you wanted to get code up and running in the cloud. You had to buy equipment, figure out power and cooling requirements, figure out networking, figure out monitoring and serviceability, figure out OS deployments and then you could start worrying about all the other problems that come with writing software for distributed systems.

All this was a huge pain to manage, especially for small companies which did not have the resources necessary to bootstrap. True global availability was also extremely expensive and so few companies really pursued that.

But at the horizon there was a new paradigm emerging. In 2006, [Amazon launched their public cloud offering](http://aws.amazon.com/about-aws/), called Amazon Web Services (AWS), which was set to revolutionize the way people deployed infrastructure.

Amazon abstracted away a huge chunk of the pain that comes with managing bare metal instances. And yet, cloud computing is still not that easy. Looking at the entire ecosystem of products AWS offers today, it is hard to figure out where to even start. You're still left with a host of difficult problems that you have to solve yourself as you scale your infrastructure to handle more and more traffic. Now you have to worry about installing your software stack, developing API endpoints, coordinating servers to handle failover, figuring out load balancing, auto scaling and auto discovery. Not to mention that you have to do this for multiple regions if you want to serve traffic globally.

There are some platforms out there that aim to abstract away some of these things, but in reality they don't solve that many problems from the list above and everyone goes back to deploying on AWS, as the scale grows beyond a certain point. [Heroku](https://www.heroku.com/) is one example in this category.

Other technologies like [Docker](https://www.docker.com/) or [CoreOS](https://coreos.com/) aim to tackle the problem in a different way. While I think the direction and the benefits are great, they still don't save us from distributed systems' complexities.

So my question to you is: What is the next paradigm shift that will dramatically change the industry again?

What if you could abstract away all the infrastructure problems and be left with just your code - just the logic that defines what your application does, and not have to worry about where it runs or how to make it available at a global scale?

[Discussion on HN](https://news.ycombinator.com/item?id=10465139)
