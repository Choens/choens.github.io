---
title: Announcing - The Analytic Toolkit
author: Andy Choens
layout: post
category: R

---

Programmers have a maxim: DO NOT REPEAT YOURSELF
([DRY](http://en.wikipedia.org/wiki/Don't_repeat_yourself)). The
Analytics Toolkit project is my attempt to follow this maxim at the
project level.

At any given moment, I have a half-dozen analysis
projects in the air. Some of these consist of only a couple of R
files. Many projects are made up of of many files, scattered over
multiple folders. It makes my life easier if these projects all look
and feel the same. For example, project specific functions should
always be in the same folder (R). And it would be nice if I already had
README file templates (Markdown or Org) set up in a consistent manner.

I have created a series of repositories on my Github account, all
starting with the word "analytic". Combined, these are what I am
referring to here as the "Analytic Toolkit". Each repository has a
specific purpose, but they are all interconnected.

- [Analytics Templates](https://github.com/Choens/analytic-templates):
      A collection of template files. For example, analysis.R, is a
      template file for a simple analysis. These files are useful
      because they provide a consistent layout and structure. Each
      file is intended to be individually useful. Clone the repository
      to your local computer and copy / paste the individual template
      files as they become useful to you.
- [Analytic Template - R](https://github.com/Choens/analytic-template-r):
  A "project template" for analysis in R. Contains a consistent set of
  folders, README files, and functions that I use for all my
  projects. I felt I was wasting time re-creating the same project
  structure over and over again. This is my solution. 
- [Analytic Config](https://github.com/Choens/analytic-config): Useful
  tools for setting up a new system.

Right now, these tools are only an outline of what I would eventually
like to create, but anyone is free to follow, fork, and contribute.
