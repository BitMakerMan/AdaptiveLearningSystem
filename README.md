# 🧠 PoliMind Adaptive Learning System (PALS)

> **"Non insegnare a tutti nello stesso modo — impara come *tu* impari."**

[![Status](https://img.shields.io/badge/status-concept%20%2F%20design%20phase-blueviolet)](https://github.com/BitMakerMan/AdaptiveLearningSystem)
[![License](https://img.shields.io/badge/license-CC%20BY--NC--ND%204.0-blue)](https://creativecommons.org/licenses/by-nc-nd/4.0/)
[![Author](https://img.shields.io/badge/author-Craicek%20%40BitMakerMan-orange)](https://github.com/BitMakerMan)
[![Version](https://img.shields.io/badge/version-0.1.0--alpha-green)]()
[![First Published](https://img.shields.io/badge/first%20published-April%202025-lightgrey)]()

---

## Indice

- [Overview](#overview)
- [Il Concetto Core: La Sinusoide della Dopamina](#il-concetto-core-la-sinusoide-della-dopamina)
- [Architettura del Sistema](#architettura-del-sistema)
  - [Core Engine — LLM Locale](#1-core-engine--llm-locale--direttore-dorchestra)
  - [Modulo Attentional DNA](#2-modulo-attentional-dna--profilazione-cognitiva)
  - [World Model 3D — Meta Quest](#3-world-model-3d--integrazione-meta-quest)
  - [Agente Multimodale](#4-agente-multimodale--dopamine-injector)
- [Workflow Operativo](#workflow-operativo)
- [Data Model e Schemi](#data-model-e-schemi)
- [Technology Stack](#technology-stack)
- [Roadmap](#roadmap)
- [Basi di Ricerca](#basi-di-ricerca)
- [Differenziatori Chiave](#differenziatori-chiave)
- [Obiettivi Finali](#obiettivi-finali)
- [Dichiarazione di Paternita Intellettuale](#dichiarazione-di-paternita-intellettuale)
- [Licenza](#licenza)

---

## Overview

**PALS (PoliMind Adaptive Learning System)** e un framework originale di apprendimento guidato da AI, progettato per sostituire i metodi di studio passivi e lineari con una **esperienza di immersione ciclica neurologically-aware**.

L'ipotesi centrale e che l'attenzione umana non operi in modo lineare: segue **pattern di oscillazione biologica** guidati dalla dinamica dei neurotrasmettitori, principalmente i cicli di ricompensa dopaminergici. PALS e costruito per sincronizzare l'esperienza di apprendimento con questi cicli, anziche combatterli.

A differenza delle piattaforme EdTech esistenti (Coursera, Khan Academy, Duolingo) che adattano la difficolta del contenuto, PALS adatta lo **stato di engagement neurologico** del learner in tempo reale, attraverso:

- Un **LLM eseguito localmente** come orchestratore cognitivo (privacy totale, zero cloud).
- **Segnali biometrici/comportamentali** per inferire la fatica mentale senza sensori invasivi.
- Un **ambiente 3D generativo** (VR) come interfaccia primaria di apprendimento.
- Un **sistema multimodale di trigger dopaminergici** per resettare il carico cognitivo nel momento preciso.

Questo progetto e stato concepito e documentato per la prima volta in **Aprile 2025** da **Craicek** nell'ambito dell'iniziativa PoliMind.

**Repository:** [github.com/BitMakerMan/AdaptiveLearningSystem](https://github.com/BitMakerMan/AdaptiveLearningSystem)

---

## Il Concetto Core: La Sinusoide della Dopamina

I sistemi di studio tradizionali falliscono a uno dei due estremi:

| Tipo di Sistema | Problema |
|---|---|
| Lineare (libri, slide, video) | Monotonia => carenza di dopamina => collasso dell'attenzione |
| Social media / gamification | Stimolazione caotica => nessuna codifica profonda => desensibilizzazione |

PALS propone una **curva di attenzione sinusoidale controllata**: un'oscillazione programmata tra carico cognitivo profondo e stimolazione di ricompensa calibrata.

```
Attenzione
   |
   |   /-----\           /-----\           /---
   |  /       \         /       \         /
   | /  CARICO \       /  CARICO \       /
   |/   FASE    \-----/   FASE    \-----/
   |          RICARICA         RICARICA
   +----------------------------------------------> Tempo
                 ^                   ^
           Boost Dopamina      Boost Dopamina
           (pre-burnout)       (pre-burnout)
```

### Definizione delle Fasi

**Fase di Carico — Deep Immersion**

Il learner viene immerso in un ambiente 3D spaziale dove le nuove informazioni vengono codificate attraverso esperienze interattive ed embodied. L'LLM orchestra la delivery dei contenuti in base al profilo Attentional DNA dell'utente.

**Fase di Scarico/Ricarica — Dopamine Boost Calibrato**

Quando i segnali comportamentali indicano il raggiungimento della saturazione cognitiva (rilevato *prima* del burnout), il sistema inietta uno stimolo di ricompensa personalizzato: una traccia musicale, un breve video, un'interazione VR gamificata. Il tipo e la durata dello stimolo derivano dal profilo dell'utente.

**Effetto Neuroplasticita**

Il ciclo ripetuto di carico cognitivo e recupero reward-driven forza il cervello a mantenere la **plasticita sinaptica**, il substrato neurologico dell'apprendimento e della consolidazione della memoria. Nel tempo, questo dovrebbe contrastare la rigidita cognitiva legata all'eta.

---

## Architettura del Sistema

```
+------------------------------------------------------------------+
|                       ARCHITETTURA PALS                          |
+------------------------------------------------------------------+
|                                                                  |
|  +--------------+     +--------------+     +--------------+     |
|  |  USER INPUT  |---->|  CORE ENGINE |---->|  3D WORLD    |     |
|  |  (VR + Bio)  |     |  (Local LLM) |     |  MODEL (VR)  |     |
|  +--------------+     +------+-------+     +--------------+     |
|                               |                                  |
|              +----------------+-----------------+               |
|              v                v                 v               |
|  +--------------+  +--------------+  +----------------+         |
|  | ATTENTIONAL  |  |  MULTIMODAL  |  |   DATABASE     |         |
|  | DNA MODULE   |  |    AGENT     |  | (Profili +     |         |
|  | (Profiler)   |  | (Triggers)   |  |  Pattern)      |         |
|  +--------------+  +--------------+  +----------------+         |
|                                                                  |
+------------------------------------------------------------------+
```

---

### 1. Core Engine — LLM Locale / Direttore d'Orchestra

Il sistema nervoso centrale di PALS. Un **LLM open-source quantizzato** (es. LLaMA 3, Mistral, o Phi-3) gira interamente sull'hardware locale dell'utente — nessun cloud, nessuna esfiltrazione di dati.

**Responsabilita:**

- Orchestrare tutti gli altri moduli tramite API interna strutturata.
- Parsare i segnali comportamentali in tempo reale dalla sessione VR.
- Prendere decisioni di fase ciclica: quando mantenere la Fase di Carico, quando triggerare la Ricarica.
- Generare narrative di contenuto personalizzate adattate alla velocita di comprensione dell'utente.
- Loggare tutti i dati di interazione nel database locale per il raffinamento del profilo.

**Architettura Privacy-First:**

Tutta l'inferenza avviene on-device. Nessun dato comportamentale dell'utente lascia mai la macchina locale. Il sistema e progettato per funzionare completamente in ambienti air-gapped.

**Modelli candidati (local inference):**

```
- Meta LLaMA 3 8B / 70B  (quantized GGUF via llama.cpp)
- Mistral 7B Instruct
- Microsoft Phi-3 Mini    (per dispositivi edge / low-VRAM)
- Google Gemma 2 9B
```

---

### 2. Modulo Attentional DNA — Profilazione Cognitiva

Il modulo di profilazione costruisce un **fingerprint cognitivo unico** per ogni utente attraverso un periodo di calibrazione iniziale.

**Segnali Tracciati (non-invasivi):**

| Segnale | Metodo di Misurazione | Stato Inferito |
|---|---|---|
| Response Latency | Timing interazioni VR | Livello di carico cognitivo |
| Comprehension Velocity | Correttezza Q&A nel tempo | Tasso di assorbimento |
| Error Pattern Distribution | Analisi fallimenti task | Bottleneck concettuali |
| Interaction Frequency Drop | Inattivita click/gaze | Onset del decadimento |
| Re-read / Re-visit Behavior | Log navigazione spaziale | Gap di consolidazione |
| Optimal Session Length | Dati sessione longitudinali | Soglia di fatica personale |

**Output — Il Profilo Attentional DNA:**

```json
{
  "user_id": "uuid-v4",
  "profile_version": "1.0",
  "created_at": "ISO-8601",
  "cognitive_parameters": {
    "avg_peak_focus_duration_min": 23,
    "fatigue_onset_signal": "interaction_frequency_drop_gt_40pct",
    "optimal_recharge_duration_min": 4,
    "preferred_reward_modalities": ["music", "short_video"],
    "comprehension_velocity_wpm_equiv": 280,
    "peak_performance_time_of_day": "09:00-11:30"
  },
  "subject_preferences": {
    "music_genres": ["lo-fi", "classical_instrumental"],
    "video_content_tags": ["nature", "comedy_short", "science_visual"],
    "vr_env_aesthetic": ["minimalist", "nature_forest", "space"]
  },
  "knowledge_graph": {
    "mastered_concepts": [],
    "in_progress_concepts": [],
    "identified_gaps": []
  }
}
```

---

### 3. World Model 3D — Integrazione Meta Quest

L'interfaccia primaria di apprendimento non e uno schermo. E un **mondo virtuale generato proceduralmente** dove la conoscenza e spaziale, embodied e interattiva.

**Pipeline di Generazione del Mondo:**

```
Input: Materia / Materiale di Studio
              |
              v
+-----------------------------+
|  Concept Graph Extraction   |  -->  Nodi = concetti, Archi = relazioni
|  (LLM)                      |
+-----------------------------+
              |
              v
+-----------------------------+
|  3D Environment Generator   |  -->  Concetti mappati in posizioni 3D
+-----------------------------+
              |
              v
+-----------------------------+
|  Quest SDK Layer            |  -->  Renderizzato via Unity / OpenXR
|  (VR Runtime)               |
+-----------------------------+
```

**Esempio — Studio di Biologia Molecolare:**

L'utente "entra" fisicamente in una cellula. Il nucleo e un edificio visitabile. I filamenti di DNA sono oggetti fisici manipolabili. La sintesi proteica e animata come una fabbrica da attraversare. Ogni interazione con un oggetto attiva una spiegazione contestuale dall'LLM orchestratore.

**Stack Tecnico (World Model):**

- **Engine:** Unity 6 con XR Interaction Toolkit
- **Generazione Procedurale:** Pipeline custom LLM-to-3D (concept graph -> scene graph -> asset placement)
- **Rendering:** Ottimizzato Meta Quest 3 (foveated rendering, target 90fps)

---

### 4. Agente Multimodale — Dopamine Injector

Un agente software con accesso autorizzato a sorgenti media locali e in streaming. La sua unica funzione e consegnare lo **stimolo giusto nel momento giusto**, basandosi sulla fase corrente della sinusoide dopaminergica e sul profilo Attentional DNA.

**Logica Decisionale del Trigger:**

```python
def evaluate_trigger(
    session_state: SessionState,
    profile: AttentionalDNA
) -> TriggerEvent | None:
    """
    Valuta i segnali della sessione in tempo reale e determina
    se un trigger di ricarica dopaminergica deve essere attivato.

    Ritorna un TriggerEvent se viene rilevata la soglia pre-burnout,
    None se l'utente e ancora nella fase di carico ottimale.

    Autore originale: Craicek (@BitMakerMan) — Aprile 2025
    Repository: github.com/BitMakerMan/AdaptiveLearningSystem
    """
    fatigue_score = compute_fatigue_score(
        interaction_drop=session_state.interaction_frequency_delta,
        response_latency=session_state.avg_response_latency_ms,
        elapsed_minutes=session_state.elapsed_focus_minutes,
        baseline=profile.cognitive_parameters
    )

    if fatigue_score >= TRIGGER_THRESHOLD:
        modality = select_optimal_modality(profile.subject_preferences)
        duration = profile.cognitive_parameters["optimal_recharge_duration_min"]
        return TriggerEvent(modality=modality, duration_min=duration)

    return None
```

**Modalita di Stimolo Supportate:**

| Modalita | Sorgente | Implementazione |
|---|---|---|
| Musica | Spotify API / Libreria locale | Auto-playlist per genere + profilo BPM |
| Video breve | YouTube API / Archivio locale | Curato da tag definiti dall'utente |
| VR Scene Shift | World engine interno | Swap di scena verso ambiente rilassante |
| Micro-game | Modulo VR interno | Esperienza interattiva casual 2-5 min |
| Social micro-reward | Interno / esterno | Ping leaderboard, achievement unlock |

---

## Workflow Operativo

```
FASE 0 — ONBOARDING & CALIBRAZIONE
+---------------------------------------------------------------+
| L'utente esegue task cognitivi strutturati (ore/giorni)       |
| L'LLM analizza: tempi di risposta, curve di accuratezza,      |
| pattern di decadimento attenzione, segnali di preferenza      |
| Output: Profilo Attentional DNA salvato localmente            |
+---------------------------------------------------------------+
                         |
                         v
FASE 1 — GENERAZIONE WORLD MODEL
+---------------------------------------------------------------+
| L'utente seleziona la materia / carica materiale di studio    |
| L'LLM estrae il concept graph                                 |
| Ambiente 3D generato o caricato dalla libreria                |
| Ambiente calibrato alle preferenze estetiche dell'utente      |
+---------------------------------------------------------------+
                         |
                         v
FASE 2 — LEARNING LOOP CICLICO  <-------------------------------+
+---------------------------------------------------------------+ |
|                                                               | |
|  +----------------------------------------------------------+ | |
|  | FASE DI CARICO                                           | | |
|  |  - L'utente esplora il mondo 3D della conoscenza in VR   | | |
|  |  - L'LLM consegna spiegazioni adattive                   | | |
|  |  - Dati di interazione loggati continuamente             | | |
|  +----------------------------------------------------------+ | |
|                         |                                     | |
|              Soglia fatica raggiunta?                         | |
|                   SI |  NO -----------------------------------> | |
|                         v                                     | |
|  +----------------------------------------------------------+ | |
|  | FASE DI RICARICA                                         | | |
|  |  - L'Agente Multimodale attiva il trigger dopaminergico  | | |
|  |  - Cambio scena / musica / video                         | | |
|  |  - Durata: calibrata sul profilo (2-8 min)               | | |
|  |  - Post-ricarica: segnale di readiness rilevato          | | |
|  +----------------------------------------------------------+ | |
|                         |                                     | |
+-------------------------+                                     | |
                          +-------------------------------------+ |
                                    LOOP ----------------------->+
```

---

## Data Model e Schemi

Tutti i dati sono archiviati **localmente** in un database SQLite strutturato (o opzionalmente un vector DB locale per embedding del knowledge graph).

```sql
-- Profilo cognitivo utente
CREATE TABLE attentional_profiles (
    user_id         TEXT PRIMARY KEY,
    created_at      DATETIME,
    updated_at      DATETIME,
    profile_json    TEXT
);

-- Log sessioni
CREATE TABLE sessions (
    session_id         TEXT PRIMARY KEY,
    user_id            TEXT REFERENCES attentional_profiles(user_id),
    subject            TEXT,
    started_at         DATETIME,
    ended_at           DATETIME,
    total_load_min     REAL,
    total_recharge_min REAL,
    concepts_covered   TEXT
);

-- Telemetria granulare degli eventi
CREATE TABLE interaction_events (
    event_id      TEXT PRIMARY KEY,
    session_id    TEXT REFERENCES sessions(session_id),
    timestamp     DATETIME,
    event_type    TEXT,
    payload_json  TEXT,
    fatigue_score REAL
);

-- Log trigger dopaminergici
CREATE TABLE trigger_events (
    trigger_id         TEXT PRIMARY KEY,
    session_id         TEXT REFERENCES sessions(session_id),
    fired_at           DATETIME,
    modality           TEXT,
    duration_min       REAL,
    pre_fatigue_score  REAL,
    post_fatigue_score REAL
);
```

---

## Technology Stack

| Layer | Tecnologia | Motivazione |
|---|---|---|
| LLM Inference | llama.cpp / Ollama | Locale, privacy-first, quantizzazione GGUF |
| LLM Models | LLaMA 3, Mistral, Phi-3 | Pesi open, eseguibili on-device |
| VR Engine | Unity 6 + XR Toolkit | Ottimizzato Quest 3, standard OpenXR |
| VR Hardware | Meta Quest 3 | Standalone, no PC tether |
| Backend Logic | Python 3.12+ | Agent core, pipeline dati, orchestrazione LLM |
| Database Locale | SQLite + ChromaDB (opzionale) | Zero-config, fully local |
| Media Integration | Spotify Web API, YouTube Data API v3 | Delivery stimoli dopaminergici |
| Comunicazione Inter-moduli | FastAPI (local REST) | LLM <-> Unity <-> Agent |

---

## Roadmap

### Fase 1 — Foundation (Mesi 1-3)

- [ ] Layer di integrazione LLM locale (Ollama + Python API wrapper)
- [ ] Engine di profilazione Attentional DNA (raccolta segnali + scoring)
- [ ] Data model SQLite e session logging
- [ ] Prototipo CLI per validazione algoritmica

### Fase 2 — World Engine (Mesi 4-6)

- [ ] Ambiente VR base Unity 6 con XR Toolkit
- [ ] Pipeline di estrazione LLM -> Concept Graph
- [ ] Ambienti 3D statici per 2-3 materie pilota
- [ ] Protocollo di comunicazione LLM <-> Unity (local REST)

### Fase 3 — Dopamine Loop (Mesi 7-9)

- [ ] Modello di rilevamento fatica cognitiva
- [ ] Implementazione Agente Multimodale (Spotify + YouTube + VR scene swap)
- [ ] Loop ciclico Load/Recharge completo in VR
- [ ] Studio utenti: 10 partecipanti, protocollo 4 settimane

### Fase 4 — Intelligence & Scale (Mesi 10-12)

- [ ] Aggiornamenti adattativi del concept graph
- [ ] Generazione procedurale ambienti 3D (pipeline LLM-to-scene)
- [ ] Tracking longitudinale metriche di neuroplasticita
- [ ] Beta pubblica + rilascio SDK open-source

---

## Basi di Ricerca

**Neuroscienze & Scienze Cognitive**

- Schultz, W. (1998). Predictive reward signal of dopamine neurons. Journal of Neurophysiology.
- Csikszentmihalyi, M. (1990). Flow: The Psychology of Optimal Experience. Harper & Row.
- Barsalou, L.W. (1999). Perceptual symbol systems. Behavioral and Brain Sciences.

**Adaptive Learning Systems**

- VanLehn, K. (2011). The relative effectiveness of human tutoring, intelligent tutoring systems, and other tutoring systems. Educational Psychologist.
- Corbett, A.T., & Anderson, J.R. (1994). Knowledge tracing: Modeling the acquisition of procedural knowledge. UMUAI.

**Spatial Learning & VR**

- Mayer, R.E. (2009). Multimedia Learning (2nd ed.). Cambridge University Press.
- Makransky, G., & Lilleholt, L. (2018). A structural equation modeling investigation of the emotional value of immersive VR in education. ETR&D.

**Neuroplasticita**

- Doidge, N. (2007). The Brain That Changes Itself. Viking Press.
- Merzenich, M.M. et al. (1996). Temporal processing deficits ameliorated by training. Science.

---

## Differenziatori Chiave

| Feature | PALS | Duolingo | Khan Academy | VR EdTech tradizionale |
|---|---|---|---|---|
| Gestione ciclo dopaminergico | SI - Core feature | NO | NO | NO |
| LLM locale (privacy totale) | SI | NO | NO | NO |
| Rilevamento fatica cognitiva | SI | NO | NO | NO |
| Apprendimento spaziale / VR | SI | NO | NO | Parziale |
| Attentional DNA profiling | SI - Originale | NO | NO | NO |
| Reward injection multimodale | SI | Parziale | NO | NO |
| Neuroplasticita come obiettivo | SI | NO | NO | NO |
| Subject-agnostic | SI | NO (solo lingue) | Parziale | Parziale |

---

## Obiettivi Finali

**1. Ringiovanimento Cerebrale**

Aumentare la neuroplasticita in soggetti adulti e anziani attraverso un engagement cognitivo ciclico e sostenuto. Il design e informato dalla ricerca che dimostra come il cervello mantenga capacita di adattamento fino alla tarda eta se appropriatamente stimolato.

**2. Efficienza 10x**

Mantenendo il learner in uno stato di Flow sostenuto (Csikszentmihalyi, 1990), PALS punta a una riduzione del 60-80% del time-to-mastery per soggetti complessi rispetto ai metodi di studio passivi.

**3. Personalizzazione Estrema**

Il profilo Attentional DNA evolve ad ogni sessione. Il sistema non ha un curriculum fisso: ricostruisce dinamicamente il percorso di apprendimento ottimale, trattando l'architettura cognitiva di ogni utente come un problema ingegneristico unico.

**4. Contrasto all'Invecchiamento Cognitivo**

Il ciclo di spompaggio e ripompaggio della sinusoide dopaminergica e progettato per mantenere l'elasticita sinaptica nel corso di mesi e anni d'uso, posizionando PALS come strumento di salute cognitiva a lungo termine.

---

## Dichiarazione di Paternita Intellettuale

**Dichiarazione di Prima Autoria — Aprile 2025**

Questo documento costituisce la specifica concettuale originale del **PoliMind Adaptive Learning System (PALS)**.

Le seguenti creazioni intellettuali sono originali di questo progetto:

- Il modello **Dopamine Sinusoid** per la gestione ciclica dell'attenzione
- La metodologia di profilazione **Attentional DNA**
- L'architettura multi-layer **LLM-VR-Agent**
- Il workflow operativo ciclico **Load/Recharge Phase**
- Il concetto di **Dopamine Injector** come agente multimodale di trigger

**Prima autoria e pubblicazione:** Aprile 2025  
**Autore:** Craicek  
**GitHub:** [github.com/BitMakerMan](https://github.com/BitMakerMan)  
**Repository:** [github.com/BitMakerMan/AdaptiveLearningSystem](https://github.com/BitMakerMan/AdaptiveLearningSystem)

La storia dei commit di questa repository funge da registro timestampato di autoria. Qualsiasi utilizzo, riproduzione o derivazione del materiale contenuto in questo documento senza attribuzione esplicita a **Craicek (@BitMakerMan)** costituisce una violazione delle condizioni di licenza.

---

## Licenza

```
Creative Commons Attribution-NonCommercial-NoDerivatives 4.0 International

Sei libero di:
  Condividere — copiare e ridistribuire il materiale in qualsiasi formato

Alle seguenti condizioni:
  Attribuzione   — Devi dare credito appropriato a Craicek (@BitMakerMan).
  NonCommerciale — Non puoi usare il materiale per scopi commerciali.
  NoDerivati     — Non puoi distribuire versioni modificate del materiale.

Testo completo: https://creativecommons.org/licenses/by-nc-nd/4.0/
```

---

*PoliMind Adaptive Learning System — Concepito da Craicek, Aprile 2025*  
*[github.com/BitMakerMan/AdaptiveLearningSystem](https://github.com/BitMakerMan/AdaptiveLearningSystem)*

> "Il cervello non e un vaso da riempire, ma un fuoco da accendere."
