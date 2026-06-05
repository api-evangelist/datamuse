# Datamuse (datamuse)

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
