# Manuale Claude Code

Un manuale di riferimento rapido per **[Claude Code](https://code.claude.com/docs/en/overview)**, in italiano: i comandi più utili organizzati per funzionalità, con ricerca istantanea e copia con un clic.

## 🔗 Consultalo online

**https://efumanti.github.io/claude-code-help/**

La pagina è pubblicata tramite GitHub Pages e si aggiorna automaticamente a ogni push su `main`.

## Cosa contiene

I comandi sono raggruppati in categorie navigabili a schede:

- **Avvio & sessione** — lanciare Claude Code, riprendere sessioni, shortcut da tastiera
- **Contesto & memoria** — gestione della finestra di contesto e del file `CLAUDE.md`
- **Navigazione sessioni** — rinominare, ramificare ed esportare le sessioni
- **Modello & costi** — scegliere il modello e monitorare i consumi
- **Permessi & sicurezza** — controllo dei tool, modalità di esecuzione, rollback
- **Automazione & scripting** — uso in pipeline CI/CD e flussi non interattivi
- **Qualità & review** — revisione del codice, refactoring e debug
- **Config & personalizzazione** — settings, hooks, comandi slash custom e variabili d'ambiente

Funzionalità della pagina:

- 🔍 **Ricerca** su comandi e descrizioni in tempo reale
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

I comandi sono definiti nell'array `categories` all'interno di `index.html`. Per aggiungere o correggere una voce è sufficiente modificare quell'array e fare push: GitHub Pages ricompila il sito automaticamente.

---

> Aggiornato a giugno 2026 · Claude Code v2.1
