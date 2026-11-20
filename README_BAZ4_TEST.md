# BAZ 4.0 – GitHub-Cloudflare-Testbranch V0.3

**Nicht produktiv einsetzen.** Der bestehende Infoscreen wird lesend eingebunden, die produktiven Daten-/OVD-Endpunkte werden nicht verändert.

## Nachgewiesene Quelle

- Live-Infoscreen: https://github.com/michaelmejtsky/infoscreen
- Hauptseite: https://michaelmejtsky.github.io/infoscreen/
- Das separate Repository `Infoscreenls1` wird **nicht** verwendet.
- Das Unterverzeichnis `infoscreen/ovd` hat aktuell eine leere API-Adresse. Es wird daher nicht als produktiver OVD-Dienst übernommen.

## Cloudflare Pages (Testprojekt)

- Git-Integration: `michaelmejtsky/DashboardAPP`
- Branch: `baz4-v0-3-infoscreen-pilot`
- Build-Befehl: leer / kein Framework
- Ausgabeverzeichnis: `/` (Repository-Stammverzeichnis)
- `_worker.js` arbeitet mit Cloudflare Pages `env.ASSETS`.
- Keine Secrets, Personen- oder Dienstplandaten in dieses öffentliche Repository übertragen.

In BAZ 4.0: Menüpunkt **Infoscreen Live**; eine eingebettete Vorschau wird erst auf Klick geladen; ein Direktlink bleibt für Browser ohne Frame-Unterstützung verfügbar.

Die neue Anwendung läuft weiter im schreibgeschützten Demomodus, solange `BAZ4_DEMO` nicht explizit auf `false` gesetzt wird. Schreibzugriffe erfordern zusätzlich die private Backend- und Cloudflare-Access-Konfiguration und Vor-Ort-Tests. **Niemals ohne Abnahme aktivieren.**

Die produktiven Branches `DashboardAPP/main`, `infoscreen/main` und `Infoscreenls1/main` bleiben unverändert.
