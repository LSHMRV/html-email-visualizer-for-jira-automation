# html-email-visualizer-for-jira-automation

Dieses Tool ermöglicht es dir, HTML-E-Mails mit Jira-Platzhaltern direkt im Browser zu gestalten und zu testen – inklusive Live-Vorschau, konfigurierbarer Platzhalterliste und Import/Export-Funktion.

## ✨ Funktionen

- Eingabefelder für Kopfzeile, Fußzeile und E-Mail-Inhalt
- Live-Vorschau der generierten HTML-E-Mail
- Syntax-Highlighting und Zeilennummern für HTML-Code (CodeMirror)
- Platzhalter-Tabelle mit Bearbeitungsfunktion
- Import/Export der Platzhalterliste als JSON-Datei
- Speicherung der Konfiguration im Browser (Local Storage)

## 🚀 Nutzung

1. Öffne die HTML-Datei im Browser (z. B. `jira_email_preview_tool_configurable_v2.html`)
2. Gib Kopfzeile, Fußzeile und E-Mail-Inhalt ein
3. Klicke auf „Vorschau generieren“
4. Bearbeite oder ergänze Platzhalter in der Tabelle
5. Exportiere oder importiere die Platzhalterliste bei Bedarf

## 🧩 Platzhalter-Konfiguration

Die Platzhalterliste wird im Tool angezeigt und kann direkt bearbeitet werden. Alternativ kannst du sie als JSON-Datei importieren/exportieren.

### Beispiel für `platzhalterliste.json`:

```json
{
  "{{issue.summary}}": {
    "name": "Zusammenfassung",
    "value": "Fehler in der Login-Funktion"
  },
  "{{issue.key}}": {
    "name": "Vorgangsschlüssel",
    "value": "ABC-123"
  },
  "{{issue.url}}": {
    "name": "Vorgangs-URL",
    "value": "https://jira.example.com/browse/ABC-123"
  }
}
