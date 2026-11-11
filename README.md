# Dynamite Fußball

Ein kleines browserbasiertes Elfmeter-Spiel: fünf Schüsse, ein beweglicher Torwart und eine Partikel-Explosion bei jedem Tor.

## Starten

`index.html` direkt im Browser öffnen oder im Projektordner einen lokalen Server starten:

```sh
python3 -m http.server 8000
```

Keine Installation, Build-Schritte oder Zugangsdaten erforderlich.

## Steuerung

- Maus oder Touch: Zielpunkt setzen.
- Pfeiltasten: Zielpunkt verschieben.
- „Schießen“ oder Leertaste: schießen. Höhere Schusskraft bedeutet einen schnelleren Ball.
- „Neue Runde“: Punktestand zurücksetzen.

Der Torwart hält nahe Schüsse in seiner Reichweite; hohe Schüsse und freie Ecken helfen. Nach fünf Schüssen erscheint das Ergebnis.

## Spielmodi

Über „Spielmodus“ zwischen Computergegner und **2 Spieler · lokal** am selben Gerät wechseln. Ein Wechsel setzt die Runde zurück.

- **Schütze:** Maus/Touch oder Pfeiltasten zum Zielen; Schuss-Button oder Leertaste zum Schießen.
- **Torwart im Zweispieler-Modus:** Vor jedem Schuss verdeckt eine Abwehrzone per Tastendruck festlegen: Q/W/E für oben links/Mitte/rechts, A/S/D für unten links/Mitte/rechts. Der Schütze schaut bei der Eingabe weg. Dafür wird eine Tastatur benötigt.
- Erst nach dieser Wahl werden Zielpunkt und Schuss freigegeben. Der Torwart bleibt sichtbar in der Mitte; seine Wahl wird erst beim Schuss aufgedeckt. Sie lässt sich bis zum nächsten Elfmeter nicht ändern, auch nicht während des Ballflugs.
- Fünf Schüsse pro Runde; die Rollen können nach einer Runde durch die Spieler getauscht werden.
- Im Computer-Modus bewegt sich der Torwart automatisch; Q/W/E/A/S/D haben dort keinen Einfluss.

Das gesamte Spiel bleibt in `index.html` enthalten und funktioniert ohne Internetverbindung.

## 2 gegen 2 · Bandenfußball

Im Spielmodus **2 gegen 2 · Bandenfußball** spielt jedes Team mit einem Menschen und einem Computer aus der Vogelperspektive. Pro Team Land sowie unterschiedliche Spieler für Mensch und Computer auswählen, dann **Anpfiff / Neues Spiel** drücken. Änderungen an der Aufstellung setzen das Spiel zurück.

- Team 1: WASD bewegen, F schießen; spielt auf das rechte Tor.
- Team 2: Pfeiltasten bewegen, Enter schießen; spielt auf das linke Tor.
- In Ballnähe schießen; die letzte Laufrichtung bestimmt die Schussrichtung. Der Computer läuft zum Ball oder bietet sich als Unterstützung an und schießt selbstständig.
- Der Ball prallt an den Banden ab; nur die beiden Toröffnungen zählen als Tore. Nach einem Tor folgt ein neuer Anstoß.
- Nach 90 Sekunden endet das Spiel mit Ergebnis. Beide Menschen benötigen dieselbe Tastatur; dieser Modus ist für den Desktop gedacht.

Auch dieser Modus benötigt keine Installation und keine Internetverbindung.
