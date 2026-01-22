# NOTES

## TODO

- [ ] Add Sitemap
    - [@astrojs/sitemap]
- [ ] Add Google Analytics
    - [The ultimate Astro + Google Analytics guide]
    - [@astro-google-analytics]
    - [Partytown]
    - [Notes #1]

## Development

In order to accept connections in container from host browser update the following in `package.json`:

```JSON
"scripts": {
    "dev": "astro dev --host 0.0.0.0 --port 4321",
},
```

[The ultimate Astro + Google Analytics guide]: https://daniel.es/blog/the-ultimate-astro-google-analytics-guide/
[Partytown]: https://docs.astro.build/en/guides/integrations-guide/partytown/
[@astrojs/sitemap]: https://docs.astro.build/en/guides/integrations-guide/sitemap/
[astro-google-analytics]: https://www.npmjs.com/package/astro-google-analytics
[Notes #1]: https://chatgpt.com/c/69714bda-ece8-832e-982a-f22269c9d62a