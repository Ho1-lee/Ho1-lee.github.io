---
layout: post
title:  "Manacher Algorithm"
date:   2021-01-27
excerpt: "Longest Palindromic Substring"
tag:
- Python
- Algorithm
- Palindromic Substring
comments: false
---

![Anaconda-logo](/assets/img/python-logo.png)    
    
<center><b>Python</b></center>

For Simple Virtual Environment, it is easier to use Python Virtual Environment than Anaconda.

## Change Python Version
1. Install Ohter Python
([Python Install site](https://www.python.org/downloads/))


2. Change Python Version

{% highlight yaml %}
#Change Version for Python Command
ho@ho1:~$ sudo update-alternatives --config python /usr/bin/python3.6
{% endhighlight %}

---

## Make Virtual Environment

{% highlight yaml %}
#Make Virtual Environment
#ho@ho1:~$ python -m venv {venv_name}
ho@ho1:~$ python -m venv my_venv
{% endhighlight %}

---

## Activate & Deactivate Virtual Environment
{% highlight yaml %}
#Make Virtual Environment
#ho@ho1:~$ source ./{venv_name}/bin/activate
ho@ho1:~$ source ./my_venv/bin/activate

#Deactivate
ho@ho1:~$ Deactivate
{% endhighlight %}

---

## Update 'pip' on Virtual Environment
{% highlight yaml %}
#Update 'pip'
ho@ho1:~$ python -m pip install --upgrade pip
{% endhighlight %}

---

## Install Module with 'pip'
{% highlight yaml %}
#Install Module
#ho@ho1:~$ python -m pip install {Module_Name}
ho@ho1:~$ python -m pip install opencv-python
{% endhighlight %}


