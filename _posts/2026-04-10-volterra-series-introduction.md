---
layout: post
title: Volterra Series for Nonlinear Systems
date: 2026-04-10
description: A brief note on Volterra series representation in nonlinear systems
tags: [nonlinear systems, volterra series, control theory]
---

## Overview

The Volterra series is a functional expansion used to represent nonlinear systems,
analogous to how convolution represents linear time-invariant (LTI) systems.

It expresses the output as a sum of multidimensional convolutions.

---

## Mathematical Form

The output can be written as:

$$
y(t) = h_0 + \int h_1(\tau_1) u(t - \tau_1) d\tau_1
+ \int \int h_2(\tau_1, \tau_2) u(t - \tau_1) u(t - \tau_2) d\tau_1 d\tau_2 + \cdots
$$

where:

- $h_1$ : linear kernel
- $h_2$ : second-order nonlinear kernel
- higher-order terms capture nonlinear interactions

---

## Interpretation

- The first term corresponds to an LTI system
- Higher-order kernels capture nonlinear effects
- It can be seen as a **Taylor expansion in function space**

---

## Remarks

- Useful for weakly nonlinear systems
- Not suitable for strongly nonlinear or discontinuous systems
- Kernel identification is often computationally expensive

---

## Example Thought

For a system:

$$
\dot{x} = Ax + Bu + f(x,u)
$$

the Volterra series can be interpreted as expanding the nonlinear term $f(x,u)$
around an operating trajectory.

---

## References

- [Wikipedia: Volterra series](https://en.wikipedia.org/wiki/Volterra_series)
- Classic nonlinear system theory textbooks

---

## Notes

- Compare with describing function method
- Relation to Wiener series