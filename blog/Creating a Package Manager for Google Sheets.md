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

There have been some attempts at building libraries and indices for Google Sheets. For example, the [Custom Function Library](https://customfunctionlibrary.com/) has compiled a number of custom functions (19 as of this writing). Others have been largely personal endeavors, such as [[Shay Capehart]]'s [Named Functions](https://docs.google.com/spreadsheets/d/1Q0ZrBIuND41MlzdXGa_TYpXItVkfPDihqCKvJfivArc/edit?gid=1804628114#gid=1804628114) or [[aHorseSplashes]]'s [Named Functions and Tools](https://docs.google.com/spreadsheets/d/12H3HHwHxNPAzDzB7RdxOO4NAVs5wvHYnRauLZLiJG9o/edit?gid=1401109056#gid=1401109056). These are wonderful resources, of course; but there are also a number of issues with them that we have to address.

### Why named functions suck

Taken at face value, named functions seem pretty handy. [[Ben L. Collins]] certainly thought so, [writing in a blog post](https://www.benlcollins.com/spreadsheets/named-functions/):

> Named Functions in Google Sheets let you save and name your own custom formulas and then re-use them in other Google Sheet files.
>
> Wow! How exciting is that?!? (Hint: _VERY_)

And that's not wrong. But currently, they are quite difficult to manage. One of the big motivations for this project, in fact, comes from a [Reddit thread on r/googlesheets](https://www.reddit.com/r/googlesheets/comments/1lcs510/what_are_some_named_functions_youve_created_that/). A very respected community member, [[mommasaid]], commented the following:

> The big issue with named functions is the inability to share / update them in any structured way.
>
> They are also a PITA to edit/update if they are complex, which is often the reason for putting them in a named function in the first place.
>
> If we could create a library sheet of version-numbered functions that other sheets could automatically import or something that could be a game changer.
>
> Or... if Google would actively release new built-in functions from a laundry list of those that would make life much easier... even better. Especially baffling to me is not at _least_ having all the Excel capability, e.g. some array-manipulation formulas are missing.)

On top of their difficulty to update and maintain, simply importing, removing, and sharing functions can be quite difficult. Consider the aforementioned libraries. If you're interested in using a function from those libraries, you have to either import the entire library or spend time looking for only the functions relevant to you.

In other words—there is a need for a named function manager. That is where [[spi]] comes in.