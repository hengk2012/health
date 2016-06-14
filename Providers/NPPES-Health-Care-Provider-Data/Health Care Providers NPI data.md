# Health Care Providers NPI data

## Summary
This data set contains the Health Care Providers data. Each line in the data set represents an NPI record.  
The NPI is a unique identification number for covered health care providers.  

## Description
In September 2007, CMS began disclosing National Plan and Provider Enumeration System (NPPES) health care provider data that are disclosable under the Freedom of Information Act (FOIA) to the public. The NPI is a 10-position, intelligence-free numeric identifier (10-digit number). The NPI must be used in lieu of legacy provider identifiers in the HIPAA standards transactions.  

This dataset will contain all of the FOIA-disclosable provider data in NPPES. It contains the fields identified in the NPPES Data Dissemination Notice and certain sub-fields related to those fields will be disclosed in the data set.   

Note: CMS will mask SSNs, IRS ITINs, and EINs when these numbers are entered in the Other Provider Identifier Number and License Number fields as <Unavail>. This action also includes the continued suppression of the EINs and the suppression of the Subpart Parent Organization TINs of all Organizations in the downloadable file. CMS expects to lift the suppression of EINs and Parent Organization TINs in the future.

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
 - Health care providers
 - Regulation & Guidance
 - Data Dissemination
- Other Titles
 - Full Replacement Monthly NPI File
 - NPPES Data Dissemination
 - NPI Data Analytics for Individual/Organization
 - NPI Data Analytics for Sole Proprietor/Subpart
 - NPI Data Analytics for male/female
 - NPI Data Analytics for US States
 - NPI Data Analytics for Countries
 - NPI Data Analytics for Taxonomy Codes

## Schema
- NPI
  - The NPI is a 10-digit unique identification number for covered health care providers. 
  - Type: Integer
  - Level: Nominal
  - Required
  - Unique
  - Format : long
  - Pattern: \d{10}
  
- Entity_Type
  - Individual or Organization  
  - Type: String
  - Values: Individual, Organization

- Replacement_NPI 
  - The NPI is a 10-digit unique identification number for covered health care providers. 
  - Type: Integer
  - Level: Nominal
  - Format : long
  - Pattern: \d{10}
  
- Employer_Identification_Number
  - Employer Identification number. The value is not disclosed by CMS 
  - Type: String
  
- Provider_Organization_Name
  - Legal Business Name 
  - Type: String
  - Maximum Length: 70
  
- Provider_Last_Name
  - Legal Name 
  - Type: String
  - Maximum Length: 35
  
- Provider_First_Name 
  - First Name 
  - Type: String
  - Maximum Length: 20
  
- Provider_Middle_Name
  - Middle Name 
  - Type: String
  - Maximum Length: 20
  
- Provider_Name_Prefix_Code
  - Name Prefix codes  
  - Type: String
  - Maximum Length: 5
  - Reference: People/Names/Name Prefixes
  
- Provider_Name_Suffix_Code 
  - Name Suffix codes  
  - Type: String
  - Maximum Length: 5
  - Reference: People/Names/Name Suffixes
  
- Provider_Credential_Text
  - Provider Credential Text
  - Type: String
  - Maximum Length: 20
  
- Provider_Other_Organization_Name
  - Organization Name
  - Type: String
  - Maximum Length: 70
  
- Provider_Other_Organization_Name_Type_Code
  - Provider Other Organization Name Type, Reference dataset 
  - Type: Integer
  - Level: Nominal
  - Format : short
  - Reference: Health Care Providers Other Provider Name Type Codes
  
- Provider_Other_Last_Name
  - Legal Name 
  - Type: String
  - Maximum Length: 35
  
- Provider_Other_First_Name 
  - First Name 
  - Type: String
  - Maximum Length: 20
  
- Provider_Other_Middle_Name
  - Middle Name 
  - Type: String
  - Maximum Length: 20
  
- Provider_Other_Name_Prefix_Code
  - Name Prefix codes  
  - Type: String
  - Maximum Length: 5
  - Reference: People/Names/Name Prefixes
  
- Provider_Other_Name_Suffix_Code 
  - Name Suffix codes  
  - Type: String
  - Maximum Length: 5
  - Reference: People/Names/Name Suffixes
  
- Provider_Other_Credential_Text
  - Provider Credential Text
  - Type: String
  - Maximum Length: 20
  
- Provider_Other_Last_Name_Type_Code
  - Provider Other Last Name Type, Reference dataset 
  - Type: Integer
  - Level: Nominal
  - Format : short
  - Reference: Health Care Providers Other Provider Name Type Codes
  
- Provider_First_Line_Business_Mailing_Address
  - First line business address 
  - Type: String
  - Maximum Length: 55
  
- Provider_Second_Line_Business_Mailing_Address
  - Second line business address
  - Type: String
  - Maximum Length: 55
  
- Provider_Business_Mailing_Address_City_Name
  - City name 
  - Type: String
  - Maximum Length: 40
  
- Provider_Business_Mailing_Address_State_Name
  - US State Code
  - Type: String
  - Maximum Length: 100
  
- Provider_Business_Mailing_Address_Postal_Code
  - Zip Code 
  - Type: String
  - Maximum Length: 20
  
- Provider_Business_Mailing_Address_Country_Code
  - Country Code
  - Type: String
  - Maximum Length: 2
  
- Provider_Business_Mailing_Address_Telephone_Number
  - Telephone number 
  - Type: String
  - Maximum Length: 20
  
- Provider_Business_Mailing_Address_Fax_Number
  - Fax number
  - Type: String
  - Maximum Length: 20
  
- Provider_First_Line_Business_Practice_Location_Address
  - First line business address
  - Type: String
  - Maximum Length: 55
  
- Provider_Second_Line_Business_Practice_Location_Address
  - Second line business address
  - Type: String
  - Maximum Length: 55

- Provider_Business_Practice_Location_Address_City_Name
  - City name 
  - Type: String
  - Maximum Length: 40
  
- Provider_Business_Practice_Location_Address_State_Name
  - US State Code
  - Type: String
  - Maximum Length: 100
  
- Provider_Business_Practice_Location_Address_Postal_Code
  - Zip Code 
  - Type: String
  - Maximum Length: 20
  
- Provider_Business_Practice_Location_Address_Country_Code
  - Country Code
  - Type: String
  - Maximum Length: 2
  
- Provider_Business_Practice_Location_Address_Telephone_Number
  - Telephone number 
  - Type: String
  - Maximum Length: 20
  
