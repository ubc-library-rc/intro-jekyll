---
layout: page
title: Setting up your system
permalink: /setup/
parent: Part 2 - Diving deeper
nav_order: 10
---

# Setting up your system

In a typical jekyll installation, you would normally build the site locally first, then publish it to the web when you are ready and have some content. In order to work locally, you first have to make sure that our computer has all the necessary software installed. Jekyll needs a full Ruby development environment so you'll need to make sure you have that configured correctly first.

You'll also want to be sure to have a good code editor on your machine to view and edit your code. We recommend using either [Atom](https://atom.io/){:target="_blank"}, [Sublime Text](https://www.sublimetext.com/){:target="_blank"}, or [Notepad++](https://notepad-plus-plus.org/){:target="_blank"}.
{: .note}

## Windows OS

Windows isn't technically a Jekyll-supported platform, but we do have two options that will allow us to work on Windows machines.

### Option 1: Install the RubyInstaller kit

The [RubyInstaller](https://rubyinstaller.org/) kit will run a self-contained environment on Windows machines.

**[Follow these instructions for option 1](https://jekyllrb.com/docs/installation/windows/#installation-via-rubyinstaller){:target="_blank"}**.

### Option 2: Bash on Windows 10

This option is for Windows 10 users only. On Windows 10, you can install and enable the [Windows Subsection for Linux](https://docs.microsoft.com/en-us/windows/wsl/install-win10?redirectedfrom=MSDN). This option might be useful to set up if you anticipate working on other projects that would require the Unix Shell.

**[Follow these instructions for option 2](https://jekyllrb.com/docs/installation/windows/#installation-via-bash-on-windows-10)**.

Once you have completed these steps check that you have Git installed by opening your bash terminal and typing:

~~~
git --version
~~~

If you do not have Git installed, [download it from here.](https://git-scm.com/download/win).

## Mac OS

The Mac operating system needs the Xcode suite to run several tools developers use to create software and applications. So to start, let's install it from the command line if you don't already have it.

### Install X-Code

First install **X-code**
<code>$ xcode-select --install</code>

This should install **GNU Compiler Ccllection (GCC)** and **Git**, but let's make sure. Verify you are running GCC
<code>$ gcc --version</code>
You should see a version number in your shell

Verify you have Git
<code>$ git --version</code>
Again, you should see a version number

### Install RVM

Install the most recent stable version of **Ruby Version Manager (RVM)**. RVM will allow you to use different versions of Ruby (which we'll install next) for website projects and your operating system

<code>$ curl -L https://get.rvm.io | bash -s stable</code>

Now lets verify RVM was installed

<code>$ rvm --version</code>

### Install Ruby with RVM

Now install the most recent stable version of **Ruby** using RVM

<code>$ rvm install "ruby-2.7.0"</code>

Then set that version as the default Ruby installation for our project

<code>$ rvm --default use 2.7.0</code>

Check that Ruby is set to the version we configured

<code>$ ruby -v</code>

And, now generate the core Ruby documentation

<code>$ rvm docs generate-ri</code>

### Install Jekyll and Bundler gems

Now that you have a full Ruby dev environment installed, let's finish by installing Jekyll and Bundler

<code>$ gem install jekyll bundler</code>

We are going to create a new project folder for our Jekyll site installation. Navigate to a folder where you want to locally install and work on your site (maybe a directory where you already have projects like this)

<code>$ cd documents/sites</code>

Create a new Jekyll project called "[your-name]-project-site"

<code>$ jekyll new [your-name]-project-site</code>

And navigate into that new project

<code>$ cd [your-name]-project-site</code>

### Serve and view your site

Now navigate into that directory

<code>$ cd [your-name]-project-site</code>

And start the server to see your blank site

<code>$ bundle exec jekyll serve</code>

Now in your web browser (preferably FireFox or Chrome) go to the address 127.0.0.1:4000 and you should see your new blank site!
