# AI Chat con TTS

Interfaccia web per chattare con un'AI compatibile OpenAI/OpenRouter, con supporto Text-to-Speech (TTS) via browser o API OpenAI.

---

## Funzionalità

- Chat AI con modelli OpenAI/OpenRouter
- Text-to-Speech:
  - Browser (Web Speech API)
  - OpenAI TTS API (tts-1, tts-1-hd)
- Configurazione API key e URL per chat e TTS
- Esportazione/importazione impostazioni (file JSON)
- Personalizzazione lingua, voce, velocità, pitch, volume
- Salvataggio configurazioni in localStorage
- Scelta percorso file export (Chrome/Edge)

---

## Setup

1. Installa dipendenze:

```bash
npm install
```

2. Avvia in sviluppo:

```bash
npm run dev
```

---

## Configurazione

- Alla prima apertura, inserisci:
  - API Key e URL per chat (es. OpenRouter)
  - API Key e URL per TTS OpenAI (opzionale)
- Puoi modificare le impostazioni in qualsiasi momento cliccando **Settings**
- Puoi esportare/importare le configurazioni da file JSON

---

## Sicurezza

- **Nessuna API key è hardcoded nel codice**
- Le API key sono salvate solo in localStorage del browser
- Ricorda: non condividere file di configurazione con API key sensibili
- Per maggiore sicurezza, usa API key con permessi limitati

---

## Compatibilità

- File System Access API (scelta percorso export) supportata su Chrome, Edge, Opera
- Su Firefox/Safari, export avvia download automatico

---

## Note

- Per usare OpenAI TTS serve una API key OpenAI con accesso a `/v1/audio/speech`
- Per chat puoi usare OpenRouter o OpenAI compatibili
- Il progetto è client-side, nessun backend

---

## Licenza

MIT
