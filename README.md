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
