# Charades Words

Free charades word lists in six languages — the companion site for
[Charades: Heads Up Party Game](https://play.google.com/store/apps/details?id=com.charadesparty.app).

Live at **https://charadesstudio-gif.github.io/charades/**

## Do not edit these files by hand

Everything here is **generated** from the app's own word files
(`client/src/lib/words/*.ts` in the private app repo) by
`scripts/build-site.mjs`. Editing a page directly means the next build silently
overwrites it.

To change the site, change the app's word data or the generator, then:

```bash
node scripts/build-site.mjs /path/to/charades-web
```

…and commit the result here.

## What gets published

- 6 languages: English, French, Spanish, Portuguese, German, Indonesian
- 9 evergreen categories per language — Animals, Food, Objects, Actions,
  Sports, Travel, Movies, Music, Celebrities
- 60 pages, ~8,500 words

Premium decks and dated trend decks are deliberately **excluded**: premium decks
stay a reason to install the app, and trend decks would go stale in the search
index.

Each page carries a canonical URL, `hreflang` links to all six languages, and an
entry in `sitemap.xml`.