- Provider_Business_Practice_Location_Address_Fax_Number
  - Fax number
  - Type: String
  - Maximum Length: 20
  
- Provider_Enumeration_Date
  - Enumeration date
  - Type: Date
  - Format: Date

- Last_Update_Date
  - Update date
  - Type: Date
  - Format: Date 
 
- NPI_Deactivation_Reason
  - Reasons for deactivation
  - Type: String
  - Values: Death, Disbandment, Fraud, Other
  - Maximum Length: 20
  
- NPI_Deactivation_Date
  - NPI Deactivation date
  - Type: Date
  - Format: Date 
 
- NPI_Reactivation_Date
  - NPI Reactivation date
  - Type: Date
  - Format: Date
 
- Provider_Gender_Code
  - Gender code
  - Type: String
  - Values: male, female
  - Maximum Length: 20
 
- Authorized_Official_Last_Name
  - Legal Name 
  - Type: String
  - Maximum Length: 35
  
- Authorized_Official_First_Name 
  - First Name 
  - Type: String
  - Maximum Length: 20
  
- Authorized_Official_Middle_Name
  - Middle Name 
  - Type: String
  - Maximum Length: 20 
 
- Authorized_Official_Title_or_Position
  - Title 
  - Type: String
  - Maximum Length: 35
  
- Authorized_Official_Telephone_Number
  - Telephone Number 
  - Type: String
  - Maximum Length: 20 
 
- Healthcare_Provider_Taxonomy_Code_1
  - Health Care Provider Taxonomy Code 
  - Type: String
  - Maximum Length: 10
  
- Provider_License_Number_1
  - License Number
  - Type: String
  - Maximum Length: 20 
 
- Provider_License_Number_State_Code_1
  - US State Code
  - Type: String
  - Maximum Length: 2
  
- Is_Healthcare_Provider_Primary_Taxonomy_1
  - true- The taxonomy is the primary taxonomy (there can be only one per NPI record),false- The taxonomy is not the primary taxonomy, null – Not answered
  - Type: Boolean
  
- Healthcare_Provider_Taxonomy_Code_2
  - Health Care Provider Taxonomy Code 
  - Type: String
  - Maximum Length: 10
  
- Provider_License_Number_2
  - License Number
  - Type: String
  - Maximum Length: 20 
 
- Provider_License_Number_State_Code_2
  - US State Code
  - Type: String
  - Maximum Length: 2
  
- Is_Healthcare_Provider_Primary_Taxonomy_2
  - true- The taxonomy is the primary taxonomy (there can be only one per NPI record),false- The taxonomy is not the primary taxonomy, null – Not answered
  - Type: Boolean
  
- Healthcare_Provider_Taxonomy_Code_3
  - Health Care Provider Taxonomy Code 
  - Type: String
  - Maximum Length: 10
  
- Provider_License_Number_3
  - License Number
  - Type: String
  - Maximum Length: 20 
 
- Provider_License_Number_State_Code_3
  - US State Code
  - Type: String
  - Maximum Length: 2
  
- Is_Healthcare_Provider_Primary_Taxonomy_3
  - true- The taxonomy is the primary taxonomy (there can be only one per NPI record),false- The taxonomy is not the primary taxonomy, null – Not answered
  - Type: Boolean
  
- Healthcare_Provider_Taxonomy_Code_4
  - Health Care Provider Taxonomy Code 
  - Type: String
  - Maximum Length: 10
  
- Provider_License_Number_4
  - License Number
  - Type: String
  - Maximum Length: 20 
 
- Provider_License_Number_State_Code_4
  - US State Code
  - Type: String
  - Maximum Length: 2
  
- Is_Healthcare_Provider_Primary_Taxonomy_4
  - true- The taxonomy is the primary taxonomy (there can be only one per NPI record),false- The taxonomy is not the primary taxonomy, null – Not answered
  - Type: Boolean
  
- Healthcare_Provider_Taxonomy_Code_5
  - Health Care Provider Taxonomy Code 
  - Type: String
  - Maximum Length: 10
  
- Provider_License_Number_5
  - License Number
  - Type: String
  - Maximum Length: 20 
 
- Provider_License_Number_State_Code_5
  - US State Code
  - Type: String
  - Maximum Length: 2
  
- Is_Healthcare_Provider_Primary_Taxonomy_5
  - true- The taxonomy is the primary taxonomy (there can be only one per NPI record),false- The taxonomy is not the primary taxonomy, null – Not answered
  - Type: Boolean
  
- Healthcare_Provider_Taxonomy_Code_6
  - Health Care Provider Taxonomy Code 
  - Type: String
  - Maximum Length: 10
  
- Provider_License_Number_6
  - License Number
  - Type: String
  - Maximum Length: 20 
 
- Provider_License_Number_State_Code_6
  - US State Code
  - Type: String
  - Maximum Length: 2
  
- Is_Healthcare_Provider_Primary_Taxonomy_6
  - true- The taxonomy is the primary taxonomy (there can be only one per NPI record),false- The taxonomy is not the primary taxonomy, null – Not answered
  - Type: Boolean
  
- Healthcare_Provider_Taxonomy_Code_7
  - Health Care Provider Taxonomy Code 
  - Type: String
  - Maximum Length: 10
  
- Provider_License_Number_7
  - License Number
  - Type: String
  - Maximum Length: 20 
 
- Provider_License_Number_State_Code_7
  - US State Code
  - Type: String
  - Maximum Length: 2
  
- Is_Healthcare_Provider_Primary_Taxonomy_7
  - true- The taxonomy is the primary taxonomy (there can be only one per NPI record),false- The taxonomy is not the primary taxonomy, null – Not answered
  - Type: Boolean
  
- Healthcare_Provider_Taxonomy_Code_8
  - Health Care Provider Taxonomy Code 
  - Type: String
  - Maximum Length: 10
  
- Provider_License_Number_8
  - License Number
  - Type: String
  - Maximum Length: 20 
 
- Provider_License_Number_State_Code_8
  - US State Code
  - Type: String
  - Maximum Length: 2
  
- Is_Healthcare_Provider_Primary_Taxonomy_8
  - true- The taxonomy is the primary taxonomy (there can be only one per NPI record),false- The taxonomy is not the primary taxonomy, null – Not answered
  - Type: Boolean
  
- Healthcare_Provider_Taxonomy_Code_9
  - Health Care Provider Taxonomy Code 
  - Type: String
  - Maximum Length: 10
  
