# Eleonardo Bajramovski (Neniku)

> Systems administrator in training · Linux · Docker · DevSecOps · Vasto, Italy

[English](#english) · [Italiano](#italiano)

---

<a name="english"></a>
## English

I've been taking hardware and software apart since 2012/2013. It started with CyanogenMod 10 on a Galaxy S3 Exynos — the camera driver had a known compatibility issue with the Exynos variant under custom ROMs, and getting it working meant tracking down a dedicated kernel module and flashing it through ClockworkMod Recovery. That kind of problem stuck with me: find the root cause, find the fix, understand why it works.

From there the path went through a OnePlus One (CyanogenOS, then OxygenOS, then Tuga Power as daily ROM), the OnePlus One Italia Telegram group, and eventually into international XDA communities where I picked up the habit of following development threads and reading changelogs like other people read the news. After the OnePlus One came a Redmi Note 3 Pro (kenzo), a Redmi Note 5 Pro (whyred), and now a OnePlus 8T — still modded. The Android side never really stopped.

Around the same time, I started doing the same on my PC: upgraded the RAM, dual-booted every OS that came out, and when Windows 10 arrived I began stripping it down to build something actually usable. That habit carried over into Linux, self-hosting, scripting, and eventually into a serious interest in security and DevSecOps.

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
| Cooling | Arctic MX-7 thermal paste · mild OC via MSI Afterburner |

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

<details>
<summary>Systems & infrastructure</summary>

Linux (Debian-based, Pop!_OS, MX Linux), Docker, Tailscale, Nginx, Windows

</details>

<details>
<summary>Scripting & automation</summary>

Bash, Python, YAML, GitHub Actions

</details>

<details>
<summary>Security</summary>

Trivy, OWASP ZAP, SBOM/supply chain analysis, DAST pipelines, FlareVM, CAINE

</details>

<details>
<summary>Homelab</summary>

Jellyfin, Sonarr, Radarr, MedicatedUSB, custom bootable USB environments

</details>

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

Kingdom Hearts and Yu-Gi-Oh are taking up most of my free time lately. I spend more time than I should reading patch notes for games I host but rarely get to play.

[LinkedIn](https://www.linkedin.com/in/eleonardo-bajramovski-7599a7372/)

---

<a name="italiano"></a>
## Italiano

Smonto hardware e software dal 2012/2013. È iniziato con CyanogenMod 10 su un Galaxy S3 Exynos — il driver della fotocamera aveva un problema di compatibilità noto sulla variante Exynos con le custom ROM, e per farlo funzionare ho dovuto scovare un modulo kernel dedicato e flasharlo tramite ClockworkMod Recovery. Quel tipo di problema mi è rimasto in testa: trovare la causa, trovare la soluzione, capire perché funziona.

Da lì il percorso è passato per un OnePlus One (CyanogenOS, poi OxygenOS, poi Tuga Power come ROM quotidiana), il gruppo Telegram OnePlus One Italia, e alla fine le community internazionali su XDA, dove ho preso l'abitudine di seguire i thread di sviluppo e leggere i changelog come altri leggono le notizie. Dopo il OnePlus One sono arrivati un Redmi Note 3 Pro (kenzo), un Redmi Note 5 Pro (whyred), e ora un OnePlus 8T — ancora moddato. Il lato Android non si è mai fermato davvero.

Nello stesso periodo ho iniziato a fare lo stesso sul PC: aggiornata la RAM, dual boot di tutto quello che usciva, e quando è arrivato Windows 10 ho cominciato a smontarlo per costruire qualcosa di effettivamente usabile. Quell'abitudine si è estesa a Linux, al self-hosting, alla scripting, e alla fine a un interesse serio per la security e il DevSecOps.

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
| Raffreddamento | Pasta termica Arctic MX-7 · leggero OC via MSI Afterburner |

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

<details>
<summary>Sistemi & infrastruttura</summary>

Linux (Debian-based, Pop!_OS, MX Linux), Docker, Tailscale, Nginx, Windows

</details>

<details>
<summary>Scripting & automazione</summary>

Bash, Python, YAML, GitHub Actions

</details>

<details>
<summary>Sicurezza</summary>

Trivy, OWASP ZAP, analisi SBOM/supply chain, pipeline DAST, FlareVM, CAINE

</details>

<details>
<summary>Homelab</summary>

Jellyfin, Sonarr, Radarr, MedicatedUSB, ambienti USB avviabili personalizzati

</details>

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

Ultimamente Kingdom Hearts e Yu-Gi-Oh occupano la maggior parte del tempo libero. Passo più tempo del necessario a leggere le note di aggiornamento di giochi che ospito sui miei server ma che riesco raramente a giocare.

[LinkedIn](https://www.linkedin.com/in/eleonardo-bajramovski-7599a7372/)
