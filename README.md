# archiveorg-i18n

Translations for archive.org. The strings are edited in Weblate (weblate.archive.org), not by pull request. Weblate commits straight to this repo.

## Layout

One folder per project, one file per language:

```
offshoot/es.xlf
```

Files are XLIFF 1.2, as written by `@lit/localize`. More projects (elements, petabox) will get their own folders later.

## How projects use it

1. When strings change on offshoot's main, its CI extracts them on top of the file here (so existing translations stay) and pushes the result straight to main. Offshoot's GitLab needs a sign-in, so this repo can't pull from it. The push uses a token scoped to this repo only.
2. Weblate picks them up and translators work on them there.
3. Weblate commits the translations back to this repo.
4. A bot opens a merge request on offshoot that pins the new translations. A person reviews and merges it.

Nothing here reaches production without that review.

## Reviewers

Per-language reviewers: TBD (WEBDEV-10125).

## License

AGPL-3.0, same as offshoot. See LICENSE.
