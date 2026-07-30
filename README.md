# Lapse

Lapse (Lapse Ltd, London) makes an iOS app that turns an iPhone into a disposable camera — a one-tap Lock Screen shutter, a film "developing" delay, and a friends-only photo journal. The product thesis is "Friends not followers": no ads, no data sales, no public follower counts. Access is invite/friends-gated Early Access, the app is free, and it is iOS only.

Backed by: Greylock, GV, Speedinvest — https://lapse.com/

## API status

**No public API.** As of the 2026-07-19 enrichment pass Lapse publishes no developer portal, documentation, API reference, SDKs, CLI, or public specs. Probing found:

- No `/.well-known/` documents on `lapse.com`, `lapse.app`, or the internal backend host — see `well-known/lapse-well-known.yml`.
- No `api.` / `developer.` / `docs.` / `status.` subdomains (all NXDOMAIN).
- No first-party client libraries on npm or PyPI.
- No verifiable Lapse GitHub organization.

Caution when re-probing: `lapse.com/<anything>` is a **username-profile catch-all** that returns HTTP 200 with the app HTML shell. A 200 alone is not evidence a document exists — verify the body.

## Artifacts

| Path | Type | Method |
|---|---|---|
| `apis.yml` | APIs.json 0.20 index | — |
| `security/lapse-domain-security.yml` | DomainSecurity | probed |
| `well-known/lapse-well-known.yml` | WellKnown | searched |
| `llms/lapse-llms.txt` | LLMsTxt | generated |
