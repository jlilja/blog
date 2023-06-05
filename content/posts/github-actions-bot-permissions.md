---
title: "Github Actions Bot Permissions"
date: 2023-06-04T15:51:02+02:00
draft: true
---

## Introduction

You might find that you want to automate more and more throught Github actions. This is all fine and dandy and there are a lot of possibilities doing that, however, you need to make sure that its properly setup. This is where Github actions permissions comes in. I'll go into detail about this.

## The story so far

So, back in 2020 Github wrote a [three part blog post](https://securitylab.github.com/research/github-actions-preventing-pwn-requests) about securing Github actions and their workflows in order to prevent unintentional usage. An example of these unintentional usages is allowing forks to run their code in the original repository's workflows which could expose the secrets in the Github action context.
