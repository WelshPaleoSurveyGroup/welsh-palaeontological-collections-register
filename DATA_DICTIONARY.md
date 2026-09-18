# Data dictionary

## Specimens

| Field | Meaning |
|---|---|
| `specimen_id` | Permanent internal specimen identifier (`WPR-SP-####`). |
| `taxon_id` | Link to the Taxa table. |
| `repository_id` | Link to the Repositories table. |
| `catalogue_number` | Repository accession/catalogue number exactly as used by the source where possible. |
| `element` | Anatomical element, specimen description, or lot content. |
| `locality_id` | Link to the Localities table. |
| `geological_unit_id` | Link to the Geological units table. |
| `collection_event_id` | Link to a collecting event when known. |
| `collector` | Collector as stated in the source. |
| `collection_date` | Collection date or best-supported date. |
| `type_status` | Holotype, paratype, syntype, lectotype, referred, non-type, etc. |
| `figured_status` | Whether the specimen is explicitly figured. |
| `identification_confidence` | Confidence in taxonomic identification. |
| `provenance_confidence` | Confidence in locality/provenance. |
| `disposition_status` | Museum accessioned, private, awaiting accession, lost/unlocated, etc. |
| `photograph_available` | Whether an accessible specimen image is known. |
| `3d_available` | Whether a CT/3D representation is known. |
| `primary_publication_id` | Link to the most relevant primary publication. |
| `source_url` | Stable catalogue, database, or primary-source URL. |
| `notes` | Evidence, conflicts, caveats, and source-specific detail. |

## Taxa

Stores accepted names, historical identifications, synonyms, higher-group placement, and confidence.

## Localities

Stores modern/historical locality wording, county/area, coordinates, coordinate precision, site type, geology link, access, and sensitivity status.

## Geological units

Stores group, formation, member, period, epoch, stage, numerical age where appropriate, lithology, references, and notes.

## Repositories

Stores institution, acronym, location, department/collection, catalogue URL, enquiry URL, online-access status, and notes.

## Publications

Stores full citation, year, DOI, taxa/localities/specimens discussed, contribution, source type, and source URL.

## Digital assets

Links specimens to photographs, IIIF resources, scans, CT data, or 3D records and records platform, licence, creator, and identifier.

## Historical provenance

Preserves original labels, old catalogue numbers, historical names, historic localities, source collections, and source references.

## Unresolved questions

Stores issues that should not be resolved by guesswork: uncertain type status, conflicting catalogue information, unclear locality, changing taxonomy, missing specimens, etc.
