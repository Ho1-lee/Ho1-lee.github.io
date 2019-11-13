---
layout: post
title:  "Anaconda 사용법"
date:   2019-11-13
excerpt: "Anaconda 사용법"
project: false
tag:
- Anaconda
- Environment
comments: true
---

![Anaconda-logo](/assets/img/anaconda-logo2.png)    
    
<center><b>Anaconda</b></center>
     
Anaconda를 통해 Python의 가상환경을 통해 개발환경을 쉽게 관리할 수 있다.<br>
기본적인 사용법을 설명한다.
      
## 설치
[아나콘다 설치 사이트](https://www.anaconda.com/distribution/#download-section) 을 통해 쉽게 Download 가능하다.<br>
*PATH 설정을 통해 CMD에서 명령어 사용 가능.<br>

---

## Version 확인 / Update

{% highlight yaml %}
#version 확인
C:\Users\oo>conda --version
#Update Conda
C:\Users\oo>conda update conda
{% endhighlight %}

---

##가상환경 생성
{% highlight yaml %}
#가상환경 생성
#C:\Users\oo>conda create --name(-n) 가상환경명 설치할패키지
C:\Users\oo>conda create --name test python=3.5
#또는
C:\Users\oo>conda create --n test python=3.5
{% endhighlight %}

---

##가상환경 활성화 / 비활성화
{% highlight yaml %}
#만들어진 가상환경 확인
C:\Users\oo>conda info --envs
#활성화
#C:\Users\oo>activate 가상환경명
C:\Users\oo>activate test
#비활성화
C:\Users\oo>conda deactivate
{% endhighlight %}

---

##패키지 설치 / 확인
{% highlight yaml %}
#가상환경 활성화
#C:\Users\oo>activate 가상환경명
C:\Users\oo>activate test
#패키지 설치
#C:\Users\oo>conda install 패키지명
C:\Users\oo>conda install
#설치된 패키지 확인
C:\Users\oo>conda list
#가상환경 캐시 정리
#인덱스 캐시, 잠긴 파일, 사용하지 않는 패키지, 소스 캐시 등을 삭제
C:\Users\oo>conda clean -all
#또는
C:\Users\oo>conda clean -a
{% endhighlight %}
