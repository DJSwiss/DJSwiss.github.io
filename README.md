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
| **LiveKit Meet** | Selbst gehostete Video-Konferenz mit HTTPS/WSS | LiveKit · WebRTC · Next.js · Caddy |
| **Verbindungen Schweiz** | ÖV-Fahrplan + Fuss-/Velo-/Auto-Routing mit Karte in einer App | Flask · Open Data CH · OSRM · Leaflet · Caddy · Docker |

### Verbindungen Schweiz – Features

Ein Dienst, der öffentlichen Verkehr und persönliche Routen unter einer Oberfläche vereint:

- **Vier Modi** in einem UI: 🚆 ÖV · 🚶 zu Fuss · 🚴 Velo · 🚗 Auto.
- **ÖV** über die freie Open-Data-Plattform Schweiz (kein API-Key) – mit mehreren
  Via-Stationen, Verkehrsmittel-Filter (Zug/Tram/Bus/Schiff/Seilbahn), Datum/Uhrzeit
  für Ab- oder Ankunft und Stationsvorschlägen.
- **Routing** (Fuss/Velo/Auto) über **selbst gehostetes OSRM** auf OpenStreetMap-Basis
  – komplett autark, keine externe Routing-API.
- **Karte** (Leaflet + OpenStreetMap): Routen und ÖV-Verbindungen als Linie, „Mein
  Standort" per GPS, Start/Ziel-Marker.
- **Details je Ergebnis**: Turn-by-turn-Wegbeschreibung bzw. ÖV-Abschnitte mit
  Zeiten/Gleisen, **Teilen** (Deep-Link) und **Kalender** (.ics-Export).
- **Eigene JSON-API** als schlanker Proxy und **HTTPS** via Caddy (nötig für GPS).

Die Seite ist statisches HTML/CSS ohne Abhängigkeiten (`index.html`) und wird über GitHub Pages ausgeliefert.
Screenshots in `shots/` stammen aus dem laufenden Betrieb; Klick auf ein Vorschaubild öffnet die Großansicht.
