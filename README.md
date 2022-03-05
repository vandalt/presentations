# Presentations

Public presentations with [reveal.js](https://revealjs.com/).

## Workflow

Each directory is a talk. To avoid copying the reveal.js repository each time, I
forked it and I'm using a branch for each presentation. Each branch is added as
a submodule here to make it accessible at https://vandalt.github.io/presentations/_SOME-PRESENTATION_.

To add a new presentation:

1. Clone fork of reveal.js as submodule: `git submodule add git@github.com:vandalt/reveal.js.git SOME-PRESENTATION`
2. Enter new submodule (which will track main reveal.js branch): `cd SOME-PRESENTATION`
3. Create branch with talk name: `git checkout -b SOME-PRESENTATION`
4. Go back to main repo: `cd ..`
5. Make submodule track new branch: `git submodule set-branch -b SOME-PRESENTATION SOME-PRESENTATION`
6. Go back in talk dir: `cd SOME-PRESENTATION`
7. Install: `npm install`
8. Present: `npm start`

When cloning the repostory and entering a submodule for the first time, still
need to checkout the branch. The `set-branch` part just makes sure the
submodules are tracking the branch by default.
