# Federal Upper Limit of Drug Pricing Manufacturer Cost
 
## Summary
The Federal Upper Limit (FUL) is 175% or more than the weighted average of the monthly average manufacturer prices (AMP) for purchasable pharmaceutically and therapeutically equivalent multiple source drug products. This data set includes FUL with Medicaid Drug Rebate information.

## Description
The Affordable Care Act revised the Federal Upper Limit (FUL) provisions to require that the Secretary calculate the FULs as no less than 175 percent of the weighted average (determined on the basis of utilization) of the most recently reported monthly average manufacturer prices (AMP) for pharmaceutically and therapeutically equivalent multiple source drug products that are available for purchase by retail community pharmacies on a nationwide basis.  In accordance with these provisions, the Centers for Medicare & Medicaid Services (CMS) issued a proposed rule (CMS-2345-P) that FULs would be calculated as 175 percent of the weighted average of AMPs.
In accordance with the final regulation with comment (CMS-2345-FC), we established an exception to the FUL calculation which allows for the use of a higher multiplier to calculate the FULs based on acquisition costs for certain multiple source drugs.  Specifically, we finalized an exception to calculating the FUL at an amount equal to 175 percent of the weighted average of the most recently reported monthly AMPs for pharmaceutically and therapeutically equivalent multiple source drugs in instances where that amount is less than the average retail community pharmacies' acquisition cost for such drugs as determined by the most current national survey of such costs.  In situations where the FUL is less than the average retail community pharmacies' acquisition cost, we will establish the FUL using a higher multiplier so that the FUL amount would equal the most current average retail community pharmacies acquisition cost as determined by the most current national survey of such costs.     
To implement this revision when we calculate the FULs each month, we intend to use the most current monthly National Average Drug Acquisition Cost pricing files.  See the Methodology and Data Elements Guide below for further information on the calculation of the Affordable Care Act FUL. 
We published the draft Affordable Care Act FULs calculated in accordance with CMS-2345-FC for two months before finalizing the FULs.  The final Affordable Care Act FULs are linked below, and will be effective on April 1, 2016 to coincide with the effective date of CMS-2345-FC.  States will have up to 30 days from the April 1, 2016 effective date to implement the FULs.  Thereafter, the FULs will be updated monthly on the Medicaid.gov website, and will be effective on the first date of the month following the publication of the update.  States will, likewise, have up to 30 days after the effective date to implement the FULs. Below is the link to the draft January 2016 and February 2016 Affordable Care Act FULs and the Methodology and Data Elements Guide used to calculate the Affordable Care Act FULs.

## Facts
- Date Created: N/A
- Date Modified: 2016-06-01
- Version: 2016.06.29
- Update Frequency: Monthly
- Temporal Coverage: 2016-03 to 2016-06-29
- Spatial Coverage: USA
- Source: Centers of Medicare and Medicaid Services
- Source License URL: https://www.medicaid.gov/medicaid-chip-program-information/by-topics/benefits/prescription-drugs/federal-upper-limits.html
- Source License Requirements: None
- Source Citation:  Federal Upper Limit Extreme Details 2015, Jan 22nd, 2016. 
- Keywords: 
 - Federal Upper Limit
 - Drug pricing
 - Drug price amount
 - Medicaid Fee
 - Medicaid Drug
 - Manufacturer
- Other Titles:
 - FUL
 - Federal Upper Limits of Drug Pricing Medicaid Fee 2016-05
 - Federal Upper Limits of Medicaid Drug Pricing 2016-05
 - Federal Upper Limits of Manufacturer Drug Pricing 2016-05

## Schema
- Product_Group 
 - Product group of the drug 
 - Type: Integer
 - Level: Nominal
 - Required

- Ingredient 
 - Ingredient of the drug 
 - Type: String
 - Required

- Strength 
 - Strength of the drug 
 - Type: String
 - Required

- Dosage 
 - Type of dosage 
 - Type: String
 - Required
 
- Route
 - Delivery method for the drug
 - Type: String
 - Required
 
- Minimum_Daily_Requirement_Unit_Type
 - AHF, CAP, EA, GM, ML, SUP, TAB, TDP 
 - Type: String
 - Required

- Weighted_Average_Average_Manufacturer_Prices
 - Monthly Weighted Average Manufacturer Prices 
 - Type: Number
 - Level: Ratio
 - Required

- Affordable_Care_Act_Federal_Upper_Limit
 - Affordable Care Act Federal Upper Limit 
 - Type: Number
 - Level: Ratio
 - Required

- Package_Size 
 - Package size 
 - Type: Number
 - Level: Ratio
 - Required

- National_Drug_Code 
 - NDC Code 
 - Type: String
 - Required

- Is_A_Rated 
 - true or false 
 - Type: Boolean
 - Required

- Multiplier_Greater_Than_175_Percent_of_Weighted_Avg_of_Average_Manufacturer_Prices 
 - "ACA FUL Increased to Equal NADAC" or "ACA FUL Equals 175 Percent of Weighted Average of AMPs"
 - Type: String
 - Required
