---
title: "Why I Switched from LaTeX to Typst (and You Might Too)"
author: "EmranH"
authorAvatarPath: "/avatar.jpg"
showAuthorAvatar: true
summary: "Moving away from latex because of readability and ease of use"
date: "2025-12-21"
description: "Moving away from latex because of readability and ease of use"
toc: true
readTime: true
autonumber: true
math: true
tags: ["design", "engineering"]
showTags: true
hideBackToTop: false
---

![typstvslatex](/images/typst.jpg)

For a long time, LaTeX has been the default choice for writing serious technical documents. Research papers, theses, books, resumes. If it needed structure and precision, LaTeX was usually the answer. I have used it for years and I still respect what it can do.

That said, respect does not always mean enjoyment.

Recently, I started using Typst, and it changed how I feel about writing technical documents. Not just how fast I can write them, but how natural the whole process feels. This post is about why Typst is slowly replacing LaTeX for me, and why it might be worth your attention too.

---

## The Real Issue with LaTeX Is Friction

LaTeX is extremely powerful. That has never been the problem. The real issue is friction.

If you have spent time with LaTeX, some of these will sound familiar:

- Syntax that feels more like an old programming language than a writing tool

- A lot of boilerplate before you write anything meaningful

- Error messages that are technically correct but practically useless

- Slow compile cycles that interrupt your flow

- Packages that sometimes conflict in confusing ways

LaTeX is optimized for producing correct output. It is not optimized for the experience of the person writing the document.

As people who build software and design systems, we recognize this immediately. When a tool fights your flow, even if it works, it drains energy.

---

## Typst Feels Like a Modern tool

Typst is a newer typesetting system built around a simple idea.

Writing technical documents should feel as smooth as writing code in a modern language or writing prose in Markdown, without giving up high-quality typography.

Typst is not a layer or top of LaTeX. It is a fresh design, and that difference is obvious as soon as you start using it.

---

## Readability Comes First

Here is a simple comparison.

```latex

\\section{Introduction}
This is an \\textbf{important} idea.

```

Where in typst:

```typst

= Introduction
This is an *important* idea.
```

Typst documents look like documents even before they are compiled.

- Headings look like headings

- Emphasis looks like emphasis

- Lists look like lists

You can open a Typst file and read it comfortably. The source itself feels close to the final result.

---

## Fast Feedback Changes Everything

Typst is fast. In many cases, the preview updates instantly.

That means:

- No waiting around for long PDF builds

- No fear that one missing character broke the whole document

- No endless trial and error just to fix layout issues

---

## A Better Mental Model

One of the most refreshing parts of Typst is how consistent it feels.

Functions behave like functions. Styles behave like styles. Layout rules feel predictable. You spend less time memorizing special cases and more time expressing intent.

In LaTeX, you often learn what works by copying patterns and hoping they keep working. In Typst, you can usually reason your way to the solution.

---

## When LaTeX Still Makes Sense

This is not a declaration of war on LaTeX.

If you are working within a strict academic pipeline, collaborating with teams that already rely on LaTeX, or submitting to journals that require specific templates, LaTeX may still be the right tool.

But for personal projects, new papers, documentation, reports, and experiments, Typst is often the more enjoyable choice.

---

## Final Thoughts

Switching from LaTeX to Typst reminded me of something important.

Tools shape how we think and how we work. When the tool is lighter, clearer, and more humane, creativity flows more easily.

Typst feels like it was designed for people who actually write. And once you experience that, it is hard to go back.

If LaTeX has ever made you feel productive but tired, Typst might be worth a serious look.
