# Eleonardo Bajramovski (Neniku)

[English](#english) · [Italiano](#italiano)

---

<a name="english"></a>
## English

Systems administrator in training, based in Vasto, Italy.

I started tinkering with hardware and software around 2012/2013, when I flashed CyanogenMod 10 on a Galaxy S3 Exynos and spent a good while fighting with the camera driver — on Exynos the camera wouldn't initialize properly under custom ROMs, until someone released a module you could flash through ClockworkMod Recovery that finally fixed it. That's more or less where everything started. Since then I've gone through a OnePlus One with CyanogenOS (then OxygenOS) — and that's when things really escalated. Through the OnePlus One Italia Telegram group I started going deeper: that's also where I first ran Tuga Power as my daily ROM. From there I joined more and more international groups, discovered XDA, and got into the habit of following what developers and modders were doing worldwide. That community pull is a big part of why I ended up where I am. After the OnePlus One I went through a Redmi Note 3 Pro (kenzo), a Redmi Note 5 Pro (whyred), and I'm currently on a OnePlus 8T — still modded. Somewhere around those same years I also started taking apart my PC: swapped RAM, tried every version of Windows that came out, and when Windows 10 arrived I began stripping it down to make it actually usable. That habit stuck.

Today my main machine is a Lenovo IdeaPad Gaming 3 (15ACH6) I call Frankenstein: 32GB RAM, two 1TB SSDs (Samsung 990 Pro + Crucial M.2 2242), display swapped for a 165Hz panel, fresh thermal paste (MX-7), mild overclock via MSI Afterburner. It dual boots a debloated Windows 11 (ChrisTitus tool + Winhance, styled with Windhawk and Start11 v2) and Pop!_OS, where I do most of my actual work and run VMs. The VMs live on a shared SSD so they're accessible from both sides of the dual boot.

On the server side I run an MX Linux machine that handles NAS storage, self-hosted media (Jellyfin), Docker containers and a Palworld dedicated server for family use — me, my brother-in-law and my nephews. Everything behind Tailscale and a reverse proxy.

The security and DevSecOps path came later, through a cybersecurity course and a lot of hands-on practice: container scanning with Trivy, DAST pipelines with OWASP ZAP, SBOM generation, GitHub Actions CI/CD. That's the direction I'm heading professionally.

### What I work with

**Systems & infrastructure**
Linux (Debian-based, Pop!_OS, MX Linux), Docker, Tailscale, Nginx reverse proxy, Windows (heavily customized)

**Scripting & automation**
Bash, Python, YAML, GitHub Actions

**Security**
Trivy, OWASP ZAP, SBOM/supply chain analysis, DAST pipelines, FlareVM, CAINE

**Homelab**
Jellyfin, Sonarr, Radarr, self-hosted game servers, MedicatedUSB, custom bootable USB environments

### Currently learning

- Container vulnerability scanning and SBOM generation
- DAST integration in CI/CD pipelines
- ZFS management
- GPU transcoding for self-hosted media

### Projects

- [Backup_script_Cyborg](https://github.com/Neniku/Backup_script_Cyborg) — hardened Bash backup with encryption, SHA256 verification, dual remote upload (SFTP + SMB), checkpoint/resume and HTML reporting. Evolution of [Backup_script_Umano](https://github.com/Neniku/Backup_script_Umano).
- [Metodi_Di_Compressione](https://github.com/Neniku/Metodi_Di_Compressione) — slides and notes on the most common compression algorithms and their real-world tradeoffs.

### Outside the terminal

Kingdom Hearts and Yu-Gi-Oh are taking up most of my non-work hours lately. I also collect Swatch watches and still spend more time than I should reading patch notes for games I host but barely have time to play.

[LinkedIn](https://www.linkedin.com/in/eleonardo-bajramovski-7599a7372/)

---

<a name="italiano"></a>
## Italiano

Amministratore di sistemi in formazione, basato a Vasto, in Abruzzo.

Ho iniziato a smontare hardware e software intorno al 2012/2013, quando ho flashato CyanogenMod 10 su un Galaxy S3 Exynos e ho passato un bel po' di tempo a combattere con il driver della fotocamera — sull'Exynos la fotocamera non si inizializzava correttamente con le custom ROM, finché qualcuno non rilasciò un modulo da flashare tramite ClockworkMod Recovery che finalmente risolse il problema. Più o meno da lì è partito tutto. Poi è arrivato il OnePlus One con CyanogenOS (poi OxygenOS) — ed è lì che le cose sono davvero esplose. Tramite il gruppo Telegram OnePlus One Italia ho iniziato ad andare sempre più in profondità: è lì che ho anche usato Tuga Power come ROM principale. Da lì sono entrato in sempre più gruppi internazionali, ho scoperto XDA, e ho preso l'abitudine di seguire quello che sviluppatori e modder stavano facendo in tutto il mondo. Quella spinta comunitaria è una parte importante del motivo per cui sono arrivato dove sono. Dopo il OnePlus One sono passato per un Redmi Note 3 Pro (kenzo), un Redmi Note 5 Pro (whyred), e ora sono su OnePlus 8T — ancora moddato. Negli stessi anni ho iniziato anche a mettere le mani sul PC: ho cambiato la RAM, provato ogni versione di Windows che usciva, e quando è arrivato Windows 10 ho cominciato a smontarlo per renderlo usabile davvero. Quella abitudine non è mai passata.

Oggi la mia macchina principale è un Lenovo IdeaPad Gaming 3 (15ACH6) che chiamo Frankenstein: 32GB di RAM, due SSD da 1TB (Samsung 990 Pro + Crucial M.2 2242), display sostituito con uno da 165Hz, pasta termica cambiata (MX-7), leggero overclock via MSI Afterburner. Ha un dual boot tra Windows 11 debloatato (ChrisTitus tool + Winhance, personalizzato con Windhawk e Start11 v2) e Pop!_OS, dove faccio la maggior parte del lavoro reale e giro le VM. Le VM stanno su un SSD condiviso così sono accessibili da entrambi i lati del dual boot.

Lato server ho una macchina MX Linux che gestisce lo storage NAS, il media server self-hosted (Jellyfin), container Docker e un server dedicato di Palworld per uso familiare — io, mio cognato e i miei nipoti. Tutto dietro Tailscale e un reverse proxy.

Il percorso verso la security e il DevSecOps è venuto dopo, tra un corso di cybersecurity e tanta pratica: container scanning con Trivy, pipeline DAST con OWASP ZAP, generazione di SBOM, CI/CD con GitHub Actions. È la direzione che sto prendendo professionalmente.

### Con cosa lavoro

**Sistemi & infrastruttura**
Linux (Debian-based, Pop!_OS, MX Linux), Docker, Tailscale, reverse proxy Nginx, Windows (pesantemente personalizzato)

**Scripting & automazione**
Bash, Python, YAML, GitHub Actions

**Sicurezza**
Trivy, OWASP ZAP, analisi SBOM/supply chain, pipeline DAST, FlareVM, CAINE

**Homelab**
Jellyfin, Sonarr, Radarr, server di gioco self-hosted, MedicatedUSB, ambienti USB avviabili personalizzati

### Cosa sto imparando

- Container vulnerability scanning e generazione SBOM
- Integrazione DAST nelle pipeline CI/CD
- Gestione ZFS
- Transcoding GPU per media server self-hosted

### Progetti

- [Backup_script_Cyborg](https://github.com/Neniku/Backup_script_Cyborg) — backup Bash con cifratura, verifica SHA256, upload ridondante (SFTP + SMB), checkpoint/resume e report HTML. Evoluzione di [Backup_script_Umano](https://github.com/Neniku/Backup_script_Umano).
- [Metodi_Di_Compressione](https://github.com/Neniku/Metodi_Di_Compressione) — slide e appunti sui principali algoritmi di compressione e i loro tradeoff reali.

### Fuori dal terminale

Ultimamente Kingdom Hearts e Yu-Gi-Oh si stanno prendendo la maggior parte del tempo libero. Colleziono anche orologi Swatch e passo ancora più tempo del dovuto a leggere patch note di giochi che hosto ma che fatico a trovare il tempo di giocare.

[LinkedIn](https://www.linkedin.com/in/eleonardo-bajramovski-7599a7372/)
