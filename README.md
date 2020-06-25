# Left4Craft Wiki

https://wiki.left4craft.org

## How to edit
Anyone with a GitHub can contribute by forking, editing, and making a pull request. *If you spot a small mistake, you can create an [issue](https://github.com/Left4Craft/wiki/issues) to get someone else to fix it.*

There is an edit button at the top (to the right of the title) on every wiki page. Clicking it will take you to the corrosponding markdown file.
Pages are stored in `/docs`.
The wiki uses [PyMdown](https://facelessuser.github.io/pymdown-extensions/) ([MkDocs-Material extension](https://squidfunk.github.io/mkdocs-material/extensions/pymdown/)) markdown.

> Collaborators (regular editors) or Left4Craft org/team members should not need to create a fork - simplfying the process.

## How to build/deploy
The wiki is a MkDocs-generated static site (hosted on GitHub Pages).
[Install mkdocs-material](https://squidfunk.github.io/mkdocs-material/getting-started/) (includes material theme and mkdocs) and all of the [extensions](https://squidfunk.github.io/mkdocs-material/extensions/admonition/) and [plugins](https://squidfunk.github.io/mkdocs-material/plugins/search/) then run `mkdocs serve` (to check locally) and `mkdocs gh-deploy` to build (`mkdocs build`) and deploy to github, from within the cloned repository directory.
