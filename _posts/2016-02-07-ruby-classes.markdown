---
layout: post
title: "Instance Variables and Methods"
date:  2016-02-07
categories: Ruby basics
---
### Methods

Instance variables and methods can be incredibly useful when used properly. Keep in mind that these will be much more limited in how far reaching they are. Of course, as the name implies, they can only be used on a specific instance of a class.

The easiest way to learn this is to jump right in to coding. I will create an object and for keeping an inventory, and a class method to find an object in there.

{% highlight ruby%}
Class Inventory
  def self.locate(item)
    p "The location of #{item} has been found."
  end
end
{% endhighlight %}

Notice the use of self to define class methods. This method will be used to search all objects of the class Inventory. Since it is affected by all, and not just one instance, of this class, the class method suits it best.

If we just wanted to do something to a single instance of this class, instance methods are the way to go.

{% highlight ruby%}
Class Inventory
  def self.locate(item)
    p "The location of #{item} has been found."
  end

  def deplete(amount)
    p "Current item has been depleted by #{amount}."
  end
end
{% endhighlight %}

They will also be called for in a different way. The class method being called on the class name and the instance(deplete) method being called on just an instance of that class, e.g., tissues, rice, pants.

### Variables

Now, when making classes with variables, the two main ones you need to worry about are instance variables and class variables. Here is how these variables are set.

{% highlight ruby%}
@variable1 = "instance variable"
@@variable2 = "class variable"
{% endhighlight %}

With instance variables, this can be different for each and every instance of a particular class. If you change it for one instance, it will not change any other instances. Now class variables are a little more far reaching. If you change a class variable anywhere, it will change it for each and every instance of the class.