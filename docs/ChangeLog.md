
# Change Log

## Changes 2021-10-12
Biggest update to the SRF in a while.
Updated Version to 4.0.0

- Added New Rules:
  - Developers can Manage Content Libraries with RWA
  - Developers can Manage Extensions with RWA
  - Default Rule for Extensions Added allows read by default unless limited with GWA
    - **QC_Extension_Read|Default** (Disabled by default)
  - Default Rule for Content Libraries Added allows read by default unless limited with GWA
    - **QC_ContentLibrary_Read|Default** (Disabled by default)


- Replaced Tag used by the Security Rules Framework from "QC" with "SRF"
- Updated All SRF Object ID's to a consistent convention to allow for modification and versioning

  **53524600-0004-2021-1031-\<Random>**
  
  | Segment  | Values                            |
  | -------- | --------------------------------- |
  |53524600|HEX: SRF|
  |0004|SRF Version|
  |2021|Year|
  |1031|MonthDay|
  |\<Random>|Unique Component|

- Updated Rules:
  - Applied New Naming Convention
  - Replaced "QC" tag with "SRF"
  - Updated ID's

- Extended RolesWithAccess to include:
  - Content Libraries
  - Extensions
  
  
## Changes 2021-04-29

### Added
- [DeepLinks](./docs/CustomProperties/DeepLinks.md)

### Changed
- Documentation
- [Security Rules](./docs/SecurityRules/Overview.md)
  - Naming conventions
- [Unit Test Cases 3.0.1](./docs/RM-UnitTestCases.md)

