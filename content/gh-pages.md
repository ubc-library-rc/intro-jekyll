---
layout: default
title: GitHub Pages
permalink: /gh-pages/
parent: Part 2 - Diving deeper
nav_order: 5
---

## Get your site online with GitHub Pages

Now that you have a Jekyll site set up locally in your system we are ready to host through Github Pages.

Before we begin, log in to Github.com and create a new repository to have it ready. The new repository should have a name that relates to your site.

1) From your terminal (the unix shell), navigate into the site folder that you set up locally. Replace "your-site-folder-name" with the name of your Jekyll site folder.

Input
{: .label .label-green}
~~~
cd your-site-folder-name
~~~

2) Now you need to "initialize" the site folder which essentially tells Git that you want it to pay attention to this folder.

Input
{: .label .label-green}
~~~
git init your-site-folder-name
~~~

Output
{: .label .label-yellow}
~~~
Initialized empty Git repository in /Users/yourusername/your-site-folder-name/.git/
~~~

3) Change directory to this new local git repository that you made.

Input
{: .label .label-green}
~~~
cd your-site-folder-name
~~~

To check that everything is okay and that git is initialized you can enter "git status" and you should see a message that tells you what branch you are on and what commits have been made (none).

Input
{: .label .label-green}
~~~
git status
~~~

Output
{: .label .label-yellow}
~~~
On branch master

No commits yet

nothing to commit (create/copy files and use "git add" to track)
~~~

From this point you have a couple of options. Github Pages is set up to look at whichever folder you specify as the site folder. For this workshop we will ask Github Pages to look at the "master" branch for site files and will not create an additional docs folder. By doing this we are essentially telling Github that all of the files in our repository are relevant to this site.

4) Add your "local" Jekyll site files to a "remote" branch -- the master branch of the new repository we made in Github. Replace "yourusername" with your Github username and "your-Github-repository" with the name of the repository that you made.

Input
{: .label .label-green}
~~~
$ git remote add origin https://github.com/yourusername/your-Github-repository.git
~~~

5) Push your site up to Github. Note that if you had made a different branch you would replace "master" with the name of that branch.

Input
{: .label .label-green}
~~~
git push -u origin master
~~~

If you do not have any commits in your repository (eg. if you did not initialize it with a README) you might run into an error. To get around this make an initial commit.
{: .note}

~~~
git commit -m "initial commit".
~~~

6) In Github, navigate to your repository landing page and then click "Settings".
Scroll down to the "Github Pages" section of settings and make sure that the site source is set to "master branch". If everything is working correctly you should see your site at a url that looks like: https://yourusername.github.io/your-repository-name/.


[See also Github's documentation on this.](https://help.github.com/en/github/working-with-github-pages/adding-a-theme-to-your-github-pages-site-using-jekyll){:target="_blank"}.
