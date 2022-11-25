---
layout: default
title: Challenge 7
nav_order: 7
has_children: false
parent: Final Project Part 2
grand_parent: Final Project
---

# Challenge 7
**Difficulty: <span style="color:red">●●●</span>**

**Link:** <a href="https://datahub.berkeley.edu/hub/user-redirect/git-pull?repo=https%3A%2F%2Fgithub.com%2FCodebreakingAtCal%2FCodebreakingLabs&urlpath=tree%2FCodebreakingLabs%2FFinal_Project%2FPart_2%2FChallenge_7%2Fchallenge-student.ipynb&branch=master">Jupyter Notebook</a>

Welcome to the 7th challenge! This challenge may be considerably harder than the previous ones, though not necessarily longer.

You managed to leak the user's password, but they changed it to something new shortly after.

On top of that, the server has decided to upgrade to AES-CTR mode instead of AES-CBC, having heard good things about its security.

The following functions have been changed:

- **encryptMessage**
- **decryptMessage**

Note: The rest of the utility functions are in utils.py, but none have been changed except for the above two. You are provided with a copy of the updated code below.

Recover the user's new password.
<details>
    <summary>HINT</summary>
    Initialization Vectors provide a source of 'randomness' to block ciphers. What happens if an IV is reused?
</details>

### Submission

Once you've recovered the password, enter it into the Gradescope page [here](https://www.gradescope.com/courses/406561/assignments/2459061) and copy-paste your **recoverPassword** function in the same assignment.