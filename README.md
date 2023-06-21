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

## Update KiCad Symbols or Footprints

### Symbols
```bash
git subtree pull --prefix symbols kicad-symbols master --squash
```

### Footprints
```bash
git subtree pull --prefix footprints kicad-footprints master --squash
```

## Misc

Diode footprints have two formats:  
1. EIAJ
2. JEDEC

KYOCERA-AVX offers a nice comparison of the two formats:  
https://datasheets.kyocera-avx.com/schottky.pdf


| EIAJ | JEDEC          |
|------|----------------|
| 0603 | SOD-523        |
| 0805 | SOD-323        |
| 1206 | SOD-123        |
| 2010 | SMA (D0-214AC) |
| 2114 | SMB (D0-214AA) |
| 3220 | SMC (D0-214AB) |
