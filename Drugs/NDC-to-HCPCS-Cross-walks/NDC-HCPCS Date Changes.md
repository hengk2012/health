# NDC-HCPCS Date Changes

## Summary
The NDC/HCPCS Date Changes dataset provides a list of dates related changes The NDC/HCPCS crosswalk file. 

## Description
The NDC/HCPCS crosswalk file provides a list of National Drug Codes (NDC) that are assigned to a Level II HCPCS along with conversion factors that are used to price the applicable billings to allow processing of claims filed using the NCPDP format.
PDAC updates the file monthly to add, revise or delete NDCs as published by Redbook. The file provides all prior updates, along with details on the changes that occurred in that month.
The PDAC only adds and updates the NDC/HCPCS that are billable to the DMEMACs. Prior to the effective PDAC contract date of August 2008, all NDCs were updated. While these are still listed on the crosswalk file, they are not updated as changes are reported in Redbook.

The NDC/HCPCS Date Changes dataset provides a list of dates related changes The NDC/HCPCS crosswalk file. 

## Facts
- Date Created: 2014-01
- Date Modified: 2016-06
- Version: 2016.06
- Update Frequency: Monthly
- Temporal Coverage: N/A
- Spatial Coverage: United States
- Source: Noridian Healthcare Solutions
- Source License URL: N/A
- Source License Requirements: Open for commercial use
- Source Citation: N/A
- Keywords: 
 - NDC to HCPCS Date Changes 
 - 2016 NDC/HCPCS Date Changes
- Other Titles
 - NDC/HCPCS CrossWalk Date Changes
 
## Schema
- NDC
  - The National Drug Code (NDC) serves as a universal product identifier for human drugs and biologics. Each NDC must be reported as an 11-digit code unique to the manufacturer of the specific drug or product. 
  - Type: Number
  - Level: Nominal 
  - Required

- Change
  - Precise the changed date
  - Type: String
  - Required

- Old_Date
  - The old date before the last change
  - Type: String
  - Required

- New_Date
  - The updated date after the last change
  - Type: Date
  - Required
