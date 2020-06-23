---
layout: default
title: Concepts and Terms
permalink: /concepts/
parent: Part 1 - The basics
nav_order: 1
---

# Concepts and terms

This section will introduce a few concepts and terms for you to be aware of before you begin configuring and creating your site.

### What are static sites?

Static sites are websites without a graphical user interface (GUI) to manage content, aka a content management system (CMS). Examples of CMSs include Drupal, WordPress, Wix, and Squarespace. While some like this back end for administering sites, CMSs often come with technical and sometimes financial costs. Services like Wix and Squarespace also restrict your ability to export your content which can be problematic if you ever want to move your site. They may require frequent updates to stay running and secure and a zoo of plugins in order to customize to your needs. This adds up to bogged down load time with unnecessary processes trying to run on a page.

Static sites come without much of the overhead that comes with a CMS. Instead they are built with human-readable markup and styling, and have the option to be extended with code like JavaScript and other scripting languages. This simple recipe is much easier for your (and your users') web browser to load. For most small sites, this is the optimal setup for cost and functionality.

Traditionally, the one major downside to working with and maintaining statics sites has been the high barrier for entry without some previous experience or knowledge with Git, the Unix Shell, HTML/CSS, and code editing. However, we will be using a "quick start" workflow in this workshop that will allow us to create a new site in a few easy steps entirely in a web browser. Nevertheless, the following sections will outline the basics of jekyll and static sites to give an overall sense of how such sites work.

### Building blocks of a static site

Static sites rely on formatting and style in order to look a particular way, as well as scripts to interact with users.

#### Structure and format

Structuring and formatting elements of your site – like placing text, images, and other content in areas on web pages – is traditionally done with hypertext markup language (**HTML**). We'll also use **Markdown** in this workshop for inserting formatted text. Markdown is a simplified way of formatting web content, and is a handy method for avoiding html markup.

#### Style

Styling your site's look and feel – like making text a certain typeface, rounding corners on your images, and making the background be a specific color – is done with cascading style sheets (**CSS**).

#### Interaction and automation

Most of the interaction that you'll see on your site is powered by a script which runs on certain events when a page loads or is scrolled, a button is clicked, a mouse hovers an object, etc. **JavaScript** is one very common scripting languages used in the web, and it integrates very well with static sites.

**For this workshop we're going to stick to Markdown.**

## Learning

- [Intro to Git and GitHub workshop](https://jeremybuhler.github.io/rc-git/){:target="_blank"}
- [Intro to the Unix Shell workshop](https://ubc-library-rc.github.io/intro-shell/){:target="_blank"}
- [Internetting is Hard (for HTML and CSS)](https://internetingishard.com/){:target="_blank"}

### Markdown

- [Adam Pritchard's Markdown Cheatsheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet){:target="_blank"} - An quick overview of Markdown format
- [Markdown Guide](https://www.markdownguide.org/){:target="_blank"} - A more in-depth introduction to using Markdown
- [Dillinger](https://dillinger.io/){:target="_blank"} - An online Markdown editor with a live preview
