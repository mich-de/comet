# Comet Browser - GitHub Mirror

<div align="center">

![Comet Browser](https://img.shields.io/badge/Comet%20Browser-Latest-blue?style=for-the-badge)
[![GitHub Release](https://img.shields.io/github/v/release/mich-de/comet?style=flat-square&logo=github)](https://github.com/mich-de/comet/releases)
[![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/mich-de/comet/download-comet.yml?style=flat-square&logo=github-actions)](https://github.com/mich-de/comet/actions)
[![License](https://img.shields.io/badge/License-MIT-green?style=flat-square)](LICENSE)
[![Website](https://img.shields.io/badge/Website-Live-brightgreen?style=flat-square&logo=github-pages)](https://mich-de.github.io/comet/)

**[English](#english)** | **[Italiano](#italiano)**

</div>

---

<a name="english"></a>

## 🌐 English

### Overview

**Comet Browser GitHub Mirror** is an unofficial repository that provides seamless access to the latest version of Comet Browser by Perplexity. This project automatically downloads the newest stable release every day and hosts it on GitHub, making it accessible even when official download channels are blocked.

### ✨ Key Features

| Feature | Description |
|---------|------------|
| 🔄 **Daily Updates** | Automatic download of the latest version every day at midnight UTC |
| 🔗 **Official Source** | Direct downloads from Perplexity's official servers |
| 🚀 **Reliable Access** | GitHub is rarely blocked by corporate firewalls |
| 🌍 **Bilingual Interface** | Website available in English and Italian |
| 📦 **Clean Releases** | Only the latest version is kept (automatic cleanup) |
| 🔒 **Secure** | No modifications, files are exactly as released by Perplexity |

### 📥 Download Options

#### Option 1: Web Interface (Recommended)
Visit **[mich-de.github.io/comet](https://mich-de.github.io/comet/)** and click the download button.

**Advantages:**
- Simple and intuitive interface
- Real-time status updates
- Last update timestamp displayed
- Works on any device with a browser
- Bilingual support

#### Option 2: Direct Link (Always Latest)
https://github.com/mich-de/comet/releases/latest/download/comet-installer-win_x64.exe


**Use this if:**
- You want to automate downloads
- You prefer command-line tools
- You need a permanent link that doesn't expire

#### Option 3: GitHub Releases Page
Navigate to [github.com/mich-de/comet/releases](https://github.com/mich-de/comet/releases) and download manually.

**Use this if:**
- You want to see version history
- You prefer GitHub's native interface
- You need detailed release notes

### 🔧 How It Works
Every Day (Midnight UTC)
↓
GitHub Actions Workflow
↓
Download Latest Comet
(from Perplexity)
↓
Publish as Release
↓
You Download
(from GitHub)
↓
Install Comet


**Detailed Process:**

1. **Automated Download** - A GitHub Actions workflow runs daily and fetches the latest Comet version from Perplexity's official API endpoint
2. **Quality Check** - The workflow verifies the download integrity and file size
3. **Release Publishing** - The file is automatically published as a GitHub Release with tag `comet-win64-latest`
4. **Old Version Cleanup** - Previous versions are automatically removed to keep the repository clean
5. **Your Access** - You download from GitHub (which is rarely blocked by firewalls)
6. **Installation** - Run the installer and use Comet normally

### 💻 System Requirements

| Requirement | Details |
|------------|---------|
| **OS** | Windows 10 / Windows 11 |
| **Architecture** | 64-bit (x64) |
| **RAM** | Minimum 4GB (8GB recommended) |
| **Disk Space** | ~200MB free space |
| **Internet** | Required for download and initial setup |

### 📋 Project Structure
comet/
├── index.html # Web interface (bilingual)
├── README.md # This file
├── .github/
│ └── workflows/
│ ├── download-comet.yml # Daily download automation
│ └── cleanup-deployments.yml # Deployment cleanup
└── releases/ # Auto-generated GitHub Releases

### 🤖 Automation Details

#### Download Workflow
- **Schedule**: Every day at 00:00 UTC
- **Trigger**: Can also be run manually via GitHub Actions
- **Source**: `https://www.perplexity.ai/rest/browser/download?platform=win_x64&channel=stable`
- **Output**: Creates/updates release with tag `comet-win64-latest`

#### Cleanup Workflow
- **Trigger**: Manual execution only
- **Function**: Removes old deployment records
- **Benefit**: Keeps repository history clean

### 🌍 Language Support

The website automatically detects your browser language and displays content accordingly:

**Supported Languages:**
- 🇬🇧 English
- 🇮🇹 Italian

**Toggle Anytime:**
- Click the language buttons (EN/IT) in the top-right corner
- Your preference is saved in your browser

### 🔐 Security & Verification

✅ **Official Downloads Only**
- Files are downloaded directly from Perplexity's official servers
- No repackaging or modifications
- Verified daily

✅ **No Tracking**
- No analytics or user tracking
- No telemetry beyond GitHub's standard logs
- Fully transparent code

✅ **Open Source**
- Complete transparency
- Anyone can review the workflows
- Community-driven

### 📊 Status & Monitoring

| Component | Status |
|-----------|--------|
| **Download Workflow** | [![Status](https://github.com/mich-de/comet/actions/workflows/download-comet.yml/badge.svg)](https://github.com/mich-de/comet/actions/workflows/download-comet.yml) |
| **Website** | [![Website Status](https://img.shields.io/website?url=https%3A%2F%2Fmich-de.github.io%2Fcomet&label=github-pages)](https://mich-de.github.io/comet/) |
| **Latest Release** | [![Release Date](https://img.shields.io/github/release-date/mich-de/comet)](https://github.com/mich-de/comet/releases/latest) |

### 🚀 Quick Start

```bash
# Method 1: Direct download (Windows PowerShell)
Invoke-WebRequest `
  -Uri "https://github.com/mich-de/comet/releases/latest/download/comet-installer-win_x64.exe" `
  -OutFile "comet-installer.exe"

# Method 2: Using curl (if installed)
curl -L -o comet-installer.exe \
  "https://github.com/mich-de/comet/releases/latest/download/comet-installer-win_x64.exe"

# Method 3: Using GitHub CLI
gh release download comet-win64-latest --repo mich-de/comet -p "*.exe"
❓ Frequently Asked Questions
Q: Is this official?

A: No, this is an unofficial mirror. It downloads from Perplexity's official servers, but is not affiliated with Perplexity.

Q: Is it safe?

A: Yes. We download directly from Perplexity and make no modifications. All code is transparent and reviewable.

Q: How often is it updated?

A: Daily at midnight UTC. You can also check the GitHub Actions workflow for detailed logs.

Q: Can I trust this?

A: Yes. The repository is public, all workflows are visible, and nothing is hidden. You can review everything.

Q: What if GitHub is blocked?

A: Try using a VPN or proxy. Alternatively, you can access Comet through other mirrors or download directly from Perplexity if possible.

Q: Does it work on Mac/Linux?

A: Currently only Windows 64-bit is provided. You can modify the workflow to include other platforms.

📞 Support
For Issues:

Open an Issue

Start a Discussion

Official Links:

Comet Official

Perplexity

⚖️ Legal & Disclaimer
This project is provided "as-is" for educational and accessibility purposes. Comet Browser and all related trademarks are the property of Perplexity. We are not affiliated with or endorsed by Perplexity.

Use at your own risk. While we take every precaution to ensure security, we cannot guarantee the safety of any downloaded files.

📄 License
This project is licensed under the MIT License. See LICENSE file for details.

🙏 Credits
Comet Browser by Perplexity

Automation by GitHub Actions

Hosting by GitHub Pages

<a name="italiano"></a>

🌐 Italiano
Panoramica
Comet Browser GitHub Mirror è un repository non ufficiale che fornisce accesso facile all'ultima versione di Comet Browser di Perplexity. Questo progetto scarica automaticamente la versione stabile più recente ogni giorno e la ospita su GitHub, rendendola accessibile anche quando i canali di download ufficiali sono bloccati.

✨ Caratteristiche Principali
Caratteristica	Descrizione
🔄 Aggiornamenti Giornalieri	Download automatico dell'ultima versione ogni giorno a mezzanotte UTC
🔗 Fonte Ufficiale	Download diretto dai server ufficiali di Perplexity
🚀 Accesso Affidabile	GitHub è raramente bloccato dai firewall aziendali
🌍 Interfaccia Bilingue	Sito web disponibile in Inglese e Italiano
📦 Release Pulite	Solo l'ultima versione viene mantenuta (pulizia automatica)
🔒 Sicuro	Nessuna modifica, i file sono esattamente come rilasciati da Perplexity
📥 Opzioni di Download
Opzione 1: Interfaccia Web (Consigliato)
Visita mich-de.github.io/comet e clicca il bottone di download.

Vantaggi:

Interfaccia semplice e intuitiva

Aggiornamenti di stato in tempo reale

Timestamp dell'ultimo aggiornamento visualizzato

Funziona su qualsiasi dispositivo con browser

Supporto bilingue

Opzione 2: Link Diretto (Sempre l'Ultimo)
https://github.com/mich-de/comet/releases/latest/download/comet-installer-win_x64.exe
Usalo se:

Vuoi automatizzare i download

Preferisci gli strumenti da riga di comando

Hai bisogno di un link permanente che non scade

Opzione 3: Pagina GitHub Releases
Naviga a github.com/mich-de/comet/releases e scarica manualmente.

Usalo se:

Vuoi vedere la cronologia delle versioni

Preferisci l'interfaccia nativa di GitHub

Hai bisogno di note di rilascio dettagliate

🔧 Come Funziona
Ogni Giorno (Mezzanotte UTC)
        ↓
  Workflow GitHub Actions
        ↓
  Scarica l'Ultimo Comet
  (da Perplexity)
        ↓
  Pubblica come Release
        ↓
   Tu Scarichi
   (da GitHub)
        ↓
   Installa Comet
Processo Dettagliato:

Download Automatico - Un workflow GitHub Actions viene eseguito ogni giorno e recupera l'ultima versione di Comet dal'endpoint API ufficiale di Perplexity

Controllo di Qualità - Il workflow verifica l'integrità del download e la dimensione del file

Pubblicazione Release - Il file viene automaticamente pubblicato come GitHub Release con tag comet-win64-latest

Pulizia Versione Vecchia - Le versioni precedenti vengono rimosse automaticamente per mantenere il repository pulito

Tuo Accesso - Scarichi da GitHub (che è raramente bloccato dai firewall)

Installazione - Esegui l'installer e usa Comet normalmente

💻 Requisiti di Sistema
Requisito	Dettagli
OS	Windows 10 / Windows 11
Architettura	64-bit (x64)
RAM	Minimo 4GB (8GB consigliato)
Spazio Disco	~200MB di spazio libero
Internet	Richiesto per il download e la configurazione iniziale
📋 Struttura del Progetto
comet/
├── index.html                      # Interfaccia web (bilingue)
├── README.md                       # Questo file
├── .github/
│   └── workflows/
│       ├── download-comet.yml      # Automazione download giornaliero
│       └── cleanup-deployments.yml # Pulizia deployment
└── releases/                       # GitHub Releases auto-generato
🤖 Dettagli Automazione
Workflow Download
Programmazione: Ogni giorno alle 00:00 UTC

Attivazione: Può anche essere eseguito manualmente tramite GitHub Actions

Fonte: https://www.perplexity.ai/rest/browser/download?platform=win_x64&channel=stable

Output: Crea/aggiorna release con tag comet-win64-latest

Workflow Pulizia
Attivazione: Solo esecuzione manuale

Funzione: Rimuove i vecchi record di deployment

Vantaggio: Mantiene la cronologia del repository pulita

🌍 Supporto Linguistico
Il sito web rileva automaticamente la lingua del tuo browser e visualizza i contenuti di conseguenza:

Lingue Supportate:

🇬🇧 Inglese

🇮🇹 Italiano

Cambia in Qualsiasi Momento:

Clicca i bottoni