- Provider_License_Number_9
  - License Number
  - Type: String
  - Maximum Length: 20 
 
- Provider_License_Number_State_Code_9
  - US State Code
  - Type: String
  - Maximum Length: 2
  
- Is_Healthcare_Provider_Primary_Taxonomy_9
  - true- The taxonomy is the primary taxonomy (there can be only one per NPI record),false- The taxonomy is not the primary taxonomy, null – Not answered
  - Type: Boolean
  
- Healthcare_Provider_Taxonomy_Code_10
  - Health Care Provider Taxonomy Code 
  - Type: String
  - Maximum Length: 10
  
- Provider_License_Number_10
  - License Number
  - Type: String
  - Maximum Length: 20 
 
- Provider_License_Number_State_Code_10
  - US State Code
  - Type: String
  - Maximum Length: 2
  
- Is_Healthcare_Provider_Primary_Taxonomy_10
  - true- The taxonomy is the primary taxonomy (there can be only one per NPI record),false- The taxonomy is not the primary taxonomy, null – Not answered
  - Type: Boolean
  
- Healthcare_Provider_Taxonomy_Code_11
  - Health Care Provider Taxonomy Code 
  - Type: String
  - Maximum Length: 10
  
- Provider_License_Number_11
  - License Number
  - Type: String
  - Maximum Length: 20 
 
- Provider_License_Number_State_Code_11
  - US State Code
  - Type: String
  - Maximum Length: 2
  
- Is_Healthcare_Provider_Primary_Taxonomy_11
  - true- The taxonomy is the primary taxonomy (there can be only one per NPI record),false- The taxonomy is not the primary taxonomy, null – Not answered
  - Type: Boolean
  
- Healthcare_Provider_Taxonomy_Code_12
  - Health Care Provider Taxonomy Code 
  - Type: String
  - Maximum Length: 10
  
- Provider_License_Number_12
  - License Number
  - Type: String
  - Maximum Length: 20 
 
- Provider_License_Number_State_Code_12
  - US State Code
  - Type: String
  - Maximum Length: 2
  
- Is_Healthcare_Provider_Primary_Taxonomy_12
  - true- The taxonomy is the primary taxonomy (there can be only one per NPI record),false- The taxonomy is not the primary taxonomy, null – Not answered
  - Type: Boolean
  
- Healthcare_Provider_Taxonomy_Code_13
  - Health Care Provider Taxonomy Code 
  - Type: String
  - Maximum Length: 10
  
- Provider_License_Number_13
  - License Number
  - Type: String
  - Maximum Length: 20 
 
- Provider_License_Number_State_Code_13
  - US State Code
  - Type: String
  - Maximum Length: 2
  
- Is_Healthcare_Provider_Primary_Taxonomy_13
  - true- The taxonomy is the primary taxonomy (there can be only one per NPI record),false- The taxonomy is not the primary taxonomy, null – Not answered
  - Type: Boolean
  
- Healthcare_Provider_Taxonomy_Code_14
  - Health Care Provider Taxonomy Code 
  - Type: String
  - Maximum Length: 10
  
- Provider_License_Number_14
  - License Number
  - Type: String
  - Maximum Length: 20 
 
- Provider_License_Number_State_Code_14
  - US State Code
  - Type: String
  - Maximum Length: 2
  
- Is_Healthcare_Provider_Primary_Taxonomy_14
  - true- The taxonomy is the primary taxonomy (there can be only one per NPI record),false- The taxonomy is not the primary taxonomy, null – Not answered
  - Type: Boolean
  
- Healthcare_Provider_Taxonomy_Code_15
  - Health Care Provider Taxonomy Code 
  - Type: String
  - Maximum Length: 10
  
- Provider_License_Number_15
  - License Number
  - Type: String
  - Maximum Length: 20 
 
- Provider_License_Number_State_Code_15
  - US State Code
  - Type: String
  - Maximum Length: 2
  
- Is_Healthcare_Provider_Primary_Taxonomy_15
  - true- The taxonomy is the primary taxonomy (there can be only one per NPI record),false- The taxonomy is not the primary taxonomy, null – Not answered
  - Type: Boolean

- Other_Provider_Identifier_1
  - Other provider identifier
  - Type: String
  - Maximum Length: 20
  
- Other_Provider_Identifier_Type_Code_1
  - The name of the health plan that issued the Other Provider Identifier 
  - Type: String
  - Maximum Length: 2 
  - Reference: Health Care Providers Other Provider Identifier Issuer Type Codes
 
- Other_Provider_Identifier_State_Code_1
  - US State Code
  - Type: String
  - Maximum Length: 2
  
- Other_Provider_Identifier_Issuer_1
  - Provider Identifier
  - Type: String
  - Maximum Length: 80
 
- Other_Provider_Identifier_2
  - Other provider identifier
  - Type: String
  - Maximum Length: 20
  
- Other_Provider_Identifier_Type_Code_2
  - The name of the health plan that issued the Other Provider Identifier 
  - Type: String
  - Maximum Length: 2 
  - Reference: Health Care Providers Other Provider Identifier Issuer Type Codes
 
- Other_Provider_Identifier_State_Code_2
  - US State Code
  - Type: String
  - Maximum Length: 2
  
- Other_Provider_Identifier_Issuer_2
  - Provider Identifier
  - Type: String
  - Maximum Length: 80 
 
- Other_Provider_Identifier_3
  - Other provider identifier
  - Type: String
  - Maximum Length: 20
  
- Other_Provider_Identifier_Type_Code_3
  - The name of the health plan that issued the Other Provider Identifier 
  - Type: String
  - Maximum Length: 2 
  - Reference: Health Care Providers Other Provider Identifier Issuer Type Codes
 
- Other_Provider_Identifier_State_Code_3
  - US State Code
  - Type: String
  - Maximum Length: 2
  
- Other_Provider_Identifier_Issuer_3
  - Provider Identifier
  - Type: String
  - Maximum Length: 80
 
- Other_Provider_Identifier_4
  - Other provider identifier
  - Type: String
  - Maximum Length: 20
  
- Other_Provider_Identifier_Type_Code_4
  - The name of the health plan that issued the Other Provider Identifier 
  - Type: String
  - Maximum Length: 2 
  - Reference: Health Care Providers Other Provider Identifier Issuer Type Codes
 
- Other_Provider_Identifier_State_Code_4
  - US State Code
  - Type: String
  - Maximum Length: 2
  
