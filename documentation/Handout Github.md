Damit das Git-Handout spezifisch für die Verwendung von Git in **VS Code** ist, werde ich die Anleitung anpassen, um die Integration von Git mit **GitHub** und **Source Control** in **VS Code** zu erklären. Hier ist eine aktualisierte Version des Handouts, das du in deiner `README.md`-Datei verwenden kannst.

---

# Git-Handout für Anfänger (VS Code Edition)

## Was ist Git und warum sollte es verwendet werden?

**Git** ist ein verteiltes Versionskontrollsystem, das es Entwicklern ermöglicht, die Entwicklung ihrer Projekte zu verfolgen, Änderungen zu versionieren und effizient in Teams zu arbeiten. Es ermöglicht:

- **Versionskontrolle**: Jede Änderung am Code wird nachvollziehbar gespeichert.
- **Teamarbeit**: Entwickler können gleichzeitig an verschiedenen Teilen eines Projekts arbeiten, ohne Konflikte zu verursachen.
- **Wiederherstellung**: Frühere Versionen des Projekts können leicht wiederhergestellt werden.

**GitHub** ist eine Plattform, die Git-Repositories hostet und die Zusammenarbeit in Teams erleichtert, indem sie Remote-Repositories für Projekte bereitstellt.

---

## Git und VS Code: Erste Schritte

### Git in VS Code einrichten

1. **VS Code herunterladen und installieren**:
   Falls noch nicht geschehen, lade [VS Code](https://code.visualstudio.com/) herunter und installiere es.

2. **Git in VS Code integrieren**:
   - Öffne VS Code und gehe in die **Source Control**-Ansicht (das Symbol mit den Gabeln links in der Seitenleiste).
   - Falls Git nicht installiert ist, wird eine Meldung angezeigt. Folge den Anweisungen, um Git zu installieren oder es in VS Code zu aktivieren.

3. **GitHub-Konto verknüpfen**:
   - Klicke in VS Code unten links auf das Git-Symbol.
   - Melde dich mit deinem GitHub-Konto an, um VS Code mit GitHub zu verknüpfen.

---

## Grundlegende Git-Befehle in VS Code

Hier sind die wichtigsten Git-Befehle, die direkt in VS Code ausgeführt werden können:

### 1. **Repository initialisieren (git init)**

- Um ein neues Git-Repository zu initialisieren, gehe in VS Code in das Terminal (`Terminal > New Terminal` oder STRG + `).
- Führe folgenden Befehl aus:
  ```bash
  git init
  ```

- Alternativ kannst du auf „Initialize Repository“ in der **Source Control**-Ansicht klicken, wenn du ein neues Projekt beginnst.

### 2. **Dateien hinzufügen (git add)**

- In der **Source Control**-Ansicht siehst du alle Änderungen, die noch nicht zur Versionierung hinzugefügt wurden. Wähle die Änderungen aus und klicke auf das „+“-Symbol, um sie zur Staging Area hinzuzufügen.
- Alternativ kannst du im Terminal folgenden Befehl ausführen:
  ```bash
  git add .
  ```

### 3. **Änderungen committen (git commit)**

- Nachdem du Dateien hinzugefügt hast, schreibe eine Commit-Nachricht direkt in der **Source Control**-Ansicht und klicke auf den Haken, um den Commit durchzuführen.
- Oder verwende im Terminal:
  ```bash
  git commit -m "Beschreibe hier deine Änderungen"
  ```

### 4. **Änderungen pushen (git push)**

- Um die lokalen Commits in dein GitHub-Repository hochzuladen, klicke in der **Source Control**-Ansicht auf „Synchronize Changes“. Das entspricht dem `git push`-Befehl.
- Alternativ kannst du den folgenden Befehl im Terminal ausführen:
  ```bash
  git push origin main
  ```

---

## Arbeiten mit Branches in VS Code

### 1. **Einen neuen Branch erstellen (git branch)**

- Klicke unten links in VS Code auf den Branch-Namen (normalerweise `main`) und wähle „Create New Branch“.
- Oder führe den folgenden Befehl im Terminal aus:
  ```bash
  git checkout -b neuer-branch-name
  ```

### 2. **Branch wechseln (git checkout)**

- Klicke erneut auf den aktuellen Branch-Namen und wähle den Branch aus, zu dem du wechseln möchtest.
- Im Terminal:
  ```bash
  git checkout branch-name
  ```

### 3. **Branch mergen und Merge-Konflikte lösen**

- Nachdem du an deinem Branch gearbeitet hast, gehe zum Hauptbranch zurück:
  ```bash
  git checkout main
  ```

- Um den Branch zu mergen, verwende den Befehl:
  ```bash
  git merge branch-name
  ```

- Bei Merge-Konflikten zeigt VS Code automatisch die betroffenen Dateien an. Verwende die **Vergleichsansicht**, um die Konflikte zu lösen, und committe die Änderungen nach der Konfliktlösung.

---

## Git mit VS Code: IntelliJ/PyCharm-Integration (ähnliche IDEs)

**VS Code** bietet ähnliche Funktionen wie die IntelliJ-Produktreihe (IntelliJ IDEA, PyCharm). Mit der Git-Integration kannst du einfach:
- Änderungen verfolgen und in die Versionskontrolle einbinden.
- Branches erstellen und verwalten.
- Pull Requests direkt in VS Code erstellen und bearbeiten.

---

## Nützliche Git-Tools und Plattformen

- **GitHub**: Eine Plattform zum Hosten von Git-Repositories und zur Zusammenarbeit in Teams.
- **GitLab**: Eine Alternative zu GitHub, die ähnliche Funktionen bietet.
- **Bitbucket**: Weitere Plattform für Git-Repositories.

---

## Pull Requests und Reviews

### 1. **Pull Request erstellen**
- Sobald du deine Arbeit abgeschlossen hast, erstelle auf GitHub einen Pull Request, um deinen Branch in den Hauptbranch zu mergen. Dies ist in VS Code über das „GitHub Pull Requests“-Plugin möglich.

### 2. **Code Reviews**
- Überprüfe die Pull Requests deiner Teammitglieder und gebe Feedback, bevor du sie genehmigst.

---

## Beitrag der Teammitglieder

- **Marcell Wolf de Lêu**: Grundlegende Git-Befehle und Branches.
- [Weitere Teammitglieder und deren Beiträge]

---

Damit hast du eine Anleitung, wie Git in **VS Code** verwendet werden kann, und wie typische Workflows mit GitHub und Source Control direkt aus der IDE gesteuert werden.

Wenn du noch Fragen hast oder Unterstützung beim Einfügen ins Repository brauchst, sag Bescheid!