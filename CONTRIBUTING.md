# How to contribute

Thank you for your interest in contributing to this effort! These SOPs are published openly with the aim of helping the greater bioinformatics community, so we love to recieve contributions. There are many ways to do so, from reporting typos, issues, suggesting content, ... etc.

 To make it easier, we created this guide- let's dive in!

# Coding/Naming conventions and style

# Documentation

# Road map (milestones we like to eventually achieve)
[] Add authors' contact details next to the pages they contribute to

# Changelog <probably this should go elsewhere?>

# Tips for contributing new content: 

(This is a quick guide adopted from https://idratherbewriting.com/documentation-theme-jekyll/)

- To add ad-hoc pages, just place the markdown file in the root directory. Add a frontmatter similar to this at top (or copy-paste and modify the contents of the file `template_frontmatter.md`). Your content should follow.

```

---
title: <title of your page- will appear at the browser window>
tags: [comma seperated list of tags] 
keywords: <relevant keywords to your content, for search engine> 
last_updated: <date of last update- appears at the bottom of the pate>
summary: <summary of the page if desired> 
sidebar: <The *.yml navigation file in _data/sidebars (see below for details)> 
hide_sidebar: true #Use this if you don't wish to include a sidebar. Otherwise, the default sops_sidebar.yml will appear
permalink: <the same name as your file, with .html extension>
---

<Your intended page content, formatted in markdown. >

```

- For the `tags`, you still need to define them in `_data/tags.yml` file

- For the sidebar, it should refer to a file of the intended table of contents to be found in _data/sidebars  An example is sops_sidebar.yml, and it can be added as below. For more information about its format, refer to [this guide] (https://idratherbewriting.com/documentation-theme-jekyll/#configure-the-sidebar) and [this](https://idratherbewriting.com/documentation-theme-jekyll/#sidebar-syntax).


```
sidebar: sops_sidebar
```

- For top navigation, simply edit the file: `_data/topnav.yml`

- To insert special boxes to your page: warning, note, tip, info, ... etc, you may use the following `div`s in your markdown:

|**Type**         | **class** |
| --------------- | -----------
| tip             | '<div class="alert alert-success" role="alert"><i class="fa fa-check-square-o"></i> <b>Tip: </b>'
| note            | '<div class="alert alert-info" role="alert"><i class="fa fa-info-circle"></i> <b>Note: </b>'
| important       | '<div class="alert alert-warning" role="alert"><i class="fa fa-warning"></i> <b>Important: </b>'
| warning         | '<div class="alert alert-danger" role="alert"><i class="fa fa-exclamation-circle"></i> <b>Warning: </b>'end: '</div>'
| callout_danger  | '<div class="bs-callout bs-callout-danger">'
| callout_default | '<div class="bs-callout bs-callout-default">'
| callout_primary | '<div class="bs-callout bs-callout-primary">'
| callout_success | '<div class="bs-callout bs-callout-success">'
| callout_info    | '<div class="bs-callout bs-callout-info">'
| callout_warning | '<div class="bs-callout bs-callout-warning">'
| hr_faded        | '<hr class="faded"/>'
| hr_shaded       | '<hr class="shaded"/>'


