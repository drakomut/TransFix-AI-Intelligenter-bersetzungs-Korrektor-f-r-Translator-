# TransFix AI

**Intelligenter Übersetzungs-Korrektor für Translator++ und RPG Maker Projekte**

TransFix AI ist ein Browser-basiertes Werkzeug zur Analyse und automatischen Korrektur von `.trans`-Dateien aus Translator++.

Das Tool erkennt typische Übersetzungsfehler in RPG Maker MV/MZ Projekten und kann diese mithilfe eines lokalen KI-Modells aus LM Studio automatisch beheben.

---

## Features

### Automatische Fehlererkennung

TransFix AI erkennt unter anderem:

* Fehlende RPG-Maker-Codes (`\C[n]`, `\>`, `\<`, `\|`, `\G`, `\{`, `\}`)
* Zusätzliche oder beschädigte Codes
* Nicht übersetzte japanische Texte
* Halluzinationen von KI-Modellen
* Fehlerhafte Zeilenumbrüche
* Zu lange Dialogtexte
* Leere Übersetzungen
* Defekte Hex-Ausgaben (`0xf000d`, `0xf000e` usw.)
* Fehlerhafte Farbcode-Blöcke

### KI-Korrektur

* Einzelne Zeilen per Knopfdruck korrigieren
* Stapelverarbeitung mehrerer Fehler
* Lokale Verarbeitung über LM Studio
* Keine Cloud-Dienste erforderlich

### Editor

* Direkte Bearbeitung von Übersetzungen
* Sofortige Fehleranalyse
* Farbige Markierung problematischer Einträge
* Such- und Filterfunktionen

### RPG Maker Unterstützung

* RPG Maker MV
* RPG Maker MZ
* Translator++
* Erhalt aller relevanten Steuerzeichen
* Dialogbox-Längen werden berücksichtigt

---

## Voraussetzungen

### Benötigte Software

* LM Studio
* Ein kompatibles Sprachmodell
* Ein aktueller Browser (Firefox empfohlen)

Empfohlene Modelle:

* Qwen 3.5
* DeepHermes 3
* Gemma 3
* Andere OpenAI-kompatible Modelle

---

## Installation

### 1. LM Studio installieren

LM Studio herunterladen und installieren.

### 2. Modell laden

Ein kompatibles Modell herunterladen und laden.

### 3. Local Server starten

In LM Studio:

* Developer → Local Server
* Start Server

### 4. CORS aktivieren

In LM Studio:

Server Options → Enable CORS

aktivieren und den Server neu starten.

### 5. Tool starten

`trans_editor.html` im Browser öffnen.

### 6. Verbindung testen

Standard-URL:

http://localhost:1234/v1

Auf **„Testen“** klicken.

---

## Verwendung

### Datei öffnen

1. `.trans` Datei laden
2. Datei auswählen
3. Analyse startet automatisch

### Einzelne Fehler korrigieren

1. Fehlerhafte Zeile auswählen
2. Auf **✦ Fix** klicken
3. KI erstellt eine korrigierte Übersetzung

### Alle Fehler korrigieren

1. Auf **🤖 Alle markierten korrigieren** klicken
2. Die KI verarbeitet alle markierten Einträge automatisch

### Speichern

Nach Abschluss:

**💾 Speichern**

Die Datei wird erneut als `.trans` gespeichert und kann direkt in Translator++ verwendet werden.

---

## Unterstützte Fehlerarten

| Fehler           | Beschreibung                               |
| ---------------- | ------------------------------------------ |
| Code fehlt       | RPG-Maker-Code wurde entfernt              |
| Code hinzugefügt | Nicht vorhandener Code wurde eingefügt     |
| Code verschoben  | Farb- oder Steuercode an falscher Position |
| Code offen       | Farbcode nicht korrekt geschlossen         |
| Hex-Müll         | 0xf000d / 0xf000e Fehler                   |
| Nicht übersetzt  | Japanischer Text vorhanden                 |
| Halluzination    | KI hat unerwünschten Inhalt erzeugt        |
| Zeilenumbruch    | Fehlerhafte `\n` Struktur                  |
| Zu lang          | Dialog passt nicht mehr ins Fenster        |
| Leer             | Keine Übersetzung vorhanden                |

---

## Datenschutz

TransFix AI arbeitet vollständig lokal.

* Keine Cloud-Anbindung
* Keine Datenübertragung an externe Server
* Alle Übersetzungen bleiben auf dem eigenen Rechner

---

## Lizenz

MIT License

---

## Danksagung

Dieses Projekt wurde für die Translator++ und RPG Maker Community entwickelt.

Besonderer Dank gilt den Entwicklern von:

* Translator++
* LM Studio
* Qwen
* DeepHermes
* RPG Maker
