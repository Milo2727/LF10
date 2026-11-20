Der Workflow startet, wenn ich etwas hochlade, einen Pull Request auf main erstelle oder ihn selbst starte.

Er läuft auf ubuntu-latest. GitHub stellt dafür einen Ubuntu-Rechner bereit.

Der Job heißt stack-test und hat 10 Schritte.

Schritt 1 benutzt actions/checkout@v7. Die anderen Schritte führen eigene Befehle aus.

Der Workflow darf die Dateien nur lesen. Das ist sicherer, weil er nichts verändern kann.

In der Vorlage wird der Test übersprungen. In meinem Repository läuft er normal.

a) Schritt 3, YAML-Syntax
b) Schritt 7, Inhalt prüfen
c) Schritt 6, Erreichbarkeit
d) Schritt 2, Compose-Datei suchen

Nur weil der Port funktioniert, heißt das nicht, dass die richtige Webseite angezeigt wird. Deshalb wird auch meine HTML-Datei geprüft.

Schritt 10 räumt nach dem Test auf, damit keine alten Container übrig bleiben.

Das ist Continuous Integration, weil Änderungen automatisch getestet werden. Auf meinen Server wird dabei nichts automatisch übertragen.



Fehler werden automatisch erkannt.

Die Tests laufen immer gleich ab und man kann die Ergebnisse später sehen.
