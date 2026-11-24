<!-- lawwatch: written from data/checks by the check trail; edit the records, not this page -->

# Monitoring: what is read and what came of it

[Italiano](README.md)

How global-law monitors every country: [global-law monitoring/](https://github.com/lexifina/global-law/tree/main/monitoring). This page is the same for Lazio only: every time an official source is read, when, and what came of it (acts added, changed and removed). The machine-readable form is [data/checks/](../data/checks/) (JSON Lines, schema `lexifina-check/1`), in `git log` as `Kind: check` commits, and month by month in [checks/](checks/).

**Last check:** 2026-11-24 01:20 UTC, Consiglio regionale del Lazio, Leggi regionali (testo coordinato): 80 addresses read; 0 added, 0 changed, 0 removed; changes found; 11 not published, 0 of them with no reason.

## Sources

| Source | Folders | How often | Last successful check | Last result | State |
| --- | --- | --- | --- | --- | --- |
| [Consiglio regionale del Lazio, Leggi regionali (testo coordinato)](https://www.consiglio.regione.lazio.it/?vw=leggiregionali) | `lr/`, `statuto/` | daily | 2026-11-24 01:20 UTC | changes found | watched: current text only, as the repository is built: a changed text is a new version dated the day it was read, credited to the Consiglio as publisher; laws the database marks as repealed as a whole are left out (one repealed after it was added is listed as no longer at the source) |

## The last 30 days

| Started (UTC) | Source | Read | Added | Changed | Removed | Not published (no reason) | Result | Commits |
| --- | --- | ---: | ---: | ---: | ---: | ---: | --- | ---: |
| [2026-11-24 01:15](checks/2026-11.md#it-consiglio-lazio-20261124t011546z) | consiglio-lazio | 80 | 0 | 0 | 0 | 11 (0) | changes found | [4](https://github.com/lexifina/italy-lazio-law/compare/6f437f7c23d0...ccfc2e3e19bd) |

## Check it yourself

```
python tools/checktrail.py                      # the latest check of every source
python tools/checktrail.py --day 2026-11-23     # every check of a day
python tools/checktrail.py --act <id>           # when an act was seen and published
git log --grep='^Kind: check' --format='%ci %s'  # the checks in the history
```

Only the official publication has legal force; the texts here are copies for reading and searching.
