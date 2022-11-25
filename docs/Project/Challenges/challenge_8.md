---
layout: default
title: Challenge 8
nav_order: 8
has_children: false
parent: Final Project Part 2
grand_parent: Final Project
---

# Challenge 8
**Difficulty: <span style="color:red">●●●</span>**

**Link:** <a href="https://datahub.berkeley.edu/hub/user-redirect/git-pull?repo=https%3A%2F%2Fgithub.com%2FCodebreakingAtCal%2FCodebreakingLabs&urlpath=tree%2FCodebreakingLabs%2FFinal_Project%2FPart_2%2FChallenge_8%2Fchallenge-student.ipynb&branch=master">Jupyter Notebook</a>


Welcome to the 8th challenge!

You only have access to the public API for the server (`login` function). You do not have access to the encrypted log of the `admin`'s session, nor the password database.

The following functions has been changed:
- **hash**
- **compareHash**

The server will use `compareHash` and `hash` to evaluate user passwords instead of hash_SHA256. The code for these is below.

Recover the password for the user `admin`.

<details>
    <summary>HINT</summary>
    Would a longer (correct) password take more time to compare than a shorter one? What about if it is partially incorrect?
</details>

### Submission

Once you've recovered the password, enter it into the Gradescope page [here](https://www.gradescope.com/courses/406561/assignments/2461059) and copy-paste your **recoverPassword** function in the same assignment.