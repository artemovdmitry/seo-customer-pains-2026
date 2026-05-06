# Methodology

## What I did

Desk research across:

- **Industry analyses** — Marketers Center and Seo.co for the quantitative breakdown of agency-termination causes; Centori.io for templated-reporting critique; Search Engine Land / Analytics That Profit for transparency norms; Ranked.ai for transition case studies; EWR Digital for direct-login standards; SEJ and CMSWire for CMO-side perspective; Xponent21 for the AI-search adaptation pressure.
- **Trustpilot reviews** of named SEO agencies (1SEO, Trust SEO Agency, SEO Outsourcing, PageTraffic, and others) — pulled qualitative quotes from real brand-side reviewers.
- **Search Engine Roundtable archives** for documented agency-failure horror stories.
- **Reddit discussions** via indexed search — third-party aggregators surface r/SEO, r/bigseo, r/marketing, r/ecommerce conversations, but I could not scrape them directly.
- **Warrior Forum and Shopify Community** threads for SMB-owner perspective.
- **SEO contract guides** (solvlegal.com, Stan Ventures, and similar) which aggregate the typical disputes around ownership and termination.

I clustered findings into eight pain themes, ranked them by frequency × intensity, mapped them to a portable-handover product fit, and segmented them by customer type.

## What I couldn't do (yet)

Direct, primary scraping of Reddit, Twitter/X, and HackerNews discussions is not currently in my toolchain. The quotes in [`pains.md`](./pains.md) are from public Trustpilot reviews and from industry analyses that quote Reddit/forum posts — meaning everything that mentions Reddit has been filtered through an agency-side editorial layer. That filter is biased: agencies write about *other* agencies' failures, not their own.

For 100+ verbatim brand-owner quotes I'd need:

- **Apify** for direct scrape of r/SEO, r/bigseo, r/marketing, r/ecommerce
- **Reddit Search API** via PullPush or a Pushshift-style archive
- A **GummySearch** dataset or equivalent Reddit-listening tool
- Twitter/X scraping via an authorised endpoint

That's roughly 4–6 hours of work with the right tools. It's the next planned upgrade to this repo. The current version is intentionally published with the limitations noted, rather than waiting until the deeper research is done.

## What I think is solid

- The **quantitative breakdown** of termination causes (the percentages in the README) — multiple independent industry sources converge on roughly the same numbers.
- The **qualitative quotes** from public Trustpilot reviews — these are real brand-owners, named-agency context, no editorial layer.
- The **thematic clustering** of eight pains by frequency and intensity — corroborated across at least three sources per pain.
- The **segmentation** by customer-type — drawn from explicit segment-by-segment analyses (Marketers Center separates SMB from mid-market explicitly; CMSWire's State of CMO 2025 is enterprise-skewed; Reddit/Warrior Forum skews SMB).
- The **handover-fit mapping** — this is opinion, but the opinion is informed by sixteen years of working all sides of the problem.

## What I'm less sure about

- **#7 Strategy alignment ranking.** I have it as Medium/Medium, but I suspect for a B2B SaaS audience it's actually High/High. The available sources skew toward agency-owner publications, which under-weight strategic complaints.
- **#8 AI-search frequency.** I marked it Low (growing fast). The "growing fast" qualifier is doing heavy lifting; in twelve months this is likely a top-three pain across every segment.
- **#1 Failure-to-deliver framing.** The 29% number is real, but the framing ("agencies lie") is hostile. A more useful framing might be "agencies and brands disagree on the time horizon for results", which is structurally fixable.

## Reproducibility

The full source list with URLs is captured in the parent project's research log (not public — I'll publish a redacted version if there's interest). Every named source in this repo can be found via a targeted Google search of the quote.

If you find a quote you can't trace, [open an issue](https://github.com/) (placeholder — link will resolve once this repo is public) and I'll either source it or pull it.