- Other_Provider_Identifier_Issuer_4
  - Provider Identifier
  - Type: String
  - Maximum Length: 80
 
- Other_Provider_Identifier_5
  - Other provider identifier
  - Type: String
  - Maximum Length: 20
  
- Other_Provider_Identifier_Type_Code_5
  - The name of the health plan that issued the Other Provider Identifier 
  - Type: String
  - Maximum Length: 2 
  - Reference: Health Care Providers Other Provider Identifier Issuer Type Codes
 
- Other_Provider_Identifier_State_Code_5
  - US State Code
  - Type: String
  - Maximum Length: 2
  
- Other_Provider_Identifier_Issuer_5
  - Provider Identifier
  - Type: String
  - Maximum Length: 80
 
- Other_Provider_Identifier_6
  - Other provider identifier
  - Type: String
  - Maximum Length: 20
  
- Other_Provider_Identifier_Type_Code_6
  - The name of the health plan that issued the Other Provider Identifier 
  - Type: String
  - Maximum Length: 2 
  - Reference: Health Care Providers Other Provider Identifier Issuer Type Codes
 
- Other_Provider_Identifier_State_Code_6
  - US State Code
  - Type: String
  - Maximum Length: 2
  
- Other_Provider_Identifier_Issuer_6
  - Provider Identifier
  - Type: String
  - Maximum Length: 80
 
- Other_Provider_Identifier_7
  - Other provider identifier
  - Type: String
  - Maximum Length: 20
  
- Other_Provider_Identifier_Type_Code_7
  - The name of the health plan that issued the Other Provider Identifier 
  - Type: String
  - Maximum Length: 2 
  - Reference: Health Care Providers Other Provider Identifier Issuer Type Codes
 
- Other_Provider_Identifier_State_Code_7
  - US State Code
  - Type: String
  - Maximum Length: 2
  
- Other_Provider_Identifier_Issuer_7
  - Provider Identifier
  - Type: String
  - Maximum Length: 80
  
- Other_Provider_Identifier_8
  - Other provider identifier
  - Type: String
  - Maximum Length: 20
  
- Other_Provider_Identifier_Type_Code_8
  - The name of the health plan that issued the Other Provider Identifier 
  - Type: String
  - Maximum Length: 2 
  - Reference: Health Care Providers Other Provider Identifier Issuer Type Codes
 
- Other_Provider_Identifier_State_Code_8
  - US State Code
  - Type: String
  - Maximum Length: 2
  
- Other_Provider_Identifier_Issuer_8
  - Provider Identifier
  - Type: String
  - Maximum Length: 80
 
- Other_Provider_Identifier_9
  - Other provider identifier
  - Type: String
  - Maximum Length: 20
  
- Other_Provider_Identifier_Type_Code_9
  - The name of the health plan that issued the Other Provider Identifier 
  - Type: String
  - Maximum Length: 2 
  - Reference: Health Care Providers Other Provider Identifier Issuer Type Codes
 
- Other_Provider_Identifier_State_Code_9
  - US State Code
  - Type: String
  - Maximum Length: 2
  
- Other_Provider_Identifier_Issuer_9
  - Provider Identifier
  - Type: String
  - Maximum Length: 80
 
- Other_Provider_Identifier_10
  - Other provider identifier
  - Type: String
  - Maximum Length: 20
  
- Other_Provider_Identifier_Type_Code_10
  - The name of the health plan that issued the Other Provider Identifier 
  - Type: String
  - Maximum Length: 2 
  - Reference: Health Care Providers Other Provider Identifier Issuer Type Codes
 
- Other_Provider_Identifier_State_Code_10
  - US State Code
  - Type: String
  - Maximum Length: 2
  
- Other_Provider_Identifier_Issuer_10
  - Provider Identifier
  - Type: String
  - Maximum Length: 80
 
- Other_Provider_Identifier_11
  - Other provider identifier
  - Type: String
  - Maximum Length: 20
  
- Other_Provider_Identifier_Type_Code_11
  - The name of the health plan that issued the Other Provider Identifier 
  - Type: String
  - Maximum Length: 2 
  - Reference: Health Care Providers Other Provider Identifier Issuer Type Codes
 
- Other_Provider_Identifier_State_Code_11
  - US State Code
  - Type: String
  - Maximum Length: 2
  
- Other_Provider_Identifier_Issuer_11
  - Provider Identifier
  - Type: String
  - Maximum Length: 80
 
- Other_Provider_Identifier_12
  - Other provider identifier
  - Type: String
  - Maximum Length: 20
  
- Other_Provider_Identifier_Type_Code_12
  - The name of the health plan that issued the Other Provider Identifier 
  - Type: String
  - Maximum Length: 2 
  - Reference: Health Care Providers Other Provider Identifier Issuer Type Codes
 
- Other_Provider_Identifier_State_Code_12
  - US State Code
  - Type: String
  - Maximum Length: 2
  
- Other_Provider_Identifier_Issuer_12
  - Provider Identifier
  - Type: String
  - Maximum Length: 80
 
- Other_Provider_Identifier_13
  - Other provider identifier
  - Type: String
  - Maximum Length: 20
  
- Other_Provider_Identifier_Type_Code_13
  - The name of the health plan that issued the Other Provider Identifier 
  - Type: String
  - Maximum Length: 2 
  - Reference: Health Care Providers Other Provider Identifier Issuer Type Codes
 
- Other_Provider_Identifier_State_Code_13
  - US State Code
  - Type: String
  - Maximum Length: 2
  
- Other_Provider_Identifier_Issuer_13
  - Provider Identifier
  - Type: String
  - Maximum Length: 80
 
- Other_Provider_Identifier_14
  - Other provider identifier
  - Type: String
  - Maximum Length: 20
  
- Other_Provider_Identifier_Type_Code_14
  - The name of the health plan that issued the Other Provider Identifier 
  - Type: String
  - Maximum Length: 2 
  - Reference: Health Care Providers Other Provider Identifier Issuer Type Codes
 
- Other_Provider_Identifier_State_Code_14
  - US State Code
  - Type: String
  - Maximum Length: 2
  
- Other_Provider_Identifier_Issuer_14
  - Provider Identifier
  - Type: String
  - Maximum Length: 80
 
- Other_Provider_Identifier_15
  - Other provider identifier
  - Type: String
  - Maximum Length: 20
  
- Other_Provider_Identifier_Type_Code_15
  - The name of the health plan that issued the Other Provider Identifier 
  - Type: String
  - Maximum Length: 2 
  - Reference: Health Care Providers Other Provider Identifier Issuer Type Codes
 
