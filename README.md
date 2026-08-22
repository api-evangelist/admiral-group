# Admiral Group (admiral-group)

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

Admiral Group plc is a FTSE 100 personal-lines insurance group headquartered in Cardiff, Wales, and listed on the London Stock Exchange since 2004. Its home market is the United Kingdom, where it is one of the largest motor insurers, trading through the Admiral, Bell, Diamond, elephant.co.uk and Veygo brands and underwriting through EUI Limited and Admiral Insurance Company Limited. Beyond UK motor it writes household, travel and pet insurance (expanded by the 2024 acquisition of RSA's UK home and pet book, including the MORE THAN brand), runs the Admiral Money consumer lending arm, owns the Confused.com price comparison site, and operates internationally as ConTe.it in Italy, L'olivier in France and Admiral Seguros in Spain.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/admiral-group/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/admiral-group/refs/heads/main/apis.yml)

## Tags

- Insurance
- United Kingdom
- Property and Casualty
- Motor Insurance
- Home Insurance
- Pet Insurance
- Travel Insurance
- Carrier
- Personal Lines
- Price Comparison
- Embedded Insurance
- Consumer Lending
- Underwriting
- Claims
- Company

## Timestamps

- **Created:** 2026-07-25
- **Modified:** 2026-07-25

## APIs

None. Admiral Group publishes no public, self-serve API.

This is an honest finding rather than a gap in research. Admiral is a direct-to-consumer and price-comparison personal-lines carrier, not a broker-channel or platform carrier, so the forcing functions that produce developer surfaces elsewhere in insurance do not reach it. The UK has no open-insurance obligation — the FCA's Open Finance work is still consultation, not rule — and the London Market modernisation programme (Blueprint Two, PPL, Whitespace, Ki) that drives the country's genuine insurance API infrastructure is a subscription-market effort aimed at brokers and syndicates, a market Admiral sits entirely outside.

What was probed on 2026-07-25:

- `developer.`, `developers.`, `docs.` and `api.` on `admiralgroup.co.uk` — all NXDOMAIN.
- `www.admiralgroup.co.uk` and its `/developers`, `/api`, `/developer`, `/partners`, `/integrations` paths — HTTP 403, bot-protected corporate investor site.
- `www.admiral.com` — HTTP 200 consumer site; `/developers`, `/developer`, `/api`, `/partners`, `/api-docs`, `/openapi.json`, `/swagger.json`, `/.well-known/openid-configuration`, `/.well-known/security.txt`, `/llms.txt` all 404. All 837 sitemap URLs enumerated: no developer, API or integration page.
- `api.admiral.com` — resolves, HTTP 502. Undocumented private backend.
- `api.veygo.com` — resolves to AWS, returns `403 {"message":"Forbidden"}`. Private API Gateway behind the Veygo apps, not a published API.
- No GitHub organisation for Admiral Group; the `Veygo` and `confusedcom` organisations exist with zero public repositories.
- No public Postman collection, no GraphQL endpoint, no `.proto`, no webhook or event catalogue, no AsyncAPI.
- The third-party API Tracker profile for Admiral Group carries an empty developer-docs, API-reference, webhooks, auth, sandbox, OpenAPI and GraphQL record — independent corroboration.

### ACORD posture

**No ACORD reference found.** No ACORD, AL3, ACORD XML, NGDS, or ACORD-certified mention appears on any Admiral Group property or in trade coverage of the group. That is consistent with the business model: ACORD messaging and agency-download plumbing serve the broker/agency channel, and Admiral distributes direct and through price comparison. Note the homonym trap — Admiral Insurance Group (`admiralins.com`), the US excess-and-surplus carrier owned by W. R. Berkley, does publish ACORD forms and is a **different company**.

### Adjacent ventures

- **Connect by Admiral** — an Admiral Pioneer embedded-insurance venture described in trade press as "API-first", built on Root's platform for point-of-sale distribution. `connectbyadmiral.com` now returns 403 and `www.` returns 404; no developer or docs subdomain resolves and no reference documentation was ever public. A B2B partner integration, never a developer program.
- **Flock** — Admiral agreed in February 2026 to acquire the UK commercial fleet insurtech for £80m. Flock runs its own self-service portal and broker channel; that surface belongs to a separate provider record and is deliberately not claimed here.

## Links

- [Admiral Group plc (corporate)](https://www.admiralgroup.co.uk/)
- [Admiral (UK consumer)](https://www.admiral.com/)
- [About Admiral](https://www.admiral.com/about-us)
- [Admiral Pioneer](https://www.admiralpioneer.com/)
- [Veygo](https://www.veygo.com/)
- [Confused.com](https://www.confused.com/)
- [LinkedIn](https://www.linkedin.com/company/admiral-group-plc)
- [Review findings](review.yml)
