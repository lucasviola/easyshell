---
title: "environment"
bg: green     #defined in _config.yml, can use html color like '#010101'
color: white  #text color
---

# Working with environment and variables

Listing local variables

`$ set`

Listing global variables

`$ env`

Printing variable content
{% highlight text linenos=table %}
$ foo='This is a variable!'
$ echo $foo
{% endhighlight %}

Looking for a local variable

`$ set | grep foo`

Exporting it to env
{% highlight text linenos=table %}
$ export foo
$ env | grep foo
{% endhighlight %}