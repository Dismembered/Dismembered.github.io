---
layout: post
title:  "Hello World Visualization"
date:   2014-06-23 13:14:36
categories: jekyll update
---

Installation:

Download and install Eclipse [here](https://www.eclipse.org/downloads/index-java8.php). Choose  `IDE for Java Developers` from the list.

Go to the Bridges website found [here](http://bridges.cs.uncc.edu/login) and create an account. After you create your account, click on your profile name name in the upper right corner to view your profile. Once in your profile, click `Generate new API key` and remember the number generated.

![ScreenShot_0](https://github.com/Dismembered/Dismembered.github.io/blob/master/images/screenshot_0.png = 800 X 450)


`Insert statements about downloading the Java Bridges Client`

Writing your first code:

**Step 1:**
Import the Bridges package.
{% highlight java  %}

import bridges.*;

{% endhighlight %}

**Step 2:**
Create a new class within the `YourName package` named `HelloWorld`.

**Step 3:**
Create a new GraphVisualizer. 
{% highlight java  %}

GraphVisualizer gv = new GraphVisualizer();

{% endhighlight %}

**Step 4:**
Initialize Bridges.
{% highlight java  %}

Bridge.init(0, "Your API key here", gv);

{% endhighlight %}

**Step 5:**
Create your first Vertex.
{% highlight java  %}

Vertex HelloWorld = new Vertex("HelloWorld", gv);

{% endhighlight %}

**Step 6:**
Submit the visualization data.
{% highlight java  %}

Bridge.complete();

{% endhighlight %}

**Step 7:**
View your visualization.

In the console there will be a string giving you a link to view your visualization.

`Check out your visuals at http://bridges.cs.uncc.edu/assignments/0/YOUR_USERNAME?apikey=YOUR_API_KEY_HERE`

Where the URL says `YOUR_USERNAME` be sure to replace it with your actual user name. Copy and paste the URL into your favorite browser to view your visualization.

