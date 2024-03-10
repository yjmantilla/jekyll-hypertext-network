---
title: README
---

# README

This is a base repository to make my flavor of a knowledge base system using Jekyll. The main feature is a custom management of references and custom graph generation.

Use gen_static_data.py to generate the static data for the site. This script will generate the data for the nodes and the graphs.
You need Jekyll to run the site.

Assumptions:

- each .md has a unique name (even if it is in different directories).
- stub.md is the default file for a non-existing note.
- No notes are beyond the first level of sub-directories. ./subdir/note.md is the deepest you can go.
- Each note has its front matter with the title at least.
- Each note has a unique title (not sure what happens if not...)
- You may need to configure foam (e.g. path of images copied to assets) and the site (e.g. theme, etc).
- Currently, it is better to download this as a zip and unzip to the root of your project. Then you can delete the .git folder and start your own repository. As GitHub does not allow to fork a repository into the same account.

Preview: https://yjmantilla.github.io/jekyll-notetaking/
