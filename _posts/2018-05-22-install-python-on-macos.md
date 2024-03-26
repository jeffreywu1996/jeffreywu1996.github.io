---
layout: post
title: Guide to install Python correctly on MacOS
category: Guides
---

I work quite a bit with python, it's my go to language whenever I need to a quick script to get something done.

In this guide, I will talk about:
* manage python with homebrew
* virtualenv
* virtualenv wrappper

### What's Homebrew
Homebrew (link) is a package manager for MacOS. If you are familiar with linux, it is the equivilant of `apt-get`.
I use homebrew to install and update most of my development tools.

### Installing python with Homebrew
Most modern system nowadays should have python installed but usually those python are never updated and are often outdated. You can check its version by typing `python --version` in your terminal.

On the MacOS, the default python used is installed by Apple. This version of python is severly outdated (In fact, Apple still uses python 2 which is deprecated now.)

To begin, you should have homebrew installed. (link to install here) If you have not done so, go to the link provided.

Next, simply type `brew install python` to install brew's version of python. As of right now, brew automaticlly installs python 3 to the folder /usr/local/bin. (Default python is at /usr/bin).

To update python, just type `brew update` and `brew upgrade`. The update will download the new versions of its dependencies and the upgrade will actually upgrade to the new versions.

## Virtualenv

Virtualenv allows you to have multiple different development environments. What this means is that I can have a project that uses python 2.7 while another uses python 3.2. Or I might want the old selenium library for legacy code while in another project I will want the newest one.
Virtualenv, or virtual environments, allow you to setup a temporary development environment for each python project.

To install, type `pip install virtualenv virtualenvwrapper`.

When you want to create a new virtualenv just type `mkvirtualenv <env name>` to initialize a new virtualenv. To activate it, type `workon <env name>`. To disable it, type `deactivate`.

So there you go, I'll update this later to talk more about the virtualenv.

WIP.
