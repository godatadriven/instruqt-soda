---
slug: soda
id: m0abucpvvb6y
type: challenge
title: Soda
teaser: The Soda workshop.
notes:
- type: text
  contents: The Soda workshop starts shortly.
tabs:
- title: Code editor
  type: service
  hostname: vscode
  path: ?folder=/home/coder/soda
  port: 8080
- title: Database
  type: service
  hostname: database
  port: 5432
difficulty: basic
timelimit: 18000
---

Soda SQL is a command line too that is already
[installed](https://docs.soda.io/soda-sql/installation.html#install) in this
environment. 

Let's open a terminal to start using Soda:

Open terminal
=============

Use the mouse, click `Three stacked dashes in the top left > Terminal > New Terminal`

Or, use a hot key, type `CTRL + SHIFT + BACKTICK`

Configure Soda
==============

First we [configure](https://docs.soda.io/soda-sql/configure.html) Soda

```
soda create postgres -d database -d postgres -u postgres -p secret
```

This command creates the `warehouse.yml`.

Open it in the text editor to see what is inside and change `host: localhost`
with `host: database`.

