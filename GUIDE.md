# How we translate Social Home

## Voice

Warm but technical, like the Home Assistant docs. Concrete beats
abstract: "your household" beats "the home of the future". Translate
the meaning, not the word order; a sentence that reads like a
translation is wrong even when every word is right.

Plain first. The app and the website talk to a parent and a protocol
nerd at the same time. Keep everyday screens everyday; technical terms
only where the English has them.

## Register

| Language | Address the reader as | Notes                                                 |
| -------- | --------------------- | ----------------------------------------------------- |
| German   | **du** (dein, dir)    | Lower-case du in running text, as Home Assistant does |
| Dutch    | **je** (jouw, jij)    |                                                       |
| French   | **vous**              |                                                       |
| Spanish  | **tú**                |                                                       |

## Names that stay in English

These are names, not words. Don't translate, decline or pluralize them
differently from English:

- **Social Home**, **Home Assistant**, **GFS** (Global Federation
  Server), **ESPHome**
- Sections with a product name: **Highlights**, **Momentum**,
  **Organize**, **Apps**, **Stickies**
- Algorithm and format names: AES-256-GCM, Ed25519, X25519, HKDF,
  WebRTC, and anything in `monospace`

German treats them as nouns with an article where needed ("die
Stickies", "in Highlights").

Sections that are ordinary words _are_ translated (Feed, Chat,
Calendar, Tasks, Pages, Gallery, Map, Timetable, Bazaar, …); see the
glossaries.

## Same words as the app

The website uses the words of the app's UI. When the app says
"Connections", the site says "Connections", in every language. If the
two disagree, the [glossary](glossary/) decides, and the other side is
fixed.

The unit that sends, stores and pairs is **your home / your
household**, never "Home Assistant", "instance", "node" or "server".
Home Assistant is named only as the way to install Social Home.

## Security and privacy wording

Say only what the code does. In every language:

- No "end-to-end" (Ende-zu-Ende, end-to-end, de bout en bout, de
  extremo a extremo). Say **sealed / encrypted home to home** (see the
  glossaries).
- No "military-grade", "zero-knowledge", "quantum-safe" or their
  translations.
- Residual risks are stated plainly, not softened by the translation.

## Placeholders, plurals, length

- Keep `{placeholders}` exactly as in English; move them where your
  grammar needs them.
- `_one` keys are the singular; they may spell out the number.
- Phone-width labels (`_short` keys, tabs, chips, buttons) must stay
  short. If your word is long, pick a shorter synonym rather than
  letting it wrap.
- Weblate shows translator notes from `client/src/i18n/locales/_notes.json`;
  read them.

## Typography

- **German:** „Anführungszeichen“, Gedankenstrich mit Leerzeichen ( – ),
  `…` as one character. Compounds with an English name take a hyphen:
  "Space-Einstellungen", "GFS-Link".
- **Dutch:** "aanhalingstekens", apostrophe plurals for words ending in
  a vowel (Pagina's, foto's).
- **French:** « guillemets » with non-breaking spaces inside; a
  non-breaking space before `: ; ! ?` and inside « ». Capitalize only
  the first word of a label ("Lien local", "Foyers jumelés").
- **Spanish:** «comillas» or "comillas"; opening ¿ and ¡.

## Website only

- The collapsible technical block is always summarized with the fixed
  line: Under the hood / Unter der Haube / Onder de motorkap / Sous le
  capot.
- Internal links carry the locale prefix (`/de/docs/…`); image paths
  don't.
