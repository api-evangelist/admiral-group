# Admiral Group (admiral-group)

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
