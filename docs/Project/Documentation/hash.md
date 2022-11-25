---
layout: default
title: Hashing / MACs
nav_order: 9
has_children: true
parent: Documentation
grand_parent: Final Project
---

# Hashing/MAC Functions

## hash_SHA256(M)

| Input      | Output |
| ----------- | ----------- |
| int M | int H(M) |

Takes in an arbitrary integer and returns its SHA256 hash (in the form of an integer).

## generateHMAC(key, data)

| Input      | Output |
| ----------- | ----------- |
| (int, bytes) key | string hex_hmac |
| bytes data |  |


Takes in a key (either int or bytes) and data bytes. Returns 
**HMAC(K, M)** in the form of a hexadecimal string.

## verifyHMAC(key, data, hmac)

| Input      | Output |
| ----------- | ----------- |
| (int, bytes) key | bool |
| bytes data |  |
| string hex_hmac |  |

Takes in a key (either int or bytes). data bytes, and a HMAC in the form of a hexadecimal string. Returns True if
**HMAC(K,M) = hmac** and False otherwise.