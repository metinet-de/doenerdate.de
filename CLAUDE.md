# DönerDate – Blog Management

**Website:** https://www.doenerdate.de
**Beschreibung:** Der Döner-Blog über die besten Dönerläden der Stadt
**WordPress-Version:** 6.9.4
**Sprache:** Deutsch
**Admin-E-Mail:** info@metinet.de

---

## Zweck dieses Ordners

Dieser Ordner dient zur **Fernverwaltung des DönerDate-Blogs** über Claude (Cowork-Modus).
Hier liegt kein App-Code – stattdessen:

- **Content-Entwürfe** (Blog-Posts, Reviews, Seiten) als Markdown-Dateien
- **Assets & Medien** (Bilder, die auf den Blog hochgeladen werden sollen)
- **Notizen & Planung** (Redaktionsplan, Ideen, SEO-Notizen)

---

## MCP-Verbindung

Claude ist über den **WordPress MCP-Adapter** direkt mit doenerdate.de verbunden.
Verfügbare Aktionen werden über das MCP-Tool `mcp__doenerdate-wordpress__*` ausgeführt.

Aktuell verfügbare Abilities:
- `core/get-site-info` – Website-Metadaten abrufen
- `core/get-environment-info` – PHP/WP-Umgebung prüfen

> Weitere Abilities (Posts erstellen, Medien hochladen, etc.) können über das WordPress-Plugin
> erweitert werden, sobald sie benötigt werden.

---

## Ordnerstruktur (Konvention)

```
doenerdate.de/
├── CLAUDE.md                  # Diese Datei – Projektübersicht
├── posts/                     # Blog-Post-Entwürfe (Markdown)
│   └── YYYY-MM-DD-titel.md
├── pages/                     # Seiten-Entwürfe
├── assets/                    # Bilder & Medien für den Upload
└── planning/                  # Redaktionsplan, Ideen, SEO
```

---

## Workflow

1. **Content erstellen** → Markdown-Datei in `posts/` ablegen
2. **Review** → Claude prüft Entwurf auf Stil, SEO, Rechtschreibung
3. **Publish** → Claude veröffentlicht per MCP direkt auf WordPress (sobald Write-Abilities verfügbar)

---

## Stil & Ton

- Locker, authentisch, mit Leidenschaft fürs Thema
- Zielgruppe: Döner-Enthusiasten in deutschen Städten
- SEO-Keywords natürlich einbauen (Stadtname + "Döner", Läden beim Namen nennen)
- Bewertungen fair und ehrlich – keine Werbetexte
