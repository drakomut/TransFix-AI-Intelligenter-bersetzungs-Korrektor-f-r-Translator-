Beschreibung

TransFix AI ist ein Werkzeug zur Qualitätskontrolle und automatischen Korrektur von Translator++-Projekten. 
Das Programm analysiert .trans-Dateien, erkennt typische Übersetzungsfehler und kann diese mithilfe eines lokalen KI-Modells aus LM Studio automatisch korrigieren. 
Es wurde speziell für RPG Maker Spiele entwickelt und berücksichtigt RPG-Maker-Steuercodes, Zeilenumbrüche und Dialogbox-Limits.

Installation
LM Studio installieren.
Ein kompatibles Sprachmodell herunterladen (z. B. Qwen, DeepHermes oder ein anderes Übersetzungsmodell).
In LM Studio den Local Server starten.
Unter Server Options die Option Enable CORS aktivieren.
trans_editor.html im Browser öffnen.
Die URL von LM Studio eintragen (standardmäßig http://localhost:1234/v1).
Die gewünschte .trans-Datei laden.
Funktionen
📂 .trans-Dateien öffnen
Lädt Translator++-Projektdateien direkt im Browser.
Keine Installation zusätzlicher Programme erforderlich.
🔍 Automatische Fehleranalyse

Erkennt unter anderem:

Fehlende RPG-Maker-Codes (\C[n], \>, \<, \|)
Zusätzliche oder fehlerhafte Codes
Nicht übersetzte japanische Texte
Halluzinationen der KI
Fehlerhafte Zeilenumbrüche
Zu lange Dialogtexte
Leere Übersetzungen
Defekte Hex-Ausgaben (0xf000d usw.)
🤖 KI-Korrektur
Korrigiert einzelne Zeilen per Knopfdruck.
Nutzt lokale KI über LM Studio.
Keine Cloud-Anbindung erforderlich.
⚡ Stapelverarbeitung
Korrigiert alle markierten Fehler automatisch.
Mehrere Einträge gleichzeitig verarbeitbar.
Fortschrittsanzeige mit Stop-Funktion.
📝 Manueller Editor
Übersetzungen können direkt bearbeitet werden.
Änderungen werden sofort überprüft.
Fehler werden farblich markiert.
💾 Speichern
Speichert die bearbeitete Datei wieder als .trans.
Kompatibel mit Translator++.
🎮 Speziell für RPG Maker
Erhält Steuercodes automatisch.
Beachtet Dialogfenster-Größen.
Unterstützt Farb-Codes und Textformatierungen.
Entfernt Furigana-Tags korrekt aus Übersetzungen.
Kurzbeschreibung für GitHub oder Download-Seite

TransFix AI ist ein Browser-Tool zur Analyse und automatischen Korrektur von Translator++-Dateien. 
Es erkennt typische Übersetzungsfehler in RPG-Maker-Projekten und kann diese mithilfe lokaler KI-Modelle aus LM Studio automatisch beheben. 
Unterstützt Batch-Verarbeitung, Fehlerprüfung und sichere Behandlung von RPG-Maker-Steuercodes.
