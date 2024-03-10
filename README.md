---
title: README
---

# README

This is a base repository to make my flavor of a hypertext graph knowledge base system using Jekyll. The main feature is a custom management of references and custom graph generation.

Use gen_static_data.py to generate the static data for the site. This script will generate the data for the nodes and the graphs.
You need Jekyll to run the site.

You can create references to other notes using the ``(())`` where the parentheses are actually square brackets. The text inside the brackets is the filename of the note. If the note doesnt exist, it will be redirected to the stub.md file.

Each new directory containing notes is a new "category", and should have a directory-name.md file in the dirs folder. The collect-stuff function in gen_static_data.py will generate the list of notes, so you can use it to generate the list of categories in that script.

Assumptions:

- each .md has a unique filename (even beyond different directories, /nodes/a.md and /a.md cannot happen).
- stub.md is the default file for a non-existing note.
- No notes are beyond the first level of sub-directories. ./subdir/note.md is the deepest you can go.
- Each note has its front matter with the title at least.
- No double square brackets in the text unless it is a reference.
- Each note has a unique title (not sure what happens if not...)
- Using [foam](https://github.com/foambubble/foam) is recommended but you may need to configure it (e.g. path of images copied to assets).
- Currently, it is better to download this as a zip and unzip to the root of your project. Then you can delete the .git folder and start your own repository. As GitHub does not allow to fork a repository into the same account. Or use this repo as template.

Preview: https://yjmantilla.github.io/jekyll-hypertext-network/
