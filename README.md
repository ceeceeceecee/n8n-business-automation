# n8n Business Automation

[![n8n](https://img.shields.io/badge/n8n-Workflow%20Templates-FF6D5A?logo=n8n)](https://n8n.io)
[![License](https://img.shields.io/badge/license-MIT-blue)](LICENSE)
[![DACH](https://img.shields.io/badge/region-DACH%20KMU-1a73e8)]()

> Fertige n8n-Workflow-Templates für typische KMU-Geschäftsprozesse — E-Mail, CRM, Marketing & Buchhaltung in einem Repo.

Ready-to-use n8n workflow templates for common SMB business processes — email, CRM, marketing & accounting in one repo.

---

## Screenshots

### Workflow-Übersicht

![n8n Workflow Übersicht](screenshots/n8n-workflow-list.png)
*Alle 4 fertigen Automatisierungen auf einen Blick — direkt in deiner n8n-Instanz importierbar.*

### E-Mail-Klassifizierung

![E-Mail-Klassifizierung](screenshots/workflow-email-klassifizierung.png)
*Eingehende E-Mails per KI (Claude/OpenAI) automatisch kategorisieren: Kunde, Lieferant, Intern.*

### Lead-Erfassung

![Lead-Erfassung](screenshots/workflow-lead-erfassung.png)
*Webhook-basierte Lead-Erfassung mit automatischer CRM-Anbindung und Slack-Benachrichtigung.*

### Social-Media-Posting

![Social-Media-Posting](screenshots/workflow-social-media.png)
*RSS-Feed-gesteuerte LinkedIn-Posts mit KI-generiertem Content.*

### Rechnungseingang

![Rechnungseingang](screenshots/workflow-rechnungseingang.png)
*Automatische Rechnungserkennung aus E-Mails mit Google Sheets-Anbindung.*

---

## Features

| Workflow | Trigger | KI | Output |
|----------|---------|----|--------|
| E-Mail-Klassifizierung | IMAP Poll | Claude / OpenAI | Gmail Labels |
| Lead-Erfassung | Webhook | — | Slack + Google Sheets |
| Social-Media-Posting | Cron (RSS) | Claude / OpenAI | LinkedIn |
| Rechnungseingang | E-Mail-Anhang | Claude / OpenAI | Google Sheets / Airtable |

---

## 🚀 Schnellstart

### Voraussetzungen

| Komponente | Version | Zweck |
|---|---|---|
| n8n | neueste | Workflow-Engine |
| Docker & Docker Compose | 20.10+ / 2.0+ | n8n selbstgehostet |
| Claude/OpenAI API Key | aktuell | KI-Verarbeitung |
| Google Account (optional) | — | Sheets, Gmail |
| Slack Workspace (optional) | — | Benachrichtigungen |

### Installation

```bash
git clone https://github.com/ceeceeceecee/n8n-business-automation.git
cd n8n-business-automation

# n8n starten (Docker)
cp .env.example .env
# .env anpassen → docker compose up -d
```

### Erste Schritte

1. **n8n öffnen** (Standard: `http://localhost:5678`)
2. **Workflows importieren** — n8n UI → Workflows → Importieren → JSON-Dateien aus `workflows/`
3. **API-Keys konfigurieren** — Claude/OpenAI Credentials in n8n anlegen
4. **Workflow aktivieren** und ersten Testlauf starten

---

## Use Cases

| Zielgruppe | Szenario | Workflow |
|------------|----------|----------|
| Kleinunternehmen | Inbox-Chaos reduzieren | E-Mail-Klassifizierung |
| Vertrieb | Leads nicht verlieren | Lead-Erfassung |
| Marketing | Social Media ohne Aufwand | Social-Media-Posting |
| Buchhaltung | Rechnungen automatisch erfassen | Rechnungseingang |

---

## Tech Stack

- **n8n** — Workflow-Engine & Orchestrierung
- **Claude / OpenAI** — KI-Textverarbeitung
- **Docker Compose** — Deployment
- **Google Sheets / Airtable** — Datenbank
- **Slack** — Benachrichtigungen

---

## Roadmap

- [ ] WhatsApp-Business Integration
- [ ] Invoice OCR mit Vision-Modell
- [ ] Multi-Sprachen-Support (EN/FR)
- [ ] n8n Cloud Template Store Publishing

---

## Contributing

1. Fork erstellen
2. Feature-Branch: `git checkout -b feature/mein-workflow`
3. Commit: `git commit -m 'Add: Mein Workflow'`
4. Push: `git push origin feature/mein-workflow`
5. Pull Request

Siehe [CONTRIBUTING.md](CONTRIBUTING.md) für Details.

---


## 👤 Autor

**Cela** — Freelancer für digitale Verwaltungslösungen
## Lizenz

[MIT](LICENSE) — frei nutzbar, kommerziell und privat.

## Author

[ceeceeceecee](https://github.com/ceeceeceecee)

## Weitere Projekte

- [AI Email Assistant](https://github.com/ceeceeceecee/ai-email-assistant) — KI-E-Mail-Assistent
- [Self-Hosted AI Chatbot](https://github.com/ceeceeceecee/self-hosted-ai-chatbot) — DSGVO-konformer Chatbot
