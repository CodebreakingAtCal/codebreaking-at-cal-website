---
layout: final_project
title: Final Project
description: A spec on all parts of the final project. 
---
# Introduction

Codebreaking aims to introduce students to cryptography and cryptanalysis. Now it is time to apply the cyrptographic content of this course to a final project. This project will be equivalent to 3 labs in terms of points. As a result, we will be breaking up the final project over 3 distinct parts. 

# Set Up 

Much like previous labs, each link will lead you to a Jupyter Notebook. Furthermore, links will be posted below each subpart for ease of access. The submissions will be done through Gradescope, requiring download of each subpart after completion. 

# Part 1: TLS Handshake 

## Introduction 

Transfer Layer Security (TLS) is a commonly used cryptographic protocol that is often paired with a transmission protocol such as SMTP for email or VoIP for voice calls. This project section will be focused on TLS and HTTP by setting up the infrastructure for a TLS connection between a client and a server. TLS implementations can involve a variety of ciphers and validation steps, but this implementation will use the ***RSA - Elliptic Curve Diffie Hellman (RSA-EDCH)*** TLS method. Each task in this part of the project is designed to use the cryptographic tools we've studied to ensure that a secure connection is established between the client and the server. 

## Important Notes

This project will allow full use of the Codebreaking Python library. As a result, many of the functions implemented in previous labs can be resued in this project. It is highly reccomended that students review previous labs during this project if they are unsure of how to use a certain function or have questions on the functions of certain ciphers or algorithms. 

## Task 1.1: Server Certificate Verification

Since our server and client know about each other's existence, our first step is to verify the Server's Certificate. A Certificate is verification by a certificate authority (IdenTrust and Digicert being the two largest) that a server's public RSA key matches to the server in their database. 

Implement the Certificate Verification step from the Client to the Server. Start by implementing verifyServerCertificate() in Client(). Then set up the infrastructure such that the server and client can connect to each other. 

HINT: Certificate Verification in this project uses RSA. Thus, both parties need each other's public key in this step. 

## Task 1.2: Elliptic Curve Parameter Generation. 

Next, our server needs to set up an Elliptic Curve for the future Diffie Hellman exchange. Use a 

##  Task 1.3: Send Elliptic Curve Parameters to the Client: 

##  Task 1.4: Generate Signed ECDH Message for Server and Client: 

##  Task 1.5: Accept Diffie Hellman Values 

##  Task 1.6: Generate Client Request

## Task 1.7: Server-side Request Verification

## Task 1.8: Create Server Login

## Task 1.9: Verify Server Login 

# Part 2: Challenges

...