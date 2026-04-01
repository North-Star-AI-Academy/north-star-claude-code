# Level 6: Git Workflows — Versiebeheer met Claude

## Doel
Leer hoe Claude Code samenwerkt met Git voor versiebeheer, branches, en worktrees.

## Theorie

Claude Code begrijpt Git natively. Het kan:
- Commits maken met goede berichten
- Branches aanmaken en beheren
- Merge conflicts oplossen
- Git worktrees gebruiken voor parallelle features

## Opdrachten

### 6.1 — Je eerste commit met Claude
Maak een wijziging en laat Claude committen:

```
Voeg een bestand toe: mijn-marketing-plan.md met een korte beschrijving
van 3 marketing doelen voor Q2 2026. Commit dit met een duidelijk bericht.
```

Let op: Claude maakt een descriptieve commit message en staged alleen relevante bestanden.

### 6.2 — Branching
```
Maak een nieuwe branch "feature/linkedin-strategie" en voeg daar een
bestand linkedin-plan.md toe met een 4-weeks content plan. Commit op
die branch.
```

### 6.3 — Git worktrees (geavanceerd)
Worktrees laten je aan meerdere branches tegelijk werken, elk in een eigen map:

```
Leg uit wat git worktrees zijn en wanneer ik ze zou gebruiken.
Geef een praktisch voorbeeld voor een marketeer die tegelijk aan
een blog post en een email campagne werkt.
```

### 6.4 — Commit geschiedenis bekijken
```
Bekijk de git log van dit project en geef een samenvatting van
de laatste 5 commits.
```

### 6.5 — Goede commit messages
Claude schrijft standaard goede commits, maar je kunt het sturen:

```
Maak een wijziging aan het README.md (voeg een sectie "Mijn Notities" toe)
en commit met een conventionele commit message (feat:, fix:, docs:, etc.)
```

## Tips
- Claude vraagt altijd toestemming voordat het commit of pusht
- Claude pusht NOOIT automatisch naar remote — je moet expliciet vragen
- Gebruik branches voor experimenten, merge naar main als je tevreden bent

## Checklist
- [ ] Je hebt een commit gemaakt via Claude
- [ ] Je hebt een branch aangemaakt
- [ ] Je begrijpt wat worktrees zijn
- [ ] Je kunt de git geschiedenis bekijken via Claude

## Klaar?
Ga door naar Level 7: `/start-exercise 7`
