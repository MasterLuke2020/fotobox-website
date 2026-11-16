# Fotobox – Informationsseite

Statische Website zur Debian-Fotobox von WeidnerNet, vorgesehen für GitHub Pages mit der Subdomain `fotobox.weidnernet.com`.

## Inhalte
- `index.html`: Informationen über die Fotobox und den Download per QR-Code
- `datenschutz.html`: **Entwurf**, Angaben vor Veröffentlichung prüfen und ergänzen
- `impressum.html`: **Entwurf**, vollständige Anbieterangaben fehlen noch
- `style.css`: responsives Styling ohne externe Schriftarten oder Tracker

## Vor Veröffentlichung
1. Vollständigen Betreiber-Namen, Anschrift und weitere gesetzlich erforderliche Angaben ergänzen.
2. Rechtsgrundlage für Aufnahmen und Cloud-Freigaben, Speicherdauer und Löschprozess festlegen.
3. Text mit den tatsächlichen Praktiken abgleichen. Gäste mit Google-Drive-Freigabelink können alle in diesem Ordner freigegebenen Bilder sehen.
4. Auf GitHub unter **Settings → Pages** die Source **Deploy from a branch**, **main**, **/(root)** aktivieren.
5. Danach bei **Settings → Pages → Custom domain** `fotobox.weidnernet.com` setzen und speichern (GitHub legt die CNAME-Datei an).
6. **Erst danach** bei World4You einen DNS-CNAME mit dem Host `fotobox` und Ziel `MasterLuke2020.github.io` hinzufügen. DNS-TXT-Verifizierung nach Bedarf konfigurieren.
7. Nach HTTPS-Bereitstellung Homepage `https://fotobox.weidnernet.com/` und Datenschutzseite `https://fotobox.weidnernet.com/datenschutz.html` in Google OAuth Branding eintragen und Publishing-Status prüfen.

**Niemals** ins öffentliche Repository stellen: Client Secret, Google-OAuth-JSON, rclone-Konfiguration, Aufnahmen oder Kundendaten.

Der vorhandene Gäste-QR-Code bleibt unabhängig von dieser Website weiterhin direkt mit dem bisherigen Google-Drive-Fotoordner verbunden.
