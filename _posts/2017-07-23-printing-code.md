---
layout: post
title: Printing source code
category: Code
---

I never thought I would need to print out code on paper.

But that changed when my CSE 150 professor required us to turn in a hard copy of our source code for HW assignments. My first thoughts were the same as yours. why? lol. Isn't turning it online much easier to grade?

But anyways, we just do whatever the professor wants us to right?

This seemed like a easy problem at first. I just go in my editor -> `File` -> `Print`. Easy right? Turns out no, or I wouldn't write this post. My editor vim did not have the print option since is wrapper inside the terminal. Then, I thought, maybe sublime text would have the option to print code. And then again, it didn't. Thus, I was stuck. But I still had to turn in my HW.
So I thought of a stupid and naive way, I just screenshot parts of my code as pictures and paste them in the word document and print.

![screenshot code](https://user-images.githubusercontent.com/13981821/28505711-33c06b26-6fdb-11e7-8913-6a5723d703cf.png)

This is what it look like. It got the job done, but it looked freakish. The image sizes were different so the code size were disproportionate and I hated it.

Then, after a couple unsuccessful searches on how to print out code on google (turns out not a lot of people still print code). I figured, vim must have some sort of way to do this.

I found two commands `:TOhtml` and `:hardcopy > out.ps`.

`:TOhtml` outputs a html version of the code that looks exactly like how it looks on my vim editor. Coloring, code highlighting and line numbers are all there. All I had to do is to open the html file with chrome and print from chrome.

`:hardcopy > out.ps` outputs a postscript file of the code. This code looks different from vim, but it still outputs.
The default settings did not print with line numbers so I had to add the line `set printoptions=number:y` to my vimrc to get it to work. Overall, I feel this is uglier than `TOhtml` which looked exactly the same as my terminal.

![terminal](https://user-images.githubusercontent.com/13981821/28506206-8f44fd06-6fde-11e7-898e-e2221f51ec84.png)
This is the code in my editor vim.

![html](https://user-images.githubusercontent.com/13981821/28506207-90adeff4-6fde-11e7-805a-03138d598cfe.png)
This is the output using `:TOhtml`

![postscript](https://user-images.githubusercontent.com/13981821/28506210-92132e86-6fde-11e7-8eb6-c53e166def0b.png)
This is the postscript output using `:hardcopy`

Both options were native to vim and they both work fine. If you have a nice looking terminal colorscheme, then, `:TOhtml` will be the choice for you. If you have an ugly terminal, don't worry, `:hardcopy` got you covered.

The takeaway from this experience is that vim really has every feature you would ever need.
