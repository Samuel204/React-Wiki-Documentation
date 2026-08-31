# ⚛ React Learning Wiki

**React Learning Wiki** è una web app personale progettata per rendere lo studio di più interattivo e pratico.

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

Sono previste due modalità:

* **Read** — esperienza focalizzata sulla lettura della documentazione
* **Practice** — documentazione e Playground affiancati per favorire l'apprendimento attivo

## 🧪 React Playground

Il Playground è **unico e globale**, non viene creato un Playground diverso per ogni documento.

L'ambiente React è già configurato con i principali Hook, come:

`useState`, `useEffect`, `useRef`, `useMemo`, `useCallback`, `useContext`.

L'utente può modificare il codice, eseguirlo tramite **Run**, visualizzare il risultato nella **Preview** e utilizzare **Reset** per tornare al codice iniziale.

Il codice del Playground viene mantenuto localmente per evitare di perdere il lavoro durante la navigazione o il refresh della pagina.

## 📚 Markdown

Gli argomenti della Wiki vengono caricati tramite file `.md`.

Il sistema permette di:

* caricare nuovi argomenti
* organizzare i topic per categoria
* visualizzare il Markdown formattato
* effettuare ricerche tra gli argomenti
* modificare o eliminare i topic

## ☁️ Persistenza

I contenuti della Wiki vengono salvati tramite **jsonStorage.net**, utilizzato come storage remoto.

Il Playground, invece, rappresenta uno spazio di lavoro personale e viene gestito localmente tramite `localStorage`.

In questo modo la documentazione e l'ambiente di pratica rimangono logicamente separati.

## 🛠️ Tecnologie

* HTML
* CSS
* JavaScript Vanilla
* React — esclusivamente per il Playground
* Markdown
* jsonstorage.net
* LocalStorage

L'obiettivo è mantenere la dashboard **leggera, semplice e senza framework**, evitando funzionalità non necessarie.

## 📐 UI / UX

Il design è ispirato alle moderne piattaforme di documentazione e agli ambienti di sviluppo.

La UI privilegia:

* minimalismo
* leggibilità
* navigazione rapida
* codice facilmente consultabile
* separazione tra teoria e pratica
* responsive design
* utilizzo in modalità embedded

L'app è progettata per essere pubblicata online e utilizzata come **Embed all'interno di Notion**.

## 🚀 Obiettivo

React Learning Wiki non vuole essere una semplice raccolta di appunti.

L'obiettivo è creare un piccolo **ambiente personale di apprendimento**, in cui la documentazione diventa il punto di partenza per sperimentare direttamente con il codice.

> **La documentazione spiega. Il Playground permette di capire davvero.**

link webapp: https://samuel204.github.io/React-Wiki-Documentation/
