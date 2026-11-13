# 🏝️ Annes Inseltag – Live-Ticker

Eine kleine 3D-Insel, auf der deine Zuschauer:innen live mitverfolgen, wie du eine Aufgabe erledigst.

- **Zuschauerseite:** `https://<dein-user>.github.io/potential-octo-couscous/` – ohne Login.
- **Regie-Pult:** dieselbe Adresse mit `#regie` am Ende – Login mit einem GitHub-Token.

## Wie es funktioniert
Alle Inhalte stehen in `data.json`. Das Regie-Pult schreibt über die GitHub-API in diese Datei,
die Zuschauerseite fragt sie alle 20 Sekunden ab. Kein Server, keine Datenbank.

## Token fürs Regie-Pult
GitHub → Settings → Developer settings → Personal access tokens → **Fine-grained tokens** → *Generate new token*
- Repository access: *Only select repositories* → `potential-octo-couscous`
- Permissions → Repository → **Contents: Read and write**

Den Token einmal im Regie-Pult einfügen; er bleibt nur in deinem Browser gespeichert.

> Hinweis: Das Repo ist öffentlich, also auch `data.json`. Schreib dort nichts rein, was nicht jeder lesen darf.
