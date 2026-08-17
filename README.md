# Akquise-Entwuerfe STIL x Architektur

Unbeauftragte Vorleistung fuer den Lead in Zeile 3 von `Akquise\LeadsMit.xlsx`
(10 Punkte, Hauptmangel `veraltet`), gebaut aus dem echten Material des
Bueros in `material/`.

## Die drei Entwuerfe

| | Entwurf 1 (dieser Ordner) | [Entwurf 2](entwurf-2-originalnah/) | [Entwurf 3](entwurf-3-editorial/) |
| --- | --- | --- | --- |
| Kurz | Feldverbund, dunkel, technisch | nah am Bestand, nur modernisiert | hell, typografisch, neu geordnet |
| Umfang | **eine Startseite** | vollstaendig, 17 Seiten | vollstaendig, 11 Seiten |
| Struktur | One-Pager mit Sprungnavigation | Menue und Untermenues wie im Original | neu gegliedert, Leistungen eigener Punkt |
| Farbwelt | Anthrazit + Orange | Weiss, Grau `#666`, Orange `#FF6600` wie im Original | warmes Weiss, Orange stark zurueckgenommen |
| Schrift | Systemgrotesk, grosse Sprünge | Arial wie im Original | Systemserife + Grotesk |
| Wiedererkennung fuer den Inhaber | gering | **hoch** | mittel |
| Stand | 11.08.2026 | 12.08.2026 | 12.08.2026 |

**Empfehlung fuer das Gespraech:** Entwurf 2 zuerst zeigen. Der Inhaber
erkennt seine Seite wieder, sieht aber sofort, was Responsivitaet, echte
Unterseiten und der Wegfall von Analytics und Cookie-Banner bringen - das
senkt die Hemmschwelle. Entwurf 3 danach als Antwort auf die Frage "und wenn
wir groesser denken?". Entwurf 1 nur, wenn ein deutlich technischeres Bild
gewuenscht ist; er ist ausserdem nur eine Startseite.

Gemeinsam ist allen dreien: keine externen Requests, keine Cookies, kein
Tracking, kein Kontaktformular. Die offenen Fragen an den Inhaber sind
dieselben - sie stehen unten und ausfuehrlicher in
[entwurf-2-originalnah/README.md](entwurf-2-originalnah/README.md).

---

# Entwurf 1 - Feldverbund

Eine Startseite. Stand: 11.08.2026.

## Gestaltungsentscheidung

> Ein Buero, dessen Inhaber als Maurergeselle angefangen hat und das heute
> Waende vorproduziert auf die Baustelle stellt - die Seite wird sichtbar aus
> Feldern gesetzt, mit schmalen Fugen dazwischen, sachlich wie eine
> Ausfuehrungsplanung.

Daraus folgt konkret:

- **Feldverbund statt Abschnittsstapel.** Jeder Bereich ist ein Raster aus
  Feldern mit 1 px Fuge, unterschiedlich gross. Die Fuge entsteht ueber `gap`
  auf eingefaerbtem Rastergrund, nicht ueber Rahmen - so laufen die Kanten
  auch dann durch, wenn Felder umbrechen.
- **Zwei Farben.** Anthrazit und das Orange aus dem eigenen Logo. Es ist
  dasselbe Orange, in dem der Liebermann-Satz an der Wand des Empfangs steht
  (zu sehen auf `bilder/buero-eingang-empfang.jpg`). Fuer Text auf hellem
  Grund wird die abgedunkelte Variante `#b85100` benutzt, weil das reine
  Orange auf Weiss nur 2.7:1 Kontrast haette.
- **Systemschrift mit grossem Groessensprung** statt einer zweiten Schriftart.
  Das Buero definiert sich ueber Technik - BIM, Revit, serielles Bauen -, nicht
  ueber Handwerksromantik. Eine Serifenschrift waere dagegen gearbeitet.
- **Das Motiv:** der Liebermann-Satz steht gross gesetzt direkt neben dem Foto,
  auf dem er an der Buerowand zu sehen ist. Ohne erklaerenden Zusatz. Zweites
  Motiv ist die 75-Tage-Zahl aus Projekt BCK09 - eine nachpruefbare Zahl, die
  kein anderes Buero so hat.

Keine Rueckfrage gestellt: Grau und Orange sind durch das Logo vorgegeben, die
sachliche Richtung durch die Inhalte. Eine zweite Richtung war nicht gleich
plausibel.

