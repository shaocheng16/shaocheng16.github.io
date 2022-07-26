---
layout: post
title:  "python performance test"
categories: blog
tags: technique
data: 
---
## python

- pydoc -w main # generating documents for python co
- using yapf to autoformat python code

```
python -m cProfile -o profile -s cputime main.py
snakeviz profile.log
```


