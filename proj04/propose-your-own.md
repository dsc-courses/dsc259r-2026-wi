---
layout: page
title: Propose Your Own Dataset 📋
description: Instructions for proposing your own dataset for the Final Project.
parent: '📊 Final Project'
nav_exclude: true
---

# Propose Your Own Dataset 📋
{:.no_toc}

## Table of Contents
{: .no_toc .text-delta }

1. TOC
{:toc}

---

Instead of using one of the three pre-approved datasets (Recipes and Ratings, League of Legends, or Power Outages), you may propose your own dataset. However, your dataset **must** be able to support every step of the project. Read the requirements below carefully before proposing.

---

## Dataset Requirements

Your proposed dataset must satisfy **all** of the following:

1. **Publicly available.** The dataset must be freely accessible online (e.g. from Kaggle, a government data portal, an academic paper, etc.). Since your final deliverable includes a public-facing website, anyone should be able to find and download the data you used. Datasets that require special access, private API keys, or paid subscriptions are not allowed.

2. **Sufficiently large.** The dataset must have at least **1,000 rows** (after any necessary cleaning) and at least **8 columns**. A very small dataset will not support meaningful exploratory data analysis, hypothesis testing, or predictive modeling.

3. **Mix of column types.** The dataset must contain both **quantitative** (numerical) and **categorical** (nominal or ordinal) columns. You need this variety to complete the Baseline Model and Final Model steps, which require you to handle different feature types in a `sklearn` `Pipeline`.

4. **Non-trivial missingness.** At least one column must have a meaningful amount of missing values (not just one or two rows). You need this to complete Step 3: Assessment of Missingness, which requires you to:
   - Reason about whether a column is NMAR.
   - Run permutation tests to determine whether the missingness of a column depends on other columns.

   If your dataset has no missing values at all, it cannot be used for this project.

5. **Supports a hypothesis test.** The dataset must lend itself to at least one interesting hypothesis test or permutation test (beyond missingness). Think about whether you can pose a meaningful question that compares groups or tests an association.

6. **Supports a prediction problem.** The dataset must have a reasonable response variable that you can predict using other columns, either as a **classification** or **regression** task. Make sure there are enough features to build both a baseline model (at least 2 features) and an improved final model (with at least 2 additional engineered features).

7. **Supports a fairness analysis.** The dataset must contain (or allow you to derive) at least two meaningful groups so that you can assess whether your predictive model performs equitably across those groups using a permutation test.

8. **Not a dataset used in DSC 259R lectures, discussions, or other assignments.** Choose something new!

---

## How to Submit Your Proposal

Submit your proposal on Gradescope by **Monday, February 16th, 2026 at 11:59PM PST** — this is one week before Checkpoint 1 is due, giving us time to review and give you a decision before the checkpoint deadline. **You may not begin the project with a custom dataset until your proposal is approved.**

Your proposal should include:

1. **Dataset name and link.** Provide the name of the dataset and a direct URL to download it.

2. **Brief description (2-3 sentences).** What does the dataset contain? How was it collected?

3. **Number of rows and columns.** State the size of the dataset.

4. **Column descriptions.** List the columns you plan to use, along with their types (quantitative, nominal, ordinal) and brief descriptions.

5. **Missingness.** Identify which column(s) have non-trivial missingness and briefly explain why you think the missingness exists (i.e. what is the data generating process that leads to these missing values?).

6. **Proposed question.** State the question you plan to investigate in Steps 1-4.

7. **Proposed prediction problem.** State the prediction problem you plan to tackle in Steps 5-8, including the response variable and whether it is a classification or regression task.

8. **Proposed fairness groups.** Describe the two groups you plan to compare in Step 8: Fairness Analysis.

---

## After Approval

Once your proposal is approved, you will follow the exact same project instructions as everyone else — the only difference is the dataset you use. All eight steps (Introduction through Fairness Analysis), the notebook requirements, and the website requirements apply to you in full.

If your proposal is **not** approved, we will let you know why and give you the option to either revise your proposal (if time permits) or choose one of the three pre-approved datasets.

{: .warning }
Do not wait until the last minute to submit your proposal. If your proposal is rejected and you need to switch to a pre-approved dataset, you will have less time to complete the project.
