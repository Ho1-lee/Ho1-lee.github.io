---
layout: post
title:  "Manacher's Algorithm"
date:   2021-01-27
excerpt: "Longest Palindromic Substring"
tag:
- Python
- Algorithm
- Palindromic Substring
comments: false
---
## What is 'palindromic string'?
![Anaconda-logo](/assets/img/palindromic.png)
    
<center><b>Palindromic String</b></center>

A string is what is a palindrome if the string read from left to right is equal to the string read from right to left.

---
## Brute Force
Brute force solution will find Palindromic Substring.
1. Find all Substring.
2. Check if it is Palindromic or not.
It has O(1) space complexity. But, it has $$O(n^3)$$ time complexity. It seems to need less time complexity.

---
## Expand Around Center
We could solve it in $$O(n^2)$$ time complexity using only constant space.
1. Fix a center. Every character can be a center.
2. Calculate how long palindromic substring can be made with the center.
3. Need to check not only [center-i:center+i] but also [center-i:center+i+1]. Be ready for case 'abba'.

---
## Manacher's Algorithm
Manacher's Algorithm is most powerful to find Palindromic Substring in a string. It has $$O(n)$$ time complexity. Let's see how it works.

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


