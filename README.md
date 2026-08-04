# Whole Foods Market

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

Whole Foods Market is an American multinational supermarket chain owned by Amazon, exclusively selling products free from hydrogenated fats and artificial colors, flavors, and preservatives. Acquired by Amazon in 2017, Whole Foods integrates with Amazon Prime for delivery, pickup, and member discounts.

**Website:** [https://www.wholefoodsmarket.com](https://www.wholefoodsmarket.com)
**Parent Company:** [Amazon](https://www.amazon.com)
**Wikipedia:** [Whole Foods Market](https://en.wikipedia.org/wiki/Whole_Foods_Market)

## Developer Note

Whole Foods Market does not offer a public developer API. Supplier integrations use EDI (Electronic Data Interchange). Consumer-facing digital services are powered by Amazon's platform.

## Supplier Integration

Suppliers integrate with Whole Foods Market through:
- **[Supplier Portal](https://www.wholefoodsmarket.com/company-info/information-potential-suppliers)** - Product applications and vendor management
- **[EXIGIS Portal](https://prod2.exigis.com/WholeFoodsMarket)** - Compliance and certificate management
- **[Vendor Reporting Portal](https://www.gocrisp.com/catalog/whole-foods-vendor-reporting-portal)** - Sales analytics via Amazon QuickSight
- **EDI Integration** - Electronic ordering, invoicing, and shipping notifications

### EDI Document Types

| EDI Code | Document | Direction |
|----------|----------|-----------|
| 850 | Purchase Order | Whole Foods → Supplier |
| 855 | PO Acknowledgment | Supplier → Whole Foods |
| 856 | Advance Shipment Notice | Supplier → Whole Foods |
| 810 | Invoice | Supplier → Whole Foods |
| 820 | Payment Remittance | Whole Foods → Supplier |

## Artifacts

### JSON Schema

| Schema | Description |
|--------|-------------|
| [whole-foods-market-product-schema.json](json-schema/whole-foods-market-product-schema.json) | Schema for Whole Foods Market grocery products |
| [whole-foods-market-edi-850-schema.json](json-schema/whole-foods-market-edi-850-schema.json) | Schema for EDI 850 Purchase Order documents |

### JSON-LD

| Context | Description |
|---------|-------------|
| [whole-foods-market-context.jsonld](json-ld/whole-foods-market-context.jsonld) | JSON-LD context mapping Whole Foods vocabulary to schema.org |

### Vocabulary

| Vocabulary | Description |
|------------|-------------|
| [whole-foods-market-vocabulary.yml](vocabulary/whole-foods-market-vocabulary.yml) | Whole Foods Market domain vocabulary, EDI terms, and product certifications |

---
*Profile generated by [API Evangelist](https://apievangelist.com)*
