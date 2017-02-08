---
layout: post
title: How to use ssh keys
---


<div class="message">
  Hello! This is my real first post. And today, I want to talk about ssh keys.
</div>

As a lazy Computer Science student that is too lazy to go to our school's computer labs to do HW but still want to graduate and pass the class, I found a way.

I can 'ssh' into our school's computer labs, and do my programming assignments on my computer thru 'ssh' as if I was actually doing my programming assignments on the acutal lab computers.

## What is ssh?
So first, What is 'ssh'?
SSH stands for Secure Shell. And what does that mean? tbh, it's not important.
What is important is that it lets you connect to a 'server' or 'computer' via your own terminal, given that you know the server's ip address. (Oh, also, you seem to need to have an account on that server as well)

For example, if I have a server with a ip address '192.168.0.1', with an account of username jeff, and password wu, I can type
```
ssh jeff@192.168.0.1
```
and this will try to connect my computer to the server with the account name 'jeff'. Now, if successful, a prompt for password will show up. Now if I type wu and press enter, I would be logged in to the server with that account.
Cool?
Yea, I know.

This is awesome, and the solution to how I have studied computer science at UCSD for 3 years now, but only been to the computer labs less than 10 times.

"Three years you say?", you may ask, "That's right!", I'll say.

"That must been thousands of times you have to ssh to the server, and each time you connect, you gotta type in the account and password?? What a bump man." you will then say ofc.

"Yea! Exactly! Being an engineer that is born to solve problems, obviously I have a solution to that!"

"What could that possibly be????" you will then ask.

## SSH key mah friend!

Ha! What does that do?
Well, my friend, it types in the password for you!
Whoa, yea, I know.

ok, lets get down to business. Lets learn how to set this up.

BTW, I decided to write on ssh keys today because of [this](https://www.youtube.com/watch?v=YQw124CtvO0) youtube video I saw on RSA-129. The man behind the encoding scheme of this ssh thing, apparently.

Bleh, I was gonna write how to do this, but a google search came up with so many good guides. So why reinvent the wheel when you can reuse one?

So, here you go guys!

[How to create an ssh key](https://www.digitalocean.com/community/tutorials/how-to-set-up-ssh-keys--2)

Thanks for reading! Hope you enjoyed it!

