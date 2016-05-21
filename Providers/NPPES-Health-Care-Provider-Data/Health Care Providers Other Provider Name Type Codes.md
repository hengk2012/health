# Health Care Providers Other Provider Name Type Codes

## Summary
This data set contains the code set for Other Provider Name Type Codes

## Description
Corresponding Fields in the “Health care providers NPI data” dataset: 
- Provider_Other_Organization_Name_Type_Code 
- Provider_Other Last_Name_Type_Code 


## Facts
- Date Created: 2007-09
- Date Modified: 2016-05-10
- Version: 2016.05
- Update Frequency: Monthly
- Temporal Coverage: 2005-05 to 2016-05
- Spatial Coverage: United States
- Source: Centers of Medicare and Medicaid Services (CMS)
- Source License URL: N/A
- Source License Requirements: N/A
- Source Citation: N/A
- Keywords:
 - National Provider Identifier Standard (NPI)
 - NPPES
 - Regulation & Guidance
 - Data Dissemination
- Other Titles
 - Other Provider Name Type Codes

## Schema
- Name_Type_Code
  - Name Type Code  
  - Type: Integer
  - Level: Nominal
  - Required
  - Unique
  - Format: short

- Name_Type_Description
  - Description  
  - Type: String
  - Maximum Length: 50

- Entity_Name_Type
  - Entity Type
  - Type: String
  - Values: Individual, Organization, Both
  - Maximum Length: 20
