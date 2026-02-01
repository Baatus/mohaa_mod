# MOHAA 100m Race Mod

Een Medal of Honor Allied Assault multiplayer mod waarbij 2 spelers tegen elkaar racen over 100 meter.

## Installatie

1. Kopieer de `main` folder naar je MOHAA installatiemap
2. Start MOHAA en open de console met `~`
3. Laad een bestaande DM map, bijvoorbeeld:
   - `map dm/mohdm1` (Stalingrad)
   - `map dm/mohdm2` (Northern Italy)
   - `map dm/mohdm3` (Destroyed Village)
   - Of elke andere DM map
4. Type in de console: `exec global/dm_race.scr::main`

**Let op:** Zorg dat je de `main` folder uit dit project kopieert naar je MOHAA installatie (niet erin, maar vervang/merge).

## Hoe te spelen

- Minimaal 2 spelers nodig
- Beide spelers worden automatisch naar de startlijn geteleporteerd
- 3-2-1-GO countdown
- Ren 100 meter naar de finish lijn
- De eerste speler die de finish bereikt wint de ronde
- Best of 5 rondes - eerste bij 3 punten wint de match
- Gebruik sprint (default Shift) voor extra snelheid

## Configuratie

Je kunt de race aanpassen in `main/race_config.scr`:
- Afstand van de race (standaard 100m = 5000 units)
- Sprint snelheid
- Aantal rondes om te winnen

## Bestanden

- `main/dm_race.scr` - Hoofd race script (execute dit)
- `main/race_config.scr` - Configuratie instellingen (optioneel)
- `main/race_hud.scr` - HUD elementen (optioneel)
- `main/player_sprint.scr` - Sprint mechanisme (optioneel)
- `main/race_100m.scr` - Legacy support (niet nodig)
