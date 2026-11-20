# BAZ 4.0 – Cloudflare-Testbranch (V0.2)

**Nur Pilot/Demomodus. Nicht produktiv für die Feuerwehr einsetzen.**

Dieser Branch enthält die zusammengehörigen Dateien für Cloudflare Pages (Git-Integration):
- `index.html` – Testoberfläche
- `styles.css` – Design
- `app.js` – Clientlogik
- `_worker.js` – API-Gateway, Anmeldung und Demomodus

## Bereitstellung

Auf Cloudflare Pages ein **neues Testprojekt** mit diesem Branch als Produktionsbranch für dieses Testprojekt erstellen. Das Build-Kommando leer lassen und das Ausgabeverzeichnis auf das Repository-Stammverzeichnis `/` setzen. Die Dateien liegen im Stammverzeichnis.

Ohne die gesonderte Freigabe `BAZ4_DEMO=false` im geschützten Testsystem ist die Anwendung ausschließlich eine schreibgeschützte Demo. Echte Datenzugriffe benötigen zusätzlich Cloudflare Access, eine freigegebene interne API und Secrets in Cloudflare – **niemals im GitHub-Code**.

**Achtung:** GitHub-Repository ist öffentlich. Keine internen Dateilinks, Google-Schlüssel, personenbezogenen Daten, Einsatzunterlagen oder echten Dienstbuchdaten committen.

Die vorherige Dashboard-App bleibt auf `main` unverändert. Dieser Branch darf nicht ungeprüft nach `main` gemergt werden.

Das separate Cloudflare-Pages-Direktupload-ZIP enthält dieselben vier Dateien. Der Python-Serverdienst ist hier bewusst nicht enthalten und darf nicht öffentlich abgelegt werden.