## Aufbau

One-Pager mit Sprungnavigation. Jeder Menuepunkt zeigt auf einen Abschnitt,
den es gibt: Das Buero, Leistungen, Projekte, Bauen 4.0, Kontakt.

## Was bewusst fehlt

- **Oeffnungszeiten.** Nirgends belegt; oeffnungszeitenbuch.de meldet
  ausdruecklich, dass keine hinterlegt sind. Auch kein "Termine nach
  Vereinbarung" - das waere geraten. Die Seite beantwortet die Erreichbarkeit
  ueber Telefon, Fax und E-Mail.
- **Impressum und Datenschutz.** Der Aufhaenger ist `veraltet`, nicht
  `kein Impressum` - der Entwurf bleibt deshalb bei einer Datei. Beides
  gehoert in den beauftragten Ausbau.
- **Kontaktformular.** Eine Anfrage soll beim Buero landen, nicht bei mir.
  Die CSP setzt `form-action 'none'`.
- **Karte.** Wuerde einen fremden Server laden; nicht erlaubt.
- **Logoleiste** (Architektenkammer, BAFA, BinBau). Die Logos liegen nur in
  31 bis 75 px Breite vor. Die Mitgliedschaften stehen deshalb als Text.
- **Teamgroesse und Gruendungsjahr des Bueros.** Nicht sauber belegt, siehe
  `material/MATERIAL.md`.

## Offene Fragen an den Inhaber

1. **Hausnummer:** Das Impressum der alten Seite schreibt "Jordanstr. 26", die
   Kontaktseite und der eigene Google-Maps-Link "26a". Im Entwurf steht 26a.
2. **E-Mail:** Das Impressum nennt "info@stilarchitektur.de" (ohne x), alle
   anderen Seiten "info@STILxArchitektur.de". Im Entwurf steht die Variante mit
   x. Auf der alten Seite sind beide Adressen nur per JavaScript sichtbar - im
   Entwurf sind es normale `mailto:`-Verweise, was Anfragen erleichtert, aber
   auch die Adresse fuer Spam-Sammler sichtbar macht. Falls das nicht gewollt
   ist: bewusst entscheiden, nicht per JavaScript verstecken.
3. **Projektzahl:** Die Uebersicht listet 57 Projekte. Im Entwurf steht
   "ueber 50", weil der Bestand von 2021 stammt.
4. **Stellenanzeigen:** Stehen seit mindestens 2021 auf der Seite. Sind sie
   noch aktuell? Im Entwurf sind sie uebernommen.
5. **Bildrechte:** Das Impressum sagt, die Fotografen seien "bei den Projekten
   benannt und verlinkt". Diese Angaben liegen in den Projekt-Unterseiten, die
   nicht mitgecrawlt wurden. Vor einem echten Livegang zu klaeren.

## Veroeffentlichen

Noch **nicht** veroeffentlicht. Vorgesehen ist ein eigener Netlify-Auftritt,
nicht ein Unterordner von meiersseiten.de:

```powershell
netlify deploy --dir . --prod --site entwurf-stilxarchitektur
```

**Vor dem Deploy `material/` ausschliessen.** Der Ordner enthaelt die
vollstaendige Kopie der fremden Website samt Bildern und PDF. `netlify.toml`
hat `publish = "."`, es wuerde also alles hochgeladen. Als Riegel steht in der
netlify.toml ein erzwungener 404 auf `/material/*`; verlassen sollte man sich
darauf nicht, sondern den Ordner beim Hochladen weglassen.

Abgesichert ist der Entwurf ausserdem durch `noindex, nofollow` im HTML,
`robots.txt` mit `Disallow: /` und den `X-Robots-Tag` aus der netlify.toml.

## Grenzen

Entwurf 1 ist eine Startseite, keine Website - Unterseiten fehlen. Wer eine
vollstaendige Seite zeigen will, nimmt Entwurf 2 oder 3.

Die Widersprueche oben sind in keinem der drei Entwuerfe geklaert, Rechtstexte
sind nicht anwaltlich geprueft. Die Texte und Bilder gehoeren dem Buero -
Verwendung nur fuer diese Entwuerfe, auf Zuruf sofort offline, nicht ins
eigene Portfolio ohne ausdrueckliche Freigabe.
