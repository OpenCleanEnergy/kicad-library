# kicad-library

This repository uses `git subtree` to manage the KiCad libraries.  
[W3docs - Git Subtree](https://www.w3docs.com/learn-git/git-subtree.html)

## Add KiCad Symbols

1. Add remote
```bash
git remote add -f kicad-symbols https://gitlab.com/kicad/libraries/kicad-symbols.git
```

2. Add the subtree
```bash
git subtree add --prefix symbols kicad-symbols master --squash
```

## Add KiCad Footprints

1. Add remote
```bash
git remote add -f kicad-footprints https://gitlab.com/kicad/libraries/kicad-footprints.git
```

2. Add the subtree
```bash
git subtree add --prefix footprints kicad-footprints master --squash
```
