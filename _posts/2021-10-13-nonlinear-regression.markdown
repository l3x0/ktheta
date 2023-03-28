---
layout: post
title:  "Nonlinear regression alternatives"
date:   2021-10-13 13:58:07 -0300
categories: soil physics
---

Nonlinear regression techniques have a fundamental role in soil physics and physics in general. They are used to fit nonlinear models to data. Nonlinear models are equations that are nonlinear in terms of the parameters, that is, the derivatives of the functions with respect to the paramaters are nonlinear functions of the parameters. 

A class of important models in soil physics and groundwater hydrology are water retention curves. These are often nonlinear equations that need to be fit to data of soil volumetric water content and matric potential. A nonlinear equation usually used to model soil and fine sediments data is the Brutsaert-van Genuchten (BvG) equation

$$ \theta = \theta_r + \frac{(\theta_s - \theta_s)}{( 1 + (\alpha |\psi|)^n)^m} $$

In which $$ \theta_r$$, $$\theta_s$$, $$\alpha$$, $$n$$ and $$m$$ are more or less physically based fitting parameters. Because this equation is nonlinear it cannot be fitted using linear regression, which is an exact procedure and would result in unique values for the fitting paramters. A numerical approximation procedure is necessary. A common technique for fitting nonlinear models is nonlinear least squares which aims to minized the sums of squares of the residuals by finding an optimal parameters vector. The most common search procedures used in commercial and noncommercial software are the Gauss-Newton and Levenberg-Marquardt. The latter is a particularly interesting alternative because it provides a bi-directional step which might have better chances of convergence than unidirectional procedures such as Gauss-Newton and the Gradient-Descent and because it is able to deal with singular matrices.   


<h2> Commercial worksheets </h2>

<h2> Libreoffice calc </h2>

<h2> Gnuplot </h2>

<h2> Python </h2>


{% highlight java %}
for (i = 1; i < n; i++){}
{% endhighlight %}



