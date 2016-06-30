# Health Care Providers Deactivated NPI

## Summary
This data set contains the NPI and deactivation date for the deactivated health care providers.   
The NPI is a unique identification number for covered health care providers.  This data set will assist users who are only interested in the deactivation information.

## Description
In September 2007, CMS began disclosing National Plan and Provider Enumeration System (NPPES) health care provider data that are disclosable under the Freedom of Information Act (FOIA) to the public. The NPI is a 10-position, intelligence-free numeric identifier (10-digit number). The NPI must be used in lieu of legacy provider identifiers in the HIPAA standards transactions.  

The FOIA-disclosable data for a health care provider (individual or organization) who deactivated an NPI will be disclosed in this data set.   

## Facts
- Date Created: 2007-09
- Date Modified: 2016-06-14
- Version: 2016.06
- Update Frequency: Monthly
- Temporal Coverage: 2005-05 to 2016-06
- Spatial Coverage: United States
- Source: Centers of Medicare and Medicaid Services (CMS)
- Source License URL: N/A
- Source License Requirements: N/A
- Source Citation: N/A
- Keywords:
 - National Provider Identifier Standard (NPI)
 - NPPES
 - Deactivated NPI
 - Regulation & Guidance
 - Data Dissemination
- Other Titles
 - Full Replacement NPI Deactivation File
 - NPPES Deactivated NPI Report
 - Deactivated NPI’s, not to be used in standard transactions by covered recipients and Health care providers

## Schema
- NPI
  - The NPI is a 10-digit unique identification number for covered health care providers. 
  - Type: Integer
  - Level: Nominal
  - Required
  - Unique
  - Format : long
  - Pattern: \d{10}

- NPPES_Deactivation_Date
  - NPI Deactivation Date 
  - Type: Date
  - Required
  - Format : Date
