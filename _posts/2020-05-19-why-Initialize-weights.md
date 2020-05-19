---
layout: post
title:  "Why Weights Initialization is Important?"
date:   2020-05-19
excerpt: "We use a specific 'Method' to Initialize Network's Weights. Why Weights Initialization is Important and Which 'Method' is better?"
tag:
- Deep Learning
- Weights Initialization
comments: false
---

When using Weights in Gaussian Distribution which has mean 0 and variance 1, Output tends to be 0 or 1. Sigmoid's Gradient Vanishing near 0 and 1 is the reason. We can figure it out with not only Changing Activation Fuction but also Initializing Weights.

![Anaconda-logo](/assets/img/Sigmoid_0_1.png)    
    
---

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

---
## Reference
https://gomguard.tistory.com/184
