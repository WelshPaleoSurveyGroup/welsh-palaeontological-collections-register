# Welsh Palaeontological Collections Register

A developing, specimen-level register of palaeontological material from Wales, wherever that material is now held.

The project is designed to answer four basic questions:

1. **What Welsh palaeontological specimens are known?**
2. **Where are they held?**
3. **Where and from what geological context were they collected?**
4. **What publications, images, 3D resources, and provenance information are linked to them?**

This repository is intended as a research infrastructure project rather than a claim to provide a complete fossil census of Wales. Records are added conservatively, with uncertainties retained explicitly rather than silently normalised.

## Current status

**Release:** v0.3 — second-pass working register  
**Date:** 18 September 2026

The current workbook contains approximately:

- 79 specimen records
- 59 taxon records
- 44 locality records
- 38 geological-unit records
- 7 repository records
- 27 digital-asset records

Current sources include direct or cross-checked records from:

- Amgueddfa Cymru – Museum Wales
- Natural History Museum, London (NHMUK)
- GB3D Type Fossils Online
- Sedgwick Museum of Earth Sciences
- British Geological Survey
- Grosvenor Museum
- primary palaeontological literature

The register is **not yet exhaustive**. Major future targets include systematic locality-by-locality harvesting, broader non-type specimen coverage, Oxford and Cambridge collections, historical literature, and citation-chain searches.

## Repository structure

```text
welsh-palaeontological-collections-register/
├── README.md
├── CHANGELOG.md
├── CONTRIBUTING.md
├── CITATION.cff
├── LICENSE.md
├── .gitignore
├── .github/
│   ├── ISSUE_TEMPLATE/
│   │   ├── specimen-addition.md
│   │   └── correction.md
│   └── pull_request_template.md
├── data/
│   ├── master/
│   │   └── Welsh_Palaeontological_Collections_Register_v0.3_second_pass.xlsx
│   ├── raw/
│   │   └── README.md
│   └── exports/
│       └── README.md
└── docs/
    ├── DATA_DICTIONARY.md
    ├── SEARCH_PROTOCOL.md
    ├── SOURCE_ATTRIBUTION.md
    ├── SENSITIVE_LOCALITIES.md
    └── ROADMAP.md
```

## Data model

The master workbook contains linked tables for:

- **Specimens** — one row per identifiable accessioned specimen or defensible specimen lot
- **Taxa** — accepted and historical taxonomic identifications
- **Localities** — geographic provenance, including precision and sensitivity
- **Geological units** — stratigraphic and age information
- **Repositories** — institutions holding Welsh material
- **Publications** — primary descriptions, revisions, datasets, and collection resources
- **Collection events** — collectors, dates, and fieldwork history
- **Digital assets** — photographs, IIIF images, 3D resources, scans, and related assets
- **Historical provenance** — old labels, historic catalogue numbers, names, and collection histories
- **Unresolved questions** — uncertainties requiring further checking
- **Search queue** — reproducible search/audit workflow
- **Candidate tables** — staging areas before permanent IDs are assigned

See [`docs/DATA_DICTIONARY.md`](docs/DATA_DICTIONARY.md) for field-level guidance.

## Permanent identifiers

The project currently uses stable internal prefixes:

| Entity | Prefix | Example |
|---|---|---|
| Specimen | `WPR-SP-####` | `WPR-SP-0001` |
| Taxon | `WPR-TAX-####` | `WPR-TAX-0001` |
| Locality | `WPR-LOC-####` | `WPR-LOC-0001` |
| Geological unit | `WPR-GEO-####` | `WPR-GEO-0001` |
| Repository | `WPR-REP-####` | `WPR-REP-0001` |
| Publication | `WPR-PUB-####` | `WPR-PUB-0001` |
| Collection event | `WPR-EVT-####` | `WPR-EVT-0001` |
| Digital asset | `WPR-ASSET-####` | `WPR-ASSET-0001` |
| Historical provenance | `WPR-HIST-####` | `WPR-HIST-0001` |
| Unresolved question | `WPR-Q-####` | `WPR-Q-0001` |

Candidate records use `WPR-SP-CAND-####` and `WPR-PUB-CAND-####` until they have been checked and promoted.

## Inclusion principle

A record is in scope when the material has a defensible **Welsh palaeontological provenance**, irrespective of where the specimen is held today. For example, a Welsh fossil in London, Cambridge, Oxford, Keyworth, or an overseas museum remains part of the Welsh collections register.

A specimen should not be promoted into the master table merely because a paper says that a museum holds “several bones”. A specimen should be uniquely identifiable by accession/catalogue number or by sufficiently specific evidence to allow it to be independently relocated.

## Sensitive localities

Some fossil localities are vulnerable to collecting pressure, access restrictions, landowner concerns, or conservation issues. Public releases should therefore generalise or suppress precise coordinates where appropriate. See [`docs/SENSITIVE_LOCALITIES.md`](docs/SENSITIVE_LOCALITIES.md).

## Search methodology

The register is built through reproducible searches across museum catalogues, scholarly databases, historical literature, institutional repositories, and geological resources. Negative searches are logged as well as positive results. See [`docs/SEARCH_PROTOCOL.md`](docs/SEARCH_PROTOCOL.md).

## Contributing

Corrections, new specimen records, repository information, historical provenance, and links to digital assets are welcome. Please read [`CONTRIBUTING.md`](CONTRIBUTING.md) before submitting an issue or pull request.

## Licensing and attribution

The project compiles metadata from multiple institutions and publications. Source institutions retain rights in their images, scans, 3D models, and any source data subject to their own licences. The project does not claim ownership of third-party material.

See [`LICENSE.md`](LICENSE.md) and [`docs/SOURCE_ATTRIBUTION.md`](docs/SOURCE_ATTRIBUTION.md).

## Citation

If you use the register in research, cite the repository version or archived release used. A machine-readable citation template is included in [`CITATION.cff`](CITATION.cff).

## Project stage

This is currently a **working research register**. Taxonomy, stratigraphy, locality precision, and type status may change as records are checked against primary descriptions and curatorial catalogues.
