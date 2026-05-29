# NFG — Nicomacos Food Graph Schema

Open vocabulary for restaurant, dish, ingredient, and food data. Provided by **NGraph Inc.**, powering [OMISEAI](https://omiseai.com/).

## Live

- Site: https://nfg.ngraph.jp/
- v0.2 context: https://nfg.ngraph.jp/schema/v0.2/context.jsonld

## Use

Embed in your HTML:

```html
<script type="application/ld+json" data-aeo="restaurant">
{
  "@context": [
    "https://schema.org",
    "https://nfg.ngraph.jp/schema/v0.2/context.jsonld"
  ],
  "@type": ["Restaurant", "nfg:SeafoodRestaurant"],
  "name": "蟹と海鮮ぼんた",
  "nfg:vadCertified": true,
  "nfg:vadSource": "owner_verified",
  "nfg:confidenceScore": 0.95
}
</script>
```

## Deploy

Static site, hosted on Cloudflare Pages. GitHub push → auto deploy.

## Versioning

- **v0.2** — current (2026-05-29)
- Pre-1.0 phase: breaking changes increment minor.
- v1.0 will be cut after community stabilization.

## License

TBD (likely CC BY 4.0 for the schema vocabulary, separate from the OMISEAI software).
