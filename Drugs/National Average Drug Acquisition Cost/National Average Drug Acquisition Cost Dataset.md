# National Average Drug Acquisition Cost Dataset

## Summary
The National Average Drug Acquisition Cost (NADAC) is designed to create a national benchmark that is reflective of the prices paid by retail community pharmacies to acquire prescription and over-the-counter covered outpatient drugs.

## Description
The NADAC is posted to reflect findings from the previous month’s survey results incorporating the weekly price changes that have occurred in the interim weeks before the next monthly NADAC file.

The NADAC for prescription and over-the-counter covered outpatient drugs is reported at the 11-digit National Drug Code (NDC) level. The NADAC is calculated at the drug grouping, drug category, and pharmacy type level.

The source of pharmacy survey data used to calculate the NADAC. ‘ C/I’ indicates data was collected from surveys of Chain/Independent pharmacies. Other pharmacy type indicators are not used at this time.

## Facts
- Date Created: 2013-11
- Date Modified: 2016-06-29
- Version: 2016.06.29
- Update Frequency: Weekly
- Temporal Coverage: 2013-09 to 2016-06-29
- Spatial Coverage: United States
- Source: US Food and Drug Administration (FDA)
- Source License URL: N/A
- Source License Requirements: Open for commercial use
- Source Citation: N/A
- Keywords: 
 - NADAC
 - Average Drug price
 - Drug price
- Other Titles
 - Average Drug Acquisition Cost
 - National Average Drug Acquisition Cost (NADAC)

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

- NADAC_Per_Unit
  - The National Average Drug Acquisition Cost per unit in USD
  - Type : Number
  - Level : Ratio
  - Required

- Effective_Date
  - The effective date of the NADAC Per Unit cost.
  - Type: Date
  - Required

- Pricing_Unit
  - Indicates the pricing unit for the associated NDC
  - Type : String
  - Required
  - Values: ML, GM, EA

- Pharmacy_Type_Indicator
  - The source of pharmacy survey data used to calculate the NADAC
  - Type: String
  - Required

- Is_OTC
  - Indicates whether or not the NDC is for an over-the-counter (OTC) product 
  - Type: Boolean
  - Required

- Explanation_Code

  - Codes that pertain to how the NADAC was calculated  
    Code 1: The NADAC was calculated using information from the most recently completed pharmacy survey.  
    Code 2: The average acquisition cost of the most recent survey was within ± 2% of the current NADAC; therefore, the NADAC was carried forward from the previous file.  
    Code 3: The NADAC based on survey data has been adjusted to reflect changes in published pricing, or as a result of an inquiry to the help desk.  
    Code 4: The NADAC was carried forward from the previous file.  
    Code 5: The NADAC was calculated based on package size.  
    Code 6: The CMS Covered Outpatient File drug category type of ‘S/I/N’ (Single Source/Innovator/Non-Innovator) has not been applied.  
    Codes 7 through 10: Reserved for future use.  
  - Type: String
  - Required
  - Values: 1, 2, 3, 4, 5, 6, 7, 8, 9, 10

- Classification_for_Rate_Setting
  - Indicates whether the NDC was considered brand (‘B’) or generic (‘G’) for the NADAC rate calculation process. If the NDC was considered brand (‘B’) and approved under an Abbreviated New Drug Application (ANDA), the indicator is shown as (‘B-ANDA’).
  - Type: String
  - Required
  - Values: B, B-ANDA, G

- Corresponding_Generic_Drug_NADAC_Per_Unit
  - The NADAC for the corresponding generic drug in USD
  - Type: Number
  - Level : Ratio
  - Currency:  USD

- Corresponding_Generic_Drug_Effective_Date
  - The effective date of when the Corresponding Generic Drug NADAC Per Unit is assigned to a multiple source brand drug NDC. This date may not correspond to the NADAC effective date for the generic drug due to the method by which the corresponding generic drug NADAC effective date is assigned.
  - Type: Date & Time

- As_of_Date
  - Last update date
  - Type: Date
  - Required
