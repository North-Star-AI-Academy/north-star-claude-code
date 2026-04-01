# Level 5: Context Management — Je context window als budget

## Doel
Begrijpen hoe de context window werkt, wanneer het vol raakt, en hoe je het efficiënt beheert.

## Theorie

Claude Code heeft een context window van ~200K tokens. Dit klinkt veel, maar het vult snel:
- Elk bestand dat Claude leest: 100-5000+ tokens
- Elke tool call en resultaat: tokens
- Je hele conversatiegeschiedenis: tokens

**De drie regels:**
1. **Begin elke taak schoon** — Start een nieuwe sessie (`/clear`) voor een nieuwe taak
2. **Comprimeer regelmatig** — Gebruik `/compact` als je merkt dat Claude trager wordt
3. **Wees specifiek** — "Fix de bug in `src/header.tsx` regel 42" is beter dan "er is een bug ergens"

## Opdrachten

### 5.1 — Context status bekijken
Kijk naar de statusbalk onderaan je terminal. Je ziet:
- Hoeveel tokens je hebt gebruikt
- Hoeveel er nog over is
- Het percentage gebruikt

Voer een paar taken uit en bekijk hoe de counter stijgt.

### 5.2 — Compact ervaren
1. Stel Claude een paar vragen (5-10 berichten)
2. Bekijk de token counter
3. Typ `/compact`
4. Bekijk hoe de counter daalt

Claude comprimeert de conversatie naar de kern — het onthoudt wat belangrijk is en vergeet de details.

### 5.3 — Efficiënt werken
Vergelijk deze twee aanpakken:

**Slecht** (verspilt context):
```
Lees alle bestanden in de exercises map en geef een samenvatting van elk.
```

**Goed** (zuinig met context):
```
Lees exercises/05-context-management/README.md en geef de kernpunten.
```

### 5.4 — Nieuwe sessie starten
Wanneer je aan een compleet nieuwe taak begint:
1. Typ `/clear` om de sessie te resetten
2. Of sluit Claude Code en start opnieuw

Dit geeft je een vers context window van 200K tokens.

### 5.5 — Sub-agents begrijpen
Claude kan sub-agents spawnen voor parallelle taken. Elke sub-agent krijgt zijn eigen context window:

```
Onderzoek tegelijkertijd:
1. De beste LinkedIn post formaten voor B2B
2. De beste tijden om te posten op LinkedIn in Europa
3. Voorbeelden van virale LinkedIn posts in de marketing niche
```

Claude stuurt drie sub-agents tegelijk — sneller en efficiënter.

## Checklist
- [ ] Je begrijpt de drie regels van context management
- [ ] Je hebt `/compact` gebruikt en het effect gezien
- [ ] Je weet wanneer je een nieuwe sessie moet starten
- [ ] Je begrijpt hoe sub-agents werken

## Klaar?
Ga door naar Level 6: `/start-exercise 6`
