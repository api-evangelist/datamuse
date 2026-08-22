# Datamuse (datamuse)

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

Datamuse operates a word-finding query engine and lexical search service for developers, educators, and creative-writing applications. The Datamuse API exposes a /words endpoint that finds words matching a rich combination of semantic, phonetic, orthographic, and vocabulary constraints (means-like, sounds-like, spelled-like, synonyms, antonyms, hypernyms, meronyms, triggers, rhymes, homophones, and more) plus a /sug autocomplete endpoint. Free for non-commercial use up to 100,000 requests per day with no API key required; commercial use, custom vocabularies, and higher rate limits are available via a paid commercial agreement. Datamuse also runs OneLook, OneLook Thesaurus, RhymeZone, Rimar.io, and CivicSearch — consumer-facing word search tools built on the same lexical infrastructure.

**APIs.json:** [https://www.datamuse.com/api/](https://www.datamuse.com/api/)

## Tags

- Word Finding
- Lexical Search
- Natural Language
- Vocabulary
- Synonyms
- Antonyms
- Rhymes
- Phonetics
- Semantic Search
- Reverse Dictionary
- Autocomplete
- Wordplay
- Creative Writing
- Vocabulary Apps
- Word Games
- Linguistics
- Open Source Projects
- Public APIs

## Timestamps

- **Created:** 2026-05-28
- **Modified:** 2026-05-29

## APIs

### Datamuse API

The Datamuse REST API exposes two operations covering word-finding (/words) and autocomplete suggestions (/sug). The /words endpoint accepts a rich combination of constraint parameters — semantic (ml, rel_syn, rel_ant, rel_trg, rel_spc, rel_gen, rel_com, rel_par, rel_jja, rel_jjb), phonetic (sl, rel_rhy, rel_nry, rel_hom, rel_cns), orthographic (sp with wildcards), and vocabulary (v=en|es) — plus ranking hints (topics, lc, rc) and result controls (max, md, qe, ipa). No authentication required for free non-commercial use up to 100k requests/day.

- **Human URL:** [https://www.datamuse.com/api/](https://www.datamuse.com/api/)
- **Base URL:** `https://api.datamuse.com`

#### Tags

- Word Finding
- Lexical Search
- Natural Language

#### Properties

- [Documentation](https://www.datamuse.com/api/)
- [API Reference](https://www.datamuse.com/api/)
- [OpenAPI](openapi/datamuse-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/datamuse.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/datamuse.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [JSON Schema](json-schema/datamuse-word-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/datamuse-suggestion-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Structure](json-structure/datamuse-word-structure.json)
- [JSON Structure](json-structure/datamuse-suggestion-structure.json)
- [J S O N- L D](json-ld/datamuse-context.jsonld)
- [Example](examples/datamuse-getwords-example.json)
- [Example](examples/datamuse-getsuggestions-example.json)
- [Rate Limits](rate-limits/datamuse-rate-limits.yml)
- [Pricing](plans/datamuse-plans-pricing.yml)

## Common Properties

- [Website](https://www.datamuse.com/)
- [Documentation](https://www.datamuse.com/api/)
- [API Reference](https://www.datamuse.com/api/)
- [Pricing](https://www.datamuse.com/api/)
- [Terms of Service](https://www.datamuse.com/api/)
- [Privacy Policy](https://www.datamuse.com/api/)
- [Support](https://www.datamuse.com/api/)
- [Spectral Rules](rules/datamuse-rules.yml)
- [Vocabulary](vocabulary/datamuse-vocabulary.yml)
- [Plans](plans/datamuse-plans-pricing.yml)
- [Rate Limits](rate-limits/datamuse-rate-limits.yml)
- [Fin Ops](finops/datamuse-finops.yml)
- [Public APIs Listing](https://github.com/public-apis/public-apis)
- [SDK](https://github.com/sjblair/Datamuse4J)
- [SDK](https://github.com/gmarmstrong/python-datamuse)
- [SDK](https://github.com/ansteh/datamuse)
- [SDK](https://github.com/ezefranca/datamuse-swift)
- [SDK](https://github.com/owenvoke/datamuse-php-api-wrapper)
- [SDK](https://github.com/kostaspt/go-datamuse)
- [SDK](https://github.com/slogemann1/datamuse-api-wrapper)
- [SDK](https://github.com/benhess02/DatamuseDotNet)
- [SDK](https://github.com/mosegontar/rubymuse)
- [Tools](https://github.com/lacausecrypto/datamuse-mcp)
- [Tools](https://github.com/pipeworx-io/mcp-datamuse)
- [Tools](https://github.com/bhayanak/datamuse-mcp-server)
- [Tools](https://github.com/pipeworx-io/mcp-words)
- [Tools](https://github.com/Eyalm321/multilingual-dictionary-mcp)
- [Features](undefined)
- [Use Cases](undefined)
- [Integrations](undefined)
- [Solutions](undefined)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
