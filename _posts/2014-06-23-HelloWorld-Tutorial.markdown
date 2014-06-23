---
layout: post
title:  "Hello World Visualization"
date:   2014-06-23 13:14:36
categories: jekyll update
---

Installation:

Download and install Eclipse [here](https://www.eclipse.org/downloads/index-java8.php). Choose  `IDE for Java Developers` from the list.

Go to the Bridges website found [here](http://bridges.cs.uncc.edu/login) and create and account. After you create your account, click on your name in the upper right corner to view your profile. Once in your profile, click `Generate new API key` and remember the number generated.

`Insert statements about downloading the Java Bridges Client`

Writing your first code:

Step 1:
Create a new class withing the `Sketch package` name HelloWorld.

Step 2:
Create a new GraphVisualizer 
{% highlight java  %}

GraphVisualizer gv = new GraphVisualizer();

{% endhighlight %}

Step 3:

Initialize Bridges
{% highlight java  %}

Bridge.init(0, "`Your API key here`", gv);

{% endhighlight %}
