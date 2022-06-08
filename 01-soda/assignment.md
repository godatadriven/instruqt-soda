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
  port: 8080
- title: Database
  type: service
  hostname: database
  port: 5432
difficulty: basic
timelimit: 3600
---

Soda SQL is a command line too that is already
[installed](https://docs.soda.io/soda-sql/installation.html#install) in this
environment. Let's open a terminal to start using Soda:

# 0. Open terminal

Use the mouse, click `Three stacked dashes in the top left > Terminal > New Terminal`

Or,

Use a hot key, type `CTRL + SHIFT + BACKTICK`

# 1. Configure Soda

First we [configure](https://docs.soda.io/soda-sql/configure.html) Soda

```
soda create postgres -d database -d postgres -u postgres -p secret
```

This creates a `warehouse.yml`. Open it in the text editor to see what is
inside and change `host: localhost` with `host: database`.

