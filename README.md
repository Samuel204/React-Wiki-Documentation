# ⚛ React Learning Wiki

**React Learning Wiki** è una web app personale progettata per rendere lo studio di React più interattivo e pratico.

L'idea nasce dalla necessità di avere in un unico ambiente sia la **documentazione teorica** sia uno spazio in cui poter sperimentare immediatamente ciò che si sta imparando.

## 🎯 Concept

La web app funziona come una **personal wiki per l'apprendimento di React**.

Gli argomenti vengono organizzati attraverso file **Markdown (`.md`)**, che rappresentano la parte teorica della knowledge base.

Ogni argomento può essere letto e approfondito direttamente nell'interfaccia, mentre un **unico React Playground globale** permette di mettere in pratica i concetti studiati senza dover cambiare ambiente.

Il flusso principale dell'app è:

**Read → Understand → Practice → Run → Experiment**

## 🖥️ Struttura

L'interfaccia è organizzata in tre aree principali:

* **Sidebar** — navigazione tra categorie e argomenti
* **Documentation** — visualizzazione e rendering dei file Markdown
* **Playground** — editor React interattivo con esecuzione e preview

## 🔐 Modalità Viewer / Admin

L'app supporta due modalità operative, selezionabili tramite il badge nella topbar:

* **Viewer** *(default)* — modalità di sola lettura per chi accede al link pubblico. I contenuti vengono caricati automaticamente dal Gist senza richiedere credenziali. Non sono visibili i controlli di modifica.
* **Admin** — modalità di editing completa. Si attiva cliccando sul badge "Viewer" e inserendo il GitHub Token nelle impostazioni. Consente di creare, modificare ed eliminare categorie e file, caricare nuovi `.md` ed esportare i contenuti.

Per uscire dalla modalità Admin è sufficiente cliccare sul badge "Admin" nella topbar.

## React Playground

Il Playground è **unico e globale**, non viene creato un Playground diverso per ogni documento.

L'ambiente React è già configurato con i principali Hook:

`useState`, `useEffect`, `useRef`, `useMemo`, `useCallback`, `useContext`

L'utente può:
- modificare il codice nell'editor
- eseguirlo tramite **Run**
- visualizzare il risultato nella **Preview**
- aprire la **Console** per i log
- usare **Reset** per tornare al codice di default
- caricare esempi direttamente dai code block della documentazione tramite il bottone **▶ Prova nel Playground**

Il codice del Playground viene salvato localmente (`localStorage`) per non perdere il lavoro durante la navigazione o il refresh.

## Markdown

Gli argomenti della Wiki vengono caricati tramite file `.md`.

Il sistema permette di:

* caricare nuovi argomenti (singoli o multipli)
* organizzare i topic per categoria
* visualizzare il Markdown formattato con syntax highlighting
* effettuare ricerche tra gli argomenti
* modificare o eliminare topic e categorie
* esportare il file corrente o tutti i file come `.zip`

I code block con linguaggio `js`, `jsx` o `javascript` mostrano automaticamente il bottone **▶ Prova nel Playground**.

## ☁️ Persistenza

I contenuti della Wiki vengono salvati tramite **[GitHub Gist](https://gist.github.com/)**, utilizzato come storage remoto.

* In modalità **Viewer** i dati vengono letti pubblicamente dal Gist senza token.
* In modalità **Admin** le modifiche vengono sincronizzate automaticamente sul Gist tramite un token GitHub con scope `gist`.

Il Playground rappresenta uno spazio di lavoro personale e viene gestito **localmente** tramite `localStorage`, indipendentemente dalla sincronizzazione remota.

## 🛠️ Tecnologie

* HTML
* CSS
* JavaScript Vanilla
* React 18 — esclusivamente per il Playground (via CDN)
* Babel Standalone — transpiling JSX nel browser
* Marked — rendering Markdown
* Highlight.js — syntax highlighting
* CodeMirror 5 — editor del Playground
* JSZip — export ZIP
* GitHub Gist API — storage remoto
* LocalStorage — persistenza locale del Playground

L'obiettivo è mantenere l'app **leggera, semplice e senza framework**, evitando dipendenze non necessarie.

## UI / UX

Il design è ispirato alle moderne piattaforme di documentazione e agli ambienti di sviluppo.

La UI privilegia:

* minimalismo e leggibilità
* navigazione rapida tra argomenti
* codice facilmente consultabile ed eseguibile
* separazione visiva tra teoria (pannello chiaro) e pratica (pannello scuro)
* responsive design con navigazione bottom bar su mobile
* resizer drag-and-drop tra documentazione e Playground su desktop
* utilizzo in modalità embedded (es. Notion)

## Obiettivo

React Learning Wiki non vuole essere una semplice raccolta di appunti.

L'obiettivo è creare un piccolo **ambiente personale di apprendimento**, in cui la documentazione diventa il punto di partenza per sperimentare direttamente con il codice.

> **La documentazione spiega. Il Playground permette di capire davvero.**

---

🔗 **Link webapp:** [https://samuel204.github.io/React-Wiki-Documentation/](https://samuel204.github.io/React-Wiki-Documentation/)