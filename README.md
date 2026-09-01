# An Elementary Proof of the Fundamental Theorem of Algebra over Rationals

This repository contains the paper **“An Elementary Proof of the Fundamental
Theorem of Algebra over Rationals”** by Liang Zhang and Xiaohua (Michael) Xuan.

> [Read the paper (PDF)](<./An Elementary Proof of Fundamental Theorem of Algebra over Rationals.pdf>)

## Overview

The paper gives a constructive, elementary version of the Fundamental Theorem
of Algebra over the rational complex numbers

$$
\mathbb{Q}(i)=\{a+ib:a,b\in\mathbb{Q}\}.
$$

Writing

$$
Q(a+ib)=a^2+b^2
$$

for quadrance, the main theorem states that for every nonconstant polynomial
$f\in\mathbb{Q}(i)[X]$ and every rational $\varepsilon>0$, there is a
$z\in\mathbb{Q}(i)$ such that

$$
Q(f(z))<\varepsilon^2.
$$

The proof uses only finite rational arithmetic and comparisons. Its main
ingredients are:

- a winding number for finite rational closed vertex lists;
- rational variation estimates for polynomial values;
- power cycles along the boundary of a rational square;
- a finite grid triangulation and cancellation of interior edges.

The paper also derives a complete approximate factorization result over
$\mathbb{Q}(i)$.

## Constructive character

The argument supplies a finite search procedure: after choosing an explicit
radius and mesh resolution, one evaluates the polynomial at the vertices of a
finite rational grid until finding a point satisfying the required quadrance
bound.

## Relation to the classical Fundamental Theorem of Algebra

For a fixed polynomial $f\in\mathbb{Q}(i)[X]$, the radius used in the proof
depends only on $f$, not on the requested precision. Taking
$\varepsilon_k=1/k$, choose $z_k\in\mathbb{Q}(i)$ in the same bounded square
such that

$$
Q(f(z_k))<\frac{1}{k^2}.
$$

By the Bolzano–Weierstrass theorem, $(z_k)$ has a convergent subsequence,
say $z_{k_j}\to z\in\mathbb{C}$. Polynomial continuity then gives

$$
Q(f(z))=\lim_{j\to\infty}Q(f(z_{k_j}))=0,
$$

and hence $f(z)=0$. Thus, after adding this classical compactness result, the
paper's rational theorem yields the usual exact-root conclusion for every
nonconstant polynomial in $\mathbb{Q}(i)[X]$.

Approximating arbitrary complex coefficients by rational complex
coefficients, together with a uniform bound for the resulting approximate
zeros, extends the conclusion to polynomials in $\mathbb{C}[X]$. In this way
the argument also recovers the classical Fundamental Theorem of Algebra.

## Authors

- Liang Zhang — corresponding author, <liang.zhang@unidt.com>
- Xiaohua (Michael) Xuan — <michael.xuan@unidt.com>

## Repository contents

- [`An Elementary Proof of Fundamental Theorem of Algebra over Rationals.pdf`](<./An Elementary Proof of Fundamental Theorem of Algebra over Rationals.pdf>) — the paper
