# MaxMind (maxmind)

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

MaxMind is an IP intelligence and fraud prevention company founded in 2002, serving over 100,000 businesses worldwide. Their GeoIP web services provide accurate IP geolocation data including country, city, ISP, organization, ASN, connection type, and VPN/proxy detection. Their minFraud services offer real-time transaction risk scoring using over 80 data points on IPs, email addresses, devices, and payment cards to help businesses detect and prevent fraud. MaxMind also offers downloadable GeoIP databases and the free GeoLite2 dataset for developers who prefer local lookups over API calls.

APIs.json: https://raw.githubusercontent.com/api-evangelist/maxmind/refs/heads/main/apis.yml

Naftiko: https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=maxmind-api-evangelist&utm_content=repo

## Tags

- IP Intelligence
- Geolocation
- Fraud Prevention
- Risk Scoring
- VPN Detection
- Proxy Detection
- ISP Data
- GeoIP

## APIs

| Name | Description |
|---|---|
| GeoIP Country Web Service | Country-level geolocation via REST API ($0.0001/query) |
| GeoIP City Plus Web Service | City-level geolocation with ISP and ASN data ($0.0003/query) |
| GeoIP Insights Web Service | Full IP intelligence with VPN/proxy detection ($0.002/query) |
| minFraud Score | Transaction risk score API ($0.005/query) |
| minFraud Insights | 80+ data point fraud scoring API ($0.015/query) |
| minFraud Factors | Component-level risk factor decomposition ($0.020/query) |

## Plans, Rate Limits, and FinOps

| Resource | Path |
|---|---|
| Plans and Pricing | [plans/maxmind-plans-pricing.yml](plans/maxmind-plans-pricing.yml) |
| Rate Limits | [rate-limits/maxmind-rate-limits.yml](rate-limits/maxmind-rate-limits.yml) |
| FinOps | [finops/maxmind-finops.yml](finops/maxmind-finops.yml) |

### Pricing Summary

MaxMind uses a unified pay-as-you-go credit model shared across all GeoIP and minFraud web service APIs. There are no monthly minimums or commitments. GeoIP database subscriptions are billed separately on monthly or annual terms. A free GeoLite2 tier is available for country and city data with reduced accuracy.

### Rate Limits

MaxMind does not enforce strict per-second rate limits for paid web service customers. Usage is metered by credit balance. Database download endpoints have a per-account daily download limit. Excessive error rates may trigger temporary throttling.

### FinOps Notes

The primary cost optimization strategies are session-level caching (reduces queries 40-80%), service tier right-sizing (match tier to fields actually consumed), and the score-based escalation pattern for minFraud (use Score as a first pass, escalate to Insights/Factors only above a risk threshold). Annual database subscriptions save 8-10% versus monthly billing.

## Timestamps

- Created: 2026-06-12
- Modified: 2026-06-12

## Common Properties

| Type | URL |
|---|---|
| Website | https://www.maxmind.com/ |
| Documentation | https://dev.maxmind.com/ |
| GitHub Organization | https://github.com/maxmind |
| LinkedIn | https://www.linkedin.com/company/maxmind |
| Blog | https://blog.maxmind.com/ |
| Pricing | https://www.maxmind.com/en/solutions/fraud-prevention/plans-pricing |
| Status Page | https://status.maxmind.com/ |
| X (Twitter) | https://x.com/maxmind |

## Maintainers

| Name | Email |
|---|---|
| Kin Lane | kin@apievangelist.com |
