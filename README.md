# Eleonardo Bajramovski

> Junior Cybersecurity &amp; DevSecOps Specialist &nbsp;&middot;&nbsp; Linux &nbsp;&middot;&nbsp; Docker &nbsp;&middot;&nbsp; Wazuh SIEM &nbsp;&middot;&nbsp; Vasto (CH)

[Italiano](#italiano) &nbsp;&middot;&nbsp; [English](#english)

---

<a name="italiano"></a>
## Italiano

Ho iniziato a smontare hardware e software intorno al 2012/2013, quando ho flashato CyanogenMod 10 su un Galaxy S3 con processore Exynos. Il problema era che il driver della fotocamera non era compatibile con le custom ROM sulla variante Exynos: la fotocamera semplicemente non partiva. La soluzione è arrivata grazie a qualcuno che aveva compilato un modulo kernel apposito, da installare tramite ClockworkMod Recovery. Da quel momento ho capito che mi interessava capire come funzionano le cose, non solo usarle.

Dopo il Galaxy S3 sono passato al OnePlus One, che all'epoca era il telefono della community per eccellenza: veniva venduto con CyanogenOS di serie, poi è passato alla OxygenOS, e io ho finito con Tuga Power come ROM quotidiana. Tramite il gruppo Telegram OnePlus One Italia ho scoperto un mondo: da lì sono entrato in community internazionali su XDA, ho iniziato a seguire thread di sviluppo, leggere changelog e capire come lavorano i developer di custom ROM. Quella porta non si è mai richiusa. Dopo il OnePlus One sono arrivati un Redmi Note 3 Pro (kenzo), un Redmi Note 5 Pro (whyred), e oggi sono su OnePlus 8T — ancora modificato.

Negli stessi anni ho iniziato a fare lo stesso con il PC. Ho cambiato le RAM quando ancora 8GB sembravano tantissimi, ho installato ogni versione di Windows che usciva, e quando è arrivato Windows 10 ho cominciato a modificarlo in modo sistematico per renderlo più leggero e personale. Quella mentalità si è poi spostata su Linux, il self-hosting, l'automazione, e alla fine su un percorso concreto nella sicurezza informatica e nel DevSecOps.

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

Il mio daily driver ormai è **GarudaOS (Arch Linux, kernel CachyOS)**, dove faccio tutto il lavoro quotidiano, affiancato in dual boot da una partizione **Windows 11** alleggerita (ChrisTitus tool, Winhance, Windhawk, Start11 v2). Le macchine virtuali vivono su una partizione SSD condivisa, raggiungibile da entrambi i sistemi.

---

### Il server

Una macchina separata con **Debian**, che ospita l'intera infrastruttura self-hosted (documentata in [homeserver-infrastructure](https://github.com/Neniku/homeserver-infrastructure)):

- Stack modulari in Docker Compose con database PostgreSQL su rete isolata e container hardened
- Media server con Jellyfin e servizi gestionali per l'attività commerciale di famiglia
- Server dedicato di Palworld per me, mio cognato e i miei nipoti
- Nessuna porta esposta su Internet: accesso esclusivamente tramite VPN mesh Zero Trust (Tailscale), reverse proxy Nginx e backup notturni cifrati con Systemd Timers

---

### Con cosa lavoro

<details>
<summary>Sistemi e infrastruttura</summary>

Linux (GarudaOS / Arch Linux, Debian, Ubuntu), Docker, Docker Compose, Podman, Kubernetes, Helm, Tailscale, Nginx, Windows

</details>

<details>
<summary>Scripting e automazione</summary>

Bash, Python, PowerShell, YAML, GitHub Actions

</details>

<details>
<summary>Sicurezza informatica</summary>

Wazuh SIEM (FIM, custom detection rules), Hadolint, Gitleaks, Trivy, Semgrep, OWASP ZAP, Nmap, Wireshark, tcpdump, Burp Suite, Metasploit, REMnux, FLARE VM, CAINE

</details>

<details>
<summary>Homelab</summary>

Jellyfin, Sonarr, Radarr, PostgreSQL, MedicatedUSB, ambienti USB personalizzati avviabili

</details>

---

### Cosa sto studiando

- Preparazione certificazione **CompTIA CySA+ (Cybersecurity Analyst)**
- Detection engineering e regole custom su **Wazuh SIEM**
- Vulnerability scanning su container, generazione di SBOM e test SAST/DAST nelle pipeline CI/CD
- Gestione ZFS e transcoding GPU per il media server

---

### Progetti

- [homeserver-infrastructure](https://github.com/Neniku/homeserver-infrastructure) — architettura completa del mio Home Server su Debian: stack Docker Compose modulari, rete Zero Trust con Tailscale (zero porte esposte), PostgreSQL isolato e hardened, monitoraggio custom e backup notturni cifrati con Systemd Timers.
- [devsecops-journey](https://github.com/Neniku/devsecops-journey) — percorso pratico intensivo su Docker, container hardening (`cap_drop`, `no-new-privileges`, Docker Secrets), pipeline GitHub Actions (Hadolint, Gitleaks, Trivy con report SARIF), Kubernetes, Helm, Wazuh SIEM e Incident Response.
- [Backup_script_Cyborg](https://github.com/Neniku/Backup_script_Cyborg) — suite Bash CLI/GUI (Zenity) per backup automatizzato con cifratura AES-256, verifica SHA-256, upload ridondante su SFTP e SMB, checkpoint/resume e report HTML finale. Evoluzione di [Backup_script_Umano](https://github.com/Neniku/Backup_script_Umano).
- [android-adb-exploit-research](https://github.com/Neniku/android-adb-exploit-research) — PoC didattica in ambiente di laboratorio autorizzato sull'esposizione della porta ADB (TCP 5555) su dispositivi Android/IoT, con analisi delle contromisure e ripristino del dispositivo.
- [Metodi_Di_Compressione](https://github.com/Neniku/Metodi_Di_Compressione) — appunti e slide sugli algoritmi di compressione più comuni e i loro casi d'uso reali.
- [ScanPy](https://github.com/GruppoDueMAEMA/ScanPy) — progetto di gruppo: scanner di rete Python multi-thread per host discovery, scansioni TCP/UDP e fingerprinting passivo del sistema operativo.

---

### Fuori dallo schermo

Ultimamente Kingdom Hearts e Yu-Gi-Oh si stanno prendendo buona parte del tempo libero. Ospito anche un server di Palworld per la famiglia, il che significa che passo più tempo a gestire il server che a giocare davvero.

[LinkedIn](https://www.linkedin.com/in/eleonardo-bajramovski/)

---

<a name="english"></a>
## English

I started taking hardware and software apart around 2012/2013, when I flashed CyanogenMod 10 on a Galaxy S3 with an Exynos processor. The camera driver wasn't compatible with custom ROMs on the Exynos variant — it simply wouldn't start. The fix came from someone who had compiled a dedicated kernel module, installed through ClockworkMod Recovery. That was the moment I realized I wanted to understand how things work, not just use them.

After the Galaxy S3 came a OnePlus One — the community phone of the era, shipped with CyanogenOS, later moved to OxygenOS, and I ended up running Tuga Power as my daily ROM. Through the OnePlus One Italia Telegram group I discovered a whole world: international XDA communities, development threads, changelogs, and the way custom ROM developers actually work. That door never closed. After the OnePlus One came a Redmi Note 3 Pro (kenzo), a Redmi Note 5 Pro (whyred), and today I'm on a OnePlus 8T — still modded.

During the same years I started doing the same with my PC. I upgraded the RAM back when 8GB felt like a lot, installed every version of Windows as it came out, and when Windows 10 arrived I began modifying it systematically to make it lighter and more personal. That mindset eventually moved into Linux, self-hosting, automation, and a concrete path in cybersecurity and DevSecOps.

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

My daily driver is now **GarudaOS (Arch Linux, CachyOS kernel)**, where I do all of my day-to-day work, dual-booted alongside a stripped-down **Windows 11** partition (ChrisTitus tool, Winhance, Windhawk, Start11 v2). Virtual machines live on a shared SSD partition, accessible from both systems.

---

### The server

A separate **Debian** machine running my self-hosted infrastructure (documented in [homeserver-infrastructure](https://github.com/Neniku/homeserver-infrastructure)):

- Modular Docker Compose stacks with an isolated, hardened PostgreSQL database
- Jellyfin media server and internal services for our family business
- Dedicated Palworld server for me, my brother-in-law and my nephews
- Zero exposed ports: everything accessed through a Zero Trust mesh VPN (Tailscale), Nginx reverse proxy, and encrypted nightly backups via Systemd Timers

---

### What I work with

<details>
<summary>Systems &amp; infrastructure</summary>

Linux (GarudaOS / Arch Linux, Debian, Ubuntu), Docker, Docker Compose, Podman, Kubernetes, Helm, Tailscale, Nginx, Windows

</details>

<details>
<summary>Scripting &amp; automation</summary>

Bash, Python, PowerShell, YAML, GitHub Actions

</details>

<details>
<summary>Security</summary>

Wazuh SIEM (FIM, custom detection rules), Hadolint, Gitleaks, Trivy, Semgrep, OWASP ZAP, Nmap, Wireshark, tcpdump, Burp Suite, Metasploit, REMnux, FLARE VM, CAINE

</details>

<details>
<summary>Homelab</summary>

Jellyfin, Sonarr, Radarr, PostgreSQL, MedicatedUSB, custom bootable USB environments

</details>

---

### Currently studying

- Preparing for the **CompTIA CySA+ (Cybersecurity Analyst)** certification
- Detection engineering and custom rules on **Wazuh SIEM**
- Container vulnerability scanning, SBOM generation, and SAST/DAST integration in CI/CD pipelines
- ZFS management and GPU transcoding for the media server

---

### Projects

- [homeserver-infrastructure](https://github.com/Neniku/homeserver-infrastructure) — complete architecture of my Debian Home Server: modular Docker Compose stacks, Zero Trust networking with Tailscale (zero exposed ports), isolated and hardened PostgreSQL, custom monitoring, and encrypted nightly backups via Systemd Timers.
- [devsecops-journey](https://github.com/Neniku/devsecops-journey) — intensive hands-on track covering Docker, container hardening (`cap_drop`, `no-new-privileges`, Docker Secrets), GitHub Actions pipelines (Hadolint, Gitleaks, Trivy with SARIF reports), Kubernetes, Helm, Wazuh SIEM, and Incident Response.
- [Backup_script_Cyborg](https://github.com/Neniku/Backup_script_Cyborg) — Bash CLI/GUI (Zenity) suite for automated backups with AES-256 encryption, SHA-256 verification, redundant upload to SFTP and SMB, checkpoint/resume on interruption, and a final HTML report. Evolution of [Backup_script_Umano](https://github.com/Neniku/Backup_script_Umano).
- [android-adb-exploit-research](https://github.com/Neniku/android-adb-exploit-research) — educational PoC conducted in an authorized lab environment on exposed ADB interfaces (TCP 5555) on Android/IoT devices, including countermeasure analysis and device restoration.
- [Metodi_Di_Compressione](https://github.com/Neniku/Metodi_Di_Compressione) — notes and slides on common compression algorithms and their real-world use cases.
- [ScanPy](https://github.com/GruppoDueMAEMA/ScanPy) — school group project: multi-threaded Python network scanner for host discovery, TCP/UDP scans, and passive OS fingerprinting.

---

### Outside the screen

Kingdom Hearts and Yu-Gi-Oh have been taking up most of my free time lately. I also host a Palworld server for the family, which means I spend more time managing the server than actually playing.

[LinkedIn](https://www.linkedin.com/in/eleonardo-bajramovski/)
