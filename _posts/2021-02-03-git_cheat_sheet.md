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
1. User information
    {% highlight yaml %}
    git config credential.helper store
    {% endhighlight %}

2. initialize / clone
    {% highlight yaml %}
    git init
    git clone [url]
    {% endhighlight %}

3. status
    {% highlight yaml %}
    git status
    {% endhighlight %}

4. pull
    {% highlight yaml %}
    git pull
    {% endhighlight %}

5. push
    {% highlight yaml %}
    git add .
    git commit -m '(comment)'
    git push -u origin master
    {% endhighlight %}

6. log
    {% highlight yaml %}
    git log
    {% endhighlight %}

7. checkout
    {% highlight yaml %}
    git checkout (hash) .
    {% endhighlight %}
