---
layout: default
title: What is Jekyll?
permalink: /jekyll/
parent: Part 2 - Diving deeper
nav_order: 1
---

# What is Jekyll?

Jekyll is a popular site generator that transforms plain text documents (Markdown, HMTL, CSS, etc.) into static sites that can easily be used for blogs and informational websites. Jekyll works very well with traditional Git and GitHub workflows, and so if you are already familiar with those, Jekyll site building will seem straightforward. If you aren't, don't worry – this workshop is meant for beginners. Jekyll is written in Ruby and so you'll notice some Ruby-specific terminology (like "Gems").

### Anatomy of a Jekyll site

Let's take a look at your new Jekyll installation and see what's there. Most of the information here is from the [Official Jekyll documentation](https://jekyllrb.com/docs/){:target="_blank"}.

#### File Structure

The default Jekyll package will install a directory of files that make up your site. Canonical information about this [file structure](https://jekyllrb.com/docs/structure/){:target="_blank"} can be found here. Your new installation should have installed a directory with a file structure that looks similar to this:
```
.
├── _config.yml
├── _drafts
├── _includes
|   ├── footer.html
|   └── header.html
├── _layouts
|   ├── default.html
|   └── post.html
├── _posts
|   ├── 2020-02-10-welcome-to-jekyll.md
├── _sass
|   ├── _base.scss
|   └── _layout.scss
├── _site
├── 404.html
├── about.md
├── Gemfile
├── Gemfile.lock
└── index.html
```
Many of the files listed here are used by Jekyll to "transform" your content into a site – which is generated on-the-fly, and stored in the folder **_site**. For this workshop we're going to concentrate on the essentials, including the **config.yml** file, posts, pages, and styling. But let's go through some of these default files and directories so we're familiar with what's there.
- **_config.yml**: This is one of the most important files listed. It includes configuration information about your site such as the site's title, admin email, description, Twitter handles, and other things that are universal about to your site. [More information about Jekyll configuration settings can be found here](https://jekyllrb.com/docs/configuration/){:target="_blank"}.
- **_drafts**: The _drafts folder is where your not-yet-published posts reside. [More info about working with drafts can be found here](https://jekyllrb.com/docs/posts/#drafts){:target="_blank"}.
- **_includes**: The _includes folder is where reusable content for your page layouts and posts is stored. This can include things like your page's header and footer. More information about includes. [More information about includes](https://jekyllrb.com/docs/includes/){:target="_blank"}.
- **_layouts**: The layouts folder contains templates for the default layout of different types of site content. For example, information about how blog posts vs. informational page are displayed. [More information about layouts](https://jekyllrb.com/docs/layouts/){:target="_blank"}.
- **_posts**: The posts folder contains all of your posts or "dynamic content", usually in Markdown or HTML format. The file names for posts must begin the the date of the post (post drafts can exist without dates). [More information about posts can be found here](https://jekyllrb.com/docs/posts/){:target="_blank"}.
- **_sass**: The sass folder is where all of your site's styling is found. More [information about sass](https://jekyllrb.com/docs/assets/#sassscss){:target="_blank"} and [Jekyll site styling](https://mademistakes.com/articles/jekyll-style-guide/){:target="_blank"}.
- **_site**: This is where all of the content transformed by the Jekyll engine is deposited. You don't have to worry about or do anything to this folder.
- **404.html**: This is a default "404" error page. People only see this if they've been directed to a page on your site that doesn't exist.
- **about.md**: This is a static page part of the Jekyll installation. It will appear in the main navigation of your site if left in the main Jekyll directory. You can delete or modify the file however you like.
- **Gemfile and Gemfile.lock**: These files were placed in the default directory if you installed Jekyll using Bundler. These define the gem dependencies for your site.
- **index.html**: This is the default landing page for your site written in HTML, but it can also be written in Markdown.

## Start your Jekyll server
Now that we've looked at the content that makes up the default Jekyll site, let's take a look at the same content as it's rendered by your internet browser. Jekyll uses a web server to transform its content into a website. So in order to see your live site, you'll need to start a local web server to see the development site correctly in your browser.

In your Unix shell start your server using the command:
~~~
$ bundle exec jekyll serve
~~~

Now head to [http://127.0.0.1:4000/](http://127.0.0.1:4000/){:target="_blank"} to see your site in your browser. You should see the default Jekyll site homepage and styling:

![site](blanksite1.png){: border="1"}

You may really like the way this default site looks and can use it as-is. Or, you might want to start building your own site from scratch. Each direction comes with its own costs and benefits. For this workshop, we're going to customize the default site and add some content. Then we'll show you how you can install themes that fit your project's look, feel, and desired functionality.

### Customize your _config.yml

Notice that your site's title and email are still set to the generic default. "Your awesome title", "your-email@example.com", and other settings can be re-configured in the <code>_config.yml</code> file. A .yml (pronounced "yammel") file is a text file that contains structured markup that Ruby consumes and understands. All of the text in the <code>_config.yml</code> is site configuration information.

In your code editor, open your <code>_config.yml</code> file. You should see the text that makes up this file – something like:

~~~
title: Your awesome title
email: your-email@example.com
description: >- # this means to ignore newlines until "baseurl:"
  Write an awesome description for your new site here. You can edit this
  line in _config.yml. It will appear in your document head meta (for
  Google search results) and in your feed.xml site description.
baseurl: "" # the subpath of your site, e.g. /blog
url: "" # the base hostname & protocol for your site, e.g. http://example.com
twitter_username: jekyllrb
github_username:  jekyll

# Build settings
theme: minima
plugins:
  - jekyll-feed
~~~

Here you can see some of the configuration settings of your Jekyll site, including your title and email. Change the site's title to "**[your name]'s Project Site**", and the email address to your email's.

Save your document and refresh your browser. You should see the changes reflected on your local site.
