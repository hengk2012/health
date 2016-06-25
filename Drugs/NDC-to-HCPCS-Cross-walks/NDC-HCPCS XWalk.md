# NDC-HCPCS XWalk

## Summary
The NDC/HCPCS crosswalk file provides a list of National Drug Codes (NDC) that are assigned to a Level II HCPCS along with conversion factors that are used to price the applicable billings to allow processing of claims filed using the NCPDP format.

## Description
The NDC/HCPCS crosswalk file provides a list of National Drug Codes (NDC) that are assigned to a Level II HCPCS along with conversion factors that are used to price the applicable billings to allow processing of claims filed using the NCPDP format.
PDAC updates the file monthly to add, revise or delete NDCs as published by Redbook. The file provides all prior updates, along with details on the changes that occurred in that month.
The PDAC only adds and updates the NDC/HCPCS that are billable to the DMEMACs. Prior to the effective PDAC contract date of August 2008, all NDCs were updated. While these are still listed on the crosswalk file, they are not updated as changes are reported in Redbook.

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
 - NDC to HCPCS Crosswalk
 - 2016 NDC/HCPCS Crosswalk
- Other Titles
 - •	NDC/HCPCS CrossWalk
 
## Schema
- NDC
  - The National Drug Code (NDC) serves as a universal product identifier for human drugs and biologics. Each NDC must be reported as an 11-digit code unique to the manufacturer of the specific drug or product. 
  - Type: Number
  - Level: Nominal 
  - Required

- NDC_Mod
  - Healthcare Common Procedure Coding System (HCPCS) Level II codes may require the use of 
modifiers to capture the exact nature of the service. The Level II modifiers are two alphabetic or 
alphanumeric digits.
  - Type: String
  - Maximum Length: 2

- HCPCS
  - HCPCS codes are used by Medicare and monitored by the CMS. HCPCS Level II codes are assigned to every service a medical practitioner provides to a Medicare patient including durable medical equipment, prosthetics and orthotics supplies. These codes are an alpha character followed by four numbers.
  - Type: String
  - Required
  - Maximum Length : 5
  
- HCPCS_Mod
  - HCPCS Level II codes may require the use of modifiers to capture the exact nature of the service. The Level II modifiers are two alphabetic or alphanumeric digits.
  - Type: String
  - Maximum Length: 2

- Relationship_Start_Date
  - The relationship start date between the NDC and HCPCS code.
  - Type: Date
  - Required

- Relationship_End_Date
  - The relationship end date between the NDC and HCPCS code.
  - Type: String
  - Required

- HCPCS_Description
  - The long description of the HCPCS Level II code.
  - Type: String
  - Required

- NDC_Label
  - Product name given to the product by the manufacturer. Additional information on product may be provided. 
  - Type: String
  - Required

- Number_of_Items_in_NDC_Package
  - The amount of product contained in the package as defined by the billing unit standard of the National Council for Prescription Drug Programs (NCPDP).
  - Type: String
  - Required

- NDC_Package_Measure
  - The total size of the package in volume or number of units contained. 
  - Type: String
  - Required

- NDC_Package_Type
  - The container or package used for the drug product, i.e. vial, bottle, bag, etc. 
  - Type: String
  - Required

- Route_of_Administration
  - Identifies the product’s intake or application method. 
  - Type: String
  - Required

- Billing_Units
  - The unit of measure when billing NDC units. Provides the two-character abbreviation corresponding to valid units of measure per the NCPDP standard.
  - Type: String
  - Required
  - Maximum Length: 2

- HCPCS_Amount_1
  - The amount of product in a HCPCS billing unit (may be found in the HCPCS description). 
  - Type: Number
  - Level: Ratio
  - Required

- HCPCS_Measure_1
  - The number of HCPCS units in one NCPDP billing unit.
  - Type: String
  - Required

- CF
  - The Conversion Factor (CF) is the rate to convert HCPCS quantity to NDC quantity. This is derived by dividing the NDC amount by the HCPCS amount
  - Type: Number
  - Level: Ratio
  - Required

- Start_Date_1
  - The Start Date #1 is the relationship start date between the NDC and HCPCS code.
  - Type: Date
  - Required

- End_Date_1
  - The End Date #1 is the relationship start date between the NDC and HCPCS code.
  - Type: String
  - Required

- Prior_Start_Date_2
  - Prior Start Date.
  - Type: Date

- Prior_End_Date_2
  - Prior End Date.
  - Type: Date

- Prior_Conversion_Factor_2
  - Prior Conversion Factor. 
  - Type: Number
  - Level: Ratio

- Prior_Start_Date_3
  - Prior Start Date.
  - Type: Date

- Prior_End_Date_3
  - Prior End Date.
  - Type: Date

- Prior_Conversion_Factor_3
  - Prior Conversion Factor. 
  - Type: Number
  - Level: Ratio
