# Dagens rutiner

En lille web-app til faste rutiner for børn: opgaver på faste tidspunkter, valg mellem aktiviteter, tidtagning, en skydebane-belønning og statistik over tidligere tider.

## Funktioner

- Tidslinje over dagens opgaver med tidspunkt, ikon og tekst
- Aktiviteter at vælge imellem pr. opgave (fx Ro-tid: læs, tegn, kortspil, putte)
- Tidtagning med rekord at slå
- Straffespark mod et fodboldmål med en hurtig målmand i fuld målhøjde efter hver opgave: 3 skud, flest point i hjørnerne, bonus for ny rekord
- Statistik: rekord, gennemsnit, sidste 7 dage, seneste tider og foretrukne aktiviteter
- Indstil er låst med en 4-cifret kode
- Nulstil dagen (kræver koden), hvis dagens opgaver skal tages forfra
- Alarm med lyd, mens appen er åben
- Kan installeres på hjemmeskærmen og virker offline

## Kom i gang med GitHub Pages

1. Opret et nyt repository og læg alle filerne i roden.
2. Gå til **Settings → Pages**, vælg branch `main` og mappen `/ (root)`, og gem.
3. Efter et minut ligger appen på `https://<brugernavn>.github.io/<repo>/`.
4. Åbn adressen på telefon eller tablet og vælg **Føj til hjemmeskærm**.

## Godt at vide

- Data gemmes i browserens lokale lager på den enkelte enhed. Rydder man browserdata, forsvinder opgaver og statistik.
- Alarmen lyder kun, når appen er åben på skærmen. En web-app kan ikke vække en låst telefon.
- Koden til Indstil er en børnelås, ikke egentlig sikkerhed. Har man glemt den, kan den nulstilles via **Glemt koden?** med et regnestykke.
- Ved ændringer i filerne: hæv `CACHE`-versionen i `sw.js`, så enhederne henter den nye udgave.

## Filer

| Fil | Indhold |
|---|---|
| `index.html` | Hele appen (HTML, CSS og JavaScript i én fil) |
| `manifest.webmanifest` | Navn og ikoner til installation |
| `sw.js` | Service worker til offline-brug |
| `icon.svg`, `icon-*.png` | App-ikoner |
