# NADAC Week File Comparison

## Summary
The NADAC Weekly Comparison file identifies the drug products with current NADAC rates that are replaced with new NADAC rates.

## Description
The National Average Drug Acquisition Cost (NADAC) i is designed to create a national benchmark that is reflective of the prices paid by retail community pharmacies to acquire prescription and over-the-counter covered outpatient drugs.

The National Average Drug Acquisition Cost (NADAC) Weekly Comparison file identifies the drug products with new NADAC rates.
The Other changes (e.g. NDC additions and terminations) to the NADAC file are not reflected.

## Facts
- Date Created: 2013-11
- Date Modified: 2016-06-29
- Version: 2016.06.29
- Update Frequency: Weekly
- Temporal Coverage: 2013-11 to 2016-06-29
- Spatial Coverage: United States
- Source: US Food and Drug Administration (FDA)
- Source License URL: N/A
- Source License Requirements: Open for commercial use
- Source Citation: N/A
- Keywords: 
 - NADAC Comparison
 - Average Drug price changes
 - Drug price changes
- Other Titles 
 - Average Drug Acquisition Cost changes
 - National Average Drug Acquisition Cost (NADAC) comparison

## Schema
- NDC_Description
  - Identifies the drug name, strength, and dosage form of the drug product 
  - Type: String
  - Required

- NDC
  - National Drug Code  
  - Type: Integer
  - Level : Nominal
  - Required
  - Maximum Length : 11 

- Old_NADAC_Per_Unit
  - The National Average Drug Acquisition Cost per pricing unit from the previous NADAC Reference File
  - Type : Number
  - Level : Ratio
  - Required

- New_NADAC_Per_Unit
  - The National Average Drug Acquisition Cost per pricing unit from the current NADAC Reference File
  - Type : Number
  - Level : Ratio
  - Required

- Classification_for_Rate_Setting
  - Indicates whether the NDC was considered brand (‘B’) or generic (‘G’) for the NADAC rate calculation process. If the NDC was considered brand (‘B’) and approved under an Abbreviated New Drug Application (ANDA), the indicator is shown as (‘B-ANDA’).
  - Type: String
  - Required
  - Values: B, B-ANDA, G

- Percent_Change
  - The difference between the New NADAC Per Unit and the Old NADAC Per Unit, divided by the Old NADAC Per Unit in %.
  - Type : String
  - Required

- Primary_Reason
  - Describes the primary reason for the NADAC Per Unit change  
    Survey Rate: The NADAC Per Unit has been updated using information from the most recently completed pharmacy survey.  
    WAC Adjustment: The NADAC Per Unit has been updated to reflect changes in published pricing.  
    Help Desk Adjustment: The NADAC Per Unit has been updated as a result of an inquiry to the help desk.  
    Brand Generic Change: The NADAC Per Unit has been updated as a result of a change in the Classification for Rate Setting.  
    Rate Group Change: The NADAC Per Unit has been updated due to placement into a new NADAC drug grouping because of a change in the NDC attributes. NDC attributes that may result in a rate group change include package size updates, brand/generic designation redeterminations and revisions to the active ingredient(s), strength, dosage form or route of administration.  
  - Type: String
  - Required

- Start_Date
  - Start Date
  - Type: Date & Time
  - Required

- End_Date
  - End Date
  - Type: Date & Time
  - Required