- Other_Provider_Identifier_State_Code_15
  - US State Code
  - Type: String
  - Maximum Length: 2
  
- Other_Provider_Identifier_Issuer_15
  - Provider Identifier
  - Type: String
  - Maximum Length: 80
 
- Other_Provider_Identifier_16
  - Other provider identifier
  - Type: String
  - Maximum Length: 20
  
- Other_Provider_Identifier_Type_Code_16
  - The name of the health plan that issued the Other Provider Identifier 
  - Type: String
  - Maximum Length: 2 
  - Reference: Health Care Providers Other Provider Identifier Issuer Type Codes
 
- Other_Provider_Identifier_State_Code_16
  - US State Code
  - Type: String
  - Maximum Length: 2
  
- Other_Provider_Identifier_Issuer_16
  - Provider Identifier
  - Type: String
  - Maximum Length: 80
 
- Other_Provider_Identifier_17
  - Other provider identifier
  - Type: String
  - Maximum Length: 20
  
- Other_Provider_Identifier_Type_Code_17
  - The name of the health plan that issued the Other Provider Identifier 
  - Type: String
  - Maximum Length: 2 
  - Reference: Health Care Providers Other Provider Identifier Issuer Type Codes
 
- Other_Provider_Identifier_State_Code_17
  - US State Code
  - Type: String
  - Maximum Length: 2
  
- Other_Provider_Identifier_Issuer_17
  - Provider Identifier
  - Type: String
  - Maximum Length: 80
 
- Other_Provider_Identifier_18
  - Other provider identifier
  - Type: String
  - Maximum Length: 20
  
- Other_Provider_Identifier_Type_Code_18
  - The name of the health plan that issued the Other Provider Identifier 
  - Type: String
  - Maximum Length: 2 
  - Reference: Health Care Providers Other Provider Identifier Issuer Type Codes
 
- Other_Provider_Identifier_State_Code_18
  - US State Code
  - Type: String
  - Maximum Length: 2
  
- Other_Provider_Identifier_Issuer_18
  - Provider Identifier
  - Type: String
  - Maximum Length: 80
 
- Other_Provider_Identifier_19
  - Other provider identifier
  - Type: String
  - Maximum Length: 20
  
- Other_Provider_Identifier_Type_Code_19
  - The name of the health plan that issued the Other Provider Identifier 
  - Type: String
  - Maximum Length: 2 
  - Reference: Health Care Providers Other Provider Identifier Issuer Type Codes
 
- Other_Provider_Identifier_State_Code_19
  - US State Code
  - Type: String
  - Maximum Length: 2
  
- Other_Provider_Identifier_Issuer_19
  - Provider Identifier
  - Type: String
  - Maximum Length: 80
 
- Other_Provider_Identifier_20
  - Other provider identifier
  - Type: String
  - Maximum Length: 20
  
- Other_Provider_Identifier_Type_Code_20
  - The name of the health plan that issued the Other Provider Identifier 
  - Type: String
  - Maximum Length: 2 
  - Reference: Health Care Providers Other Provider Identifier Issuer Type Codes
 
- Other_Provider_Identifier_State_Code_20
  - US State Code
  - Type: String
  - Maximum Length: 2
  
- Other_Provider_Identifier_Issuer_20
  - Provider Identifier
  - Type: String
  - Maximum Length: 80
 
- Other_Provider_Identifier_21
  - Other provider identifier
  - Type: String
  - Maximum Length: 20
  
- Other_Provider_Identifier_Type_Code_21
  - The name of the health plan that issued the Other Provider Identifier 
  - Type: String
  - Maximum Length: 2 
  - Reference: Health Care Providers Other Provider Identifier Issuer Type Codes
 
- Other_Provider_Identifier_State_Code_21
  - US State Code
  - Type: String
  - Maximum Length: 2
  
- Other_Provider_Identifier_Issuer_21
  - Provider Identifier
  - Type: String
  - Maximum Length: 80
 
- Other_Provider_Identifier_22
  - Other provider identifier
  - Type: String
  - Maximum Length: 20
  
- Other_Provider_Identifier_Type_Code_22
  - The name of the health plan that issued the Other Provider Identifier 
  - Type: String
  - Maximum Length: 2 
  - Reference: Health Care Providers Other Provider Identifier Issuer Type Codes
 
- Other_Provider_Identifier_State_Code_22
  - US State Code
  - Type: String
  - Maximum Length: 2
  
- Other_Provider_Identifier_Issuer_22
  - Provider Identifier
  - Type: String
  - Maximum Length: 80
 
- Other_Provider_Identifier_23
  - Other provider identifier
  - Type: String
  - Maximum Length: 20
  
- Other_Provider_Identifier_Type_Code_23
  - The name of the health plan that issued the Other Provider Identifier 
  - Type: String
  - Maximum Length: 2 
  - Reference: Health Care Providers Other Provider Identifier Issuer Type Codes
 
- Other_Provider_Identifier_State_Code_23
  - US State Code
  - Type: String
  - Maximum Length: 2
  
- Other_Provider_Identifier_Issuer_23
  - Provider Identifier
  - Type: String
  - Maximum Length: 80
 
- Other_Provider_Identifier_24
  - Other provider identifier
  - Type: String
  - Maximum Length: 20
  
- Other_Provider_Identifier_Type_Code_24
  - The name of the health plan that issued the Other Provider Identifier 
  - Type: String
  - Maximum Length: 2 
  - Reference: Health Care Providers Other Provider Identifier Issuer Type Codes
 
- Other_Provider_Identifier_State_Code_24
  - US State Code
  - Type: String
  - Maximum Length: 2
  
- Other_Provider_Identifier_Issuer_24
  - Provider Identifier
  - Type: String
  - Maximum Length: 80
 
- Other_Provider_Identifier_25
  - Other provider identifier
  - Type: String
  - Maximum Length: 20
  
- Other_Provider_Identifier_Type_Code_25
  - The name of the health plan that issued the Other Provider Identifier 
  - Type: String
  - Maximum Length: 2 
  - Reference: Health Care Providers Other Provider Identifier Issuer Type Codes
 
- Other_Provider_Identifier_State_Code_25
  - US State Code
  - Type: String
  - Maximum Length: 2
  
- Other_Provider_Identifier_Issuer_25
  - Provider Identifier
  - Type: String
  - Maximum Length: 80
 
- Other_Provider_Identifier_26
  - Other provider identifier
  - Type: String
  - Maximum Length: 20
  
