# Lapse

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

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
