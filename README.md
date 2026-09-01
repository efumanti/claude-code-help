# Manuale Claude Code

Un manuale di riferimento rapido per **[Claude Code](https://code.claude.com/docs/en/overview)**, in italiano: i comandi più utili organizzati per funzionalità, con ricerca istantanea e copia con un clic.

## 🔗 Consultalo online

**https://efumanti.github.io/claude-code-help/**

La pagina è pubblicata tramite GitHub Pages e si aggiorna automaticamente a ogni push su `main`.

## Cosa contiene

302 voci raggruppate in dodici categorie navigabili a schede:

- **Avvio & sessione** — installare e lanciare Claude Code, riprendere sessioni, shortcut da tastiera
- **Contesto & memoria** — finestra di contesto, `CLAUDE.md`, `.claude/rules/` e memoria automatica
- **Sessioni & cronologia** — scorrere e cercare nella conversazione, transcript mode, nominare, ramificare, esportare e riavvolgere
- **Modello, effort & costi** — scelta del modello, livelli di effort, fast mode e consumi
- **Permessi & sicurezza** — modalità di permesso (inclusa auto mode), regole sui tool, sandbox
- **Agenti & parallelismo** — subagent, sessioni in background, workflow dinamici, messaggi tra sessioni
- **Automazione & scripting** — pipeline CI/CD, output strutturato, worktree isolati
- **Cloud, web & mobile** — Remote Control, sessioni cloud, routine programmate, canali, Chrome
- **Qualità & review** — code review, verifica sull'app reale, diagnostica
- **Artifacts & design** — pagine vive su claude.ai, `/design`, visualizzazioni
- **Skills, plugin & MCP** — estendere Claude Code e collegarlo ai sistemi esterni
- **Config & personalizzazione** — settings, hook, aspetto, renderer del terminale e variabili d'ambiente

Funzionalità della pagina:

- 🔍 **Ricerca** su comandi e descrizioni in tempo reale, con evidenziazione del termine cercato
- ✨ **Filtro "Solo novità"** — mostra le 54 voci introdotte o cambiate da fine giugno 2026 in poi
- 📋 **Copia con un clic** — basta cliccare un comando per copiarlo negli appunti
- 🌗 **Tema chiaro/scuro** automatico in base alle preferenze di sistema

## Struttura del progetto

```
.
├── index.html   # il manuale completo (pagina autonoma, HTML + CSS + JS)
└── README.md
```

È una singola pagina statica autosufficiente: nessuna build, nessuna dipendenza da installare. Per consultarla in locale basta aprire `index.html` nel browser.

## Contribuire

I comandi sono definiti nell'array `categories` all'interno di `index.html`. Ogni voce ha la forma:

```js
{ cmd: "/comando", desc: "Che cosa fa.", n: 1 }
```

Il campo `n: 1` è opzionale e marca la voce come novità: le assegna il badge arancione e la fa comparire nel filtro **Solo novità**. Va usato per ciò che la documentazione ufficiale segnala come introdotto o cambiato dopo l'ultima revisione della pagina.

Per aggiungere o correggere una voce è sufficiente modificare quell'array e fare push: GitHub Pages ricompila il sito automaticamente.

---

> Aggiornato a settembre 2026 · Claude Code v2.1.248
