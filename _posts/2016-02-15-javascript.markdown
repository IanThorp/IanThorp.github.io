---
layout: post
title: "Ruby vs JavaScript: Hashes and Objects"
date: 2016-02-15
categories: Ruby basics, JavaScript basics
---
Ruby and Javascript are similar in a lot of ways. Both are object oriented and both scripting languages. They even have a similar way to build what is called a hash in ruby. They actually build the hashes and objects in a very similar way, but do have some slight differences.

Ruby
{% highlight ruby %}
hash_name = { hash_key: hash_value}
{% endhighlight %}

JavaScript
{% highlight javascript %}
var hashName = { hashKey: hashValue}
{% endhighlight %}

The main difference here is that you need to put the word "var" before the object in JavaScript. Otherwise, in Ruby, snake_case is prefered while JavaScript prefers camelCase. This is not necessary for the code to work, but a style preference.

Calling the values will also be done in a similar way.

Ruby
{% highlight ruby %}
hash_name[:hash_key] --> hash_value
{% endhighlight %}

JavaScript
{% highlight javascript%}
hashName.hashKey --> hashValue
{% endhighlight %}

Both of these scripting languages have their strengths and weaknesses. In general, Javascript is used more often for front end web development and ruby is used more often for back end web development. If you want to become a full stack developer, it is important to know both and know them well.