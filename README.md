# Eleonardo Bajramovski

> Junior Cybersecurity &amp; DevSecOps Specialist &nbsp;&middot;&nbsp; Linux &nbsp;&middot;&nbsp; Docker &nbsp;&middot;&nbsp; Wazuh SIEM &nbsp;&middot;&nbsp; Vasto (CH)

[Italiano](#italiano) &nbsp;&middot;&nbsp; [English](#english) &nbsp;&middot;&nbsp; [LinkedIn](https://www.linkedin.com/in/eleonardo-bajramovski/) &nbsp;&middot;&nbsp; [eleonardo.b@proton.me](mailto:eleonardo.b@proton.me)

---

<a name="italiano"></a>
## Italiano

Ho iniziato a smontare hardware e software intorno al 2012/2013, quando ho flashato CyanogenMod 10 su un Galaxy S3 con processore Exynos. Il problema era che il driver della fotocamera non era compatibile con le custom ROM sulla variante Exynos: la fotocamera semplicemente non partiva. La soluzione è arrivata grazie a qualcuno che aveva compilato un modulo kernel apposito, da installare tramite ClockworkMod Recovery. Da quel momento ho capito che mi interessava capire come funzionano le cose, non solo usarle.

Dopo il Galaxy S3 sono passato al OnePlus One, che all'epoca era il telefono della community per eccellenza: veniva venduto con CyanogenOS di serie, poi è passato alla OxygenOS, e io ho finito con Tuga Power come ROM quotidiana. Tramite il gruppo Telegram OnePlus One Italia ho scoperto un mondo: da lì sono entrato in community internazionali su XDA, ho iniziato a seguire thread di sviluppo, leggere changelog e capire come lavorano i developer di custom ROM. Quella porta non si è mai richiusa. Dopo il OnePlus One sono arrivati un Redmi Note 3 Pro (kenzo), un Redmi Note 5 Pro (whyred), e oggi sono su OnePlus 8T — ancora modificato.

Negli stessi anni ho iniziato a fare lo stesso con il PC: upgrade hardware, modifiche sistematiche a Windows 10/11 per eliminare il superfluo e poi il passaggio definitivo a Linux come unico sistema quotidiano. Quella passione per il *"capire cosa gira sotto il cofano"* si è trasformata in un percorso strutturato: un biennio di specializzazione in **Cybersecurity**, un tirocinio intensivo sul mondo **DevSecOps** (container hardening, pipeline CI/CD sicure, Kubernetes, Wazuh SIEM) e un homelab su Debian che oggi ospita oltre venti container in produzione per la mia famiglia e per un'attività commerciale reale.

---

### La macchina (Workstation)

Il mio PC principale si chiama **Frankenstein** — un Lenovo IdeaPad Gaming 3 (15ACH6) modificato pezzo per pezzo nel tempo:

| Componente | Specifiche |
|---|---|
| Sistema Operativo | **GarudaOS (Arch Linux)** &nbsp;&middot;&nbsp; kernel `CachyOS` |
| CPU | AMD Ryzen 5 5600H |
| GPU | NVIDIA RTX 3050 |
| RAM | 32 GB Lexar DDR4 3200 MHz |
| Archiviazione | Samsung 990 Pro 1 TB (NVMe) &nbsp;+&nbsp; Crucial 1 TB (M.2 2242) |
| Display | Pannello da 165 Hz (sostituito) |
| Raffreddamento | Pasta termica Arctic MX-7 |

Oggi gira interamente su **GarudaOS (Arch Linux, kernel CachyOS)**: con le ottimizzazioni del kernel CachyOS va talmente bene che non c'è nemmeno più bisogno di fare overclock manuale, e ho abbandonato definitivamente il dual boot con Windows (che ormai tengo solo in macchine virtuali isolate quando serve per laboratori o analisi).

---

### Il server (Home Server &amp; NAS)

Una macchina dedicata con **Debian 13 (Trixie)** che ospita l'intera infrastruttura self-hosted (documentata in dettaglio in [homeserver-infrastructure](https://github.com/Neniku/homeserver-infrastructure)):

| Componente | Specifiche |
|---|---|
| Sistema Operativo | **Debian GNU/Linux 13 (Trixie)** &nbsp;&middot;&nbsp; kernel `6.12` |
| CPU &amp; iGPU | Intel Core i3-12100 (12th Gen) &nbsp;&middot;&nbsp; Intel UHD Graphics 730 (QuickSync) |
| RAM | 16 GB DDR4 |
| Storage (5 dischi / ~8.1 TB) | `110 GB` SSD (OS, Docker, DB) &nbsp;&middot;&nbsp; `293 GB` SSD (`/cache` transcoding/download) &nbsp;&middot;&nbsp; `2x 3.6 TB` HDD (`/data_film`, `/data_serie`) &nbsp;&middot;&nbsp; `458 GB` HDD (`/backup`) |

Sopra ci girano **22 container Docker** divisi in stack modulari sotto `/opt/appdata/`:

- **Sicurezza &amp; Infrastruttura:** nessuna porta esposta su Internet (accesso solo via VPN mesh Zero Trust **Tailscale**), reverse proxy **Nginx** isolati, password manager **Vaultwarden**, **docker-socket-proxy** (per non esporre `/var/run/docker.sock` direttamente a **Portainer** e **Homepage**) e un servizio custom `docker-alerter` per il monitoraggio dello stato dei container.
- **Gestionale Attività Commerciale:** stack self-hosted (**FastAPI**, **Next.js**, **Nginx** e **PostgreSQL 16** isolato su rete dedicata `db-net` con container read-only, `tmpfs` e `no-new-privileges`).
- **Media &amp; Transcoding Hardware:** **Jellyfin** e cluster **Tdarr** (server + nodo) con transcoding hardware via Intel QuickSync sulla UHD 730, affiancati da Jellyseerr, Sonarr, Radarr, Prowlarr, Jackett, Tracearr, qBittorrent e FlareSolverr (con meccanismo `.mounted` sui dischi fisici per bloccare l'avvio dei container se un HDD non è montato).
- **Backup &amp; Continuità:** backup notturni cifrati e automatizzati tramite **Systemd Timers** (`edicola87-backup.timer` e `vaultwarden-backup.timer`) sul disco dedicato `/backup`, più server dedicato di **Palworld** per la famiglia.

---

### Con cosa lavoro

| Area | Strumenti e Tecnologie |
|---|---|
| **Sistemi &amp; Infrastruttura** | Linux (GarudaOS / Arch Linux, Debian, Ubuntu), Docker, Docker Compose, Podman, Kubernetes, Helm, Tailscale, Nginx, Systemd, VirtualBox, VMware |
| **Sicurezza &amp; Monitoring** | Wazuh SIEM (agenti, FIM, regole di rilevamento custom), Hadolint, Gitleaks, Trivy (SARIF/SBOM), Semgrep, OWASP ZAP, Nmap, Wireshark, tcpdump, Burp Suite, Metasploit, REMnux, FLARE VM |
| **Scripting, CI/CD &amp; DB** | Bash, Python, PowerShell, GitHub Actions, Git, PostgreSQL, YAML |
| **Self-Hosting &amp; Homelab** | Vaultwarden, docker-socket-proxy, Portainer, Homepage, Jellyfin, Tdarr (QuickSync GPU transcoding), stack *Arr, MedicatedUSB |

---

### Cosa sto studiando

- Preparazione certificazione **CompTIA CySA+ (Cybersecurity Analyst)**
- Detection engineering, analisi log e regole custom su **Wazuh SIEM**
- Vulnerability scanning su container, generazione di SBOM e test SAST/DAST nelle pipeline CI/CD

---

### Progetti

- [homeserver-infrastructure](https://github.com/Neniku/homeserver-infrastructure) — architettura completa del mio Home Server su Debian 13: 22 container in stack Docker Compose modulari, rete Zero Trust con Tailscale (zero porte esposte), `docker-socket-proxy`, PostgreSQL isolato e hardened, transcoding GPU e backup notturni cifrati con Systemd Timers.
- [devsecops-journey](https://github.com/Neniku/devsecops-journey) — percorso pratico intensivo su Docker, container hardening (`cap_drop`, `no-new-privileges`, Docker Secrets), pipeline GitHub Actions (Hadolint, Gitleaks, Trivy con report SARIF), Kubernetes, Helm, Wazuh SIEM e Incident Response.
- [Backup_script_Cyborg](https://github.com/Neniku/Backup_script_Cyborg) — suite Bash CLI/GUI (Zenity) per backup automatizzato con cifratura AES-256, verifica SHA-256, upload ridondante su SFTP e SMB, checkpoint/resume e report HTML finale. Evoluzione di [Backup_script_Umano](https://github.com/Neniku/Backup_script_Umano).
- [android-adb-exploit-research](https://github.com/Neniku/android-adb-exploit-research) — PoC didattica in ambiente di laboratorio autorizzato sull'esposizione della porta ADB (TCP 5555) su dispositivi Android/IoT, con analisi delle contromisure e ripristino del dispositivo.
- [Metodi_Di_Compressione](https://github.com/Neniku/Metodi_Di_Compressione) — appunti e slide sugli algoritmi di compressione più comuni e i loro casi d'uso reali.
- [ScanPy](https://github.com/GruppoDueMAEMA/ScanPy) — progetto di gruppo: scanner di rete Python multi-thread per host discovery, scansioni TCP/UDP e fingerprinting passivo del sistema operativo.

---

### Fuori dallo schermo

Ultimamente Kingdom Hearts e Yu-Gi-Oh si stanno prendendo buona parte del tempo libero. Ospito anche un server di Palworld per la famiglia, il che significa che passo più tempo a gestire il server che a giocare davvero.

[LinkedIn](https://www.linkedin.com/in/eleonardo-bajramovski/) &nbsp;&middot;&nbsp; [eleonardo.b@proton.me](mailto:eleonardo.b@proton.me)

---

<a name="english"></a>
## English

I started taking hardware and software apart around 2012/2013, when I flashed CyanogenMod 10 on a Galaxy S3 with an Exynos processor. The camera driver wasn't compatible with custom ROMs on the Exynos variant — it simply wouldn't start. The fix came from someone who had compiled a dedicated kernel module, installed through ClockworkMod Recovery. That was the moment I realized I wanted to understand how things work, not just use them.

After the Galaxy S3 came a OnePlus One — the community phone of the era, shipped with CyanogenOS, later moved to OxygenOS, and I ended up running Tuga Power as my daily ROM. Through the OnePlus One Italia Telegram group I discovered a whole world: international XDA communities, development threads, changelogs, and the way custom ROM developers actually work. That door never closed. After the OnePlus One came a Redmi Note 3 Pro (kenzo), a Redmi Note 5 Pro (whyred), and today I'm on a OnePlus 8T — still modded.

During the same years I started doing the same with my PC: hardware upgrades, stripping down Windows 10/11, and eventually switching permanently to Linux as my sole daily driver. That curiosity for *"understanding what happens under the hood"* grew into a structured path: a two-year specialization in **Cybersecurity**, an intensive **DevSecOps** internship (container hardening, secure CI/CD pipelines, Kubernetes, Wazuh SIEM), and a Debian home server running 22 containers in production for my family and a real retail business.

---

### The machine (Workstation)

My main PC is called **Frankenstein** — a Lenovo IdeaPad Gaming 3 (15ACH6) rebuilt piece by piece over time:

| Component | Spec |
|---|---|
| Operating System | **GarudaOS (Arch Linux)** &nbsp;&middot;&nbsp; `CachyOS` kernel |
| CPU | AMD Ryzen 5 5600H |
| GPU | NVIDIA RTX 3050 |
| RAM | 32 GB Lexar DDR4 3200 MHz |
| Storage | Samsung 990 Pro 1 TB (NVMe) &nbsp;+&nbsp; Crucial 1 TB (M.2 2242) |
| Display | 165 Hz panel (replaced) |
| Cooling | Arctic MX-7 thermal paste |

It now runs entirely on **GarudaOS (Arch Linux, CachyOS kernel)**: thanks to the CachyOS kernel optimizations it runs so smoothly that manual overclocking isn't needed anymore, and I dropped the Windows dual boot for good (Windows now only lives inside isolated virtual machines when needed for labs or analysis).

---

### The server (Home Server &amp; NAS)

A dedicated **Debian 13 (Trixie)** machine running my self-hosted infrastructure (documented in detail in [homeserver-infrastructure](https://github.com/Neniku/homeserver-infrastructure)):

| Component | Spec |
|---|---|
| Operating System | **Debian GNU/Linux 13 (Trixie)** &nbsp;&middot;&nbsp; kernel `6.12` |
| CPU &amp; iGPU | Intel Core i3-12100 (12th Gen) &nbsp;&middot;&nbsp; Intel UHD Graphics 730 (QuickSync) |
| RAM | 16 GB DDR4 |
| Storage (5 drives / ~8.1 TB) | `110 GB` SSD (OS, Docker, DB) &nbsp;&middot;&nbsp; `293 GB` SSD (`/cache` transcoding/downloads) &nbsp;&middot;&nbsp; `2x 3.6 TB` HDD (`/data_film`, `/data_serie`) &nbsp;&middot;&nbsp; `458 GB` HDD (`/backup`) |

It runs **22 Docker containers** organized into modular stacks under `/opt/appdata/`:

- **Security &amp; Infrastructure:** zero ports exposed to the internet (accessible exclusively via **Tailscale** Zero Trust mesh VPN), isolated **Nginx** reverse proxies, **Vaultwarden** password manager, **docker-socket-proxy** (preventing direct `/var/run/docker.sock` exposure to **Portainer** and **Homepage**), and a custom `docker-alerter` service monitoring container health.
- **Retail Business Management Stack:** self-hosted stack (**FastAPI**, **Next.js**, **Nginx**, and **PostgreSQL 16** isolated on a dedicated `db-net` network with a read-only root filesystem, `tmpfs`, and `no-new-privileges`).
- **Media &amp; Hardware Transcoding:** **Jellyfin** and a **Tdarr** cluster (server + node) using Intel QuickSync hardware transcoding on the UHD 730, alongside Jellyseerr, Sonarr, Radarr, Prowlarr, Jackett, Tracearr, qBittorrent, and FlareSolverr (protected by a `.mounted` guard file mechanism that prevents containers from starting if a physical drive fails to mount).
- **Backups &amp; Continuity:** automated encrypted nightly backups scheduled via **Systemd Timers** (`edicola87-backup.timer` and `vaultwarden-backup.timer`) onto the dedicated `/backup` drive, plus a dedicated family **Palworld** server.

---

### What I work with

| Area | Tools &amp; Technologies |
|---|---|
| **Systems &amp; Infrastructure** | Linux (GarudaOS / Arch Linux, Debian, Ubuntu), Docker, Docker Compose, Podman, Kubernetes, Helm, Tailscale, Nginx, Systemd, VirtualBox, VMware |
| **Security &amp; Monitoring** | Wazuh SIEM (agents, FIM, custom detection rules), Hadolint, Gitleaks, Trivy (SARIF/SBOM), Semgrep, OWASP ZAP, Nmap, Wireshark, tcpdump, Burp Suite, Metasploit, REMnux, FLARE VM |
| **Scripting, CI/CD &amp; DB** | Bash, Python, PowerShell, GitHub Actions, Git, PostgreSQL, YAML |
| **Self-Hosting &amp; Homelab** | Vaultwarden, docker-socket-proxy, Portainer, Homepage, Jellyfin, Tdarr (QuickSync GPU transcoding), *Arr stack, MedicatedUSB |

---

### Currently studying

- Preparing for the **CompTIA CySA+ (Cybersecurity Analyst)** certification
- Detection engineering, log analysis, and custom rules on **Wazuh SIEM**
- Container vulnerability scanning, SBOM generation, and SAST/DAST integration in CI/CD pipelines

---

### Projects

- [homeserver-infrastructure](https://github.com/Neniku/homeserver-infrastructure) — complete architecture of my Debian 13 Home Server: 22 containers in modular Docker Compose stacks, Zero Trust networking with Tailscale (zero exposed ports), `docker-socket-proxy`, isolated and hardened PostgreSQL, GPU transcoding, and encrypted nightly backups via Systemd Timers.
- [devsecops-journey](https://github.com/Neniku/devsecops-journey) — intensive hands-on track covering Docker, container hardening (`cap_drop`, `no-new-privileges`, Docker Secrets), GitHub Actions pipelines (Hadolint, Gitleaks, Trivy with SARIF reports), Kubernetes, Helm, Wazuh SIEM, and Incident Response.
- [Backup_script_Cyborg](https://github.com/Neniku/Backup_script_Cyborg) — Bash CLI/GUI (Zenity) suite for automated backups with AES-256 encryption, SHA-256 verification, redundant upload to SFTP and SMB, checkpoint/resume on interruption, and a final HTML report. Evolution of [Backup_script_Umano](https://github.com/Neniku/Backup_script_Umano).
- [android-adb-exploit-research](https://github.com/Neniku/android-adb-exploit-research) — educational PoC conducted in an authorized lab environment on exposed ADB interfaces (TCP 5555) on Android/IoT devices, including countermeasure analysis and device restoration.
- [Metodi_Di_Compressione](https://github.com/Neniku/Metodi_Di_Compressione) — notes and slides on common compression algorithms and their real-world use cases.
- [ScanPy](https://github.com/GruppoDueMAEMA/ScanPy) — school group project: multi-threaded Python network scanner for host discovery, TCP/UDP scans, and passive OS fingerprinting.

---

### Outside the screen

Kingdom Hearts and Yu-Gi-Oh have been taking up most of my free time lately. I also host a Palworld server for the family, which means I spend more time managing the server than actually playing.

[LinkedIn](https://www.linkedin.com/in/eleonardo-bajramovski/) &nbsp;&middot;&nbsp; [eleonardo.b@proton.me](mailto:eleonardo.b@proton.me)
