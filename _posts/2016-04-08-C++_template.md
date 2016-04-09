---
layout: post
title: "STL"
publish: true
---

c++ find function in STL:

{% highlight c++ linenos %}
template<class InputIterator, class T>
  InputIterator find (InputIterator first, InputIterator last, const T& val)
{
  while (first!=last) {
    if (*first==val) return first;
    ++first;
  }
  return last;
}
{% endhighlight %}

c++ insert function:

{% highlight cpp linenos %}

{% endhighlight %}

istream InputIterator

**insert:only for random access iterator!!**

{% highlight cpp linenos %}
template<class InputIterator, class OutputIterator>
  OutputIterator copy (InputIterator first, InputIterator last, OutputIterator result)
{
  while (first!=last) {
    *result = *first;
    ++result; ++first;
  }
  return result;//do remember the return!!!!
}
{% endhighlight %}

http://www.cplusplus.com/reference/vector/vector/insert/
Value to be copied (or moved) to the inserted elements.
Member type value_type is the type of the elements in the container, defined in deque as an alias of its first template parameter (T).
??

{% highlight cpp linenos %}
//some comments
{% endhighlight %}

### Function Object

- Function Ob
- defining member function operator() in their member

*Example:*
{% highlight cpp linenos %}

class CMyAverage  {
public:
double operator()( int a1, int a2, int a3 ) { // overload ()
return (double)(a1 + a2 + a3) / 3;
}
};
 CMyAverage average;  // function object
 cout << average(3,2,3); // it behaves like a function call

{% endhighlight %}

#### A template in STL
{% highlight cpp linenos %}
template <class InputIterator, class T>
   T accumulate (InputIterator first, InputIterator last, T init)
{
  while (first!=last) {
    init = init + *first;  // or: init=binary_op(init,*first) for the binary_op version binary_op This can either be a function pointer or a function object.
    ++first;
  }
  return init;
}
{% endhighlight %}

note:

{% highlight cpp linenos %}
SumSquaresClass<int> s;
result = accumulate(v.begin(),v.end(),0,s)
{% endhighlight %}

Equivalent to

{% highlight cpp linenos %}
//some comments
{% endhighlight %}

You cann't use the STL sort for list;
for it need a parameter of Random Access Iterator
