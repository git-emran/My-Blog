---
title: "Static sites in Hugo"
author: "Emran Hossain"
authorAvatarPath: "/avatar.jpg"
summary: "Creating static sites fast and efficiently with Hugo."
date: ""
description: "Art is a fuel for the soul"
toc: true
readTime: true
autonumber: true
math: true
tags: ["design", "engineering"]
showTags: true
hideBackToTop: false
---

## Static sites Do you like them ?

Do you like Static sites ? I do, They are fast. Easy to create. Easy to maintain. This blog is a static site. Building a static site from scratch and maintaining it is not that difficult, but I will NOT say that it is easy. Someone coming from a non-technical background, just forget it.

That is why people created static site generators. They help you generate and publish static sites with ease. If you are interested to get started, I want to point you in the direction of Hugo, I am not sponsored by them, I just use the product because it is somewhat easy to use. IF I can use it, you can too. By you, I mean anyone who is struggling to create lets say a blog or a quick portfolio site. I mentioned Hugo, lets at least understand what they are.

I mentioned static site generators, if you don't know what that is Let me regurgitate from Google, Static sites are websites built with fixed HTML, CSS, and JavaScript files, serving the same content to every user without needing server-side processing or databases, making them fast, secure, and simple for content that doesn't change often.

## What is Hugo ?

Hugo helps you generate static sites. You write in Markdown and publish, that's it. I am not going to explain how to use Hugo templates and all the details. But I am going to help you to get started and at the end of the day have a live static blog that you can easily.

Hugo is ideal for:

- Personal blogs

- Portfolio websites

- Documentation sites

- Marketing pages

- Content heavy websites

Lets create that site. But first Prerequisites.

## Prerequisites

Before starting, make sure you have:

- A GitHub account

- Node.js installed (optional, but useful)

- Git installed

- A Vercel account

- Hugo installed on your machine

Because we are using Vercel to deploy out static site.

To check if Hugo is installed:

```bash
hugo version

```

## Create a New Hugo Site

Open your terminal and run:

```bash
hugo new site my-hugo-site
cd my-hugo-site

```

This creates a basic Hugo project structure.

Key folders you should know:

- `content` contains your pages and posts. You can go into the post folder and start creating `.md` files.

- `themes` contains Hugo themes, there is nothing much to do there unless you want to modify something.

- `layouts` contains templates.

- `static` contains images, fonts, and other static assets. You can store your website images there.

- `config.toml` (or yaml/json) contains site configuration.

## Add a Theme

Hugo does not come with a default theme, so you will need to add one.

You can browse themes at the Hugo Themes website. For this example, we will use a theme as a Git submodule.

```bash
git init
git submodule add https://github.com/theNewDynamic/gohugo-theme-ananke themes/ananke

```

Now Update your config file. Which is `hugo.toml` file

```bash
theme = "ananke"

```

## Create your first Page
