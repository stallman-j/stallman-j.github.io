---
title: Using Sublime Text with Markdown
#subtitle: Hopefully everything you need and lots of things you hopefully won't
# https://bookdown.org/yihui/rmarkdown/html-document.html#floating-toc
layout: single
toc: true
toc_label: "Contents"
toc_min_header: 1
toc_max_header: 2
toc_sticky: true
author_profile: true
date: "2024-10-02"
---

# Create a Pandoc Build System in Sublime

1. Install Pandoc
2. Install SumatraPDF
3. I followed this link from [Rowan Nicholls](https://rowannicholls.github.io/sublime_text/pandoc.html) to just create a build system so I could get Markdown files converted to PDF that then show up in SumatraPDF viewer, and adapted it just a little because my Sublime Text couldn't find the SumatraPDF executable.

```{shell}
{
    "shell_cmd": "pandoc -o \"$file.pdf\" \"$file\" && start \"C:\\Program Files\\SumatraPDF\" \"$file.pdf\"",
    "selector": "text.html.markdown",
}
```