# Zellbiologie

## Zellmodell im Browser

Die Grafik ist nach dem ersten erfolgreichen Deployment unter
<https://chaoscatalogue.github.io/Zellbiologie/> erreichbar. Der Workflow
`Deploy cell model to GitHub Pages` veröffentlicht bei Änderungen an
`main` automatisch `Zellmodell-Code.txt` als `index.html`. Diese Datei ist die
einzige Quelle für die gehostete Grafik; neue Modellfunktionen müssen dort
ergänzt werden.
`Zellmodell-Grafik.html` ist eine separate Kopie und nicht die Quelle für die
gehostete Seite. Der Workflow läuft nach jedem Push auf `main` und kann
zusätzlich manuell gestartet werden.

**Einmalige GitHub-Einrichtung erforderlich:** Das Repository bleibt privat,
die veröffentlichte Website ist öffentlich. GitHub Pages unterstützt dieses
Setup nur mit einem dafür geeigneten kostenpflichtigen Plan; der aktuelle
GitHub-Free-Plan liefert dafür HTTP 422. Repository-Eigentümer müssen Pages
für das private Repository mit einem geeigneten Plan freischalten und unter
**Settings → Pages** als Build-Quelle **GitHub Actions** auswählen. Die
Repository-Sichtbarkeit muss dafür nicht geändert werden. Anschließend
veröffentlicht der vorbereitete Workflow bei jedem Push auf `main` oder bei
manuellem Start die jeweils aktuelle `Zellmodell-Code.txt`.