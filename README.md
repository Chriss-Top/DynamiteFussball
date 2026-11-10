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
