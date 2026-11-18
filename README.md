# Eleonardo Bajramovski

> Junior Cybersecurity &amp; DevSecOps Specialist &nbsp;&middot;&nbsp; Linux &nbsp;&middot;&nbsp; Docker &nbsp;&middot;&nbsp; Wazuh SIEM &nbsp;&middot;&nbsp; Vasto (CH)

[Italiano](#italiano) &nbsp;&middot;&nbsp; [English](#english) &nbsp;&middot;&nbsp; [LinkedIn](https://www.linkedin.com/in/eleonardo-bajramovski/) &nbsp;&middot;&nbsp; [eleonardo.b@proton.me](mailto:eleonardo.b@proton.me)

---

<a name="italiano"></a>
## Italiano

Ho iniziato a smontare hardware e software intorno al 2012/2013, quando ho flashato CyanogenMod 10 su un Galaxy S3 con processore Exynos. Il problema era che il driver della fotocamera non era compatibile con le custom ROM sulla variante Exynos: la fotocamera semplicemente non partiva. La soluzione è arrivata grazie a qualcuno che aveva compilato un modulo kernel apposito, da installare tramite ClockworkMod Recovery. Da quel momento ho capito che mi interessava capire come funzionano le cose, non solo usarle.

Dopo il Galaxy S3 sono passato al OnePlus One, che all'epoca era il telefono della community per eccellenza: veniva venduto con CyanogenOS di serie, poi è passato alla OxygenOS, e io ho finito con Tuga Power come ROM quotidiana. Tramite il gruppo Telegram OnePlus One Italia ho scoperto un mondo: da lì sono entrato in community internazionali su XDA, ho iniziato a seguire thread di sviluppo, leggere changelog e capire come lavorano i developer di custom ROM. Quella porta non si è mai richiusa. Dopo il OnePlus One sono arrivati un Redmi Note 3 Pro (kenzo), un Redmi Note 5 Pro (whyred), e oggi sono su OnePlus 8T — ancora modificato.

Negli stessi anni ho iniziato a fare lo stesso con il PC: upgrade hardware, modifiche sistematiche al sistema operativo per eliminare il superfluo e poi il passaggio definitivo a Linux come unico ambiente quotidiano. Quella passione per il *"capire cosa gira sotto il cofano"* si è trasformata in un percorso strutturato: un biennio di specializzazione in **Cybersecurity**, un tirocinio intensivo sul mondo **DevSecOps** (container hardening, pipeline CI/CD sicure, Kubernetes, Wazuh SIEM) e un Home Server su Debian che gestisco quotidianamente.

---

### La macchina (Workstation)

Il mio PC principale si chiama **Frankenstein** — un Lenovo IdeaPad Gaming 3 (15ACH6) aggiornato pezzo per pezzo nel tempo:

- **Sistema Operativo:** **GarudaOS (Arch Linux)** con kernel `CachyOS`
- **CPU:** AMD Ryzen 5 5600H
- **GPU:** NVIDIA RTX 3050
- **RAM:** 32 GB Lexar DDR4 3200 MHz
- **Archiviazione:** Samsung 990 Pro 1 TB (NVMe) + Crucial 1 TB (M.2 2242)
- **Display &amp; Raffreddamento:** Pannello da 165 Hz (sostituito) e pasta termica Arctic MX-7

Gira esclusivamente su **GarudaOS (Arch Linux, kernel CachyOS)** come unico sistema operativo: le ottimizzazioni del kernel CachyOS garantiscono prestazioni e reattività eccellenti out-of-the-box, mentre i laboratori di analisi girano all'interno di macchine virtuali isolate.

---

### Il server (Home Server &amp; NAS)

Una macchina dedicata con **Debian 13 (Trixie)** (Intel Core i3-12100 con iGPU UHD 730 QuickSync, 16 GB di RAM e 5 dischi dedicati tra SSD per OS/cache e HDD per storage e backup per ~8.1 TB totali), documentata in [homeserver-infrastructure](https://github.com/Neniku/homeserver-infrastructure):

- **Sicurezza &amp; Infrastruttura:** nessuna porta esposta su Internet (accesso solo tramite VPN mesh Zero Trust **Tailscale**), reverse proxy **Nginx**, password manager **Vaultwarden**, **docker-socket-proxy** (per non esporre `/var/run/docker.sock` direttamente a **Portainer** e **Homepage**) e un servizio custom `docker-alerter` per il monitoraggio dello stato dei container.
- **Media &amp; Transcoding Hardware:** **Jellyfin** e cluster **Tdarr** (server + nodo) con transcoding hardware via Intel QuickSync sulla UHD 730, affiancati dallo stack *Arr (Jellyseerr, Sonarr, Radarr, Prowlarr, Jackett, Tracearr, qBittorrent, FlareSolverr) protetto dal meccanismo `.mounted` sui dischi fisici per impedire l'avvio dei container se un HDD non è montato.
- **Backup &amp; Servizi:** backup notturni cifrati e automatizzati tramite **Systemd Timers** (`vaultwarden-backup.timer` e `dpkg-db-backup.timer`) sul disco dedicato `/backup`, più server dedicato di **Palworld** per la famiglia.

---

### Con cosa lavoro

- **Sistemi &amp; Infrastruttura:** Linux (GarudaOS / Arch Linux, Debian, Ubuntu), Docker, Docker Compose, Podman, Kubernetes, Helm, Tailscale, Nginx, Systemd, VirtualBox, VMware
- **Sicurezza &amp; Monitoring:** Wazuh SIEM (agenti, FIM, regole di rilevamento custom), Hadolint, Gitleaks, Trivy (SARIF/SBOM), Semgrep, OWASP ZAP, Nmap, Wireshark, tcpdump, Burp Suite, Metasploit, REMnux, FLARE VM, CAINE
- **Scripting &amp; CI/CD:** Bash, Python, PowerShell, GitHub Actions, Git, YAML
- **Self-Hosting &amp; Homelab:** Vaultwarden, docker-socket-proxy, Portainer, Homepage, Jellyfin, Tdarr (QuickSync GPU transcoding), stack *Arr, MedicatedUSB

---

### Cosa sto studiando

- Preparazione certificazione **CompTIA CySA+ (Cybersecurity Analyst)**
- Detection engineering, analisi log e regole custom su **Wazuh SIEM**
- Vulnerability scanning su container, generazione di SBOM e test SAST/DAST nelle pipeline CI/CD

---

### Progetti

- [homeserver-infrastructure](https://github.com/Neniku/homeserver-infrastructure) — architettura completa del mio Home Server su Debian 13: stack Docker Compose modulari, rete Zero Trust con Tailscale (zero porte esposte), `docker-socket-proxy`, Vaultwarden, transcoding GPU e backup notturni cifrati con Systemd Timers.
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

During the same years I started doing the same with my PC: hardware upgrades, stripping down the OS, and eventually switching permanently to Linux as my sole daily environment. That curiosity for *"understanding what happens under the hood"* grew into a structured path: a two-year specialization in **Cybersecurity**, an intensive **DevSecOps** internship (container hardening, secure CI/CD pipelines, Kubernetes, Wazuh SIEM), and a Debian Home Server that I manage daily.

---

### The machine (Workstation)

My main PC is called **Frankenstein** — a Lenovo IdeaPad Gaming 3 (15ACH6) upgraded piece by piece over time:

- **Operating System:** **GarudaOS (Arch Linux)** with `CachyOS` kernel
- **CPU:** AMD Ryzen 5 5600H
- **GPU:** NVIDIA RTX 3050
- **RAM:** 32 GB Lexar DDR4 3200 MHz
- **Storage:** Samsung 990 Pro 1 TB (NVMe) + Crucial 1 TB (M.2 2242)
- **Display &amp; Cooling:** 165 Hz panel (replaced) and Arctic MX-7 thermal paste

It runs exclusively on **GarudaOS (Arch Linux, CachyOS kernel)** as its sole operating system: the CachyOS kernel optimizations deliver great performance and responsiveness out of the box, while analysis labs run inside isolated virtual machines.

---

### The server (Home Server &amp; NAS)

A dedicated **Debian 13 (Trixie)** machine (Intel Core i3-12100 with UHD 730 QuickSync iGPU, 16 GB RAM, and 5 dedicated drives across OS/cache SSDs and storage/backup HDDs totaling ~8.1 TB), documented in [homeserver-infrastructure](https://github.com/Neniku/homeserver-infrastructure):

- **Security &amp; Infrastructure:** zero ports exposed to the internet (accessible exclusively via **Tailscale** Zero Trust mesh VPN), **Nginx** reverse proxy, **Vaultwarden** password manager, **docker-socket-proxy** (preventing direct `/var/run/docker.sock` exposure to **Portainer** and **Homepage**), and a custom `docker-alerter` service monitoring container health.
- **Media &amp; Hardware Transcoding:** **Jellyfin** and a **Tdarr** cluster (server + node) using Intel QuickSync hardware transcoding on the UHD 730, alongside the *Arr stack (Jellyseerr, Sonarr, Radarr, Prowlarr, Jackett, Tracearr, qBittorrent, FlareSolverr) protected by a `.mounted` guard file mechanism that prevents containers from starting if a physical drive fails to mount.
- **Backups &amp; Services:** automated encrypted nightly backups scheduled via **Systemd Timers** (`vaultwarden-backup.timer` and `dpkg-db-backup.timer`) onto the dedicated `/backup` drive, plus a dedicated family **Palworld** server.

---

### What I work with

- **Systems &amp; Infrastructure:** Linux (GarudaOS / Arch Linux, Debian, Ubuntu), Docker, Docker Compose, Podman, Kubernetes, Helm, Tailscale, Nginx, Systemd, VirtualBox, VMware
- **Security &amp; Monitoring:** Wazuh SIEM (agents, FIM, custom detection rules), Hadolint, Gitleaks, Trivy (SARIF/SBOM), Semgrep, OWASP ZAP, Nmap, Wireshark, tcpdump, Burp Suite, Metasploit, REMnux, FLARE VM, CAINE
- **Scripting &amp; CI/CD:** Bash, Python, PowerShell, GitHub Actions, Git, YAML
- **Self-Hosting &amp; Homelab:** Vaultwarden, docker-socket-proxy, Portainer, Homepage, Jellyfin, Tdarr (QuickSync GPU transcoding), *Arr stack, MedicatedUSB

---

### Currently studying

- Preparing for the **CompTIA CySA+ (Cybersecurity Analyst)** certification
- Detection engineering, log analysis, and custom rules on **Wazuh SIEM**
- Container vulnerability scanning, SBOM generation, and SAST/DAST integration in CI/CD pipelines

---

### Projects

- [homeserver-infrastructure](https://github.com/Neniku/homeserver-infrastructure) — complete architecture of my Debian 13 Home Server: modular Docker Compose stacks, Zero Trust networking with Tailscale (zero exposed ports), `docker-socket-proxy`, Vaultwarden, GPU transcoding, and encrypted nightly backups via Systemd Timers.
- [devsecops-journey](https://github.com/Neniku/devsecops-journey) — intensive hands-on track covering Docker, container hardening (`cap_drop`, `no-new-privileges`, Docker Secrets), GitHub Actions pipelines (Hadolint, Gitleaks, Trivy with SARIF reports), Kubernetes, Helm, Wazuh SIEM, and Incident Response.
- [Backup_script_Cyborg](https://github.com/Neniku/Backup_script_Cyborg) — Bash CLI/GUI (Zenity) suite for automated backups with AES-256 encryption, SHA-256 verification, redundant upload to SFTP and SMB, checkpoint/resume on interruption, and a final HTML report. Evolution of [Backup_script_Umano](https://github.com/Neniku/Backup_script_Umano).
- [android-adb-exploit-research](https://github.com/Neniku/android-adb-exploit-research) — educational PoC conducted in an authorized lab environment on exposed ADB interfaces (TCP 5555) on Android/IoT devices, including countermeasure analysis and device restoration.
- [Metodi_Di_Compressione](https://github.com/Neniku/Metodi_Di_Compressione) — notes and slides on common compression algorithms and their real-world use cases.
- [ScanPy](https://github.com/GruppoDueMAEMA/ScanPy) — school group project: multi-threaded Python network scanner for host discovery, TCP/UDP scans, and passive OS fingerprinting.

---

### Outside the screen

Kingdom Hearts and Yu-Gi-Oh have been taking up most of my free time lately. I also host a Palworld server for the family, which means I spend more time managing the server than actually playing.

[LinkedIn](https://www.linkedin.com/in/eleonardo-bajramovski/) &nbsp;&middot;&nbsp; [eleonardo.b@proton.me](mailto:eleonardo.b@proton.me)
