# MOHAA 100m Race Mod

Een Medal of Honor Allied Assault multiplayer mod waarbij 2 spelers tegen elkaar racen over 100 meter.

## Installatie

1. Kopieer **de bestanden uit de `main` folder** naar je MOHAA `main` folder:
   - Van: `mohaa_race_mod\main\*.scr`
   - Naar: `C:\Program Files (x86)\EA Games\Medal of Honor Allied Assault\main\`
   - Het eindresultaat moet zijn: `C:\...\MOHAA\main\dm_race.scr` (niet `main\main\dm_race.scr`!)

2. Start MOHAA en open de console met `~`

3. Laad een bestaande DM map, bijvoorbeeld:
   - `map dm/mohdm1` (Stalingrad)
   - `map dm/mohdm2` (Northern Italy)
   - `map dm/mohdm3` (Destroyed Village)
   - Of elke andere DM map

4. Type in de console: `exec global/dm_race.scr::main`

## Hoe te spelen

- Minimaal 2 spelers nodig
- Beide spelers worden automatisch naar de startlijn geteleporteerd
- 3-2-1-GO countdown
- Ren 100 meter naar de finish lijn
- De eerste speler die de finish bereikt wint de ronde
- Best of 5 rondes - eerste bij 3 punten wint de match

**Sprint:** MOHAA heeft geen native sprint support via scripting. Spelers kunnen handmatig een snelheidsboost gebruiken via console commando's indien gewenst.

## Configuratie

Je kunt de race aanpassen in `main/race_config.scr`:
- Afstand van de race (standaard 100m = 5000 units)
- Sprint snelheid
- Aantal rondes om te winnen

## Technische Details

**Gebaseerd op MOHAA modding voorbeelden:**
- Scripts gebruiken standaard MOHAA script syntax (geen kleurcodes)
- Print commando's: `iprintln`, `iprintlnbold`, `iprint`
- Voor geavanceerde HUD: gebruik `stufftext` met `globalwidgetcommand`
- Threading met `thread` en `waitthread`
- Variabelen met `local.` en `level.` prefix

**Compatibiliteit:**
- MOHAA versie 1.11 en hoger
- Werkt op alle DM maps
- Multiplayer ready (dedicated server support)

- `main/dm_race.scr` - Hoofd race script (execute dit)
- `main/race_config.scr` - Configuratie instellingen (optioneel)
- `main/race_hud.scr` - HUD elementen (optioneel)
- `main/player_sprint.scr` - Sprint mechanisme (optioneel)
- `main/race_100m.scr` - Legacy support (niet nodig)
