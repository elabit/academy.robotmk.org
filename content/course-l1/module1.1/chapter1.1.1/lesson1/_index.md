---
title: 'lesson1'
date: 2024-05-01T23:21:07+02:00
draft: true
weight: 1
---


# This is Lesson1. 

Lesson pages will contain the **workshop script** in a readable form, including a lot of images.  

## What I want to achieve

**Side by side to each lesson** there should be a markdown file which holds the **hugo-reveal slides** for that content. Slides are always on lesson level!

Slides should not appear in the menu. 

By having the lesson content and the slide in the same folder, I want them to **use the same image resources.**  
(=The lesson folder should encapsulate the resources for docs and the slides.)

In the Workshop, I want to show the relearn site on the beamer and from each lesson, open then [a link to the slides]("tbd").

## What I did

- installed both themes (reveal, relearn), set in hugo.yaml
- Set outputformat in hugo.yaml (unclear: is there a need to change the basename?)
- The lesson folder contains a `_index.md` with the lesson content
- side by side to that there is the `slide.md`. It contains in the frontmatter: 

I also added the frontmatter as suggested 
```yaml
outputs: Reveal
_build:
    render: always
    list: never
    publishResources: true
```

## The problem

- The slide does not get rendered at all.