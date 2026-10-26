# NFG — Nicomachos Food Graph Schema

Open vocabulary for restaurant, dish, ingredient, and food data. Provided by **NGraph Inc.**, powering [OMISEAI](https://omiseai.com/).

## Live

- Site: https://nfg.ngraph.jp/
- v0.3 context: https://nfg.ngraph.jp/schema/v0.3/context.jsonld
- v0.2 context: https://nfg.ngraph.jp/schema/v0.2/context.jsonld（引き続き配信）
- 日本語: https://nfg.ngraph.jp/ ／ English: https://nfg.ngraph.jp/en/

## Use

Embed in your HTML:

```html
<script type="application/ld+json" data-aeo="restaurant">
{
  "@context": [
    "https://schema.org",
    "https://nfg.ngraph.jp/schema/v0.3/context.jsonld"
  ],
  "@type": ["Restaurant", "nfg:SeafoodRestaurant"],
  "name": "Sakanaya (fictional)",
  "nfg:vadCertified": true,
  "nfg:vadSource": "owner_verified",
  "nfg:confidenceScore": 0.95
}
</script>
```

## Deploy

Static site, hosted on Cloudflare Pages. GitHub push → auto deploy.

## Versioning

- **v0.3** — current (2026-10-26)：実サイトで使っていた KaisekiRestaurant・habitat・courseFlow・certificationTag を定義に追加。seasonStart/seasonEnd は実データに合わせ MM-DD（xsd:date 指定を外す）。vadSource の値は規格書 §7.7 の4つ（ai_inferred / owner_verified / official_published / third_party）
- **v0.2** — 2026-05-29（引き続き配信）
- Pre-1.0 phase: breaking changes increment minor.
- v1.0 will be cut after community stabilization.

## License

TBD (likely CC BY 4.0 for the schema vocabulary, separate from the OMISEAI software).
