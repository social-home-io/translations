# Social Home translations

Shared hints for translating Social Home: the app
([`socialhome`](https://github.com/social-home-io/socialhome), UI
strings in `client/src/i18n/locales/`, translated in Weblate) and the
website ([`website`](https://github.com/social-home-io/website),
`social-home.io`).

The point is simple: **one word for one thing, in every place.** A
parent reading the German website should meet the same words they tap
in the German app.

## What's here

| File                               | What it holds                                                                   |
| ---------------------------------- | ------------------------------------------------------------------------------- |
| [`GUIDE.md`](GUIDE.md)             | How we translate: tone, register, names that stay, typography, security wording |
| [`glossary/de.md`](glossary/de.md) | German terms                                                                    |
| [`glossary/nl.md`](glossary/nl.md) | Dutch terms                                                                     |
| [`glossary/fr.md`](glossary/fr.md) | French terms                                                                    |
| [`glossary/es.md`](glossary/es.md) | Spanish terms (app only; the website has no Spanish version yet)                |

English is the source everywhere. The glossaries list the English term,
the translation, and notes on grammar, compounds and words to avoid.

## How to use it

- **Translating by hand or in Weblate:** read `GUIDE.md` once, then
  keep your language's glossary open.
- **Claude Code / other agents:** both repos' `CLAUDE.md` say to clone
  this repo next to them before translating:

  ```sh
  git clone https://github.com/social-home-io/translations.git ../translations
  ```

  and to follow `../translations/GUIDE.md` and
  `../translations/glossary/<locale>.md`.

## When the glossary and a translation disagree

The glossary wins. Fix the translation, in the app and on the website,
in the same week if you can. If you think the glossary is wrong, open a
PR here first, then change the app and the site to match.

## Proposing a term

Open a PR that adds or changes a row in every glossary the term
touches, with a short reason. If the term is new in the app, add it
when the English string lands, so Weblate translators find it.
