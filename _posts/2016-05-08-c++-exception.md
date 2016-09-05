---
layout: post
title: "c++ exception"
publish: true
---
transfer control to special function called *handler*

the type of the argument passed by the throw expression is checked against it, and only in the case they match, the exception is caught by that handler.

{% highlight c++ linenos %}
try {
  // code here
}
catch (int param) { cout << "int exception"; }
catch (char param) { cout << "char exception"; }
catch (...) { cout << "default exception"; }
{% endhighlight %}

the last handler would catch any exception thrown of a type that is neither int nor char.
