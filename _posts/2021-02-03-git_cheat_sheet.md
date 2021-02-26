---
layout: post
title:  "Git Cheat Sheet"
date:   2021-01-27
excerpt: "git Command"
tag:
- Git
- Github
- Command
comments: false
---
## Git

Git is the Open source manager system which can be used GitHub. Let's see commonly used Git commands.

---
## Commands
- User information
{% highlight yaml %}
git config credential.helper store
{% endhighlight %}

- initialize / clone
{% highlight yaml %}
git init
git clone [url]
{% endhighlight %}

- remote add
{% highlight yaml %}
git remote add origin [url]
#if 'already exist' error
git remote rm origin
{% endhighlight %}

- status
{% highlight yaml %}
git status
{% endhighlight %}

- pull
{% highlight yaml %}
git pull
{% endhighlight %}

- push
{% highlight yaml %}
git add .
git commit -m '(comment)'
git push -u origin master
{% endhighlight %}

- log
{% highlight yaml %}
git log
{% endhighlight %}

- checkout
{% highlight yaml %}
git checkout (hash) .
{% endhighlight %}
