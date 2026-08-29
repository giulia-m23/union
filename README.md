# Ünion

Everything about your university path in one place, and free: requirements, deadlines, real costs, and the students who already got in.

It has never been that easy. Now it is.

**Live demo:** `https://union-demo-v1.netlify.app` — it opens with a key. Ask me and I'll send it.

---

## The problem

A wrong ranking is embarrassing. A wrong admission requirement costs a twenty-year-old a year of their life. Those are not the same kind of mistake, and most of the tools in this space treat them as if they were: they optimise for looking complete.

The information a student actually needs, current requirements, real deadlines, what the intake looks like for someone with their background, is scattered across a few hundred university websites, written in a different structure by every one of them, and it changes every year. Nobody collects it. So students decide their next five years on forum threads and guesswork.

## What Union does

Union puts that information in one place, in the student's language, and is explicit about how much it trusts each piece.

- **Search in plain language.** «economia a Londra sotto i 20.000» or «psychology in Paris, taught in English» resolves to an actual filter, in Italian or English, and the app says back what it understood so a misreading is visible instead of silent.
- **A university card that answers the real questions.** Requirements, deadlines, tuition, rankings for the specific course rather than the institution, campus life, and where each figure came from with the date it was checked.
- **Students who already got in.** Profiles and conversations that show what an accepted application actually looked like.
- **A globe, not a list.** Because choosing a country is a different decision from choosing a course, and it deserves its own screen.

## The rule that shapes it

Where a figure has not been verified at the source, the warning appears **above** the numbers, not below them. A caveat placed underneath arrives after the reader has already believed the number. Deadlines a university has not published yet are labelled indicative and start no countdown. Admission rates by applicant background are shown as demonstrative estimates, because that data does not exist publicly, and closing that gap is the actual point of the project.

It makes the app look less complete than it could. It is also the only thing that, repeated for a few years, earns the trust that makes a student check here first.

## Screenshots

`DA COMPLETARE: 3–4 schermate, la ricerca, il globo, una scheda ateneo, la chat`

## Built with

React Native and Expo (SDK 57), TypeScript, Expo Router, Reanimated, react-native-svg. It runs on iOS, Android and the web from one codebase. The demo above is the web export.

Two things worth naming, because they are where the engineering went:

- **Translation is a machine, not a task.** Text is translated inside the shared `Text` component and keyed by the Italian phrase itself, so a new language is a dictionary file and no code changes at all. Italian and English are in; the rest is a translation away.
- **A regression net that runs on the writing.** Seven scripts check things a test suite usually cannot: that no phrase escapes the translator, that every tappable element responds to touch, that every colour pairing clears WCAG contrast in both themes, that the same question in two languages produces the same filter, and that no card falls back to an average when the real figure is missing.

## The code

The source is private. The reason is not secrecy about the technique, it is that the interesting part of this project is the data and the judgement about what to show, and that part is not finished. If you want to read the code, ask me and I'll give you access.

## Author

Giulia Moroni — Milan — https://www.linkedin.com/in/giuliamoroni/

© 2026 Giulia Moroni. All rights reserved. No licence is granted.

*The 35 universities and 107 courses in the demo were checked one by one against official sources. Student names, faces and conversations are invented and labelled as such in the app. University photographs come from Wikimedia Commons under Creative Commons licences, credited inside the app on each card.*
