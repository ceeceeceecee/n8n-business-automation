# n8n Business Automation

[![n8n](https://img.shields.io/badge/n8n-Workflow%20Templates-FF6D5A?logo=n8n)](https://n8n.io)
[![Lizenz](https://img.shields.io/badge/Lizenz-MIT-green.svg)](LICENSE)
[![DACH](https://img.shields.io/badge/Zielgruppe-DACH%20KMU-blue.svg)]()

> Fertige n8n-Workflow-Templates für typische KMU-Geschäftsprozesse im DACH-Raum.

Ready-to-use n8n workflow templates for common SMB business processes in the DACH region.

---

## 📋 Workflow-Übersicht

| # | Workflow | Beschreibung |
|---|----------|-------------|
| 1 | **E-Mail-Klassifizierung** | Eingehende E-Mails automatisch kategorisieren (Kunde/Lieferant/Intern) |
| 2 | **Lead-Erfassung** | Webhook-basierte Lead-Erfassung mit automatischer Benachrichtigung |
| 3 | **Social-Media-Posting** | RSS-Feeds zu LinkedIn-Beiträgen mit KI-Unterstützung |
| 4 | **Rechnungseingang** | Rechnungen automatisch erfassen und in Google Sheets/Airtable ablegen |

## 🚀 Voraussetzungen

- [n8n](https://n8n.io) (selbstgehostet oder Cloud)
- Docker & Docker Compose
- Accounts für: Claude/OpenAI API, Google, Slack (je nach Workflow)

## 📦 Installation

### 1. Repo klonen

```bash
git clone https://github.com/ceeceeceecee/n8n-business-automation.git
cd n8n-business-automation
```

### 2. n8n starten (Docker)

```bash
cp .env.example .env
# .env anpassen
docker compose up -d
```

### 3. Workflows importieren

n8n öffnen → **Workflows importieren** → JSON-Datei aus `workflows/` auswählen.

## 📸 Screenshots

> Screenshots werden nachgereicht.

<!-- ![E-Mail-Klassifizierung](docs/screenshots/email-klassifizierung.png) -->

## 🛠️ Use Cases für KMU

- **E-Mail-Management:** Inbox-chaos reduzieren durch automatische Klassifizierung
- **Vertrieb:** Leads nicht mehr verlieren — sofortige Erfassung und Benachrichtigung
- **Marketing:** Social Media Presence ohne manuellen Aufwand
- **Buchhaltung:** Rechnungen automatisch erfasst und nachverfolgbar

## 🗺️ Roadmap

- [ ] Workflow: Terminbestätigung (Kalender + E-Mail)
- [ ] Workflow: Kundendatenbank-Sync (HubSpot ↔ Google Sheets)
- [ ] Workflow: Onboarding-Automatisierung
- [ ] Multi-Tenant Support für Agenturen
- [ ] DSGVO-Datenschutzerklärung-Vorlage für jeden Workflow

## 🤝 Mitmachen

Siehe [CONTRIBUTING.md](CONTRIBUTING.md).

## 📄 Lizenz

[MIT](LICENSE) — frei verwendbar, auch kommerziell.

---

Erstellt von [Cela](https://github.com/ceeceeceecee) — Freelancer für Automatisierung & KI-Lösungen.
