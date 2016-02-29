---
layout: post
title: "Cycle: Using Enumerables and Enumerators"
date: 2016-01-31
categories: Ruby basics
---
The words enumerables and enumerators may be words that you have never heard before. If you are not into programming or math, there is a good chance you are not familar with them. Basically, an Enumerator is a method that will go over each element of a enumerable, one at a time. Enumerables that you are using will often be arrays or hashes.

Now, there are many different enumerable methods out there. [Ruby-docs](http://ruby-doc.org/) is a great place to check all of these out and learn exactly how to implement them. Today, I will go over one of my favorites, called the cycle method.

Cycle is a method that can definitely save you some time and help make code DRY. Before I found this method, I was using a counter variable to actually keep track of how many times I performed a method on an array or hash. Although this worked, it definitely was not the cleanest way to write the code. With cycle, you will need an n value, an object, and a code block.

{% highlight ruby %}
cycle(n){ |obj| block }
{% endhighlight %}

This will call the block for each and every element of the enumerable "n" times. Now, optionally you can leave the "n" blank, and this will repeat the block on every element infinitely. If you are not careful with this, you can create an infinite loop. View some examples below.

{% highlight ruby %}
array = ["one", "two", 3]
array.cycle { |i| puts i}
array.cycle(2) { |i| puts i}
{% endhighlight %}

The first cycle will print out "one","two", 3 ... infinitely. The second cycle will print out the same, but only twice. This brings you a total of 6 elements executed.

Now go forth and have fun with enumberables. There are a multitude of things you can do with these fancy methods, and they definitely make you job as a developer a bit easier and a bit cleaner.