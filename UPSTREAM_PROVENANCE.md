# Upstream provenance -- unresolved question

This document records an unresolved licensing question about the
origin of this CDN bundle. It is a flag for the Virtual Pharmacist Ltd
commercial / legal track and does not itself answer the question.

## Background

An internal third-party-library inventory identified the overall
structure and stylesheet patterns of the assets in this repository as
consistent with a commercial admin-dashboard theme sold through
ThemeForest. Candidate upstream families surfaced by the fingerprint
match include (in alphabetical order):

- Hyper (HyperUI / Coderthemes Hyper)
- Skote (Themesbrand Skote)
- Velzon (Themesbrand Velzon)

Each of these themes is sold under an Envato Regular Licence by default.
The Regular Licence permits use in a single end product where end users
are not charged for access, and explicitly does not cover:

- Multi-tenant SaaS where access is gated behind a subscription
- Distribution of the theme files as a separable component (which a
  public CDN is)
- Transfer of the theme licence to a third party (such as a corporate
  acquirer)

Envato sells an **Extended Licence** which expands the permitted use
to multi-end-user SaaS, but transfer to an acquirer still requires
written permission from the original author or Envato.

## Why this matters

Any third-party SCA / commercial-licensing review will fingerprint the
bundle's structure against well-known commercial templates. If the
bundle matches a known ThemeForest theme, the reviewer will flag it and
will request:

1. Evidence of the original purchase
2. Evidence that the licence in use covers multi-tenant SaaS hosting
3. Evidence that the licence can transfer to any acquirer in a sale
   or material change of control

If those three pieces of evidence cannot be produced, the reviewer will
treat the theme as a commercial-licensing blocker.

## Action required (legal / commercial track)

This question is NOT something the engineering team can resolve. It
requires:

1. The original commercial-template purchase receipt (Envato invoice
   or upstream vendor invoice) -- if one exists.
2. A licence-of-record check (Regular vs Extended on Envato).
3. Confirmation in writing from Envato or the upstream vendor that
   the licence in use covers multi-tenant SaaS CDN hosting and
   transfers in the event of a sale.

If the licence cannot be confirmed to cover this product's usage and
sale, the practical paths forward are (engineering-led, but only after
a legal decision):

- Replace the theme with one whose licence does cover this usage (for
  example, a permissively-licensed open-source admin theme, or an
  internally-built CSS).
- Negotiate an Extended Licence plus a transfer addendum with the
  upstream vendor.

Either path is a multi-week project; both are tracked internally.
