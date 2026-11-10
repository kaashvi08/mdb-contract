# MDB Mobile flows

Interactive React/TypeScript mobile web implementation of the supplied MDB Copy Figma file. Built with Vinext and plain CSS, using the original downloaded Figma artwork and SVG assets.

## Run

```sh
npm install
npm run dev
```

## Included

- Fourteen onboarding/offer screens, selectable brand placeholders, payout preference, loading transition, plan selection, and discount offer.
- Settlements with featured cards, category filtering, information menu, and the supplied settlement-detail screen.
- Wallet with empty and populated states, estimated-payout explanation, and claim records.
- Forms with empty and populated states, status filtering, four visual variants, and downloadable demo records.
- Desktop preview controls and a scaled mobile canvas. Selections and records persist in browser local storage.
- Keyboard-operable controls, modal focus management, reduced-motion support, and accessible selection states.

## Design references

- In-app: https://www.figma.com/design/EzXXXTKlR56sPRPed3q09t/MDB-Copy?node-id=1-32666
- Onboarding: https://www.figma.com/design/EzXXXTKlR56sPRPed3q09t/MDB-Copy?node-id=1-33551

## Boundaries

This is an interactive prototype. Checkout and claim submission are explicit demo actions; there is no payment processing, account authentication, legal filing, or verified settlement feed. The design provides only one detail screen, which is used by the sample settlement cards. Official terms, privacy documents, and support destinations were not supplied. The brand choices intentionally preserve the Figma “Insert Logo Here” placeholders. Monetary claims and dates reproduce the supplied design and are not independently verified. OS fonts and emoji can vary by device.

The wallet keeps the design's $94, three claimed, and two notified sample figures in its empty state. Populated record counts reflect the loaded demo data. The forms header count and selected navigation state are updated dynamically rather than reproducing the inconsistent static values in some Figma variants.

## Validation

- TypeScript: `npx tsc --noEmit` passed.
- Production build passed.
- Browser-tested onboarding, payout choice, loading, plan activation, category filtering, claim acknowledgement/save, form filtering, wallet information, empty states, and mobile overflow.
- Downloaded Figma assets checked for non-empty files and successful browser loading.