- Other_Provider_Identifier_Type_Code_26
  - The name of the health plan that issued the Other Provider Identifier 
  - Type: String
  - Maximum Length: 2 
  - Reference: Health Care Providers Other Provider Identifier Issuer Type Codes
 
- Other_Provider_Identifier_State_Code_26
  - US State Code
  - Type: String
  - Maximum Length: 2
  
- Other_Provider_Identifier_Issuer_26
  - Provider Identifier
  - Type: String
  - Maximum Length: 80
 
- Other_Provider_Identifier_27
  - Other provider identifier
  - Type: String
  - Maximum Length: 20
  
- Other_Provider_Identifier_Type_Code_27
  - The name of the health plan that issued the Other Provider Identifier 
  - Type: String
  - Maximum Length: 2 
  - Reference: Health Care Providers Other Provider Identifier Issuer Type Codes
 
- Other_Provider_Identifier_State_Code_27
  - US State Code
  - Type: String
  - Maximum Length: 2
  
- Other_Provider_Identifier_Issuer_27
  - Provider Identifier
  - Type: String
  - Maximum Length: 80
  
- Other_Provider_Identifier_28
  - Other provider identifier
  - Type: String
  - Maximum Length: 20
  
- Other_Provider_Identifier_Type_Code_28
  - The name of the health plan that issued the Other Provider Identifier 
  - Type: String
  - Maximum Length: 2 
  - Reference: Health Care Providers Other Provider Identifier Issuer Type Codes
 
- Other_Provider_Identifier_State_Code_28
  - US State Code
  - Type: String
  - Maximum Length: 2
  
- Other_Provider_Identifier_Issuer_28
  - Provider Identifier
  - Type: String
  - Maximum Length: 80
 
- Other_Provider_Identifier_29
  - Other provider identifier
  - Type: String
  - Maximum Length: 20
  
- Other_Provider_Identifier_Type_Code_29
  - The name of the health plan that issued the Other Provider Identifier 
  - Type: String
  - Maximum Length: 2 
  - Reference: Health Care Providers Other Provider Identifier Issuer Type Codes
 
- Other_Provider_Identifier_State_Code_29
  - US State Code
  - Type: String
  - Maximum Length: 2
  
- Other_Provider_Identifier_Issuer_29
  - Provider Identifier
  - Type: String
  - Maximum Length: 80
 
- Other_Provider_Identifier_30
  - Other provider identifier
  - Type: String
  - Maximum Length: 20
  
- Other_Provider_Identifier_Type_Code_30
  - The name of the health plan that issued the Other Provider Identifier 
  - Type: String
  - Maximum Length: 2 
  - Reference: Health Care Providers Other Provider Identifier Issuer Type Codes
 
- Other_Provider_Identifier_State_Code_30
  - US State Code
  - Type: String
  - Maximum Length: 2
  
- Other_Provider_Identifier_Issuer_30
  - Provider Identifier
  - Type: String
  - Maximum Length: 80
 
- Other_Provider_Identifier_31
  - Other provider identifier
  - Type: String
  - Maximum Length: 20
  
- Other_Provider_Identifier_Type_Code_31
  - The name of the health plan that issued the Other Provider Identifier 
  - Type: String
  - Maximum Length: 2 
  - Reference: Health Care Providers Other Provider Identifier Issuer Type Codes
 
- Other_Provider_Identifier_State_Code_31
  - US State Code
  - Type: String
  - Maximum Length: 2
  
- Other_Provider_Identifier_Issuer_31
  - Provider Identifier
  - Type: String
  - Maximum Length: 80
 
- Other_Provider_Identifier_32
  - Other provider identifier
  - Type: String
  - Maximum Length: 20
  
- Other_Provider_Identifier_Type_Code_32
  - The name of the health plan that issued the Other Provider Identifier 
  - Type: String
  - Maximum Length: 2 
  - Reference: Health Care Providers Other Provider Identifier Issuer Type Codes
 
- Other_Provider_Identifier_State_Code_32
  - US State Code
  - Type: String
  - Maximum Length: 2
  
- Other_Provider_Identifier_Issuer_32
  - Provider Identifier
  - Type: String
  - Maximum Length: 80
 
- Other_Provider_Identifier_33
  - Other provider identifier
  - Type: String
  - Maximum Length: 20
  
- Other_Provider_Identifier_Type_Code_33
  - The name of the health plan that issued the Other Provider Identifier 
  - Type: String
  - Maximum Length: 2 
  - Reference: Health Care Providers Other Provider Identifier Issuer Type Codes
 
- Other_Provider_Identifier_State_Code_33
  - US State Code
  - Type: String
  - Maximum Length: 2
  
- Other_Provider_Identifier_Issuer_33
  - Provider Identifier
  - Type: String
  - Maximum Length: 80
 
- Other_Provider_Identifier_34
  - Other provider identifier
  - Type: String
  - Maximum Length: 20
  
- Other_Provider_Identifier_Type_Code_34
  - The name of the health plan that issued the Other Provider Identifier 
  - Type: String
  - Maximum Length: 2 
  - Reference: Health Care Providers Other Provider Identifier Issuer Type Codes
 
- Other_Provider_Identifier_State_Code_34
  - US State Code
  - Type: String
  - Maximum Length: 2
  
- Other_Provider_Identifier_Issuer_34
  - Provider Identifier
  - Type: String
  - Maximum Length: 80
 
- Other_Provider_Identifier_35
  - Other provider identifier
  - Type: String
  - Maximum Length: 20
  
- Other_Provider_Identifier_Type_Code_35
  - The name of the health plan that issued the Other Provider Identifier 
  - Type: String
  - Maximum Length: 2 
  - Reference: Health Care Providers Other Provider Identifier Issuer Type Codes
 
- Other_Provider_Identifier_State_Code_35
  - US State Code
  - Type: String
  - Maximum Length: 2
  
- Other_Provider_Identifier_Issuer_35
  - Provider Identifier
  - Type: String
  - Maximum Length: 80
 
- Other_Provider_Identifier_36
  - Other provider identifier
  - Type: String
  - Maximum Length: 20
  
- Other_Provider_Identifier_Type_Code_36
  - The name of the health plan that issued the Other Provider Identifier 
  - Type: String
  - Maximum Length: 2 
  - Reference: Health Care Providers Other Provider Identifier Issuer Type Codes
 
- Other_Provider_Identifier_State_Code_36
  - US State Code
  - Type: String
  - Maximum Length: 2
  
