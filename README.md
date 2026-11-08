# Creator-OS — documentazione legale

Questa repository contiene le **pagine HTML rivolte agli utenti** del
progetto Creator-OS. La documentazione tecnica e le prove di prodotto
sono mantenute altrove: [creator-os](https://github.com/simopedra13/creator-os),
[Board](https://github.com/simopedra13/creator-os-board) e
[Wiki](https://github.com/simopedra13/creator-os-wiki).

| File | Documento | Data riportata nel documento |
|---|---|---|
| [index.html](index.html) | Informativa privacy | 15 ottobre 2026 |
| [condizioni.html](condizioni.html) | Condizioni d'uso | 15 ottobre 2026 |
| [cancellazione.html](cancellazione.html) | Istruzioni cancellazione dati | 28 settembre 2026 |

**Aggiornamento inventario: 8 novembre 2026.** Questa nota non modifica
nessuna dichiarazione legale, la relativa data, né le pagine pubblicate.

## Evento tecnico del 2026-11-08: non è una modifica delle condizioni

La [PR #13](https://github.com/simopedra13/creator-os/pull/13)
è stata integrata nel solo repository applicativo, commit `32466cd`.
Corregge il conteggio delle pagine dei caroselli e valida/annulla
patch editoriali malformate. **281 test Python offline verdi prima del merge**.
Non è stato eseguito un deploy su `demo.spaziokura.com` nell'attività
documentata; non è stata attestata una variazione del trattamento dei dati.

Le prove Anthropic Writer/Editor nella
[PR #12](https://github.com/simopedra13/creator-os/pull/12) sono su
**fixture interamente sintetiche**, isolate e non integrate in `main`.
Non implicano che i dati degli utenti siano stati inviati ad Anthropic,
né autorizzano a modificare informativa o condizioni senza verificare
i flussi effettivi. Il confronto Qwen non è una misura controllata.

## Verifiche necessarie prima di aggiornare l'informativa

Il testo vigente può contenere affermazioni materiali relative a
localizzazione, destinatari, trasferimenti, retention e diritti degli
interessati. **Non aggiornarle basandosi su ipotesi di architettura.**

- Identificare **nel runtime effettivo** quali dati personali entrano
  nei prompt dei provider LLM, quali provider sono usati, chi sono i
  destinatari/responsabili e se vi sono trasferimenti.
- Verificare flussi OAuth, analytics, logging, backup/offsite,
  email e cancellazione dei dati, insieme agli accordi e alle
  configurazioni effettivamente attive.
- Confrontare tali fatti con le affermazioni delle tre pagine HTML;
  distinguere un bugfix interno da una nuova finalità di trattamento.
- Richiedere revisione privacy/legale competente delle affermazioni,
  dei riferimenti e delle procedure prima di aggiornare le pagine
  per gli utenti. Aggiornare **anche la data visibile** al momento
  dell'effettiva modifica dei documenti.
- Validare eventuali modifiche HTML, link, contatti e percorso
  pubblico; non confondere commit su GitHub e deploy della pagina.

**Nessuna di queste verifiche è stata completata in questa ricognizione.**
È intenzionale lasciare invariati `index.html`,
`condizioni.html` e `cancellazione.html` finché non si disponga
delle evidenze operative e della revisione richiesta.

Stato tecnico e altri repository:
[STATO_ECOSISTEMA_2026-11-08](https://github.com/simopedra13/creator-os/blob/main/docs/STATO_ECOSISTEMA_2026-11-08.md).
