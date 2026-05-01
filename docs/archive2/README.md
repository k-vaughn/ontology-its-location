## Location referencing methodology modules (scaffold)

This directory scaffolds a modular structure for ITS location referencing **methodologies** (not interface standards).

- **Status**: initial scaffold only; existing `docs/*.ttl` files remain unchanged.
- **Namespace**: all modules use `https://w3id.org/itsdata/location/v1/` (one namespace per repository).
- **Network dependency**: transport network primitives are intended to be reused from City Data Model Part 3 Transport (`https://w3id.org/citydata/part3/v1/`).

### Modules
- `core.ttl`, `core-shacl.ttl`: shared abstractions (`LocationReference`, collections/itineraries)
- `geometry-pattern.ttl`, `geometry-shacl.ttl`: coordinate/geometry primitives (GeoSPARQL integration)
- `quality-pattern.ttl`, `quality-shacl.ttl`: positional quality / uncertainty
- Method modules (each has a matching `*-shacl.ttl`):
  - `coordinate-location-*`
  - `area-location-*`
  - `network-location-*`
  - `linear-referencing-*`
  - `offset-location-*`
  - `address-location-*`
  - `external-id-location-*`

### Adapters
Standard-specific alignments live under `adapters/` (Alert-C, OpenLR, TPEG), and should primarily map their constructs onto the methodology modules without duplicating primitives.

