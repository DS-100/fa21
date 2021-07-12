---
layout: page
title: Lecture 16 – Cross-Validation and Regularization
nav_exclude: true
---

# Lecture 16 – Cross-Validation and Regularization

Presented by Anthony D. Joseph, Joseph Gonzalez, Suraj Rampure, Paul Shao

Content by Joseph Gonzalez, Suraj Rampure, Paul Shao

- [slides](https://docs.google.com/presentation/d/1MaQJxLvnb7oQZAWaEbBL_1ebNNvPiZHgHPB_QnWtVz8/edit?usp=sharing)
- [video playlist](https://www.youtube.com/playlist?list=PLQCcNQgUcDfov87Pclq27yt7qrgzJigz3)
- [code](https://data100.datahub.berkeley.edu/hub/user-redirect/git-sync?repo=https://github.com/DS-100/sp21&subPath=lec/lec16/&branch=main)
- code HTML: [Part 1](../../resources/assets/lectures/lec16/lec16-part1-cv.html), [Part 2](../../resources/assets/lectures/lec16/lec16-part2-regularization.html)

**Important:** Read this before proceeding with the lectures, as it details what materials you should focus on. (This is also largely recapped in Video 16.1.).

Sections 16.1 through 16.4 discuss train-test splits and cross-validation.
- 16.1, in addition to giving an overview of the lecture, walks through why we need to split our data into train and test in the first place, and how cross-validation works. It primarily consists of slides.
- 16.2 and 16.3 walk through the process of creating a basic train-test split, and evaluating models that we've fit on our training data using our testing data. Code is in "Part 1".
- 16.4 walks through the process of implementing cross-validation. In this video there references to a `Pipeline` object in `scikit-learn`. This is **not** in scope for us, so do not worry about its details. Code is in "Part 1".

Sections 16.5 and 16.6 discuss regularization.
- 16.5 discusses why we need to regularize, and how penalties on the norm of our parameter vector accomplish this goal.
- 16.6 explicitly lists the optimal model parameter when using the L2 penalty on our linear model (called "ridge regression").


There are also three **supplementary** videos accompanying this lecture. They don't introduce any new material, but may still be helpful for your understanding. They are listed as supplementary and not required since the runtime of this lecture is already quite long. They do not have accompanying Quick Checks for this reason.
- 16.7 and 16.8 walk through implementing ridge and LASSO regression in a notebook. These videos are helpful in explaining how regularization and cross-validation are used in practice. These videos again use `Pipeline`, which is not in scope. Code is in "Part 2".


- 16.9 is another **supplementary** video, created by Paul Shao. It gives a great high-level overview of both the bias-variance tradeoff and regularization.  **The instructors highly recommend this video.**



<table>
<colgroup>
<col style="width: 25%" />
<col style="width: 25%" />
<col style="width: 25%" />
</colgroup>
<thead>
<tr class="header">
<th></th>
<th>Video</th>
<th>Quick Check</th>
</tr>
</thead>
<tbody>
<tr>
<td><strong>16.1</strong> <br>Lecture overview. Training error vs. testing error. Why we need to split our data into train and test. How cross-validation works, and why it is useful.</td>
<td><iframe width="300" height="300" height src="https://youtube.com/embed/y6ZW4nZtlhI" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe></td>
<td><a href="https://docs.google.com/forms/d/e/1FAIpQLSeyzg8cTdWXADSk5Ki7EVaOm1h5R_V2iqTfg5Ozv481YRdt4Q/viewform" target="\_blank">16.1</a></td>
</tr>
<tr>
<td><strong>16.2</strong> <br>Using scikit-learn to construct a train-test split.</td>
<td><iframe width="300" height="300" height src="https://youtube.com/embed/_Bzfy7BTjz0" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe></td>
<td><a href="https://docs.google.com/forms/d/e/1FAIpQLSeRph43oLp3hAmD5uH42BMquAoeGAQeey6XCaLsEbUsEZItzg/viewform" target="\_blank">16.2</a></td>
</tr>
<tr>
<td><strong>16.3</strong> <br>Building a linear model and determining its training and test error.</td>
<td><iframe width="300" height="500" height src="https://youtube.com/embed/2i7yj4JhIkw" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe></td>
<td><a href="https://docs.google.com/forms/d/e/1FAIpQLSdRetxoBG08ztF3RUrodibq7N1DzOVkT9AHIkKVNflnkStFNA/viewform" target="\_blank">16.3</a></td>
</tr>
<tr>
<td><strong>16.4</strong> <br>Implementing cross-validation, and using it to help select a model.</td>
<td><iframe width="300" height="300" height src="https://youtube.com/embed/m8580Et4pjY" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe></td>
<td><a href="https://docs.google.com/forms/d/e/1FAIpQLSfi_PiJCgRsdzrI9vwyRKHUV5B37WZfaEh0u6HA-che0Ii3-w/viewform" target="\_blank">16.4</a></td>
</tr>
<tr>
<td><strong>16.5</strong> <br>An overview of regularization.</td>
<td><iframe width="300" height="300" height src="https://youtube.com/embed/NqKtsZpHmRY" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe></td>
<td><a href="https://docs.google.com/forms/d/e/1FAIpQLSfEckJSRCSCkVz_JxGhrf2MtcctLWcT9NBMQFtF3GGcRIRvVw/viewform" target="\_blank">16.5</a></td>
</tr>
<tr>
<td><strong>16.6</strong> <br>Ridge regression and LASSO regression.</td>
<td><iframe width="300" height="300" height src="https://youtube.com/embed/B-labBbXj_c" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe></td>
<td><a href="https://docs.google.com/forms/d/e/1FAIpQLSfz0-SU11o_wgeIUmIoV7VKtCNgwm4WZVrXU-WWsBwPxekIlg/viewform" target="\_blank">16.6</a></td>
</tr>
<tr>
<td><strong>16.7</strong> <br>*Supplemental.* Using ridge regression and cross-validation in scikit-learn.</td>
<td><iframe width="300" height="300" height src="https://youtube.com/embed/frdGPG10dOA" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe></td>
<td><a>N/A</a></td>
</tr>
<tr>
<td><strong>16.8</strong> <br>*Supplemental.* Using LASSO regression and cross-validation in scikit-learn.</td>
<td><iframe width="300" height="300" height src="https://youtube.com/embed/hqZNVrZ3flw" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe></td>
<td><a>N/A</a></td>
</tr>
<tr>
<td><strong>16.9</strong> <br>*Supplemental.* An overview of the bias-variance tradeoff, and how it interfaces with regularization.</td>
<td><iframe width="300" height="300" height src="https://youtube.com/embed/U2J75Iq2nrk" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe></td>
<td><a>N/A</a></td>
</tr>
