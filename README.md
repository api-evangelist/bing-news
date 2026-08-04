# Bing News Search

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

Microsoft Bing News Search REST API enables developers to retrieve relevant news articles,
trending topics, and category-filtered news with image thumbnails and publisher metadata.
The API provides search queries against Bing's news index, returning results with titles,
descriptions, URLs, publication dates, and related media content.

This repository contains an APIs.json 0.19 provider profile for the Bing News Search API.

## Endpoints

| Endpoint | Description |
|----------|-------------|
| `GET https://api.bing.microsoft.com/v7.0/news/search` | Returns news articles relevant to a search query |
| `GET https://api.bing.microsoft.com/v7.0/news` | Returns top news articles by category |
| `GET https://api.bing.microsoft.com/v7.0/news/trendingtopics` | Returns news topics trending on social networks |

## Authentication

All requests require the `Ocp-Apim-Subscription-Key` header containing a valid Azure subscription key.

## Repository Structure

- `apis.yml` - APIs.json 0.19 provider profile
- `plans/bing-news-plans-pricing.yml` - Pricing tiers (Free F1, Standard S1)
- `rate-limits/bing-news-rate-limits.yml` - Rate limits and endpoint parameters
- `finops/bing-news-finops.yml` - FinOps / FOCUS-aligned cost management definitions

## Notes

The Bing Search Services public APIs were retired on August 11, 2025. Microsoft's
replacement path is Grounding with Bing Search, available inside Azure AI Foundry.

## Links

- [Documentation](https://learn.microsoft.com/en-us/previous-versions/bing/search-apis/bing-news-search/overview)
- [API Reference](https://learn.microsoft.com/en-us/previous-versions/bing/search-apis/bing-news-search/reference/endpoints)
- [Pricing](https://www.microsoft.com/en-us/bing/apis/pricing)
- [Terms of Service](https://www.microsoft.com/en-us/bing/apis/legal)

## Maintainer

Kin Lane (kin@apievangelist.com)
