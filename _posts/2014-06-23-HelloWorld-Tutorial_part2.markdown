---
layout: post
title:  "Hello World Visualization - Part 2"
date:   2014-06-23 13:14:36
categories: jekyll update
---

Writing your first code:

**Step 1:**

> Create a new class within your project. `File`->`Class`.

![drawing](/images/screenshot_6.png)

**Step 2:**

> In the new window set the `Package` field to your name. Set the `Name` field to HelloWorld (this is the name of the class). Tick the box to create `public static void main(String[] args)` (this will have Eclipse create a main method for you within your newly created class). Then click `Finish` in the lower right corner.

![drawing](/images/screenshot_7.png)

**Step 3:**

> Import the Bridges package.

{% highlight java  %}

import bridges.*;

{% endhighlight %}

**Step 4:**

> Create a new GraphVisualizer. 

{% highlight java  %}

GraphVisualizer gv = new GraphVisualizer();

{% endhighlight %}

**Step 5:**

> Initialize Bridges. Your API key should have been generated in Part 1, this is where it goes.

{% highlight java  %}

Bridge.init(0, "Your API key here", gv);

{% endhighlight %}

**Step 6:**

> Create your first Vertex. HelloWorld is what we are going to name our first vertex.

{% highlight java  %}

Vertex HelloWorld = new Vertex("HelloWorld", gv);

{% endhighlight %}

**Step 7:**

> Submit the visualization data.

{% highlight java  %}

Bridge.complete();

{% endhighlight %}

**Step 8:**

> Finally we need to run our program.
In the console there will be a string giving you a link to view your visualization.

`Check out your visuals at http://bridges.cs.uncc.edu/assignments/0/YOUR_USERNAME?apikey=YOUR_API_KEY_WILL_BE_HERE`

> Copy and paste the URL into your favorite browser in order to view your visualization. Where the URL says `YOUR_USERNAME` be sure to replace it with your Bridges user name.
