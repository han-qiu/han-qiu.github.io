---
layout: post
title: "Learn HTML"
publish: true
---

## HTML Introduction

### What is HTML?
- Hyper Text Markup Language

{% highlight html linenos %}
<!DOCTYPE html>
<html>
<head>
<title>Page Title</title>
</head>
<body>

<h1>My First Heading</h1>
<p>My first paragraph.</p>

</body>
</html>
{% endhighlight %}

- The DOCTYPE declaration defines the document type to be HTML
- The text between <html> and </html> describes an HTML document
- The text between <head> and </head> provides information about the document
- The text between <title> and </title> provides a title for the document
- The text between <body> and </body> describes the visible page content
- The text between <h1> and </h1> describes a heading
- The text between <p> and </p> describes a paragraph

### HTML Documents

### HTML Headings

{% highlight html linenos %}
<h1> </h1>
...
<h6> </h6>
{% endhighlight %}

### HTML Paragraphs

{% highlight html linenos %}
<p> </p>
{% endhighlight %}

### HTML Links
<a href="http://www.w3schools.com">This is a link</a>

### HTML Images
{% highlight html linenos %}

<img src="w3schools.jpg" alt="W3Schools.com" width="104" height="142">
{% endhighlight %}
### Empty HTML Elements
{% highlight html linenos %}
<br>
{% endhighlight %}

### HTML tags are not case sensitive

### Attrivutes
- All HTML elements can have attributes
- The HTML title attribute provides additional "tool-tip" information
- The HTML href attribute provides address information for links
- The HTML width and height attributes provide size information for images
- The HTML alt attribute provides text for screen readers
- At W3Schools we always quote attributes with double quotesAt W3Schools we always use lowercase HTML attribute names

### some tags
The HTML <meta> element is also meta data.

It can be used to define the character set, and other information about the HTML document.

In the chapter about HTML styles you discover more meta elements:

The HTML <style> element is used to define internal CSS style sheets.

The HTML <link> element is used to define external CSS style sheets.

### HTML Display
Any number of spaces, and any number of new lines, count as only one space.

The HTML <pre> element defines preformatted text.

The text inside a <pre> element is displayed in a fixed-width font (usually Courier), and it preserves both spaces and line breaks:
