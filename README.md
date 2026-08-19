# Eleonardo Bajramovski (Neniku)

[English](#english) · [Italiano](#italiano)

---

<a name="english"></a>
## English

Systems administrator in training, based in Vasto, Italy.

I've been taking hardware and software apart since 2012/2013. It started with CyanogenMod 10 on a Galaxy S3 Exynos — the camera wouldn't initialize under custom ROMs because of a driver issue specific to the Exynos variant, and it took finding the right kernel module to flash via ClockworkMod Recovery to get it working. That kind of problem stuck with me: find the root cause, find the fix, understand why it works.

From there the path went through a OnePlus One (CyanogenOS, then OxygenOS, then Tuga Power as daily ROM), the OnePlus One Italia Telegram group, and eventually into international XDA communities where I picked up the habit of following development threads and reading changelogs like other people read the news. After the OnePlus One came a Redmi Note 3 Pro (kenzo), a Redmi Note 5 Pro (whyred), and now a OnePlus 8T — still modded. The Android side never really stopped.

Around the same time I was doing all of this on phones, I started doing the same on my PC. Swapped RAM, dual-booted everything that came out, and when Windows 10 arrived I started stripping it down to build something actually usable. That habit carried over into Linux, self-hosting, scripting, and eventually into a proper interest in security and DevSecOps.

---

### The machine

My main box is a Lenovo IdeaPad Gaming 3 (15ACH6) I call **Frankenstein** — not because it looks bad, but because it's been rebuilt piece by piece:

| Component | Spec |
|---|---|
| CPU | AMD Ryzen 5 5600H |
| GPU | NVIDIA RTX 3050 |
| RAM | 32GB Lexar DDR4 3200MHz |
| Storage | Samsung 990 Pro 1TB (NVMe) + Crucial 1TB (M.2 2242) |
| Display | 165Hz panel (replaced) |
| Cooling | Arctic MX-7 thermal paste, mild OC via MSI Afterburner |

It dual boots **Windows 11** (stripped with ChrisTitus tool and Winhance, styled with Windhawk and Start11 v2) and **Pop!_OS**, where I do most of the actual work. VMs live on a shared SSD partition, accessible from both sides.

---

### The server

A separate MX Linux machine running:
- Jellyfin media server
- Docker containers for various self-hosted services
- Palworld dedicated server (for me, my brother-in-law and my nephews)
- Everything behind Tailscale and an Nginx reverse proxy

---

### What I work with

**Systems & infrastructure**
Linux (Debian-based, Pop!_OS, MX Linux), Docker, Tailscale, Nginx, Windows

**Scripting & automation**
Bash, Python, YAML, GitHub Actions

**Security**
Trivy, OWASP ZAP, SBOM/supply chain analysis, DAST pipelines, FlareVM, CAINE

**Homelab tools**
Jellyfin, Sonarr, Radarr, MedicatedUSB, custom bootable USB environments

---

### Currently learning

- Container vulnerability scanning and SBOM generation
- DAST integration in CI/CD pipelines
- ZFS management
- GPU transcoding for self-hosted media

---

### Projects

- [Backup_script_Cyborg](https://github.com/Neniku/Backup_script_Cyborg) — hardened Bash backup: encryption, SHA256 verification, dual remote upload (SFTP + SMB), checkpoint/resume, HTML report. Evolution of [Backup_script_Umano](https://github.com/Neniku/Backup_script_Umano).
- [Metodi_Di_Compressione](https://github.com/Neniku/Metodi_Di_Compressione) — notes and slides on compression algorithms and their real-world tradeoffs.

---

### Outside the terminal

Kingdom Hearts and Yu-Gi-Oh are taking up most of my free time lately. I collect Swatch watches and spend more time than I should reading patch notes for games I host but barely get to play.

[LinkedIn](https://www.linkedin.com/in/eleonardo-bajramovski-7599a7372/)

---

<a name="italiano"></a>
## Italiano

Amministratore di sistemi in formazione, basato a Vasto, in Abruzzo.

Smonto hardware e software dal 2012/2013. È iniziato con CyanogenMod 10 su un Galaxy S3 Exynos — la fotocamera non si inizializzava con le custom ROM a causa di un problema del driver specifico della variante Exynos, e ci è voluto trovare il modulo giusto da flashare tramite ClockworkMod Recovery per farlo funzionare. Quel tipo di problema mi è rimasto in testa: trovare la causa, trovare la soluzione, capire perché funziona.

Da lì il percorso è passato per un OnePlus One (CyanogenOS, poi OxygenOS, poi Tuga Power come ROM quotidiana), il gruppo Telegram OnePlus One Italia, e alla fine le community internazionali su XDA, dove ho preso l'abitudine di seguire i thread di sviluppo e leggere i changelog come altri leggono le notizie. Dopo il OnePlus One sono arrivati un Redmi Note 3 Pro (kenzo), un Redmi Note 5 Pro (whyred), e ora un OnePlus 8T — ancora moddato. Il lato Android non si è mai fermato davvero.

Nello stesso periodo in cui facevo tutto questo sui telefoni, ho iniziato a fare lo stesso sul PC. Cambiate le RAM, dual boot di tutto quello che usciva, e quando è arrivato Windows 10 ho cominciato a smontarlo per costruire qualcosa di effettivamente usabile. Quell'abitudine si è trasferita su Linux, il self-hosting, lo scripting, e alla fine su un interesse serio per la security e il DevSecOps.

---

### La macchina

Il mio PC principale è un Lenovo IdeaPad Gaming 3 (15ACH6) che chiamo **Frankenstein** — non perché sia brutto, ma perché è stato ricostruito pezzo per pezzo:

| Componente | Specifiche |
|---|---|
| CPU | AMD Ryzen 5 5600H |
| GPU | NVIDIA RTX 3050 |
| RAM | 32GB Lexar DDR4 3200MHz |
| Storage | Samsung 990 Pro 1TB (NVMe) + Crucial 1TB (M.2 2242) |
| Display | Pannello 165Hz (sostituito) |
| Raffreddamento | Pasta termica Arctic MX-7, leggero OC via MSI Afterburner |

Dual boot tra **Windows 11** (ripulito con ChrisTitus tool e Winhance, personalizzato con Windhawk e Start11 v2) e **Pop!_OS**, dove faccio la maggior parte del lavoro reale. Le VM stanno su una partizione SSD condivisa, accessibile da entrambi i lati.

---

### Il server

Una macchina separata con MX Linux che gestisce:
- Jellyfin come media server
- Container Docker per vari servizi self-hosted
- Server dedicato di Palworld (per me, mio cognato e i miei nipoti)
- Tutto dietro Tailscale e un reverse proxy Nginx

---

### Con cosa lavoro

**Sistemi & infrastruttura**
Linux (Debian-based, Pop!_OS, MX Linux), Docker, Tailscale, Nginx, Windows

**Scripting & automazione**
Bash, Python, YAML, GitHub Actions

**Sicurezza**
Trivy, OWASP ZAP, analisi SBOM/supply chain, pipeline DAST, FlareVM, CAINE

**Homelab**
Jellyfin, Sonarr, Radarr, MedicatedUSB, ambienti USB avviabili personalizzati

---

### Cosa sto imparando

- Container vulnerability scanning e generazione SBOM
- Integrazione DAST nelle pipeline CI/CD
- Gestione ZFS
- Transcoding GPU per media server self-hosted

---

### Progetti

- [Backup_script_Cyborg](https://github.com/Neniku/Backup_script_Cyborg) — backup Bash con cifratura, verifica SHA256, upload ridondante (SFTP + SMB), checkpoint/resume e report HTML. Evoluzione di [Backup_script_Umano](https://github.com/Neniku/Backup_script_Umano).
- [Metodi_Di_Compressione](https://github.com/Neniku/Metodi_Di_Compressione) — appunti e slide sugli algoritmi di compressione e i loro tradeoff reali.

---

### Fuori dal terminale

Ultimamente Kingdom Hearts e Yu-Gi-Oh si stanno prendendo la maggior parte del tempo libero. Colleziono orologi Swatch e passo più tempo del dovuto a leggere patch note di giochi che hosto ma che fatico a trovare il tempo di giocare.

[LinkedIn](https://www.linkedin.com/in/eleonardo-bajramovski-7599a7372/)
