# Eleonardo Bajramovski

> Amministratore di sistemi in formazione &nbsp;&middot;&nbsp; Linux &nbsp;&middot;&nbsp; Docker &nbsp;&middot;&nbsp; DevSecOps &nbsp;&middot;&nbsp; Vasto (CH)

[Italiano](#italiano) &nbsp;&middot;&nbsp; [English](#english)

---

<a name="italiano"></a>
## Italiano

Ho iniziato a smontare hardware e software intorno al 2012/2013, quando ho flashato CyanogenMod 10 su un Galaxy S3 con processore Exynos. Il problema era che il driver della fotocamera non era compatibile con le custom ROM sulla variante Exynos: la fotocamera semplicemente non partiva. La soluzione è arrivata grazie a qualcuno che aveva compilato un modulo kernel apposito, da installare tramite ClockworkMod Recovery. Da quel momento ho capito che mi interessava capire come funzionano le cose, non solo usarle.

Dopo il Galaxy S3 sono passato al OnePlus One, che all'epoca era il telefono della community per eccellenza: veniva venduto con CyanogenOS di serie, poi è passato alla OxygenOS, e io ho finito con Tuga Power come ROM quotidiana. Tramite il gruppo Telegram OnePlus One Italia ho scoperto un mondo: da lì sono entrato in community internazionali su XDA, ho iniziato a seguire thread di sviluppo, leggere changelog e capire come lavorano i developer di custom ROM. Quella porta non si è mai richiusa. Dopo il OnePlus One sono arrivati un Redmi Note 3 Pro (kenzo), un Redmi Note 5 Pro (whyred), e oggi sono su OnePlus 8T — ancora modificato.

Negli stessi anni ho iniziato a fare lo stesso con il PC. Ho cambiato le RAM quando ancora 8GB sembravano tantissimi, ho installato ogni versione di Windows che usciva, e quando è arrivato Windows 10 ho cominciato a modificarlo in modo sistematico per renderlo più leggero e personale. Quella mentalità si è poi spostata su Linux, il self-hosting, l'automazione, e alla fine su un interesse concreto per la sicurezza informatica e il DevSecOps.

---

### La macchina

Il mio PC si chiama **Frankenstein** — un Lenovo IdeaPad Gaming 3 (15ACH6) modificato pezzo per pezzo nel tempo:

| Componente | Specifiche |
|---|---|
| CPU | AMD Ryzen 5 5600H |
| GPU | NVIDIA RTX 3050 |
| RAM | 32 GB Lexar DDR4 3200 MHz |
| Archiviazione | Samsung 990 Pro 1 TB (NVMe) &nbsp;+&nbsp; Crucial 1 TB (M.2 2242) |
| Display | Pannello da 165 Hz (sostituito) |
| Raffreddamento | Pasta termica Arctic MX-7 &nbsp;&middot;&nbsp; overclock leggero via MSI Afterburner |

Gira in dual boot tra **Windows 11** — alleggerito con ChrisTitus tool e Winhance, personalizzato graficamente con Windhawk e Start11 v2 — e **Pop!_OS**, dove faccio la maggior parte del lavoro. Le macchine virtuali vivono su una partizione SSD condivisa, raggiungibile da entrambi i sistemi.

---

### Il server

Una macchina separata con MX Linux, che fa da server per tutto:

- Media server con Jellyfin
- Vari servizi self-hosted in container Docker
- Server dedicato di Palworld per me, mio cognato e i miei nipoti
- Tutto esposto tramite Tailscale e un reverse proxy Nginx

---

### Con cosa lavoro

<details>
<summary>Sistemi e infrastruttura</summary>

Linux (Debian, Pop!_OS, MX Linux), Docker, Tailscale, Nginx, Windows

</details>

<details>
<summary>Scripting e automazione</summary>

Bash, Python, YAML, GitHub Actions

</details>

<details>
<summary>Sicurezza informatica</summary>

Trivy, OWASP ZAP, analisi SBOM e supply chain, pipeline DAST, FlareVM, CAINE

</details>

<details>
<summary>Homelab</summary>

Jellyfin, Sonarr, Radarr, MedicatedUSB, ambienti USB personalizzati avviabili

</details>

---

### Cosa sto studiando

- Vulnerability scanning su container e generazione di SBOM
- Integrazione di test DAST nelle pipeline CI/CD
- Gestione ZFS
- Transcoding GPU per il media server

---

### Progetti

- [Backup_script_Cyborg](https://github.com/Neniku/Backup_script_Cyborg) — script Bash per backup automatizzato con cifratura, verifica SHA256, upload ridondante su SFTP e SMB, checkpoint per riprendere in caso di interruzione e report HTML finale. Evoluzione di [Backup_script_Umano](https://github.com/Neniku/Backup_script_Umano).
- [Metodi_Di_Compressione](https://github.com/Neniku/Metodi_Di_Compressione) — appunti e slide sugli algoritmi di compressione più comuni e i loro casi d'uso reali.
- [ScanPy](https://github.com/GruppoDueMAEMA/ScanPy) — progetto di gruppo realizzato a scuola: scanner di rete Python multi-thread per host discovery, scansioni TCP/UDP e fingerprinting passivo del sistema operativo.

---

### Fuori dallo schermo

Ultimamente Kingdom Hearts e Yu-Gi-Oh si stanno prendendo buona parte del tempo libero. Ospito anche un server di Palworld per la famiglia, il che significa che passo più tempo a gestire il server che a giocare davvero.

[LinkedIn](https://www.linkedin.com/in/eleonardo-bajramovski-7599a7372/)

---

<a name="english"></a>
## English

I started taking hardware and software apart around 2012/2013, when I flashed CyanogenMod 10 on a Galaxy S3 with an Exynos processor. The camera driver wasn't compatible with custom ROMs on the Exynos variant — it simply wouldn't start. The fix came from someone who had compiled a dedicated kernel module, installed through ClockworkMod Recovery. That was the moment I realized I wanted to understand how things work, not just use them.

After the Galaxy S3 came a OnePlus One — the community phone of the era, shipped with CyanogenOS, later moved to OxygenOS, and I ended up running Tuga Power as my daily ROM. Through the OnePlus One Italia Telegram group I discovered a whole world: international XDA communities, development threads, changelogs, and the way custom ROM developers actually work. That door never closed. After the OnePlus One came a Redmi Note 3 Pro (kenzo), a Redmi Note 5 Pro (whyred), and today I'm on a OnePlus 8T — still modded.

During the same years I started doing the same with my PC. I upgraded the RAM back when 8GB felt like a lot, installed every version of Windows as it came out, and when Windows 10 arrived I began modifying it systematically to make it lighter and more personal. That mindset eventually moved into Linux, self-hosting, automation, and a concrete interest in security and DevSecOps.

---

### The machine

My PC is called **Frankenstein** — a Lenovo IdeaPad Gaming 3 (15ACH6) rebuilt piece by piece over time:

| Component | Spec |
|---|---|
| CPU | AMD Ryzen 5 5600H |
| GPU | NVIDIA RTX 3050 |
| RAM | 32 GB Lexar DDR4 3200 MHz |
| Storage | Samsung 990 Pro 1 TB (NVMe) &nbsp;+&nbsp; Crucial 1 TB (M.2 2242) |
| Display | 165 Hz panel (replaced) |
| Cooling | Arctic MX-7 thermal paste &nbsp;&middot;&nbsp; light OC via MSI Afterburner |

It dual boots **Windows 11** — stripped down with ChrisTitus tool and Winhance, customized visually with Windhawk and Start11 v2 — and **Pop!_OS**, where I do most of my actual work. Virtual machines live on a shared SSD partition, accessible from both systems.

---

### The server

A separate MX Linux machine that handles everything:

- Jellyfin media server
- Various self-hosted services in Docker containers
- Dedicated Palworld server for me, my brother-in-law and my nephews
- Everything exposed through Tailscale and an Nginx reverse proxy

---

### What I work with

<details>
<summary>Systems & infrastructure</summary>

Linux (Debian, Pop!_OS, MX Linux), Docker, Tailscale, Nginx, Windows

</details>

<details>
<summary>Scripting & automation</summary>

Bash, Python, YAML, GitHub Actions

</details>

<details>
<summary>Security</summary>

Trivy, OWASP ZAP, SBOM and supply chain analysis, DAST pipelines, FlareVM, CAINE

</details>

<details>
<summary>Homelab</summary>

Jellyfin, Sonarr, Radarr, MedicatedUSB, custom bootable USB environments

</details>

---

### Currently studying

- Container vulnerability scanning and SBOM generation
- DAST integration in CI/CD pipelines
- ZFS management
- GPU transcoding for the media server

---

### Projects

- [Backup_script_Cyborg](https://github.com/Neniku/Backup_script_Cyborg) — Bash script for automated backups with encryption, SHA256 verification, redundant upload to SFTP and SMB, checkpoint/resume on interruption, and a final HTML report. Evolution of [Backup_script_Umano](https://github.com/Neniku/Backup_script_Umano).
- [Metodi_Di_Compressione](https://github.com/Neniku/Metodi_Di_Compressione) — notes and slides on common compression algorithms and their real-world use cases.
- [ScanPy](https://github.com/GruppoDueMAEMA/ScanPy) — school group project: multi-threaded Python network scanner for host discovery, TCP/UDP scans, and passive OS fingerprinting.

---

### Outside the screen

Kingdom Hearts and Yu-Gi-Oh have been taking up most of my free time lately. I also host a Palworld server for the family, which means I spend more time managing the server than actually playing.

[LinkedIn](https://www.linkedin.com/in/eleonardo-bajramovski-7599a7372/)
