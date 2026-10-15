<div align="center">

# 🥊 TWIN STRIKE: K.O. RUSH
### *Mobile Pixel Edition // 16-Bit Endless Arcade Brawler*

[![Play on Vercel](https://img.shields.io/badge/🎮_GIOCA_ORA-twin--strike.vercel.app-00f5d4?style=for-the-badge&logo=vercel&logoColor=black)](https://twin-strike.vercel.app/)
[![GitHub Repo](https://img.shields.io/badge/GitHub-include--Nico%2FTWIN--STRIKE-ff2a85?style=for-the-badge&logo=github&logoColor=white)](https://github.com/include-Nico/TWIN-STRIKE)
[![HTML5](https://img.shields.io/badge/HTML5-Canvas_2D-ffd000?style=for-the-badge&logo=html5&logoColor=black)](#)

<br />

**Un frenetico brawler arcade endless in pixel art 16-bit con controlli 2-Tap / 3-Button, progettato per dispositivi mobile (iOS & Android) e desktop.**

### 👉 **[GIOCA SUBITO NEL BROWSER: twin-strike.vercel.app](https://twin-strike.vercel.app/)** 👈

</div>

---

## 📖 Panoramica del Progetto

**Twin Strike: K.O. Rush** è un action game arcade basato sul ritmo, sui riflessi e sulla precisione. Sviluppato interamente come Web App single-file zero-dependency, combina un motore di rendering pixel art procedurale su Canvas 2D (HiDPI/Retina-ready), effetti sonori chiptune sintetizzati in tempo reale tramite Web Audio API e un sistema completo di progressione salvato direttamente nel browser.

---

## 🕹️ Meccaniche di Gioco e Controlli

I nemici attaccano da entrambi i lati del tatami[cite: 1]. Il giocatore deve attendere che entrino nella **Hit Zone** prima di sferrare il colpo, evitando di attaccare a vuoto[cite: 1].

* **Hit Zone & Zona Perfect**: Colpisci i nemici quando entrano nelle fasce colorate a terra (ciano a sinistra, magenta a destra)[cite: 1]. Colpirli nella fascia interna dorata attiva un **Perfect Hit**, garantendo punti extra, ricarica Super accelerata e bonus in crediti[cite: 1].
* **Whiff (Colpo a vuoto)**: Attaccare quando nessun nemico è a portata espone il lottatore per una frazione di secondo e azzera la combo[cite: 1].
* **Parry & Twin Strike (`L + R` / Tasto Centrale)**:
  * Respinge ed elimina all'istante i nemici corazzati in carica (**Charger**)[cite: 1].
  * Se sono presenti nemici a portata sia a sinistra che a destra, esegue un doppio attacco simultaneo (**Twin Strike**)[cite: 1].
* **Super Overdrive**: Raggiunto il 100% della barra Furia, la pressione del comando centrale (`L + R`) scatena la tecnica speciale unica del combattente equipaggiato[cite: 1].

### Schema Comandi

| Azione | Touch / Mobile (iOS & Android) | Tastiera (Desktop) |
| :--- | :--- | :--- |
| **Pugno Sinistro** | Tap metà sinistra schermo / Pad `◀` | `A` oppure `Freccia Sinistra (←)` |
| **Calcio Destro** | Tap metà destra schermo / Pad `▶` | `D` oppure `Freccia Destra (→)` |
| **Parry / Super** | Pad centrale `⚡ PARRY` o Tap simultaneo SX+DX | `Spazio`, `W` oppure `Freccia Su (↑)` |
| **Rigioca Rapido** | Pulsante a schermo | `Spazio` (nella schermata K.O.) |

---

## 🥋 Roster Combattenti & Stili Colore (Skin)

Il gioco include **5 Brawler sbloccabili**, ciascuno dotato di sprite animati su misura, animazioni di K.O. dedicate, **3 Stili Colore (Skin)**, un'abilità passiva e una mossa Super Overdrive[cite: 1]:

| Fighter | Ruolo | Abilità Passiva | ★ Super Overdrive | Stili Colore (Skin) |
| :--- | :--- | :--- | :--- | :--- |
| **RYUJI** | *Karateka* | **Secondo Fiato**: Sopravvive a 1 K.O. per match respingendo tutti i nemici. | **Drago Shoryu**: Montante draconico che spazza via tutti i nemici a schermo. | *Dojo Bianco*, *Ombra Satsui*, *Drago d'Oro* |
| **VEX** | *Cyber Kunoichi* | **Passo Fantasma**: Il whiff dura la metà (175ms) e dimezza la combo invece di azzerarla. | **Chrono Slash (4s)**: Attiva un quadrante temporale che rallenta i nemici del 50%. | *Neon Shinobi*, *Rosso Akira*, *Artico Stealth* |
| **TITAN** | *Mecha Brute* | **Pugno Demolitore**: Elimina i Tank corazzati in 1 solo colpo se colpiti in zona Perfect. | **Armatura Magma (5s)**: Invulnerabilità totale; chi tocca Titan esplode all'impatto. | *Forgia Magma*, *Eva-01 Cyber*, *Crio Titanio* |
| **KITSUNE** | *Volpe d'Oro* | **Occhio d'Oro**: Zona Perfect +30% più ampia e +1 Credito ad ogni Perfect (1 HP max). | **Tempesta d'Oro (6s)**: Evoca un portale Torii che triplica le monete ottenute. | *Inari Reale*, *Spirito Sakura*, *Fuoco Fatuo* |
| **CYPHER** | *Monaco Matrix* | **Riflesso Zen**: Con Combo $\ge 30$ intercetta e colpisce automaticamente i Ninja in salto. | **Doppio Ologramma (6s)**: Evoca cloni digitali che replicano gli attacchi sul lato opposto. | *Codice Zen*, *Monaco Solare*, *Synth Glitch* |

> 💡 **Sala Prove Interattiva**: Dalla schermata *Fighters* è possibile testare in tempo reale tutte le animazioni di ogni personaggio (`IDLE`, `PUGNO SX`, `CALCIO DX`, `PARRY`, `SUPER UNICA`, `K.O.`) e cambiare la Skin attiva[cite: 1].

---

## 👾 Archetipi Nemici

* **Cyber-Punk Striker** (`1 HP`): Assaltatore rapido standard[cite: 1].
* **Heavy Juggernaut Tank** (`2-3 HP`): Colosso corazzato che richiede più colpi (viene respinto a ogni impatto prima di andare K.O.)[cite: 1].
* **Kage Shinobi Ninja** (`1 HP`): Giunto al limite della Hit Zone, esegue un salto mortale scavalcando il giocatore e atterrando sul lato opposto[cite: 1].
* **Oni Mecha Berserker (Charger)** (`1 HP`): Carica ad alta velocità; immune agli attacchi standard, deve essere neutralizzato con un **Parry (`L+R`)**[cite: 1].
* **Golden Treasure Goblin** (`4 HP`): Mecha dorato raro che conferisce un ricco bottino di crediti se sconfitto prima che riesca a fuggire[cite: 1].

---

## 🏯 Dojo Shop & Casse Bottino K.O.

### Potenziamenti Permanenti (Dojo)
* **Cuori di Ferro** (`Max LV.3`): +1 Cuore massimo in arena[cite: 1].
* **Allungo Marziale** (`Max LV.5`): +8px di ampiezza della Hit Zone per livello[cite: 1].
* **Focus Zen** (`Max LV.5`): +0.4s di durata del timer combo e incremento del moltiplicatore massimo[cite: 1].
* **Spirito Ardente** (`Max LV.5`): Riduce i colpi necessari per caricare la barra Super[cite: 1].
* **Sponsor Dojo** (`Max LV.5`): +15% di crediti extra a fine partita per livello[cite: 1].

### Gadget Monouso
* **Drone Scudo Pixel**: Annulla il primo danno subito o il primo errore (whiff) salvando la combo[cite: 1].
* **Turbo Start x4**: Permette di iniziare il match direttamente con combo 30 e moltiplicatore `x4`[cite: 1].

### 🎁 Cassa K.O. (Ogni 20.000 Punti)
Ogni **20.000 punti cumulativi** ottenuti nelle partite sblocca una **Cassa Bottino K.O.**[cite: 1]. Aprendola, il giocatore può scegliere tra:
1. **+1.250 Crediti** immediati[cite: 1].
2. **Una nuova Skin esclusiva** (con priorità automatica per i Brawler già posseduti)[cite: 1].

---

## 💾 Salvataggio Persistente & Backup Cloud-less

I progressi (crediti, record, avanzamento casse, combattenti, skin e potenziamenti) vengono salvati in automatico nel `localStorage` del browser[cite: 1]:
* **Autosave**: Scrittura immediata a fine incontro, ad ogni acquisto e alla chiusura della scheda (`pagehide` / `visibilitychange`)[cite: 1].
* **Esporta / Importa Codice di Backup**: Dal menu ⚙️ **Salvataggio** in alto a destra è possibile copiare una stringa codificata in Base64 dei propri progressi per salvarla o trasferirla su un altro dispositivo (es. da PC a smartphone)[cite: 1].

---

## 🛠️ Stack Tecnologico

* **HTML5 & CSS3**: Struttura responsive Mobile-First con supporto `100dvh`, `safe-area-inset` per iOS/Android, filtro CRT Scanlines disattivabile e UI pixel-bevel[cite: 1].
* **Tailwind CSS + Google Fonts**: Tipografie arcade (`Press Start 2P`, `Silkscreen`, `VT323`) e icone `Phosphor Icons`[cite: 1].
* **Vanilla JavaScript (ES6+)**:
  * `PixelRenderer`: Rendering procedurale su matrici ASCII-art a 24 righe con gestione dinamica delle palette, afterimages, particellari e screen-shake[cite: 1].
  * `Sound`: Sintetizzatore chiptune Web Audio API integrato a latenza zero[cite: 1].
  * `SaveSystem` & `CrateSystem`: Gestione stato, migrazione chiavi legacy e sistema gacha deterministico[cite: 1].

---

## 🚀 Avvio Locale e Installazione Mobile

### Esecuzione in Locale
Il progetto non richiede dipendenze esterne o build step.

```bash
# Clona il repository
git clone [https://github.com/include-Nico/TWIN-STRIKE.git](https://github.com/include-Nico/TWIN-STRIKE.git)

# Entra nella cartella
cd TWIN-STRIKE

# Apri index.html nel browser oppure avvia un server statico
python3 -m http.server 8080
