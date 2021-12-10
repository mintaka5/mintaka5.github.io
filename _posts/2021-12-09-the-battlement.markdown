---
layout: post
title:  "the battlement!"
date:   2021-12-09 12:18:00 -0800
categories: programming java javafx cryptography cellular scaffold security identity anonymity 
---

## who needs walls?
A new project I am designing and developing, called [*battlement*](https://github.com/white5moke/battlement), stems from an idea I wrote in Python 3 or 4 years ago, called *castlewall*. The idea behind that old code was to have a way to approach a protected object and request access to it, without having to engage with the it to provision credentials. The guest object provides a knowledge proof, and the keeper of the protected object will somehow concede this knowledge as truth. It was too one-dimensional, and never came to fruition. 

## the spawning of agents
Thus spawned, *battlement*! The battlement is made up of `n` (`n-1` *explained later here*) agents that account for the gatekeeper, an agent who is only responsible for aggregating truth values from `n` agents, and determining if the guest agent is worth granting access. One agent (re: `n-1`) is reserved as a truth negotiator for the guest agent. Truthiness =)

Here's a brief sketch of my idea:

![napkin sketch of battlement](https://cj5x-bucket-00005.s3.us-west-2.amazonaws.com/main.png)

VALUE IS SOUL!