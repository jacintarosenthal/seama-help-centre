# Seama Help Centre

Mintlify source for Seama's guided Getting Started journey and task-based Help Centre.

## Content status

This build contains the complete information-architecture foundation and the validated P0 launch content from the live Seama audit completed on 26 August 2026. It deliberately avoids presenting direct Xero-side results or mobile-specific steps as verified because those tests remain gated.

## Preview and check

From this directory:

```sh
mint validate
mint broken-links
mint a11y
mint dev --no-open
```

The current Mintlify CLI requires Node.js 20.17 or later.

## Editorial rules

- Mintlify is the maintained source after publication.
- Use exact Seama interface labels in procedures.
- Use only synthetic data in screenshots and examples.
- Reproduce a workflow before changing its `lastVerified` date.
- Do not remove the OCR, Xero, financial-state, or stale-state safeguards unless the underlying product behavior has been retested.
- Add new task pages to `docs.json`; do not mirror menus for their own sake.

## Next publishing pass

The validated plan defines approximately 110–140 P0/P1 pages. Add the remaining focused task pages category by category after product review, using the existing launch pages as the content pattern.
