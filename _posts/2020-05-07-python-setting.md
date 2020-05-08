---
layout: post
title:  "Python Virtual Environment Setting"
date:   2020-05-07
excerpt: "How to Set Basical Python Virtual Environment"
tag:
- Python
- Environment
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
C:\Users\oo>sudo update-alternatives --config python /usr/bin/python3.6
{% endhighlight %}

---

## Version Check / Update

{% highlight yaml %}
#version Check
C:\Users\oo>conda --version

#Update Conda
C:\Users\oo>conda update conda
{% endhighlight %}

---

## Create Virtual Environment
{% highlight yaml %}
#Create Virtual Environment
#C:\Users\oo>conda create --name(-n) <b>EnvironmentName PackageName</b>
C:\Users\oo>conda create --name test python=3.5
#Or
C:\Users\oo>conda create --n test python=3.5
{% endhighlight %}

---

## Virtual Environment Activation / Deactivation
{% highlight yaml %}
#list of Virtual Environment
C:\Users\oo>conda info --envs

#Activation
#C:\Users\oo>activate <b>EnvironmentName</b>
C:\Users\oo>activate test

#Deactivation
C:\Users\oo>conda deactivate
{% endhighlight %}

---

## Package Install / Check
{% highlight yaml %}
#Virtual Environment Activation
#C:\Users\oo>activate <b>EnvironmentName</b>
C:\Users\oo>activate test

#Package Install
#C:\Users\oo>conda install <b>PackageName</b>
C:\Users\oo>conda install numpy

#Check Installed Package
C:\Users\oo>conda list
{% endhighlight %}
---
## Remove / Clean
{% highlight yaml %}
#Remove Virtual Environment
#C:\Users\oo>conda remove --name <b>EnvironmentName</b>
C:\Users\oo>conda remove --name tensorflow35 --all

#Delete useless(Index cache, locked file, unused package, source cache) things
C:\Users\oo>conda clean -all
#Or
C:\Users\oo>conda clean -a
{% endhighlight %}
