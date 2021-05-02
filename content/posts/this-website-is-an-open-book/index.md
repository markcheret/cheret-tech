---
title: "This Website Is an Open Book"
date: 2021-05-02T14:36:41+02:00
draft: false
categories: ["online content"]
tags: [HUGO, gitops, gitflow, workflow]
resources:
- name: "featured-image"
  src: "this-website-is-an-open-book.png"
---

This website is an open book and I'm going to share with you, what that means, why that is and how it works. It took me a good while to get to this point, so I figured it would be helpful for others to speed along their process.

## What does this mean?

This website is built using [HUGO, a static site generator](https://gohugo.io/), it runs on [GitHub Pages](https://pages.github.com/) and is built from [my markcheret/cheret-tech git repository](https://github.com/markcheret/cheret-tech). It's all open to the public: the raw material from which this website is built, the process of how to get there and the resulting website.

## How does it work?

I'm using a [GitOps Workflow](https://www.gitops.tech/) to commit my content to [the main branch of my website's git repository](https://github.com/markcheret/cheret-tech/tree/main). A few [GitHub Actions](https://github.com/features/actions) set up, hosted in [my markcheret/workflows repository](https://github.com/markcheret/workflows) take care of building and deploying the static content to the [GitHub Pages environment of my repository](https://github.com/markcheret/cheret-tech/tree/gh-pages) every time I [merge pull requests](https://docs.github.com/en/github/collaborating-with-issues-and-pull-requests/merging-a-pull-request) to the main branch. Among other things, I have an automated spellcheck, a syntax check for the [markdown](https://en.wikipedia.org/wiki/Markdown) files used to build the content of the website and some image compression for convenience and quicker loading times.

This website is using the [uBlogger Theme by uPagge](https://ublogger.netlify.app/) with some [SCSS](https://sass-lang.com/) overloads for styling I'm also making use of the [HUGO templating system](https://gohugo.io/templates/introduction/) to control some of the behaviour of the theme that I don't like. As an example, when you click my portrait on the [cheret.tech front page](https://cheret.tech/) the original theme opens [my about page](https://cheret.tech/about/) in a new tab, whereas I want it to be loaded in the same window. For the pictures in the posts I'm using [Pablo by Buffer.com](https://pablo.buffer.com/), which makes it very easy to find license free pictures and put some quick text on them. The format is also adaptable to all kinds of uses for different social media and mobile-compatible. All of the legally required pages live in [my git repository with legal documents](https://github.com/markcheret/legal) and are automatically copied to the content directory of all of my websites when they change. So I always have an up-to-date version of that.

## Why do it like this?

I'm using the [GitFlow](https://datasift.github.io/gitflow/IntroducingGitFlow.html) workflow and [GitOps](https://www.gitops.tech/) principle for all of my and my clients' projects. This goes from configuring backups, via hosting microservice configuration, to source code and now also my web content. It all starts with a git repository, which is the description and single source of truth of the target infrastructure. It is automatically being tested, built and deployed from there. It's repeatable, transparent and secure. Since I'm already implementing this process, it only makes sense to use that built-up muscle memory and deliver content reliably with a proven process.

Having implemented all of this process, I have a very quick turnaround time from a content idea (which I can put near the code by opening a GitHub issue using the [GitHub mobile app](https://github.com/mobile)), to fleshing it out inside the corresponding [GitHub Issue](https://guides.github.com/features/issues/) and go to work wherever I have a browser or computer with access to my repositories. Turning the GitHub issue into actual content in no time. It took me less than an hour from the idea for this post, [opening an issue](https://github.com/markcheret/cheret-tech/issues/59), researching over 20 links to [merging the pull request](https://github.com/markcheret/cheret-tech/pull/60), which publishes the fresh content.
