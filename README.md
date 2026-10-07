# Tavirio Games – GitHub-Pages-Vorbereitung

Stand: 7. Oktober 2026. Für Veröffentlichung unter https://derking36.github.io/.

## Bestand

Die öffentliche GitHub-API listet für DerKing36 derzeit `tavirio-legal`
(Standardbranch `main`, GitHub Pages aktiv). Eine öffentliche User-Site
`derking36.github.io` wurde nicht gefunden. Die Prüfung war ohne Anmeldung;
private Repositories konnten damit nicht ausgeschlossen werden. Eine anschließende
authentifizierte API-Prüfung als DerKing36 bestätigte ebenfalls, dass das
User-Site-Repository noch nicht vorhanden ist.

Unter `C:\Projekte` war weder diese User-Site noch ein Legal-Checkout vorhanden.
Die vorhandenen Projekte und das Legal-Repository wurden nicht geändert.
Die Legal-Dateinamen wurden direkt aus dem GitHub-Repository gelesen.

## Dateien

- `index.html`: responsive Entwicklerwebsite, Wortavia, Arronexa, rechtliche Links.
- `styles.css`: lokale Styles, Smartphone-/Desktop-Breakpoints, Tastaturfokus.
- `favicon.svg`: lokales Tavirio-Symbol.
- `app-ads.txt`: eine Seller-Zeile, UTF-8 ohne BOM, abschließendes LF.
- `.nojekyll`: statische Dateien ohne Jekyll-Verarbeitung.
- `README.md`: Vorbereitung und Veröffentlichungsschritte.

Keine Frameworks, JavaScript-Abhängigkeiten, Tracker, externen Fonts oder
Build-Artefakte. Keine robots.txt-Sperre. Keine Zugangsdaten oder privaten Daten.
Die angegebene Kontaktadresse ist die bestehende öffentliche Entwickleradresse.

## Verifizierte Rechtsseiten

Alle sechs Seiten antworteten bei der Prüfung mit HTTP 200 und passenden Titeln:

- https://derking36.github.io/tavirio-legal/datenschutz.html
- https://derking36.github.io/tavirio-legal/datenloeschung.html
- https://derking36.github.io/tavirio-legal/impressum.html
- https://derking36.github.io/tavirio-legal/privacy-en.html
- https://derking36.github.io/tavirio-legal/data-deletion-en.html
- https://derking36.github.io/tavirio-legal/legal-notice-en.html

Der Nutzer hat die öffentliche Wortavia-Play-URL bereitgestellt:
https://play.google.com/store/apps/details?id=games.tavirio.wortavia
Sie antwortete mit HTTP 200. Google Play zeigt „Wortavia – Word Search“ von
„Tavirio Games“. Der Link ist in `index.html` eingebaut.
Arronexa wird ausschließlich als Projekt in Entwicklung beschrieben.

## Lokale Prüfung

HTML-Grundstruktur, Tag-Verschachtelung, lokale Dateien und Fragmentziele: PASS.
CSS enthält responsive Breakpoints bei 760 und 360 Pixeln und reduzierte Bewegung.
`app-ads.txt` wurde bytegenau geprüft: 59 Bytes, keine BOM, abschließendes LF.
SHA-256: `4A29633F2472A89123E035D3E34C3B6A754DD05C0D346A9A0B32275D9FD669A2`.
Inhalt:

```text
google.com, pub-4778506813295881, DIRECT, f08c47fec0942fa0
```

Eine visuelle Browserprüfung ist noch offen: Die integrierte Browservorschau
blockierte den lokalen `file:`-Aufruf. Vor Veröffentlichung `index.html` selbst
im Browser öffnen und auf Smartphone-/Desktop-Breite prüfen.

## Manuelle Veröffentlichung auf GitHub

1. Im Account **DerKing36** prüfen, ob `derking36.github.io` bereits existiert.
   Falls vorhanden, zuerst Inhalte prüfen und diese Dateien konservativ integrieren.
2. Falls nicht vorhanden, öffentliches Repository **derking36.github.io** anlegen.
3. `index.html`, `styles.css`, `favicon.svg`, `app-ads.txt` und `.nojekyll`
   direkt im Repository-Root auf Branch **main** ablegen. README kann mit hinein.
4. Settings → Pages → Build and deployment → Deploy from a branch:
   **main**, **/(root)**. HTTPS aktivieren/beibehalten. Keine Custom Domain nötig.
5. Nach dem Pages-Deployment live prüfen:
   - https://derking36.github.io/
   - https://derking36.github.io/app-ads.txt
   Die zweite URL muss HTTP 200 und die unveränderte Seller-Zeile als Text liefern.
6. Die sechs bisherigen `/tavirio-legal/`-URLs erneut aufrufen. Das separate
   Legal-Repository, seine Dateien und seine Pages-Konfiguration beibehalten.

## Google Play und AdMob

Nach erfolgreicher Live-Prüfung in Google Play bei Wortavias Store-Eintrag im
Website-Feld unter Entwicklerkontakt **https://derking36.github.io/** eintragen.
Die bestehenden Datenschutz-URLs bleiben ihre bisherigen Legal-URLs.
Anschließend in AdMob die app-ads.txt-Prüfung erneut anstoßen; der Crawler soll
**https://derking36.github.io/app-ads.txt** finden. Änderungen müssen erst
veröffentlicht und von Google neu eingelesen werden.

Die Veröffentlichung erfolgt auf ausdrücklichen Auftrag im separaten öffentlichen
Repository `DerKing36/derking36.github.io`, Branch `main`, Pages-Quelle `/(root)`.
Wortavia, das bestehende Legal-Repository und Play-Console-Einstellungen werden
bei dieser Veröffentlichung nicht verändert.
