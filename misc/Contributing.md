If you are interested in contributing to sheets.wiki, you'll have to understand the basics of [Git](https://en.wikipedia.org/wiki/Git) , making [pull requests](https://github.blog/developer-skills/github/beginners-guide-to-github-creating-a-pull-request/), and [Obsidian](https://obsidian.md/). You can also suggest edits in the [[Spreadsheets Discord Community]].

If you are unfamiliar with making pull requests, W3 Schools has an [excellent tutorial](https://www.w3schools.com/git/git_remote_fork.asp?remote=github).
If you are unfamiliar with Obsidian, please refer to [their documentation](https://help.obsidian.md/install).
If you need assistance with this, you can ask in the SDC.

Edits and new articles should be in accordance with the [[Style Guide]].

### Quickstart

1. Fork [the sheets.wiki articles repository](https://github.com/Astral1119/quartz-sheets-wiki) and clone it to your machine.
2. [Create an Obsidian vault](https://help.obsidian.md/manage-vaults#Create+vault+from+an+existing+folder) from your forked repository.
3. Make whatever edits you'd like. Make sure to `git pull` relatively often.
4. Push to your fork and make a pull request. A maintainer will review and potentially merge it.

### Recommended plugins

Obsidian supports a number of community plugins that greatly enhance the editing experience. The only plugin I would really recommend adding is [Shiki Highlighter](https://github.com/mProjectsCode/obsidian-shiki-plugin), configured to support `gse`.

### FAQ

#### Why Obsidian/Quartz instead of an actual wiki framework?

Ordinary wikis require a server to handle editing, and sheets.wiki doesn't really need that since it's so lightweight. It's what we call a *static site*—its server just sends static pages, and doesn't receive information other than requests for said pages.

#### Why can't I edit the wiki on the website?

sheets.wiki used to support this kind of editing through [Decap CMS](https://decapcms.org), a system which essentially used my Github account to push edits via Github. While this worked, the experience was deeply unsatisfying compared to Obsidian. While this complicates some things—having to make pull requests, for instance—I think it ultimately leads to a superior editor experience.

#### Will sheets.wiki ever change frameworks?

Probably, but not for a while.