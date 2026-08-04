# Halo Investing

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

Halo Investing is a Chicago-based financial technology company that operates a marketplace for
"protective investments" — structured notes, multi-manager structured note SMAs, buffered ETFs,
annuities and insurance — connecting financial advisors, RIAs and financial institutions with more
than 40 global banking and insurance issuers. Founded in 2015 by Biju Kulathakal and Jason Barsema,
the platform lets advisors analyze, customize, price, execute and monitor outcome-based products
from a single dashboard. Its affiliate Halo Securities LLC is an SEC-registered broker-dealer and a
member of FINRA/SIPC.

## API surface

**Halo Investing publishes no public API, developer portal, API documentation, SDK, CLI, MCP server,
or machine-readable contract** as of 2026-08-04. Contract discovery probed both real hosts —
`haloinvesting.com` and the authenticated advisor platform `notes.haloinvesting.com` — across the
OpenAPI/Swagger, GraphQL, MCP and `/.well-known/` (including A2A agent card) surfaces. Every probe
missed. No GitHub organization exists and no first-party client library is published to npm, PyPI,
RubyGems, crates.io or NuGet. Advisor-side API integration is offered through the third-party
**Schwab OpenView Gateway** (operated by Performance Technologies, Inc.), not a Halo-published API.

Two catch-all traps on this domain produce false positives, and are recorded in
`well-known/halo-investing-well-known.yml` so future rounds do not mistake them for artifacts:

- The WordPress marketing site returns **HTTP 200 with an HTML article for every unknown path**, so
  `/llms.txt`, `/openapi.json`, `/security/` and `/trust/` all "succeed" as soft-404s.
- `*.haloinvesting.com` is a **wildcard DNS record**, so `api.`, `developer.`, `status.`, `trust.`
  and `mcp.` all resolve and answer 502 without being real hosts.

## Links

- Website — https://haloinvesting.com/
- Platform login — https://notes.haloinvesting.com/logon
- Request access — https://haloinvesting.com/request-access/
- Important disclosures (Reg BI, Form CRS, FINRA/SIPC) — https://haloinvesting.com/important-disclosures/
- Schwab Advisor Services listing — https://advisorservices.schwab.com/provider-solutions/Halo-Investing-Protective-Investments-Marketplace
- Forge Global secondary-market listing — https://forgeglobal.com/halo-investing_stock/
