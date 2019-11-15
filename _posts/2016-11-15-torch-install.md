---
layout: post
title:  "Pytorch Installation using Anaconda"
date:   2019-11-15
excerpt: "Pytorch Installation"
project: false
tag:
- Anaconda
- Environment
- Pytorch
comments: false
---

![Anaconda-logo](/assets/img/anaconda-logo2.png)
![Pytorch-logo](/assets/img/pytorch_logo.jpeg)
<center><b>Anaconda+pytorch</b></center>


## Pytorch Installation using Anaconda
<b>Windows</b>
{% highlight yaml %}
#Cuda Version Check
C:\Users\oo>nvcc --version

#Activate Virtual Environment
#C:\Users\oo>activate <b>EnvironmentName</b>
C:\Users\oo>activate torch37

#Install Pytorch(GPU)
#C:\Users\oo>conda install pytorch torchvision cudatoolkit=<b>Cuda Version</b> -c pytorch
C:\Users\oo>conda install pytorch torchvision cudatoolkit=10.1 -c pytorch

#Install Pytorch(CPU)
C:\Users\oo>conda install pytorch-cpu –c pytorch
