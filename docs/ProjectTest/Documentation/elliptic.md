---
layout: default
title: Elliptic Curves
nav_order: 11
has_children: true
parent: Documentation
grand_parent: Final Project
---

# Elliptic Curve Functions

## isElliptic(E, p)

| Input      | Output |
| ----------- | ----------- |
| int[2] E | bool |
| int p |  |

Takes in an elliptic curve **E** in the form **[A,B]** as well as its modulus **p**. Returns whether **E** is a valid elliptic curve (does not have a zero discriminant).

## evaluateP(x, E, p)

| Input      | Output |
| ----------- | ----------- |
| x  float[] | float[2] |
| int[2] E |  |
| int p |  |

Takes in an elliptic curve **E** in the form **[A,B]**, modulus **p**, and x-coordinate **x**. Returns **[y_1, y_2]** such that **(x, y_1)** and **(x, y_2)** are points on **E** (can sometimes just return [0] if only **(x, 0)** exists). If no such points exist, returns **[]**.

## pointOnCurve(P, E, p)

| Input      | Output |
| ----------- | ----------- |
| x float[] | bool |
| int[2] E |  |
| int p |  |

Takes in an elliptic curve **E** in the form **[A,B]**, modulus **p**, and x-coordinate **x**. Returns whether there is at least one point on the curve with an x-coordinate of **x**.

## addPoints(P, Q, E, p)

| Input      | Output |
| ----------- | ----------- |
| P (x,y) | (float x, float y) |
| Q (x,y) |  |
| int[2] E |  |
| int p |  |

Takes in an elliptic curve **E** in the form **[A,B]**, modulus **p**, and points **P**, **Q**. Returns **P \oplus Q**, where **\oplus** denotes elliptic curve addition.

## doubleAndAdd(P, n, E, p)

| Input      | Output |
| ----------- | ----------- |
| P (x,y) | (float x, float y) |
| Q (x,y) |  |
| int[2] E |  |
| int p |  |

Takes in an elliptic curve **E** in the form **[A,B]**, modulus **p**, scalar **n**, and point **P**. Returns **nP**, where **nP** denotes adding **P** to itself **n** times.

## messageToPoint(m, E, p, K=100)

| Input      | Output |
| ----------- | ----------- |
| int m | (float x, float y) |
| int[2] E |  |
| int p|  |
| int K|  |

Converts integer **m** to a unique elliptic curve point over the curve **E** with modulus **p**. Uses **K=100** by default.

## pointToMessage(P, K=100)

| Input      | Output |
| ----------- | ----------- |
| P (x,y) | int |
| Q (x,y) |  |

Converts elliptic curve point **P** to a unique integer, using tolerance **K**. **K = 100** by default. 


## generateECDH(generatorPoint, E, p, N)

| Input      | Output |
| ----------- | ----------- |
| generatorPoint (x,y) | (float x, float y) nP |
| int[2] E | int n |
| int p |  |
| int N |  |


Given point **P**, order **N**, curve **E** and modulus **p**, returns (nP, n) where **n** is within **[2, N-1]** (inclusive). **n** is the secret Diffie-Hellman key while **nP** is the public value.

## combineECDH(publicPoint, k, E, p)

| Input      | Output |
| ----------- | ----------- |
| publicPoint (x,y) | (float x, float y) nP |
| int k |  |
| int[2] E | int n |
| int p |  |

Given publicPoint **bP**, secret **a**, curve **E** and modulus **p**, returns **a(bp) = (ab)P** as the shared ECDH secret. Works in either direction, as long as the publicPoint is the one multiplied with the other secret than **k**.