---
layout: post
title: How to use ssh keys
category: Code
tags: [ssh, code]
---


<div class="message">
  Hello! This is my first genuine technical post, and today I want to discuss SSH keys.
</div>

As a busy Computer Science student, I often find it impractical to visit the school computer labs for homework assignments. Instead, I use SSH to remotely connect to the lab computers and complete my programming assignments.

## What is SSH?
SSH stands for Secure Shell. Essentially, it lets you connect to a remote server or computer through your terminal—provided that you know the server's IP address and have a valid account.

For example, if you have a server with the IP address `192.168.0.1`, and an account with the username `jeff`, you can run:

```
ssh jeff@192.168.0.1
```

If the connection is successful, a password prompt appears. When you enter your password, you are logged in to the remote server.

Over the past three years at UCSD, I have remotely connected many times. Repeatedly typing usernames and passwords can quickly become tedious. To solve this problem, I discovered SSH keys, which automate the login process.

## SSH Keys: Your New Best Friend

SSH keys allow you to log in without manually entering your password every time. They work by using a pair of cryptographic keys to authenticate your connection.

For a detailed guide on setting up SSH keys, check out this tutorial:

[How to create an SSH key](https://www.digitalocean.com/community/tutorials/how-to-set-up-ssh-keys--2)

Thanks for reading, and I hope you find this guide helpful!
