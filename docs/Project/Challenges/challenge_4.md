---
layout: default
title: Challenge 4
nav_order: 4
has_children: false
parent: Final Project Part 2
grand_parent: Final Project
---

# Challenge 4
**Difficulty: <span style="color:#F9DB24">●●</span>**

**Link:** <a href="https://datahub.berkeley.edu/hub/user-redirect/git-pull?repo=https%3A%2F%2Fgithub.com%2FCodebreakingAtCal%2FCodebreakingLabs&urlpath=tree%2FCodebreakingLabs%2FFinal_Project%2FPart_2%2FChallenge_4%2Fchallenge-student.ipynb&branch=master">Jupyter Notebook</a>

Welcome to the fourth challenge! Here, you will be taking the role of an **active attacker** rather than a passive one. You will be given the function **interceptMessage(data)** within the class **Interceptor** which intercepts every communication between the client and server will be called with.

For example, if the client sends "data", then the function interceptMessage("data") gets called and the server gets the **output** of interceptMessage("data") as the data.

On top of that, the following functions have been changed:
- **generateSignedECDH**
- **verifyECDHMessage**

Recover the user's password.

<details>
    <summary>HINT</summary>
    If integrity isn't verified, what can an attacker do to the message in transit?
</details>

### Submission

Once you've recovered the password, enter it into the Gradescope page [here](https://www.gradescope.com/courses/406561/assignments/2458295) and copy-paste your **Interceptor** class in the same assignment.