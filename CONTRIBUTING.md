# Contributing to Marketplace Service Template

> ⚠️ **BOUNTY POOL IS PAUSED** (2026-04-28). We are not merging PRs that
> duplicate the 9 services already live at https://agents.proxies.sx/marketplace/.
> Only PRs targeting **substantively novel verticals** with **all 7 artifacts**
> in [`PULL_REQUEST_TEMPLATE.md`](.github/PULL_REQUEST_TEMPLATE.md) will be
> reviewed. Incomplete submissions are closed without review.

Thanks for your interest in contributing! This is the builder template for the [Proxies.sx Data Marketplace](https://agents.proxies.sx/marketplace/).

## Ways to Contribute

### 1. Build a Marketplace Service (Bounty)

The main way to contribute is by building a new data API service.

**Steps:**
1. Check the live catalog at https://agents.proxies.sx/marketplace/ — services already there will not be re-bountied
2. Pick a NOVEL vertical (Amazon, Twitter/X, TikTok, Facebook Marketplace, Zillow, Food Delivery, Crypto Markets, App Store, Gmail, etc.)
3. Comment on a relevant bounty issue OR open one to discuss before building
4. Fork this repo
5. Build your service in `src/service.ts`
6. Deploy to a public URL (Cloudflare Workers, Render, Railway, Fly.io)
7. Record a 3-min video walkthrough of 3 full x402 payment-and-response cycles
8. Submit a PR following the template — all 7 artifacts mandatory

**Bounty payments:** $SX tokens, paid after merge and deployment verification.
**Bounty pool currently:** paused. New high-quality novel-vertical PRs may still be reviewed at owner discretion if they meet the bar.

### 2. Improve the Template

Bug fixes, documentation improvements, and developer experience enhancements are welcome.

### 3. Report Issues

Found a bug or have a feature request? [Open an issue](https://github.com/bolivian-peru/marketplace-service-template/issues/new).

## Submission Requirements

Every bounty PR **must** include all 7 artifacts in [`PULL_REQUEST_TEMPLATE.md`](.github/PULL_REQUEST_TEMPLATE.md):

1. **Live deployment URL** publicly reachable, returns HTTP 402 with pricing
2. **Video walkthrough (≤3 min)** of 3 full x402 payment-and-response cycles against the live URL
3. **`proof/` directory** with ≥3 raw real API responses
4. **Output schema documentation** per [quality standards in issue #112](https://github.com/bolivian-peru/marketplace-service-template/issues/112)
5. **Error handling** for CAPTCHA / rate-limit / login wall / proxy failure / empty results
6. **No mocks in tests** — tests hit the live deployment
7. **Comparison table** vs SerpAPI / Apify / Outscraper for the vertical

PRs without ALL 7 are closed without review.

## Code Standards

- TypeScript (strict mode)
- Use the existing patterns in `src/service.ts`
- No hardcoded credentials — use environment variables
- No unnecessary dependencies — keep it lean
- Test your service works behind a proxy

## Security

- Never commit credentials, API keys, or private keys
- Never add `eval()`, `Function()`, or dynamic code execution
- Never add external HTTP calls to unknown servers
- All user input must be validated
- See [SECURITY.md](SECURITY.md) for the full checklist

## Getting Help

- **Telegram (group):** [t.me/proxies_sx](https://t.me/proxies_sx)
- **Telegram (support):** [@sxproxies](https://t.me/sxproxies)
- **Twitter:** [@sxproxies](https://x.com/sxproxies)
- **Email:** agents@proxies.sx
- **Discussions:** [GitHub Discussions](https://github.com/bolivian-peru/marketplace-service-template/discussions)
