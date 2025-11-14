> [!INFO]
> sheets.wiki is—as its name implies—a wiki, and thus follows similar principles. However, note that this style guide **does not** apply to blog posts.

Generally, this wiki follows Wikipedia's [Manual of Style](https://en.wikipedia.org/wiki/Wikipedia:Manual_of_Style). However, there are a number of differences, outlined below.

### General principles

Wikipedia does not allow [original research](https://en.wikipedia.org/wiki/Wikipedia:No_original_research). sheets.wiki does, provided it has been vetted by a maintainer. This includes original spreadsheets, provided you commit to not deleting them without informing a maintainer. The standard for verification is to either open a pull request containing all relevant information or to raise the matter through the [[Spreadsheets Discord Community]].

Wikipedia has a number of rules around [external linking](https://en.wikipedia.org/wiki/Wikipedia:External_links). sheets.wiki does not, and external linking to reputable sources is encouraged, including in the main text. However, please prioritize references to internal pages (e.g. sheets.wiki pages).

sheets.wiki is not a guidebook. For instructions and advice on how to use functions and techniques, instead write blog posts (which will then be accessible through the function or technique's backlinks). You may link to guides, both external and within the sheets.wiki blog, under a section labeled `Guides`.

Don't be afraid to create dead links. We can always fill them in later.

Articles should generally have at least one wikilink and at least one tag. This makes navigation much easier.

### References and citations

Unlike Wikipedia, which uses [`<ref>` tags](https://en.wikipedia.org/wiki/Wikipedia:Citing_sources), sheets.wiki prefers [Markdown links](https://www.markdownguide.org/basic-syntax/#links).

### Formatting

#### Functions and formulae

Functions, when possible, should be written capitalized and as [inline code](https://help.obsidian.md/syntax#Inline+code) (e.g. `LAMBDA`). Formulae should use [code blocks](https://help.obsidian.md/syntax#Code+blocks) with the `gse` language code.

All formulae should be written using North American syntax (i.e., comma-separated arguments and North American array literals). Similarly, wiki entries should use North American spellings.

Both "formulae" and "formulas" are accepted plural forms of "formula".

#### Errors

Error literals like `#VALUE!` should always be formatted as either inline code or code blocks to prevent them from being interpreted as tags.

#### Headers

The largest header size you should use is `h3` (e.g. ###). Headers should have empty lines before and after in order to separate it from content.

Similarly to Wikipedia, headers should generally not be in title case. However, for consistency with the official documentation, exceptions are made for "Sample Usage" and "See Also".

#### Article names

Article names should generally not be in title case. They should also be in singular form. This does not apply to blog posts, meta articles, or other original content like this page.

#### Sections

Here is a list of common sections and what they should contain, in order. This table is based off of the official documentation.

| Name         | Description                                                                         |
| ------------ | ----------------------------------------------------------------------------------- |
| Sample Usage | An example of how a function or technique should be used.                           |
| Syntax       | The exact and full syntax of a function or technique. See below.                    |
| See Also     | Annotated links to related functions and techniques.                                |
| Examples     | Should be followed by lists of examples, and/or an `iframe` to a sheet of examples. |
| Notes        | Any additional information. See below.                                              |

##### Syntax

The syntax section should have a code block with the function or formula, followed by a list of each argument and brief descriptions for each. Optional arguments should be denoted using brackets (e.g. `[optional]`) and repeated arguments should be denoted using an ellipsis.

##### Notes

Notes should contain a list of helpful tidbits that do not warrant a dedicated section and can vary in style and tone.

### Other

If you modify one of the #generated articles, **make sure to replace the generated tag with #modified**. If you do not, your edits may be overwritten.