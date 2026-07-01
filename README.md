# Portfolio · Self-Hosted Services

Vorzeige-Seite meiner selbst gehosteten Dienste auf einem Raspberry-Pi-Homeserver.

**Live:** https://djswiss.github.io

## Dienste

| Dienst | Zweck | Stack |
|--------|-------|-------|
| **aihub** | Zentraler KI-Hub mit Chat, Sprach-/Videobots und Messaging-Integrationen | Gradio · Ollama · LiveKit · Jitsi · Piper |
| **aiagent** | Lokaler Multi-User-KI-Agent mit Web-UI | Docker · Caddy · Nix |
| **finance** | Buchhaltung & Belege mit KI-Klassifikation | Firefly III · paperless-ngx · Gotify |
| **skilltest** | Adaptiver Kompetenztest mit KI-Lehrer | Flask · SQLite · Chart.js |
| **notebookllm** | Grounded RAG mit Inline-Zitaten, mehrsprachig | RAG · bge-m3 · Vektor-DB |
| **inventar** | Inventarverwaltung | FastAPI · MariaDB |
| **netdata** | Echtzeit-Server-Monitoring | Netdata |
| **portainer** | Docker-Verwaltungs-UI | Portainer CE |
| **Home Assistant** | Smart-Home-Steuerung, lokal | Automationen · Dashboards |
| **Pi-hole** | Netzwerkweiter Ad-/Tracker-Blocker | DNS-Sinkhole |
| **SearXNG** | Datenschutzfreundliche Meta-Suchmaschine | Self-Hosted |

Die Seite ist statisches HTML/CSS ohne Abhängigkeiten (`index.html`) und wird über GitHub Pages ausgeliefert.
Screenshots in `shots/` stammen aus dem laufenden Betrieb; Klick auf ein Vorschaubild öffnet die Großansicht.
