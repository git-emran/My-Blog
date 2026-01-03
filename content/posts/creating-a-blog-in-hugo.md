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

Do you like Static sites ? I do, They are fast. Easy to create. Easy to maintain. This blog is a static site. Building a static site from scratch and maintaining it is not that difficult, but I will NOT say that it is easy. But if you have a bit of knowledge of HTML CSS JavaScript or a Little of just Markdown knowledge you can publish your first site by following this step-by-step guide.

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

Create a new page using Hugo’s CLI:

```bash
hugo new posts/hello-world.md

```

Open the file and update the font matter:

```bash
---
title: "Hello World"
date: 2026-01-01
draft: false
---

Welcome to my Hugo site deployed with Vercel.

```

## Run the Site Locally

Start the local development server:

```bash
hugo server

```

## Build the Static Files

When you are ready to deploy, Hugo generates static files using:

```bash
hugo

```

This creates a `public` folder containing all the HTML, CSS, and JavaScript files. This folder is what Vercel will serve.

## Push your site to GitHub

Create a new GitHub repository and push your code:

```bash
git add .
git commit -m "Initial Hugo site"
git branch -M main
git remote add origin https://github.com/your-username/my-hugo-site.git
git push -u origin main

```

## Deploy the Site on Vercel

- Go to Vercel and log in

- Click New Project

- Import your GitHub repository

- Configure the project

For Hugo, use these settings:

- Framework Preset: Other

- Build Command: hugo

- Output Directory: public

Do Not forget to keep your environment variables into a `.env` file. And add it to gitignore.

## Good Job! You are set!

I am going to assume if you came here, Your site is now live. But in case you didn't, just open Gemini or ChatGPT or Grok just try to debug with an AI, do not ask for the full solution of the problem, but also ask to explain what each step does. Because if you are solving a problem, better understand where it's coming from.

Hugo and Vercel form a powerful combination for anyone who wants a fast, reliable, and maintainable static website. Whether you are building a blog, portfolio, or documentation site, this setup gives you professional grade hosting with almost no operational overhead.

Once you get comfortable with this workflow, you will likely never want to go back to traditional hosting again. But traditional hosting is also fun.
