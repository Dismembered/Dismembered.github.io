---
layout: post
title:  "Hello World Visualization"
date:   2014-06-23 13:14:36
categories: jekyll update
---

Installation and Setup:

Download and install Eclipse [here](https://www.eclipse.org/downloads/index-java8.php). Choose  `IDE for Java Developers` from the list.

Go to the Bridges website found [here](http://bridges.cs.uncc.edu/login) and create an account. After you create your account, click on your profile name name in the upper right corner to view your profile. Once in your profile, click `Generate new API key` and remember the number generated.

**Step 1:**
Start Eclipse and click `File` -> `Java Project`.

![drawing](/images/screenshot_0.png)

**Step 2:**
In the new window change the `Project name` field input your name. Then click `Finish` in the lower right hand corner.

![drawing](/images/screenshot_1.png)

**Step 3:**
Right-click your package (it should be your name) in the `Package Explorer` then click `Configure` -> `Convert to Maven Project`.

![drawing](/images/screenshot_2.png)

**Step 4:**
In the new window change the `Artifact Id` field to Hello World then click `Finish` in the lower right hand corner.

![drawing](/images/screenshot_3.png)

**Step 5:**
Double-click the pom.xml in the `Package Explorer` to open it. Click the `pom.xml` tab at the bottom of the scren to activate it. You should now see something like this.

![drawing](/images/screenshot_4.png)

**Step 6:**
Not sure where this came from.

![drawing](/images/screenshot_5.png)

Congratulations, you are now ready to start writing code!


Writing your first code:

**Step 1:**
`File`->`Class`.

![drawing](/images/screenshot_6.png)

**Step 2:**
In the new window set the `Package` field to your name. Set the `Name` field to HelloWorld (this is the name of the class). Tick the box to create `public static void main(String[] args)` (this will have Eclipse create a main method for you within your newly created class). Then click `Finish` in the lower right corner.

![drawing](/images/screenshot_7.png)

**Step 3:**
Import the Bridges package.
{% highlight java  %}

import bridges.*;

{% endhighlight %}

**Step 4:**
Create a new GraphVisualizer. 
{% highlight java  %}

GraphVisualizer gv = new GraphVisualizer();

{% endhighlight %}

**Step 5:**
Initialize Bridges.
{% highlight java  %}

Bridge.init(0, "Your API key here", gv);

{% endhighlight %}

**Step 6:**
Create your first Vertex.
{% highlight java  %}

Vertex HelloWorld = new Vertex("HelloWorld", gv);

{% endhighlight %}

**Step 7:**
Submit the visualization data.
{% highlight java  %}

Bridge.complete();

{% endhighlight %}

**Step 8:**
View your visualization.

In the console there will be a string giving you a link to view your visualization.

`Check out your visuals at http://bridges.cs.uncc.edu/assignments/0/YOUR_USERNAME?apikey=YOUR_API_KEY_HERE`

Where the URL says `YOUR_USERNAME` be sure to replace it with your actual user name. Copy and paste the URL into your favorite browser to view your visualization.

