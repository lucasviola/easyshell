---
title: "environment"
bg: #1A5946    
color: white  #text color
fa-icon: file-code-o
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

Useful environment variables

- `$PS1` your prompt setup
- `$PATH` your path setup 
- `$USER` your current user

The most important files regarding your environment are:

1. `$ ~/.profile`
2. `$ ~/.bashrc`

Both of them are shell scripts and contain instructions which are executed when you log in.

Permanently exporting variables to your PATH: 

`$ echo 'export $PATH="$PATH:/path/to/file/"' >> ~/.bashrc