- Other_Provider_Identifier_Issuer_36
  - Provider Identifier
  - Type: String
  - Maximum Length: 80
 
- Other_Provider_Identifier_37
  - Other provider identifier
  - Type: String
  - Maximum Length: 20
  
- Other_Provider_Identifier_Type_Code_37
  - The name of the health plan that issued the Other Provider Identifier 
  - Type: String
  - Maximum Length: 2 
  - Reference: Health Care Providers Other Provider Identifier Issuer Type Codes
 
- Other_Provider_Identifier_State_Code_37
  - US State Code
  - Type: String
  - Maximum Length: 2
  
- Other_Provider_Identifier_Issuer_37
  - Provider Identifier
  - Type: String
  - Maximum Length: 80
 
- Other_Provider_Identifier_38
  - Other provider identifier
  - Type: String
  - Maximum Length: 20
  
- Other_Provider_Identifier_Type_Code_38
  - The name of the health plan that issued the Other Provider Identifier 
  - Type: String
  - Maximum Length: 2 
  - Reference: Health Care Providers Other Provider Identifier Issuer Type Codes
 
- Other_Provider_Identifier_State_Code_38
  - US State Code
  - Type: String
  - Maximum Length: 2
  
- Other_Provider_Identifier_Issuer_38
  - Provider Identifier
  - Type: String
  - Maximum Length: 80
 
- Other_Provider_Identifier_39
  - Other provider identifier
  - Type: String
  - Maximum Length: 20
  
- Other_Provider_Identifier_Type_Code_39
  - The name of the health plan that issued the Other Provider Identifier 
  - Type: String
  - Maximum Length: 2 
  - Reference: Health Care Providers Other Provider Identifier Issuer Type Codes
 
- Other_Provider_Identifier_State_Code_39
  - US State Code
  - Type: String
  - Maximum Length: 2
  
- Other_Provider_Identifier_Issuer_39
  - Provider Identifier
  - Type: String
  - Maximum Length: 80
 
- Other_Provider_Identifier_40
  - Other provider identifier
  - Type: String
  - Maximum Length: 20
  
- Other_Provider_Identifier_Type_Code_40
  - The name of the health plan that issued the Other Provider Identifier 
  - Type: String
  - Maximum Length: 2 
  - Reference: Health Care Providers Other Provider Identifier Issuer Type Codes
 
- Other_Provider_Identifier_State_Code_40
  - US State Code
  - Type: String
  - Maximum Length: 2
  
- Other_Provider_Identifier_Issuer_40
  - Provider Identifier
  - Type: String
  - Maximum Length: 80
 
- Other_Provider_Identifier_41
  - Other provider identifier
  - Type: String
  - Maximum Length: 20
  
- Other_Provider_Identifier_Type_Code_41
  - The name of the health plan that issued the Other Provider Identifier 
  - Type: String
  - Maximum Length: 2 
  - Reference: Health Care Providers Other Provider Identifier Issuer Type Codes
 
- Other_Provider_Identifier_State_Code_41
  - US State Code
  - Type: String
  - Maximum Length: 2
  
- Other_Provider_Identifier_Issuer_41
  - Provider Identifier
  - Type: String
  - Maximum Length: 80
 
- Other_Provider_Identifier_42
  - Other provider identifier
  - Type: String
  - Maximum Length: 20
  
- Other_Provider_Identifier_Type_Code_42
  - The name of the health plan that issued the Other Provider Identifier 
  - Type: String
  - Maximum Length: 2 
  - Reference: Health Care Providers Other Provider Identifier Issuer Type Codes
 
- Other_Provider_Identifier_State_Code_42
  - US State Code
  - Type: String
  - Maximum Length: 2
  
- Other_Provider_Identifier_Issuer_42
  - Provider Identifier
  - Type: String
  - Maximum Length: 80
 
- Other_Provider_Identifier_43
  - Other provider identifier
  - Type: String
  - Maximum Length: 20
  
- Other_Provider_Identifier_Type_Code_43
  - The name of the health plan that issued the Other Provider Identifier 
  - Type: String
  - Maximum Length: 2 
  - Reference: Health Care Providers Other Provider Identifier Issuer Type Codes
 
- Other_Provider_Identifier_State_Code_43
  - US State Code
  - Type: String
  - Maximum Length: 2
  
- Other_Provider_Identifier_Issuer_43
  - Provider Identifier
  - Type: String
  - Maximum Length: 80
 
- Other_Provider_Identifier_44
  - Other provider identifier
  - Type: String
  - Maximum Length: 20
  
- Other_Provider_Identifier_Type_Code_44
  - The name of the health plan that issued the Other Provider Identifier 
  - Type: String
  - Maximum Length: 2 
  - Reference: Health Care Providers Other Provider Identifier Issuer Type Codes
 
- Other_Provider_Identifier_State_Code_44
  - US State Code
  - Type: String
  - Maximum Length: 2
  
- Other_Provider_Identifier_Issuer_44
  - Provider Identifier
  - Type: String
  - Maximum Length: 80
 
- Other_Provider_Identifier_45
  - Other provider identifier
  - Type: String
  - Maximum Length: 20
  
- Other_Provider_Identifier_Type_Code_45
  - The name of the health plan that issued the Other Provider Identifier 
  - Type: String
  - Maximum Length: 2 
  - Reference: Health Care Providers Other Provider Identifier Issuer Type Codes
 
- Other_Provider_Identifier_State_Code_45
  - US State Code
  - Type: String
  - Maximum Length: 2
  
- Other_Provider_Identifier_Issuer_45
  - Provider Identifier
  - Type: String
  - Maximum Length: 80
 
- Other_Provider_Identifier_46
  - Other provider identifier
  - Type: String
  - Maximum Length: 20
  
- Other_Provider_Identifier_Type_Code_46
  - The name of the health plan that issued the Other Provider Identifier 
  - Type: String
  - Maximum Length: 2 
  - Reference: Health Care Providers Other Provider Identifier Issuer Type Codes
 
- Other_Provider_Identifier_State_Code_46
  - US State Code
  - Type: String
  - Maximum Length: 2
  
- Other_Provider_Identifier_Issuer_46
  - Provider Identifier
  - Type: String
  - Maximum Length: 80
 
- Other_Provider_Identifier_47
  - Other provider identifier
  - Type: String
  - Maximum Length: 20
  
