# ADR-001 — Stack e hosting

> Scheletro da compilare. Le sezioni con `_[da compilare]_` sono lasciate all'architect.
> Le ipotesi marcate **[SIM]** appartengono alla simulazione e valgono finché non vengono cambiate.
> Prezzi, licenze e limiti dei servizi: scrivere "da verificare" se non controllati alla fonte.

## 1. Stato
_[da compilare: Proposta | In revisione | Approvato | Approvato con condizioni | Respinto | Sostituito]_

## 2. Data
_[da compilare]_

## 3. Deciso da
_[da compilare: Architect (decisione tecnica); Board (approvazione di budget e priorità)]_

## 4. Story e requisiti collegati
- US-07 Repository, pipeline, HTTPS
- US-08 Chiavi e proxy (dipende da questa ADR)
- US-63 Architettura iniziale e ADR
- Requisiti non funzionali Must: HTTPS/HSTS, chiavi solo lato server, rate limiting, GDPR e dati minimi, p95 < 3 s, accessibilità WCAG 2.1 AA, browser datati, costi contenuti, monitoraggio e backup con ripristino provato
- Vincoli del PO: costo gratuito o quasi; nessuna chiave nel browser; stack semplice e mantenibile da volontari

## 5. Contesto
_[da compilare: perché serve questa decisione ora, cosa sblocca, cosa succede se si rimanda.]_

### 5.1 Fatti
_[da compilare]_

### 5.2 Ipotesi di simulazione
| # | Ipotesi | Stato |
|---|---|---|
| S1 | 3 sviluppatori volontari, almeno uno con competenza Java, nessuno con esperienza DevOps seria | modificata |
| S2 | Tetto di spesa 25 €/mese, tutto compreso (hosting, dominio, email transazionale) | modificata |
| S3 | Dati in UE | da confermare |
| S4 | Browser minimi: ultime 2 versioni principali più uno di 5–6 anni fa | da confermare |
| S5 | Poche centinaia di utenti, picchi da giugno | da confermare |
| S6 | Dopo il go-live, 1 volontario manutentore | da confermare |

### 5.3 Domande aperte
- Competenze reali degli altri due sviluppatori
- Ore/mese di manutenzione accettabili
- Soglia di allarme sul budget
- Quota di budget riservata a ADR-003 (provider meteo)

## 6. Criteri di decisione
_[da compilare: elenco dei criteri, peso di ciascuno e motivo del peso.]_

| Criterio | Peso | Motivo del peso |
|---|---|---|
| Costo mensile totale (euro) | _[ ]_ | _[ ]_ |
| Costo operativo (ore/mese di volontariato) | _[ ]_ | _[ ]_ |
| Competenze del team / bus factor | _[ ]_ | _[ ]_ |
| Manutenibilità da volontari | _[ ]_ | _[ ]_ |
| Sicurezza (segreti, HTTPS, rate limiting) | _[ ]_ | _[ ]_ |
| Dati in UE / GDPR / backup e ripristino | _[ ]_ | _[ ]_ |
| Prestazioni (p95 < 3 s) e compatibilità con browser datati | _[ ]_ | _[ ]_ |
| Uscita dal fornitore (costo di migrazione) | _[ ]_ | _[ ]_ |
| _[altro]_ | _[ ]_ | _[ ]_ |

## 7. Opzioni considerate
_[da compilare: almeno 2–3 opzioni reali. Duplicare il blocco per ciascuna.]_

### Opzione A — _[nome]_
- **Descrizione:** _[ ]_
- **Pro:** _[ ]_
- **Contro:** _[ ]_
- **Costo mensile stimato:** _[da verificare]_
- **Stima di setup (SP):** _[ ]_

### Opzione B — _[nome]_
- **Descrizione:** _[ ]_
- **Pro:** _[ ]_
- **Contro:** _[ ]_
- **Costo mensile stimato:** _[da verificare]_
- **Stima di setup (SP):** _[ ]_

### Opzione C — _[nome]_
- **Descrizione:** _[ ]_
- **Pro:** _[ ]_
- **Contro:** _[ ]_
- **Costo mensile stimato:** _[da verificare]_
- **Stima di setup (SP):** _[ ]_

## 8. Confronto
_[da compilare: tabella opzioni × criteri con punteggio e totale.]_

## 9. Decisione
_[da compilare: una frase chiara.]_

## 10. Motivi
_[da compilare: perché questa opzione rispetto alle altre, collegando ai criteri e ai pesi.]_

## 11. Conseguenze
_[da compilare: cosa diventa più facile, cosa più difficile, cosa si accetta di perdere. Includere ripartizione stimata del budget da 25 €/mese.]_

## 12. Rischi
| Rischio | Probabilità | Impatto | Mitigazione |
|---|---|---|---|
| _[ ]_ | _[ ]_ | _[ ]_ | _[ ]_ |

## 13. Verifica
_[da compilare: come e quando si controlla che la decisione funzioni (misure, soglie, data di revisione).]_

## 14. Riferimenti
_[da compilare: fonti consultate, con data di consultazione.]_

## 15. Storico
| Data | Stato | Nota |
|---|---|---|
| _[ ]_ | Proposta | Creazione dello scheletro |
