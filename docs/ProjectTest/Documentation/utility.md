---
layout: default
title: Utility
nav_order: 8
has_children: true
parent: Documentation
grand_parent: Final Project
---

# Utility Functions

## egcd(a,b) or extendedGCD(a,b)

| Input      | Output |
| ----------- | ----------- |
| int a      | int d (Greatest common divisor)       |
| int b      | int x       |
| int b      | int y (ax + by = d)       |

Runs Euclid's Extended Algorithm to find **x,y,d** such that 
**ax + by = d** and **d = gcd(a,b)**.

## modularInverse(a,m)

| Input      | Output |
| ----------- | ----------- |
| int a      | int a_inv       |
| int m      |      |

Outputs the modular inverse of **a mod m**.

## findSquareRoot(N, p)

| Input      | Output |
| ----------- | ----------- |
| int N      | int[] roots       |
| int p     |      |

Finds the square root of **p mod m**, that is 
**a^2 = p mod m** in the form **[a,-a]** (mod p). If there are no roots, it returns [].

## millerRabinWitnessQ(a,n)

| Input      | Output |
| ----------- | ----------- |
| int a      | bool       |
| int n     |      |

Returns whether **a** is a Miller-Rabin witness of **p**. If you are unsure what this means, don't worry, it is primarily for internal use in generating prime numbers.

## findPrime(l, u)

| Input      | Output |
| ----------- | ----------- |
| int l      | int p       |
| int u     |      |

Returns a prime between **l** and **u-1** inclusive. **p** is prime 
with high probability (though not 100%, but this is inconsequential).

## int_to_bytes(x)

| Input      | Output |
| ----------- | ----------- |
| int x      | bytes       |

Returns the byte array representation of a given integer.

## getExpansion(n,m)

| Input      | Output |
| ----------- | ----------- |
| int n      | int[]       |
| int m    |      |


Returns the base-m expansion of n, in increasing order of 
exponents. For example getExpansion(5, 2) finds the binary represenation of 6 as [0,1,1] = **110** in base 2. For internal use.

##  textToInt(s)

| Input      | Output |
| ----------- | ----------- |
| string s      | int s       |

Returns the integer representation of a string using ASCII 
ordinals.

##   intToText(m)

| Input      | Output |
| ----------- | ----------- |
| int m      | string s       |

Returns the text representation of an integer using ASCII 
ordinals.


## bxor(b1, b2)

| Input      | Output |
| ----------- | ----------- |
| bytes b1     | bytes b      |
| bytes b2     | bytes b      |


Returns the XOR of two byte arrays.

## getRandomBytes(n) or get_random_bytes(n)

| Input      | Output |
| ----------- | ----------- |
| int n     | bytes      |


Returns a bytearray consisting of **n** random bytes.

