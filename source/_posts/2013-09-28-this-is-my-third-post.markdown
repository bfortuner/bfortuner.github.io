---
layout: post
title: "This is my third post"
date: 2013-09-28 15:41
comments: true
categories: 
---

![test image]({{ root_url }}/assets/geometry.jpg "This is the annotation")

##Setting Up Blog Posts

Now that you have a grasp of partials, static pages, and Jekyll’s basics, let’s move onto transforming the website you’ve built into a blog. In this tutorial, I will be going over how to build a blog using pure Jekyll. There are alternatives, including Octopress, that make the blogging experience a little bit easier (it comes with some nice plugins and such, but nothing we can’t recreate on our own), but the purpose of this tutorial is to teach you how Jekyll works. If you would like to read more about Octopress and what it offers, feel free to visit their website.

Anyhow, building a blog with Jekyll is actually quite easy. It doesn’t require too much work to display posts because Jekyll was originally conceived with blogging in mind. At a high level, setting up Jekyll’s blogging system is very similar to “the loop” in Wordpress. If you’ve ever built a Wordpress theme or know the basics of how Wordpress works, you’ll be at home with Jekyll.

For those unfamiliar with the concept of a “post loop,” it is essentially a way of asking a blogging platform to return a list of posts. In most cases, it will be posts 1-10, after which they will overflow onto the second page and so on and so forth. In this loop, we iterate over each post “object” and spit out HTML for each post, which means the code is the same to display 1, 10, or even a hundred posts.

###Post Dummy Content

Before we write a post loop, we will need some dummy content so we can see the results.

The _posts folder contains all of the blog posts’ content and metadata. Jekyll is pretty smart, so we can also mix Markdown, HTML, and other formats in this folder. For example, the more complicated articles on my website (such as Moore’s Law of the Mind) are written in .html files, whereas regular posts are simply Markdown.

To create a blog post, drop a Markdown file into the _posts folder. However, there is a specific naming structure for posts and the files must be named in this way: