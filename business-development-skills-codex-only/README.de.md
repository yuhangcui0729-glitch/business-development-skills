# Business Development — Drei Coaching-Skills für Codex (EN/DE)

Dieses Repository enthält drei Workshops für die Lehrveranstaltung Business Development (2026W). Die Skills können **auf Englisch oder Deutsch** verwendet werden:

1. **Business Model Canvas Coach** — ein erstes Geschäftsmodell entwickeln und Annahmen hinterfragen.
2. **Market & Marketing Coach** — SWOT, Wettbewerb, Positionierung und Marketing-Mix.
3. **Finance & Legal Issues** — Kosten, Preise, Vertrieb, Förderung und rechtliche Fragen in Österreich.

[English instructions](README.md)

## Anleitung für Studierende: Installation in Codex

**Voraussetzung:** Zugang zu einer Codex-Umgebung, die Skills und den `$skill-installer` unterstützt, sowie Internetzugang zu GitHub. Die Anleitung gilt für **Codex**, nicht für die normale Skills-Oberfläche von ChatGPT. Die Verfügbarkeit hängt vom Konto und von der Codex-Version ab.

1. Öffne **Codex** und beginne eine neue Unterhaltung.
2. Schicke die folgenden Befehle jeweils **als Nachricht im Codex-Chat** (nicht im Terminal). Ersetze `YOUR-USERNAME` durch den GitHub-Benutzernamen bzw. die Organisation. Wenn das Repository anders heißt, passe auch `business-development-skills` an.

   **Workshop 1 — Business Model Canvas**

   ```text
   $skill-installer install https://github.com/YOUR-USERNAME/business-development-skills/tree/main/skills/business-model-canvas-coach
   ```

   **Workshop 2 — Market & Marketing**

   ```text
   $skill-installer install https://github.com/YOUR-USERNAME/business-development-skills/tree/main/skills/market-and-marketing-coach
   ```

   **Workshop 3 — Finance & Legal Issues**

   ```text
   $skill-installer install https://github.com/YOUR-USERNAME/business-development-skills/tree/main/skills/finance-and-legal-issues
   ```

3. **Starte Codex nach der Installation neu**, damit die Skills erkannt werden. Normalerweise muss jeder Skill nur einmal installiert werden.
4. Beginne **für jeden Workshop einen eigenen Chat** und verwende in allen drei Workshops dieselbe Geschäftsidee. Aktiviere den jeweiligen Skill ausdrücklich:

   ```text
   Use the business-model-canvas-coach skill. Los geht's!
   ```

   Danach:

   ```text
   Use the market-and-marketing-coach skill. Los geht's!
   ```

   Zum Schluss:

   ```text
   Use the finance-and-legal-issues skill. Los geht's!
   ```

   Gib zu Beginn des zweiten und dritten Workshops auch die abschließende Zusammenfassung des vorherigen Workshops an.
5. Begründe deine Entscheidungen, hinterfrage KI-Vorschläge und entwickle deine Idee eigenständig weiter. Beachte für **Abgabe und Reflexion** die aktuelle Prüfungsanleitung auf Moodle.

**Wenn die Installation nicht klappt:** Prüfe, ob das Repository öffentlich ist, der GitHub-Benutzername im Link stimmt und deine Codex-Version `$skill-installer` unterstützt. Die Befehle gehören in den Codex-Chat, nicht ins Terminal. Bei bereits installierten Skills gelten die Update-Anweisungen deiner Codex-Version.

**Wichtig zur Abgabe:** Nicht jede Codex-Umgebung bietet dieselbe Funktion zum Teilen vollständiger Chats wie ChatGPT. Kläre bei Bedarf mit der Lehrperson, wie die Gespräche abgegeben werden sollen.

## Repository-Struktur

```text
business-development-skills/
├── README.md
├── README.de.md
└── skills/
    ├── business-model-canvas-coach/
    ├── market-and-marketing-coach/
    └── finance-and-legal-issues/
```

Jeder Skill-Ordner enthält `SKILL.md`, ergänzende `references/` und Assets. Der ganze Ordner muss erhalten bleiben.

## Für die Lehrperson: GitHub-Veröffentlichung

1. Unter https://github.com/new ein **öffentliches** Repository erstellen, z. B. `business-development-skills`.
2. Kein zusätzliches README beim Erstellen auswählen.
3. Das bereitgestellte Repository-ZIP entpacken und **alle Inhalte** (beide READMEs und den Ordner `skills/`) hochladen; anschließend committen.
4. In den drei Installationsbeispielen `YOUR-USERNAME` durch den tatsächlichen GitHub-Namen ersetzen und erst dann den Link mit den Studierenden teilen.

## Rechte und Datenschutz

Es wurde keine Lizenz hinzugefügt. Vor der öffentlichen Veröffentlichung ggf. Rechte an Materialien und Bildern prüfen und über eine Lizenz entscheiden. Individuelle Studierenden-Chats gehören nicht in dieses Repository.

Referenz: [OpenAI Skill Installer](https://github.com/openai/skills/blob/main/skills/.system/skill-installer/SKILL.md).
