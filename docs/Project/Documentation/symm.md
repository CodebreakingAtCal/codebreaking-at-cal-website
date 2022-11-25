---
layout: default
title: Symmetric Encryption
nav_order: 9
has_children: true
parent: Documentation
grand_parent: Final Project
---

# Symmetric Encryption

## encryptAES(key,data)

| Input      | Output |
| ----------- | ----------- |
| (bytes,int) key | { string iv, string ciphertext }|
| bytes data |  |

Takes in a {16,24,32}-byte `key` (either bytes or int) and arbitrary-length bytes `data`. Runs AES-CBC on these parameters and outputs { iv, ciphertext } as their 
base 64 representations.

**NOTE: It is easier to use Server.encryptMessage(string) (or Client.encryptMessage in the same way, assuming the Server has established a valid connection**.

## decryptAES(key,data)

| Input      | Output |
| ----------- | ----------- |
| (bytes,int) key | string plaintext|
| string encrypted |  |

Takes in a {16,24,32}-byte `key` (either bytes or int) and a JSON-formatted string containing {iv, ciphertext} in Base-64 representation. Returns the ciphertext as a string.

**NOTE: It is easier to use Server.decryptMessage(string) (or Client.decryptMessage in the same way), assuming the Client has established a valid connection**.

