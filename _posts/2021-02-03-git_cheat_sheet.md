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
git config --global user.name "(id)"
{% endhighlight %}

{% highlight yaml %}
class Solution:
    def longestPalindrome(self, s: str) -> str:
        #step1
        T = '#'.join(f'#{s}#')
        n = len(T)
        A = [0] * n
        r = p = 0
        #step2
        for i in range(1, n - 1):
        #step4,5
            A[i] = (r > i) and min(r - i, A[2 * p - i]) 
        #step6
            while i - 1 - A[i] >= 0 and i + 1 + A[i] < n and \
                    T[i + 1 + A[i]] == T[i - 1 - A[i]]:
                A[i] += 1
        #step3
            if i + A[i] > r:
                p, r = i, i + A[i]
        maxLen, centerIndex = max((n, i) for i, n in enumerate(A))
        return s[(centerIndex - maxLen) // 2: (centerIndex + maxLen) // 2]
{% endhighlight %}


