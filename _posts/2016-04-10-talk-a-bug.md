---
layout: post
title: "talk about a bug"
publish: true
---

### Reference
[Extra, Extra - Read All About It: Nearly All Binary Searches and Mergesorts are Broken](http://googleresearch.blogspot.ca/2006/06/extra-extra-read-all-about-it-nearly.html)

### bug

{% highlight c++ linenos %}
int mid =(low + high) / 2;
{% endhighlight %}

It fails if the sum of low and high is greater than maximum positive value(2^32-1)

### How to fix it?

general solution:

{% highlight java linenos %}
int mid = low + (high-low)/2
{% endhighlight %}

in java:

{% highlight java linenos %}
int mid = (low + high) >>> 1;
{% endhighlight %}

in c/c++

{% highlight java linenos %}
mid = ((unsigned int)low + (usigned int)high) >> 1;
{% endhighlight %}
