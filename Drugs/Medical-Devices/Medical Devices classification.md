# Medical Devices classification

## Summary
The Medical Devices classification Database contains medical device names and associated information developed by the Center for Devices and Radiological Health (CDRH) in support of its mission
## Description
The Medical Devices Classification Database contains medical device names and associated information developed by the Center for Devices and Radiological Health (CDRH) in support of its mission. This database contains device names and their associated product codes. The name and product code identify the generic category of a device for FDA. The Product Code assigned to a device is based upon the medical device product classification designated under 21 CFR Parts 862-892.

## Facts
- Date Created: 2014-06
- Date Modified: 2016-06-29
- Version: 2016.06.29
- Update Frequency: weekly
- Temporal Coverage: N/A
- Spatial Coverage: United States
- Source: Food and Drug Administration (FDA)
- Source License URL: N/A
- Source License Requirements: Open for commercial use
- Source Citation: N/A
- Keywords: 
 - Medical Devices classification
 - Device Classification Panels
 - Product Code
- Other Titles
 - Product Code Classification Database
 - Device Classification 

## Schema
- REVIEW_PANEL
  - REVIEW_PANEL
  - Type: String
  - Maximum Length : 2

- MEDICALSPECIALTY
  - medical specialty panel responsible for reviewing the product
  - Type: String
  - Maximum Length : 2
  
- PRODUCTCODE
  - Product Code
  - Type: String
  - Required
  - Maximum Length : 3

- DEVICENAME
  - Device Category Name
  - Type: String
  - Required

- DEVICECLASS
  - level of CDRH regulation
  - Type: String
  - Required
  - Values: 1, 2, 3, f, N, U 
  - Maximum Length : 1

- UNCLASSIFIED_REASON
  - Unclassified Reason Code
  - Type: String
  - Maximum Length : 2
  
- Is_GMPEXEMPTFLAG
  - GMP Exempt Flag
  - Type: Boolean
  - Required

- THIRDPARTYFLAG
  - Third Party Review Eligible
  - Type: String
  - Required
  - Values: N, P, Y
  - Maximum Length : 1
  
- REVIEWCODE
  - Third Party Review Code
  - Type: String

- REGULATIONNUMBER
  - Regulation number of classification regulation which identifies this device
  - Type: String

- SUBMISSION_TYPE_ID
  - Submission Type ID
  - Type: Number
  - Level: Nominal

- DEFINITION
  - Definition
  - Type: String

- PHYSICALSTATE
  - Physical state of product
  - Type: String

- TECHNICALMETHOD
  - Technical method
  - Type: String

- TARGETAREA
  - Target area in body
  - Type: String

- Is_Implant_Flag
  - Implant product
  - Type: Boolean

- Is_Life_Sustain_support_flag
  - Life Sustain product
  - Type: Boolean
