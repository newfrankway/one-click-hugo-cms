---
title: What a Shortcode is
date: 2022-06-09T19:05:14.189Z
description: "Shortcodes are simple snippets inside your content files calling
  built-in or custom templates. "
image: img/about-single-origin.jpg
---
Hugo loves Markdown because of its simple content format, but there are times when Markdown falls short. Often, content authors are forced to add raw HTML (e.g., video `<iframe>`’s) to Markdown content. We think this contradicts the beautiful simplicity of Markdown’s syntax.

Hugo created **shortcodes** to circumvent these limitations.

A shortcode is a simple snippet inside a content file that Hugo will render using a predefined template. Note that shortcodes will not work in template files. If you need the type of drop-in functionality that shortcodes provide but in a template, you most likely want a [partial template](https://gohugo.io/templates/partials/) instead.

In addition to cleaner Markdown, shortcodes can be updated any time to reflect new classes, techniques, or standards. At the point of site generation, Hugo shortcodes will easily merge in your changes. You avoid a possibly complicated search and replace operation.