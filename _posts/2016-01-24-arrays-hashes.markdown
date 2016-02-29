---
layout: post
title:  "Arrays and Hashes"
date:   2016-01-24 17:57:13 -0800
categories: Ruby basics
---
Welcome welcome welcome. This past week over at Dev Bootcamp I have been going over lots of Ruby practice. The thing that seemed to be the toughest for me was figuring out these darn arrays and hashes. Now, these are very similar concepts, but with one major difference: keys vs indices.

Let's start with the slightly simpler of the two, arrays. Array is basically going to be a list of values. These individual values in the same array could be any object (numbers, strings, booleans). The objects do have to be organized some way though, so we can find them again later. They are organized into an ordered numerical index. So the first object you have in your array will be at index 0, second object at index 1, third object at index 2, and so on. An array can be as big or small as you like. It could literally be empty and still be an array. This is the go to technique for data organization. Check out a couple different ways to make an array below.

{% highlight ruby %}
a = [value_1, value_2, value_3]
a[index] = value
{% endhighlight %}

Now hashes work a little bit differently, but share some properties as well. Hashes can also any size, contain values, and these values can be any object. The big difference is how they are organized. Instead of an index to be a place holder for a value, hashes use what we call keys. Now keys can be any object as well, but, unlike values, they are unique. So everything in a hash in organized into these key => value pairs. Check out a couple different ways to create new hashes below.

{% highlight ruby %}
hash_name = {key_1 => value_1 , key_2 => value_2}
Hash.new
{% endhighlight %}

Now the question is, "which one do you use?" On one hand, arrays are nice for ordered data. If your data has a specific way it hsould be read out, the numerical index that is already set up is the perfect way to organize and retrieve all of your data. If the order does not matter so much, but you want to be able to easily retrieve individual elements, hashes might be the way to go. Imagine you are making a dictionary, and wanted to find the word "interesting." With an array, you would have to know its index by heart (unlikely) or search through the entire array one by one to find it. If set up the dictionary as a hash , with the word as the key, it would be much simpler to just find the key.

Overall, the main difference between a has and array is how the data is organized, either in a index => value pair or a set of key => value pairs. Both are very powerful, but definitely have their own strengths. Good luck on playin with both of them. Have fun coding!