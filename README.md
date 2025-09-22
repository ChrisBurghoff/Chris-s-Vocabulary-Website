# 📚 Privater Vokabeltrainer

Ein einfacher, **passwortgeschützter** Vokabeltrainer zum Selbstlernen.  
Alles läuft **lokal im Browser** – keine Cloud, keine externen Abhängigkeiten.  
Ideal für den privaten Gebrauch oder als Lernhilfe unterwegs.

---

## ✨ Features

- 🔒 **Zugangsschutz**  
  Vor dem Start wird ein Passwort abgefragt.  
  Standard: `AbCd-1234` (hartkodiert im Code).

- 💾 **Fortschritt speichern**  
  - Automatische Speicherung im `localStorage` des Browsers.  
  - **Export/Import**: Fortschritt kann als `progress.json` heruntergeladen und auf anderen Geräten wieder importiert werden.

- 📂 **Vokabeldateien**  
  - Standardmäßig wird beim Laden `vocabulary.json` aus demselben Ordner eingelesen.  
  - Eigene Vokabeldateien im JSON‑Format können zusätzlich importiert werden (werden nicht gespeichert).  
  - Beispielstruktur:
    ```json
    [
      {"de":"Apfel","en":"apple","section":"Obst","example":"Ich esse einen ___."},
      {"de":"laufen","en":"to run","section":"Verben","example":"Ich ___ schnell."}
    ]
    ```

- 📝 **Abfrage-Logik**  
  - Richtung: **Deutsch → Englisch**  
  - Case‑sensitive Prüfung  
  - Zufällige Auswahl, falsche Antworten werden nach hinten verschoben  
  - Nach falscher Antwort oder Überspringen: Lösung + Beispielsatz werden angezeigt

- 📱 **Mobile-optimiert**  
  - Große Buttons, responsive Layout  
  - Eingabefeld mit deaktivierter Autokorrektur, Autokapitalisierung und Vorschlägen  
  - Enter bestätigt Eingaben automatisch

- 🧩 **Sections & Testmodus**  
  - Vokabeln sind nach `section` gruppiert  
  - Zusätzlich gibt es eine **„Alle Vokabeln“**‑Section für einen kompletten Test über alle Wörter

- 🆘 **Hilfemodal**  
  - Kurze Anleitung direkt in der App verfügbar

---

## 🚀 Installation & Nutzung

1. Repository klonen oder ZIP herunterladen:
   ```bash
   git clone https://github.com/<dein-user>/<dein-repo>.git
   ```
2. `index.html` und `vocabulary.json` im selben Ordner ablegen.
3. `index.html` im Browser öffnen.
4. Passwort eingeben → loslegen!


## 📤 Fortschritt übertragen

- **Export:** Klick auf `Export Data` → `progress.json` wird heruntergeladen  
- **Import:** Klick auf `Import Data` → `progress.json` auswählen → Fortschritt wird übernommen

---

## ⚠️ Hinweise

- Alles läuft **lokal** – keine Daten werden ins Internet übertragen.  
- Fortschritt ist **browsergebunden**. Für andere Geräte: Export/Import nutzen.  
- Eigene Vokabeldateien müssen nach jedem Neustart neu importiert werden.

---

## 🛠️ Technische Details

- Eine einzige `index.html` mit **inline CSS & Vanilla JS**  
- Keine externen Bibliotheken  
- Speicherung ausschließlich über `localStorage`

---

## 📄 Lizenz

Dieses Projekt ist für den **privaten Gebrauch** gedacht.  
Passe es gerne an deine eigenen Bedürfnisse an.