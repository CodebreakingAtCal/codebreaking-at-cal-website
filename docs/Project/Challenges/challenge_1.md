---
layout: default
title: Challenge 1
nav_order: 1
has_children: false
parent: Final Project Part 2
grand_parent: Final Project
---

# Challenge 1
**Difficulty: <span style="color:green">●</span>**

**Link:** <a href="https://datahub.berkeley.edu/hub/user-redirect/git-pull?repo=https%3A%2F%2Fgithub.com%2FCodebreakingAtCal%2FCodebreakingLabs&urlpath=tree%2FCodebreakingLabs%2FFinal_Project%2FPart_2%2FChallenge_1%2Fchallenge-student.ipynb&branch=master">Jupyter Notebook</a>

Welcome to the first challenge! The Part 1 system has been copied in the notebook given.

You've compromised the user's computer after they finished their session with the server. Unfortunately for you, they've erased their password, but you were able to find **their ECDH secret value**, as well as all communication between the client and server (mostly encrypted).

Recover the user's password.
<details>
    <summary>HINT</summary>
    If you know the client's secret and public value, you can just follow the same steps as the client in ECDH to recover the shared secret.
</details>

### Submission

Once you've recovered the password, enter it into the Gradescope page [here](https://www.gradescope.com/courses/406561/assignments/2458985) and copy-paste your **recoverPassword** function in the same assignment.