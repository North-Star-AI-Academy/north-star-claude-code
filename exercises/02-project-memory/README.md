# Level 2: Project Memory — Laat Claude je project onthouden

## Doel
Begrijpen hoe CLAUDE.md werkt en waarom het cruciaal is. Zonder CLAUDE.md verspilt Claude tot 33.000 tokens aan het "begrijpen" van je project — elke keer opnieuw.

## Theorie

Claude Code leest automatisch deze bestanden:
1. **`CLAUDE.md`** in je project root — projectregels en context
2. **`~/.claude/CLAUDE.md`** — persoonlijke regels (voor al je projecten)
3. **`.claude/settings.json`** — technische instellingen

## Opdrachten

### 2.1 — Analyseer het bestaande CLAUDE.md
Vraag Claude: "Analyseer het CLAUDE.md bestand van dit project. Wat staat erin en waarom?"

### 2.2 — Maak je eigen CLAUDE.md
Maak een nieuw project aan (simulatie) en schrijf er een CLAUDE.md voor:

```
Maak een map `mijn-marketing-project/` met een CLAUDE.md bestand voor een
fictief marketingbureau. Het bureau heet "Bright Spark" en is gespecialiseerd
in B2B SaaS marketing. Ze gebruiken HubSpot, Figma, en schrijven content in
het Nederlands.
```

Een goed CLAUDE.md bevat:
- Wat het project is (1-2 zinnen)
- Tech stack / tools
- Conventies (taal, tone of voice, naamgeving)
- Belangrijke bestanden en mappenstructuur
- Wat Claude wel en niet mag doen

### 2.3 — Globale regels instellen
Maak een persoonlijk regelsbestand:

```
Maak een bestand ~/.claude/CLAUDE.md met mijn persoonlijke voorkeuren:
- Ik ben een marketeer, geen developer
- Antwoord altijd in het Nederlands tenzij ik Engels vraag
- Houd uitleg simpel en praktisch
- Gebruik geen technisch jargon zonder uitleg
```

### 2.4 — Product Context instellen
Gebruik de product-context skill:
```
/product-context
```
Vul de vragen in voor je eigen bedrijf of een fictief bedrijf. Dit bestand wordt automatisch gebruikt door alle marketing skills.

## Checklist
- [ ] Je begrijpt wat CLAUDE.md doet
- [ ] Je hebt een eigen CLAUDE.md geschreven
- [ ] Je hebt globale regels ingesteld
- [ ] Je hebt een product-context.md aangemaakt

## Klaar?
Ga door naar Level 3: `/start-exercise 3`