- Other_Provider_Identifier_Type_Code_47
  - The name of the health plan that issued the Other Provider Identifier 
  - Type: String
  - Maximum Length: 2 
  - Reference: Health Care Providers Other Provider Identifier Issuer Type Codes
 
- Other_Provider_Identifier_State_Code_47
  - US State Code
  - Type: String
  - Maximum Length: 2
  
- Other_Provider_Identifier_Issuer_47
  - Provider Identifier
  - Type: String
  - Maximum Length: 80
 
- Other_Provider_Identifier_48
  - Other provider identifier
  - Type: String
  - Maximum Length: 20
  
- Other_Provider_Identifier_Type_Code_48
  - The name of the health plan that issued the Other Provider Identifier 
  - Type: String
  - Maximum Length: 2 
  - Reference: Health Care Providers Other Provider Identifier Issuer Type Codes
 
- Other_Provider_Identifier_State_Code_48
  - US State Code
  - Type: String
  - Maximum Length: 2
  
- Other_Provider_Identifier_Issuer_48
  - Provider Identifier
  - Type: String
  - Maximum Length: 80
 
- Other_Provider_Identifier_49
  - Other provider identifier
  - Type: String
  - Maximum Length: 20
  
- Other_Provider_Identifier_Type_Code_49
  - The name of the health plan that issued the Other Provider Identifier 
  - Type: String
  - Maximum Length: 2 
  - Reference: Health Care Providers Other Provider Identifier Issuer Type Codes
 
- Other_Provider_Identifier_State_Code_49
  - US State Code
  - Type: String
  - Maximum Length: 2
  
- Other_Provider_Identifier_Issuer_49
  - Provider Identifier
  - Type: String
  - Maximum Length: 80
 
- Other_Provider_Identifier_50
  - Other provider identifier
  - Type: String
  - Maximum Length: 20
  
- Other_Provider_Identifier_Type_Code_50
  - The name of the health plan that issued the Other Provider Identifier 
  - Type: String
  - Maximum Length: 2 
  - Reference: Health Care Providers Other Provider Identifier Issuer Type Codes
 
- Other_Provider_Identifier_State_Code_50
  - US State Code
  - Type: String
  - Maximum Length: 2
  
- Other_Provider_Identifier_Issuer_50
  - Provider Identifier
  - Type: String
  - Maximum Length: 80

- Is_Sole_Proprietor
  - true- Entity Type 1 Provider (Individual) is a Sole Proprietor, false- Entity Type 1 Provider (Individual) is NOT a Sole Proprietor, null – Not answered
  - Type: Boolean
 
- Is_Organization_Subpart
  - true- Entity Type 1 Provider (Organization) is a Subpart, false- Entity Type 1 Provider (Organization) is NOT a Subpart,null – Not answered
  - Type: Boolean
 
- Parent_Organization_LBN
  - Provider Organization Subpart Legal Business Name 
  - Type: String
  - Maximum Length: 70
 
- Parent_Organization_TIN
  - Provider Organization Subpart TIN
  - Type: String
  - Maximum Length: 9
 
- Authorized_Official_Name_Prefix_Code
  - Name Prefix codes  
  - Type: String
  - Maximum Length: 5
  - Reference: People/Names/Name Prefixes
  
- Authorized_Official_Name_Suffix_Code 
  - Name Suffix codes  
  - Type: String
  - Maximum Length: 5
  - Reference: People/Names/Name Suffixes
  
- Authorized_Official_Credential_Text
  - Provider Credential Text
  - Type: String
  - Maximum Length: 20
 
- Healthcare_Provider_Taxonomy_Group_Code_1
  - Group Taxonomy Codes:Multi-Speciality Group,Single Speciality Group
  - Type: String
  - Maximum Length: 70
 
- Healthcare_Provider_Taxonomy_Group_Code_2
  - Group Taxonomy Codes:Multi-Speciality Group,Single Speciality Group
  - Type: String
  - Maximum Length: 70 
 
- Healthcare_Provider_Taxonomy_Group_Code_3
  - Group Taxonomy Codes:Multi-Speciality Group,Single Speciality Group
  - Type: String
  - Maximum Length: 70
 
- Healthcare_Provider_Taxonomy_Group_Code_4
  - Group Taxonomy Codes:Multi-Speciality Group,Single Speciality Group
  - Type: String
  - Maximum Length: 70
 
- Healthcare_Provider_Taxonomy_Group_Code_5
  - Group Taxonomy Codes:Multi-Speciality Group,Single Speciality Group
  - Type: String
  - Maximum Length: 70
 
- Healthcare_Provider_Taxonomy_Group_Code_6
  - Group Taxonomy Codes:Multi-Speciality Group,Single Speciality Group
  - Type: String
  - Maximum Length: 70
 
- Healthcare_Provider_Taxonomy_Group_Code_7
  - Group Taxonomy Codes:Multi-Speciality Group,Single Speciality Group
  - Type: String
  - Maximum Length: 70
 
- Healthcare_Provider_Taxonomy_Group_Code_8
  - Group Taxonomy Codes:Multi-Speciality Group,Single Speciality Group
  - Type: String
  - Maximum Length: 70
 
- Healthcare_Provider_Taxonomy_Group_Code_9
  - Group Taxonomy Codes:Multi-Speciality Group,Single Speciality Group
  - Type: String
  - Maximum Length: 70
 
- Healthcare_Provider_Taxonomy_Group_Code_10
  - Group Taxonomy Codes:Multi-Speciality Group,Single Speciality Group
  - Type: String
  - Maximum Length: 70
 
- Healthcare_Provider_Taxonomy_Group_Code_11
  - Group Taxonomy Codes:Multi-Speciality Group,Single Speciality Group
  - Type: String
  - Maximum Length: 70
 
- Healthcare_Provider_Taxonomy_Group_Code_12
  - Group Taxonomy Codes:Multi-Speciality Group,Single Speciality Group
  - Type: String
  - Maximum Length: 70
 
- Healthcare_Provider_Taxonomy_Group_Code_13
  - Group Taxonomy Codes:Multi-Speciality Group,Single Speciality Group
  - Type: String
  - Maximum Length: 70
 
- Healthcare_Provider_Taxonomy_Group_Code_14
  - Group Taxonomy Codes:Multi-Speciality Group,Single Speciality Group
  - Type: String
  - Maximum Length: 70
 
- Healthcare_Provider_Taxonomy_Group_Code_15
  - Group Taxonomy Codes:Multi-Speciality Group,Single Speciality Group
  - Type: String
  - Maximum Length: 70
