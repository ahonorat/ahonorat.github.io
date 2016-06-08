---
layout: post
title:  "Algorithm to find dimensions of a flattened index"
date:   2016-06-08 22:04:00 +0200
category: Algo
tags: [algorithm, dimensions, indexation]
---

## How to retrieve each dimension's index from a flattened single integer index

Pseudo-code example for the flattened ```index```, in the four dimensions
```W, X, Y, Z```:

~~~java
int tmp1 = index;
int tmp2 = X * Y * Z;

int w = tmp1 / tmp2;

tmp1 = tmp1 % tmp2;
tmp2 = X * Y;

int x = tmp1 / tmp2;

tmp1 = tmp1 % tmp2;
tmp2 = X;

int y = tmp1 / tmp2;

tmp1 = tmp1 % tmp2;
tmp2 = 1;

int z = tmp1 / tmp2;
~~~

This algorithm could easily be generalized for an arbritary number of dimensions,
example will be provided another time ...