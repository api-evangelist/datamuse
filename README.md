# Datamuse

Datamuse operates a word-finding query engine and lexical search service for developers, educators, and creative-writing applications. The Datamuse API exposes a `/words` endpoint that finds words matching a rich combination of semantic, phonetic, orthographic, and vocabulary constraints (means-like, sounds-like, spelled-like, synonyms, antonyms, hypernyms, meronyms, triggers, rhymes, homophones, and more) plus a `/sug` autocomplete endpoint. Free for non-commercial use up to 100,000 requests per day with no API key required; commercial use, custom vocabularies, and higher rate limits are available via a paid commercial agreement.

Datamuse also runs OneLook, OneLook Thesaurus, RhymeZone, Rimar.io, and CivicSearch — consumer-facing word-search tools built on the same lexical infrastructure.

- **APIs.yml:** [apis.yml](apis.yml)
- **Website:** https://www.datamuse.com/
- **Documentation:** https://www.datamuse.com/api/
- **API Reference:** https://www.datamuse.com/api/

## Type and Tier

- **x-type:** company
- **x-tier:** 3 (bulk-registered from public-apis)
- **Source:** [public-apis/public-apis](https://github.com/public-apis/public-apis) — category: Open Source Projects

## API Surface

| Method | Endpoint | Summary | Min Plan |
|---|---|---|---|
| GET | `/words` | Find Words Matching Constraints | Free Non-Commercial |
| GET | `/sug` | Get Autocomplete Suggestions | Free Non-Commercial |

Base URL: `https://api.datamuse.com` &middot; Auth: none (no API key required).

### Query Parameters at a Glance

| Family | Parameters | Purpose |
|---|---|---|
| Semantic | `ml`, `rel_syn`, `rel_ant`, `rel_trg`, `rel_spc`, `rel_gen`, `rel_com`, `rel_par`, `rel_jja`, `rel_jjb` | Reverse-dictionary, synonyms, antonyms, hypernyms, hyponyms, holonyms, meronyms, triggers, adjective-noun pairings |
| Phonetic | `sl`, `rel_rhy`, `rel_nry`, `rel_hom`, `rel_cns` | Sounds like, perfect rhymes, near rhymes, homophones, consonant matches |
| Orthographic | `sp` | Wildcard spelling patterns (`*`, `?`) |
| Statistical | `rel_bga`, `rel_bgb` | Frequent followers / predecessors per Google Books Ngrams |
| Context | `topics`, `lc`, `rc` | Document topics, left context word, right context word |
| Result control | `max`, `md`, `qe`, `ipa` | Result size, metadata flags (d/p/s/r/f), query echo, IPA pronunciations |
| Vocabulary | `v` | `en` (default, 550k terms), `es` (500k terms), or custom |
| Autocomplete (/sug) | `s`, `max`, `v` | Prefix string, max results, vocabulary |

## Artifacts

### Contract
- [openapi/datamuse-openapi.yml](openapi/datamuse-openapi.yml) — full OpenAPI 3.1 contract for `/words` and `/sug` with every documented query parameter.

### Schemas
- [json-schema/datamuse-word-schema.json](json-schema/datamuse-word-schema.json) — `/words` response object.
- [json-schema/datamuse-suggestion-schema.json](json-schema/datamuse-suggestion-schema.json) — `/sug` response object.

### JSON Structure
- [json-structure/datamuse-word-structure.json](json-structure/datamuse-word-structure.json)
- [json-structure/datamuse-suggestion-structure.json](json-structure/datamuse-suggestion-structure.json)

### JSON-LD Context
- [json-ld/datamuse-context.jsonld](json-ld/datamuse-context.jsonld) — maps Datamuse word objects onto OntoLex, SKOS, and LexInfo vocabularies.

### Examples
- [examples/datamuse-getwords-example.json](examples/datamuse-getwords-example.json) — reverse-dictionary lookup with metadata.
- [examples/datamuse-getsuggestions-example.json](examples/datamuse-getsuggestions-example.json) — autocomplete with spelling correction.

### Spectral Rules
- [rules/datamuse-rules.yml](rules/datamuse-rules.yml) — enforces operationId, Title Case summaries, snake_case query parameters, HTTPS servers, and 429 documentation.

### Naftiko Capabilities
- [capabilities/shared/datamuse-shared.yaml](capabilities/shared/datamuse-shared.yaml) — per-API operation primitives.
- [capabilities/word-discovery.yaml](capabilities/word-discovery.yaml) — combined semantic-relation discovery.
- [capabilities/rhyme-and-phonetics.yaml](capabilities/rhyme-and-phonetics.yaml) — rhymes, near rhymes, homophones, sounds-like.
- [capabilities/reverse-dictionary.yaml](capabilities/reverse-dictionary.yaml) — tip-of-the-tongue lookup with optional spelling hint.
- [capabilities/autocomplete.yaml](capabilities/autocomplete.yaml) — type-ahead suggestions with spelling correction.

### Vocabulary
- [vocabulary/datamuse-vocabulary.yml](vocabulary/datamuse-vocabulary.yml) — resources, endpoints, constraints, relations, ranking hints, metadata flags, vocabularies, plans, capabilities.

### Commercial & FinOps
- [plans/datamuse-plans-pricing.yml](plans/datamuse-plans-pricing.yml) — Free Non-Commercial (100k req/day, no key) and Commercial (negotiated).
- [rate-limits/datamuse-rate-limits.yml](rate-limits/datamuse-rate-limits.yml) — per-IP 100k/day on the free tier; commercial quotas negotiated.
- [finops/datamuse-finops.yml](finops/datamuse-finops.yml) — FOCUS mapping, allocation tags, optimization plays (caching, debouncing, scoping with `max`).

## Plan and Feature Gating

| Plan | Price | Quota | Custom Vocab | API Key | Commercial Use | SLA |
|---|---|---|---|---|---|---|
| Free Non-Commercial | $0 | 100,000 req/day | No | No | No | No |
| Commercial | Negotiated | Negotiated | Yes | Optional | Yes | Per contract |

To arrange commercial use, custom vocabularies, or elevated rate limits, contact Datamuse via the link on the API documentation page.

## Community SDKs

Datamuse does not maintain an official GitHub organization; the community has published wrappers in many languages:

| Language | Repository |
|---|---|
| Java | [sjblair/Datamuse4J](https://github.com/sjblair/Datamuse4J) |
| Python | [gmarmstrong/python-datamuse](https://github.com/gmarmstrong/python-datamuse) |
| Node.js | [ansteh/datamuse](https://github.com/ansteh/datamuse) |
| Swift | [ezefranca/datamuse-swift](https://github.com/ezefranca/datamuse-swift) |
| PHP | [owenvoke/datamuse-php-api-wrapper](https://github.com/owenvoke/datamuse-php-api-wrapper) |
| Go | [kostaspt/go-datamuse](https://github.com/kostaspt/go-datamuse) |
| Rust | [slogemann1/datamuse-api-wrapper](https://github.com/slogemann1/datamuse-api-wrapper) |
| .NET | [benhess02/DatamuseDotNet](https://github.com/benhess02/DatamuseDotNet) |
| Ruby | [mosegontar/rubymuse](https://github.com/mosegontar/rubymuse) |

## MCP Servers and AI Tooling

Multiple community Model Context Protocol servers expose the Datamuse API to LLM agents:

- [lacausecrypto/datamuse-mcp](https://github.com/lacausecrypto/datamuse-mcp)
- [pipeworx-io/mcp-datamuse](https://github.com/pipeworx-io/mcp-datamuse)
- [bhayanak/datamuse-mcp-server](https://github.com/bhayanak/datamuse-mcp-server) — 12+ word-finding tools.
- [pipeworx-io/mcp-words](https://github.com/pipeworx-io/mcp-words)
- [Eyalm321/multilingual-dictionary-mcp](https://github.com/Eyalm321/multilingual-dictionary-mcp) — combines Datamuse with ConceptNet and Wiktionary.

## Tags

Word Finding, Lexical Search, Natural Language, Vocabulary, Synonyms, Antonyms, Rhymes, Phonetics, Semantic Search, Reverse Dictionary, Autocomplete, Wordplay, Creative Writing, Vocabulary Apps, Word Games, Linguistics, Open Source Projects, Public APIs

## Timestamps

- **Created:** 2026-05-28
- **Modified:** 2026-05-29

## Maintainers

- **Kin Lane** — kin@apievangelist.com
