# archiveorg-translations

Translations for archive.org. The strings are edited in Weblate (weblate.archive.org), not by pull request. Weblate commits straight to this repo.

## Layout

One folder per project, one file per language:

```
offshoot/es.xlf
```

Files are XLIFF 1.2, as written by `@lit/localize`. More projects (elements, petabox) will get their own folders later.

## How projects use it

1. Offshoot extracts its source strings and sends the updated `.xlf` files here.
2. Weblate picks them up and translators work on them there.
3. Weblate commits the translations back to this repo.
4. A bot opens a merge request on offshoot that pins the new translations. A person reviews and merges it.

Nothing here reaches production without that review.

## Reviewers

Per-language reviewers: TBD (WEBDEV-10125).
