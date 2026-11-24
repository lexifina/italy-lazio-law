<!-- lawwatch: written from data/checks by the check trail; edit the records, not this page -->

# Monitoraggio: che cosa si legge e con quale esito

[English](README.en.md)

Come global-law monitora ogni paese: [global-law monitoring/](https://github.com/lexifina/global-law/tree/main/monitoring). Questa pagina fa lo stesso per Lazio soltanto: ogni lettura di una fonte ufficiale, quando è avvenuta e con quale esito (atti aggiunti, modificati e rimossi). La forma leggibile dalle macchine è [data/checks/](../data/checks/) (JSON Lines, schema `lexifina-check/1`), in `git log` come commit `Kind: check`, e mese per mese in [checks/](checks/).

**Ultimo controllo:** 2026-11-24 01:20 UTC, Consiglio regionale del Lazio, Leggi regionali (testo coordinato): 80 indirizzi letti; 0 aggiunti, 0 modificati, 0 rimossi; modifiche trovate; 11 non pubblicati, di cui 0 senza motivo.

## Fonti

| Fonte | Cartelle | Frequenza | Ultimo controllo riuscito | Ultimo esito | Stato |
| --- | --- | --- | --- | --- | --- |
| [Consiglio regionale del Lazio, Leggi regionali (testo coordinato)](https://www.consiglio.regione.lazio.it/?vw=leggiregionali) | `lr/`, `statuto/` | ogni giorno | 2026-11-24 01:20 UTC | modifiche trovate | sorvegliata: solo testo vigente, come il repository è costruito: un testo modificato è una nuova versione datata il giorno della lettura, attribuita al Consiglio come editore; le leggi che la banca dati indica come abrogate per intero sono escluse (una abrogata dopo l'inserimento risulta non più alla fonte) |

## Gli ultimi 30 giorni

| Inizio (UTC) | Fonte | Letti | Aggiunti | Modificati | Rimossi | Non pubblicati (senza motivo) | Esito | Commit |
| --- | --- | ---: | ---: | ---: | ---: | ---: | --- | ---: |
| [2026-11-24 01:15](checks/2026-11.md#it-consiglio-lazio-20261124t011546z) | consiglio-lazio | 80 | 0 | 0 | 0 | 11 (0) | modifiche trovate | [4](https://github.com/lexifina/italy-lazio-law/compare/6f437f7c23d0...ccfc2e3e19bd) |

## Verificalo da te

```
python tools/checktrail.py                      # l'ultimo controllo di ogni fonte
python tools/checktrail.py --day 2026-11-23     # tutti i controlli di un giorno
python tools/checktrail.py --act <id>           # quando un atto è stato visto e pubblicato
git log --grep='^Kind: check' --format='%ci %s'  # i controlli nella cronologia
```

Ha valore legale solo la pubblicazione ufficiale; i testi qui sono copie per la lettura e la ricerca.
