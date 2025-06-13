---
version: 0.1.0
maintainer: Astral Café
last-updated: 2025-06-12
title: CORE
tags:
  - CORE-lib
---

The [CORE library](https://docs.google.com/spreadsheets/d/13UCmWS5fzYTqxzRI5iEaJnc9ad9poMm6ZyxX9HlYbGE) provides implementations for functional data structures and a suite of helper functions for mid-level manipulation.

Currently, the only data structure implemented is [[CHVEC]].

### General principles

Containers in the CORE library all have an abstracted interface. They can be interacted with via payloads.



Values are interpreted on a container-to-container basis. For instance, `CHVEC` interprets numbers as indices and strings as objects to `push` by default.

### General-purpose functions

#### THROW

`THROW` creates a `#REF!` error with a custom error message.

#### HASH and HASH_EQ

`HASH` creates an eight-byte hash of any value or container. `HASH_EQ` is a version of [[EQ]] that evaluates equality based on `HASH` outputs.

