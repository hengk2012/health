# NDC-HCPCS Conversion Factor Changes

## Summary
The NDC/HCPCS Conversion Factor Changes dataset provides a list of conversion factors comparing to The last month NDC/HCPCScrosswalk file. 

## Description
The NDC/HCPCS crosswalk file provides a list of National Drug Codes (NDC) that are assigned to a Level II HCPCS along with conversion factors that are used to price the applicable billings to allow processing of claims filed using the NCPDP format.
PDAC updates the file monthly to add, revise or delete NDCs as published by Redbook. The file provides all prior updates, along with details on the changes that occurred in that month.
The PDAC only adds and updates the NDC/HCPCS that are billable to the DMEMACs. Prior to the effective PDAC contract date of August 2008, all NDCs were updated. While these are still listed on the crosswalk file, they are not updated as changes are reported in Redbook.

The NDC/HCPCS Conversion Factor Changes dataset provides a list of conversion factors comparing to The last month NDC/HCPCScrosswalk file. 

## Facts
- Date Created: 2014-01
- Date Modified: 2016-05
- Version: 2016.05
- Update Frequency: Monthly
- Temporal Coverage: N/A
- Spatial Coverage: United States
- Source: Noridian Healthcare Solutions
- Source License URL: N/A
- Source License Requirements: Open for commercial use
- Source Citation: N/A
- Keywords: 
 - NDC to HCPCS Conversion Factor Changes
 - 2016 NDC/HCPCS Conversion Factor Changes
- Other Titles
 - NDC/HCPCS CrossWalk Conversion Factor Changes
 
## Schema
- NDC
  - The National Drug Code (NDC) serves as a universal product identifier for human drugs and biologics. Each NDC must be reported as an 11-digit code unique to the manufacturer of the specific drug or product. 
  - Type: Integer
  - Level: Nominal 
  - Required
  - Maximum Length: 13
  
- NDC_Mod
  - Healthcare Common Procedure Coding System (HCPCS) Level II codes may require the use of 
modifiers to capture the exact nature of the service. The Level II modifiers are two alphabetic or 
alphanumeric digits.
  - Type: String

- HCPCS
  - HCPCS codes are used by Medicare and monitored by the CMS. HCPCS Level II codes are assigned to every service a medical practitioner provides to a Medicare patient including durable medical equipment, prosthetics and orthotics supplies. These codes are an alpha character followed by four numbers. processing.
  - Type: String
  - Required
  - Maximum Length : 5
  
- HCPCS_Mod
  - HCPCS Level II codes may require the use of modifiers to capture the exact nature of the service. The Level II modifiers are two alphabetic or alphanumeric digits.
  - Type: String

- NEW_CF
  - New converation factor by NDC
  - Type: Number
  - Level: Ratio 
  - Required
