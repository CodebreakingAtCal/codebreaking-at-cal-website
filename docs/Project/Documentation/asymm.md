---
layout: default
title: Asymmetric Encryption / Digitial Signatures
nav_order: 10
has_children: true
parent: Documentation
grand_parent: Final Project
---

# Asymmetric Encryption / Digitial Signatures

## generateRSAKeypair(b)

| Input      | Output |
| ----------- | ----------- |
| int bits | int e |
|   | int N |
|  | int d |

Generates an RSA public/private keypair with **b** bits for each number. The tuple (e, N, d) is returned with **e** representing the public exponent, **N** representing the modulus, and **d** representing the RSA private key.

## encryptRSA(message, e, N)

| Input      | Output |
| ----------- | ----------- |
| int message | int ciphertext |
|  int e |  |
| int N |  |

Encrypts the given integer message using the RSA public key 
(e, N). Returns the ciphertext as an integer.

## decryptRSA(encrypted, d, N)

| Input      | Output |
| ----------- | ----------- |
| int encrypted | int plaintext |
|  int d |  |
| int N |  |

Decrypts the given integer RSA ciphertext using the RSA private key **d** and modulus **N**. Returns the plaintext as an integer.

## signRSA(d, M, N)

| Input      | Output |
| ----------- | ----------- |
| int private_key | int signature |
|  int message |  |
| int N |  |

Signs the given integer message using the RSA private key 
**d** over modulus **N**. Returns the signature as an integer.

## verifyRSA(e, S, N, M)

| Input      | Output |
| ----------- | ----------- |
| int e | bool |
|  int signature |  |
| int N |  |
| int expected |  |


Verifies that the given RSA signature corresponds to the expected message. Returns True or False.
