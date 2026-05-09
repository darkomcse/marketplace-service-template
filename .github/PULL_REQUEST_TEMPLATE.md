<!--
  ⚠️  BOUNTY POOL IS PAUSED (2026-04-28)
  PRs duplicating live services or missing required artifacts are closed
  immediately. Read the checklist below — submit COMPLETE or don't submit.
-->

## Service

**Vertical:** <!-- e.g. Pinterest Pin Search, Bing News, etc. NOT in live catalog at https://agents.proxies.sx/marketplace/ -->
**Bounty issue (if any):** #
**Live deployment URL:** <!-- e.g. https://my-service.fly.dev — must respond HTTP 402 right now -->

## Required artifacts (all 7 must be present — no exceptions)

- [ ] **Live deployment URL** publicly reachable, returns HTTP 402 with current pricing/recipient
- [ ] **Video walkthrough (≤3 min)** showing 3 full x402 payment-and-response cycles end-to-end against the live URL — link below
- [ ] **`proof/` directory** with ≥3 raw real API responses (JSON), each annotated with query + proxy IP + timestamp
- [ ] **Output schema documentation** in README — every field has type + description (per [issue #112](https://github.com/bolivian-peru/marketplace-service-template/issues/112))
- [ ] **Error handling** for: CAPTCHA, rate-limit, login wall, proxy failure, empty results — documented + tested
- [ ] **No mocks in tests** — tests hit the live deployment
- [ ] **Comparison table** vs SerpAPI / Apify / Outscraper (or equivalent) for this vertical

## Video link

<!-- Unlisted YouTube, Loom, or attached MP4. Must show real on-chain payment, not mocked. -->

## Comparison

| Provider | Price/req | Latency p50 | Output schema | Edge |
|---|---|---|---|---|
| SerpAPI | | | | |
| Apify | | | | |
| **This PR** | | | | |

## Why is this not already in the live catalog?

<!-- One paragraph: which vertical, why customers want it, why our existing 9 services don't cover it. -->

---

**By submitting:** I confirm all 7 artifacts above are present in this PR. Incomplete submissions are closed without review.
