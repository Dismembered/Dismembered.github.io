---
layout: post
title:  "Hello World Visualization - Part 3"
categories: jekyll update
---

## Continuing your graph visualization:
-----
At the end of this section of the tutorial you will know how to create edges and manipulate Vertex and Edge properties. This is what you will be creating.

![drawing](/images/screenshot_10.png)

When we left off last we had just created our first visualization and displayed our first vertex. It should have looked something like this.

![drawing](/images/screenshot_9.png)

Lets start off by managing the properties of that vertice. Each vertex and edge that we create have access to an array of properties to manage their look. The first property we will look at is the color property.

## Step 1: Changing the vertex color

> First we want to using the vertex that we want to manipulate and call the appropriate method, in this case the .setColor() method. Bridges is set up to accept strings as a color value or the CSS color value.

> Note: If you do not choose a value that is in our list you will recieve an InvalidValueException. Thats okay just choose a different color.

{% highlight java %}

HelloWorld.setColor("red"); OR HelloWorld.setColor("#FF0000");

{% endhighlight %}

![drawing](/images/screenshot_11.png)

## Step 2: Further vertex manipulation

> This only requires further method calls on the same vertex to change its properties. We should also go ahead and create another vertex for the next part of the tutorial.

{% highlight java %}

HelloWorld.setSize(15);
HelloWorld.setOpacity(0.5);

Vertex GoodByeWorld = new Vertex("GoodByeWorld", gv);

{% endhighlight %}

![drawing](/images/screenshot_12.png)

[Return to Part 1](http://dismembered.github.io/jekyll/update/2014/06/23/HelloWorld-Tutorial_part1/)

[Return to Part 2](http://dismembered.github.io/jekyll/update/2014/06/23/HelloWorld-Tutorial_part2/)
