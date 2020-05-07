---
layout: post
title:  "Anaconda Manual"
date:   2019-11-13
excerpt: "How to Set Anaconda Environment(Basic)"
tag:
- Anaconda
- Environment
comments: false
---

![Anaconda-logo](/assets/img/anaconda-logo2.png)    
    
<center><b>Anaconda</b></center>

It is easy to manage Python Developing Environment with Anaconda which can make Virtual Environment.
I will talk about Basic Manual.

## Install
[Anaconda Install site](https://www.anaconda.com/distribution/#download-section)
*available to use on CMD by setting environment PATH

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
