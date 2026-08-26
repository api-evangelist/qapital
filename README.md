# Qapital

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
> **Not from the company, and here with a question?** You are welcome here — we would rather be the
> front line and point you the right way than have a good report go nowhere. What this repository
> can answer is narrow, though, so it is worth knowing who you are actually looking for:
>
> - **A question about how the API works, an account, billing, or a bug in the service** — that is
>   the company's own support, not us. We profile this API; we do not operate it and cannot see
>   your account.
> - **A bug in an open-source project we only catalog** — file it on that project's own repository.
>   This has happened with a real and correct bug report that reached us instead of the people who
>   could fix it, which helped nobody.
> - **Anything about this listing itself** — the description, the tags, the rating, a missing or
>   wrong artifact — is ours. Open an issue here.
> - **Not sure, or something general about API Evangelist or APIs.io** — open an issue on the
>   [APIs.io Inbox](https://github.com/api-search/inbox) and we will route it.
>
> **This repository contains no software, and we will never ask you to download anything.** There is
> no build, release, installer, or binary here — only text and machine-readable API descriptions, so
> there is nothing here that can be "corrupt" or need "repairing". Any issue, comment, or email
> claiming otherwise and offering a download link is not from us and is hostile. Do not follow the
> link; it is a lure. Report it to GitHub and, if you like, tell us at
> [info@apievangelist.com](mailto:info@apievangelist.com) so we can take it down.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

Qapital is a consumer personal-finance company founded in 2013 — "born in Stockholm, raised in New
York City" — that packages saving, spending, investing and budgeting into a single mobile membership
app built on behavioral-economics research. Its Rules engine automates transfers into user-defined
Goals, a Dream Team feature lets two people save collaboratively, Qapital Invest offers risk-weighted
portfolios through SEC-registered advisory and brokerage partners, and a Qapital Visa debit card and
Spending account run on FDIC-member partner banking. Qapital reports 3.5m+ app downloads and roughly
$3B collectively saved by members.

## API surface

**Qapital publishes no public API.** As of 2026-08-26 there is no developer portal, no API
reference, no OpenAPI / AsyncAPI / GraphQL contract, no SDK, no CLI, no MCP server and no A2A agent
card. `developer.qapital.com` and `docs.qapital.com` do not resolve; `api.qapital.com` resolves to an
AWS load balancer but answers every anonymous request with `503 Service Unavailable` because it is
the private backend for the mobile apps. Every `/.well-known/` path on `www.qapital.com` returns 404.

The only public programmable surface is the [Qapital service on IFTTT](https://ifttt.com/qapital) —
four polling triggers, three Pro+ queries and one action — captured in
[`integrations/qapital-ifttt.yml`](integrations/qapital-ifttt.yml).

## What is in this profile

| Artifact | File |
|---|---|
| Membership plans and pricing | [`plans/qapital-plans-pricing.yml`](plans/qapital-plans-pricing.yml) |
| Rate limits (measured zero) | [`rate-limits/qapital-rate-limits.yml`](rate-limits/qapital-rate-limits.yml) |
| `/.well-known/` probe (all 404 / 503) | [`well-known/qapital-well-known.yml`](well-known/qapital-well-known.yml) |
| Trust center — SOC 2 Type I, FDIC, SEC/FINRA partners | [`security/qapital-trust-center.yml`](security/qapital-trust-center.yml) |
| Domain security probe | [`security/qapital-domain-security.yml`](security/qapital-domain-security.yml) |
| Conformance | [`conformance/qapital-conformance.yml`](conformance/qapital-conformance.yml) |
| IFTTT integration surface | [`integrations/qapital-ifttt.yml`](integrations/qapital-ifttt.yml) |
| llms.txt | [`llms/qapital-llms.txt`](llms/qapital-llms.txt) |

## Links

- Website — https://www.qapital.com/
- Pricing — https://www.qapital.com/pricing/
- Security — https://www.qapital.com/security/
- Help Center — https://help.qapital.com/en/
- Blog — https://www.qapital.com/blog/
- GitHub — https://github.com/qapital
- Terms — https://www.qapital.com/terms/
- Privacy — https://www.qapital.com/terms/privacy-policy/
