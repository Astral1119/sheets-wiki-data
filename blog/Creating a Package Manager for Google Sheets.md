---
author: Astral Café
---

> [!WARNING]
> All opinions in this blog post are the author's own. This blog post is anecdote-driven, except where otherwise noted.

Starting on [August 24th, 2022](https://support.google.com/docs/thread/177089883/google-sheets-new-features-named-functions-powerful-functions-bundle), Google started rolling out [[named functions]] in the same update as [[LAMBDA]] and [[XLOOKUP]]. Both `LAMBDA` and `XLOOKUP` have become standard in modern spreadsheet usage; yet, in my experience, named functions have encountered far less adoption.

From where I stand, I see a few reasons why this might be the case. But first, a quick review. (If you're already familiar with named functions, feel free to skip to the next section.)

### What are named functions?

Put simply, named functions allow users to create their own functions and use them from anywhere in the sheet. Pedantically, it assigns names to `LAMBDA` functions and elevates them to a global [scope](https://en.wikipedia.org/wiki/Scope_(computer_science)).

In the backend, named functions are just `LAMBDA`s. You can confirm this by exporting a Google Sheet as an `.xslx` file and reading the metadata.

### What is a package manager?

Per [Wikipedia](https://en.wikipedia.org/wiki/Package_manager),

> A **package manager** or **package management system** is a collection of [software tools](https://en.wikipedia.org/wiki/Programming_tool) that automates the process of installing, upgrading, configuring, and removing [computer programs](https://en.wikipedia.org/wiki/Computer_program) for a [computer](https://en.wikipedia.org/wiki/Computer) in a consistent manner.

In Google Sheets, this means helping manage named function libraries.

### Why named functions suck

Taken at face value, named functions seem pretty handy. [[Ben L. Collins]] certainly thought so, [writing in a blog post](https://www.benlcollins.com/spreadsheets/named-functions/):

> Named Functions in Google Sheets let you save and name your own custom formulas and then re-use them in other Google Sheet files.
>
> Wow! How exciting is that?!? (Hint: _VERY_)

And that's not wrong, necessarily. But there's a couple of major issues that we should probably address.

There have been some attempts at building libraries and indices for Google Sheets, but none of them have caught on. For instance, the [Custom Function Li]