# GMDM-IOP
Official Grid Model Data Management (GMDM) profile repository used by EPRI's Vendor Forum and related tooling.

This repository contains the RDFS profile artifacts, example instance data, and supporting files used for validating and demonstrating GMDM exchange profiles.

## Repository Layout

### Information Model/
Enterprise Architect model file used as a reference: `CIM_Grid18v15_Enterprise14v04_Market04v18_GMDM_v1.3.eap`

### Profiles/
RDFS profile artifacts and JSON schema files that define exchange profiles:
- `Asset.rdfs-2020.rdfs` - Asset profile
- `DiagramLayout.rdfs-2020.rdfs` - Diagram layout profile
- `GeographicalLocation.rdfs-2020.rdfs` - Geographical location profile
- `MarketDER.draft-2020-12.schema.json` - Market DER JSON schema
- `MarketNode.rdfs-2020.rdfs` - Market node profile
- `UnbalancedConnectivity.rdfs-2020.rdfs` - Unbalanced connectivity profile
- `UnbalancedElectrical.rdfs-2020.rdfs` - Unbalanced electrical profile

### Instance Data/
Example CIM instance XML files organized by source system:

#### Models/from Bentley/
Facilities SubTransmission exports from Bentley systems:
- `Facilities SubTransmission/` - Contains three substations with connectivity and naming convention files

#### Models/from GEV/
Facilities Distribution exports from GEV systems:
- `Facilities Distribution/` - Contains geographical location and unbalanced connectivity data for three circuits:
  - Central Neighborhood
  - Industrial District
  - Old Town

#### Models/from GMDM/
Master grid model data organized by voltage level and profile:
- `Master Complete/` - Complete consolidated model files (asset, connectivity, electrical, location, marketnode)
- `Master D-to-SubT-Boundary/` - Distribution to SubTransmission boundary interfaces
- `Master Distribution/` - Distribution level assets, connectivity, electrical, and geographical location
- `Master SubTransmission/` - SubTransmission level assets, connectivity, electrical, and geographical location
- `merge.xml` - Merge configuration file

## Data Organization
The instance data follows GMDM naming conventions with profile identifiers:
- `CN` - Connectivity profile (Naming Convention)
- `GL` - Geographical Location profile
- `EL` - Electrical profile
- `Asset` - Asset profile

Each file is versioned and dated to track the evolution of the model data.

## License
See LICENSE at the repository root for license details.
