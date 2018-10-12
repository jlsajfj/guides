---
title: Chain Rule Introduction
---
# Chain Rule Introduction

Chain Rule is used to compute the derivative of a composition of functions.

Let _F_ be a real valued function which is a composite of two functions _f_ and _g_  i.e. `F(x) = f(g(x))`and both f(x) and g(x) are differentiable.
Let the derivative D{F(x)} is denoted as F'(x).

By Chain Rule, 

<a href="https://www.codecogs.com/eqnedit.php?latex=F'(x)=f'(g(x))\cdot&space;g'(x)" target="_blank"><img src="https://latex.codecogs.com/gif.latex?F'(x)=f'(g(x))\cdot&space;g'(x)" title="F'(x)=f'(g(x))\cdot&space;g'(x)" /></a>

Suppose, g(x) = t then F(x) = f(g(x)) can be rewritten as F(x)=f(t)
then in Leibniz's notation Chain Rule can be rewritten as : 

<a href="https://www.codecogs.com/eqnedit.php?latex=\frac{d(F)}{dx}=\frac{df}{dt}\cdot&space;\frac{dt}{dx}" target="_blank"><img src="https://latex.codecogs.com/gif.latex?\frac{d(F)}{dx}=\frac{df}{dt}\cdot&space;\frac{dt}{dx}" title="\frac{d(F)}{dx}=\frac{df}{dt}\cdot \frac{dt}{dx}" /></a>



### Example 1.   To compute derivative of sin(ax+b)

Solution : The function can be visualized as a composite of two functions. F(x)= f(g(x))

<a href="https://www.codecogs.com/eqnedit.php?latex=t=g(x)=ax&plus;b" target="_blank"><img src="https://latex.codecogs.com/gif.latex?t=g(x)=ax&plus;b" title="t=g(x)=ax+b" /></a> and <a href="https://www.codecogs.com/eqnedit.php?latex=f(t)=sin(t)" target="_blank"><img src="https://latex.codecogs.com/gif.latex?f(t)=sin(t)" title="f(t)=sin(t)" /></a>

<a href="https://www.codecogs.com/eqnedit.php?latex=\frac{df}{dt}=cos(t)" target="_blank"><img src="https://latex.codecogs.com/gif.latex?\frac{df}{dt}=cos(t)" title="\frac{df}{dt}=cos(t)" /></a>

<a href="https://www.codecogs.com/eqnedit.php?latex=\frac{dt}{dx}=a" target="_blank"><img src="https://latex.codecogs.com/gif.latex?\frac{dt}{dx}=a" title="\frac{dt}{dx}=a" /></a>

Now by Chain Rule: 

<a href="https://www.codecogs.com/eqnedit.php?latex=\frac{d(F)}{dx}=\frac{df}{dt}\cdot\frac{dt}{dx}" target="_blank"><img src="https://latex.codecogs.com/gif.latex?\frac{d(F)}{dx}=\frac{df}{dt}\cdot\frac{dt}{dx}" title="\frac{d(F)}{dx}=\frac{df}{dt}\cdot\frac{dt}{dx}" /></a>

<a href="https://www.codecogs.com/eqnedit.php?latex=\frac{d(F)}{dx}=a\cdot&space;cost(t)=a\cdot&space;cos(ax&plus;b)" target="_blank"><img src="https://latex.codecogs.com/gif.latex?\frac{d(F)}{dx}=a\cdot&space;cost(t)=a\cdot&space;cos(ax&plus;b)" title="\frac{d(F)}{dx}=a\cdot cost(t)=a\cdot cos(ax+b)" /></a>

OR 

We can directly apply the formula <img src="https://latex.codecogs.com/gif.latex?F'(x)=f'(g(x))\cdot&space;g'(x)=cos(ax&plus;b)\cdot&space;a" title="F'(x)=f'(g(x))\cdot g'(x)=cos(ax+b)\cdot a" />


## For a function composite of more than two function :

Let _F_ be a real valued function which is a composite of four functions _r s t u_  i.e. `F(x)=r(s(t(u(x))))` and all the functions _r(x) s(x) t(x) u(x)_ are differentiable.
Let the derivative D{F(x)} is denoted as F'(x).

By Chain Rule, 
#### _`F'(x) = r'(s(t(u(x)))).s'(t(u(x))).t'(u(x)).u'(x)`_

Suppose, a = u(x), b = t(a), c = s(b) then F(x)=r(s(t(u(x)))) can be re-written as F(x)=r(c) 

then, F(x)=r(c) => d(F)/dx = dr/dc . dc/dx                ___ (eqn 1)

c = s(b) => dc/dx = ds/db . db/dx                          ___ (eqn 2)

b = t(a) => db/dx = dt/da . da/dx                          ___ (eqn 3)

a = u(x) => da/dx = du/dx                                  ___ (eqn 4)

Putting the value of eqn 2 3 4 in eqn 1, we will get :

#### `d(F)/dx = dr/dc . ds/db . dt/da . du/dx`


### Example 2.   To compute derivative of sin(cos((mx+n)^3))

Solution : The function can be visualized as a composite of four functions. F(x)= r(s(t(u(x))))

where a = u(x) = mx+n

b = t(a) = a^3 

c = s(b) = cos(b) then F(x)=r(s(t(u(x)))) can be re-written as F(x)= r(c) =sin(c) 

Now, By chain rule :
d(F)/dx = dr/dc . ds/db . dt/da . du/dx

=> d(F)/dx = cos(c) . -sin(b) . 3a^2 . m

=> d(F)/dx = cos(cos((mx+n)^3)) . -sin((mx+n)^3)) . 3(mx+n)^2 . m

OR 

We can directly apply the formula, 

F'(x) = r'(s(t(u(x)))).s'(t(u(x))).t'(u(x)).u'(x) = cos(cos((mx+n)^3)) . -sin((mx+n)^3)) . 3(mx+n)^2 . m
