# README

# Quick start

## create container and enter

Bash shell

```sh
docker run -it -v $(pwd)/data:/data janninematt/pandoc_ubuntu:v0.2 /bin/bash
```

Fish shell

```
docker run -it -v (pwd)/data:/data janninematt/pandoc_ubuntu:v0.2 /bin/bash
```

## generate pdf

```
pandoc --latex-engine=xelatex --toc --smart <source markdown file> -o <output pdf file>
```

# Why not just using entry command

[Pandoc](https://pandoc.org/) have so many feature and extremly powerful.

I intend provide the enviroment and leave rest to user.

# Example

```
---
title: "My Title"
CJKmainfont: 'AR PL UKai TW'
date: \today
geometry: "left=2cm,right=2cm,top=2cm,bottom=2cm"
output: pdf_document
---

# Charpter 1 你好

你好 World
```
