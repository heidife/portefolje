# Porteføljeside: Heidi F. Enger Otone

Dette er porteføljesiden til Heidi F. Enger Otone (innhold og kommunikasjon, Oslo). Den legges ved jobbsøknader, så den skal være kort og vise arbeidene, ikke CV-en.

## Om Heidi og hvordan du jobber med henne
- Skriv til henne på norsk, konkret og uformelt.
- Hun lærer GitHub og Claude Code. Forklar kort hva du gjør og hvorfor, gjerne med enkle bilder. Bruk vanlige ord og ikke faguttrykk uten forklaring.
- Vær ærlig og si ifra hvis noe er en dårlig idé.

## Oppbygging
- Én fil: `index.html` (HTML, CSS og JavaScript i samme fil). Bilder ligger i `img/`.
- Publiseres med GitHub Pages fra `main`-grenen. En push til `main` oppdaterer siden etter et minutt eller to.
- Siden har menyen **Hjem** og **Arbeid**, og sidene styres med `#` i adressen:
  - `#hjem` (standard): rundt portrett (`img/heidi.jpeg`), navn, kort tekst om Heidi, LinkedIn og e-post. Deretter «/Tidligere arbeid» med tre ikonbokser, og «/Hva gjør jeg» med sammenleggbare lister.
  - `#arbeid`: de samme tre ikonboksene.
  - `#tekster`, `#kampanje`, `#foto`: én side per kategori med arbeidene i et rutenett.
  - `#lofavor`: egen prosjektside for LOfavør-saken. Teksten ligger i `CASE_HTML` i `index.html`.
- De tre ikonboksene er Tekst og innhold (ark med penn), Kampanje og CRM (megafon) og Foto (kamera). Ikonene er tegnet direkte i koden (SVG) og har en liten animasjon når man holder musa over.
- Innholdet ligger i JavaScript-objektene nederst i `index.html`:
  - `WORKS`: hvert arbeid (tittel, kicker-linje, rolle, bilde, lenke eller bildeliste)
  - `SERIES`: de fire artiklene i Livsløpserien
  - `SLOTS`: hvilke arbeider som vises i hver kategori (`texts`, `campaign`, `photos`)
  - `CATS`: kobler adressen (`tekster`, `kampanje`, `foto`) til tittel og riktig `SLOTS`-liste
- Nytt arbeid: legg bildet i `img/` (komprimert, maks ca. 1200 px bredt), legg til et innslag i `WORKS` og sett det inn i riktig `SLOTS`-liste.
- Sjekk at alle bildefiler som `index.html` viser til faktisk finnes i `img/`. Filnavnet må stemme helt, også endelsen (`.jpg` og `.jpeg` er ikke det samme).

## Designregler (hentet fra CV-en hennes i Figma)
- Kun svart og hvitt (og svake gråtoner). Ingen farger.
- Skrift: Montserrat på hele siden (lastes fra Google Fonts). Små detaljer (type, kunde, år, e-post, etiketter som «/Tidligere arbeid») står i liten skrift, ofte med store bokstaver og luft mellom bokstavene. Tidligere var det Inter og IBM Plex Mono. Det står fortsatt igjen i koden, men Montserrat overstyrer det.
- Rent og luftig: hvert arbeidskort viser bare bilde, kicker-linje (type · kunde · år), tittel og én linje om hva Heidi gjorde. Ingen merker eller lange beskrivelser.

## Fakta om arbeidene
- Kundehistoriene og Livsløpserien er laget for Fremtind og publisert på sparebank1.no.
- LOfavør-saken er et markedssamarbeid mellom Fremtind og LOfavør (2025–2026). Kortet har ikke bilde, bare «+35 %» på grå bakgrunn (bevisst valg). Annonsene (`lo-ad-1.jpg` til `lo-ad-3.jpg`) er skjermbilder fra kampanjen, ikke foto tatt av Heidi.
- Bildene i vannlekkasje-saken og alle fotoprosjektene er tatt av Heidi.
- Bildene i barneforsikring-saken og Livsløpserien er IKKE tatt av Heidi. Ikke krediter dem til henne.
