# Bing News Search

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
