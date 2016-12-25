---
layout: post
title: "my Codings"
publish: true
---
**This post is to review my Codings. I hope it will grow very large**

## STL practice

### 1.List

#### Description

写一个程序完成以下命令：

new id ——新建一个指定编号为id的序列(id<10000)

add id num——向编号为id的序列加入整数num

merge id1 id2——合并序列id1和id2中的数，并将id2清空

unique id——去掉序列id中重复的元素

out id ——从小到大输出编号为id的序列中的元素，以空格隔开

#### Input

第一行一个数n，表示有多少个命令( n＜＝２０００００)。以后n行每行一个命令。

#### Sample Input

{% highlight c++ linenos %}
16
new 1
new 2
add 1 1
add 1 2
add 1 3
add 2 1
add 2 2
add 2 3
add 2 4
out 1
out 2
merge 1 2
out 1
out 2
unique 1
out 1
{% endhighlight %}

### Sample OutputI

{% highlight c++ linenos %}
1 2 3
1 2 3 4
1 1 2 2 3 3 4

1 2 3 4
{% endhighlight %}

### Solution

It's just about the basic operation of list and string

{% highlight c++ %}
front()//return a reference
back() //return a reference to the last element in the list;
insert()
crbegin()//

merge()// ordered
splice()//unordered
{% endhighlight %}
