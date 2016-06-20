# Manufacturer and User Facility Device Experience Database

## Summary
MAUDE data represents reports of adverse events involving medical devices the datasets consist of voluntary reports since June 1993, user facility reports since 1991, distributor reports since 1993, and manufacturer reports since August 1996.

## Description
Manufacturer and User Facility Device Experience Database represents reports of adverse events involving medical devices.  
The dataset contains 75 fields including a MDR Report key,the Report Number and and the date of the event.

## Facts
- Date Created: 2010
- Date Modified: 2016-04-20
- Version: 2016.04.01
- Update Frequency: Weekly
- Temporal Coverage: 1991 To 2016-04-01
- Spatial Coverage: USA
- Source: U.S. Food and Drug Administration (FDA)
- Source License URL: N/A
- Source License Requirements: Open for commercial use
- Source Citation: N/A 
- Keywords: 
 - Maude
 - Device Experience 
- Other Titles
 - Medical devices adverse events
 - FDA MAUDE Dataset

## Schema
- MDR_REPORT_KEY
  - MDR Report Key
  - Type: String
  - Required

- EVENT_KEY
  - Event Key
  - Type: String

- REPORT_NUMBER
  - Report Number
  - Type: String
  - Required

- REPORT_SOURCE_CODE
  - Report Source Code
  - Type: String
  - Values: D, M, P, U
  - Required

- Is_MANUFACTURER_LINK_FLAG_
  - Manufacturer Link Flag (internal information flag)
  - Type: Boolean
  - Required

- NUMBER_DEVICES_IN_EVENT
  - Number Devices in Event
  - Type: String

- NUMBER_PATIENTS_IN_EVENT
  - Number Patient in Event
  - Type: String

- DATE_RECEIVED
  - Date Received
  - Type: Date
  - Required

- Is_ADVERSE_EVENT_FLAG
  - Adverse Event Flag
  - Type: Boolean

- Is_PRODUCT_PROBLEM_FLAG
  - Product Problem Flag
  - Type: Boolean

- DATE_REPORT
  - Date Report
  - Type: Date

- DATE_OF_EVENT
  - Date of Event
  - Type: Date 

- REPROCESSED_AND_REUSED_FLAG
  - Single Use Flag (Reprocessor Flag)
  - Type: String
  - Values: Y, N, I, *

- REPORTER_OCCUPATION_CODE
  - Reporter Occupation Code
  - Type: String

- HEALTH_PROFESSIONAL
  - Health Professional
  - Type: String
  - Values: Y, N, I, *

- INITIAL_REPORT_TO_FDA
  - Initial Report to FDA
  - Type: String
  - Values: Y, N, I, *, U

- DATE_FACILITY_AWARE
  - Date Facility Aware 
  - Type: String

- REPORT_DATE
  - Report Date
  - Type: Date

- REPORT_TO_FDA
  - Report to FDA
  - Type: String
  - Values: Y, N, I, *
  - Required

- DATE_REPORT_TO_FDA
  - Date Report to FDA
  - Type: Date

- EVENT_LOCATION
  - Event Location Code Key
  - Type: String
  - Required

- DATE_REPORT_TO_MANUFACTURER
  - Date Report to Manufacturer
  - Type: Date

- MANUFACTURER_CONTACT_T_NAME
  - Manufacturer Contact Title Name
  - Type: String

- MANUFACTURER_CONTACT_F_NAME
  - Manufacturer Contact Title First Name
  - Type: String

- MANUFACTURER_CONTACT_L_NAME
  - Manufacturer Contact Title Last Name
  - Type: String

- MANUFACTURER_CONTACT_STREET_1
  - Manufacturer Contact Street 1
  - Type: String

- MANUFACTURER_CONTACT_STREET_2
  - Manufacturer Contact Street 2
  - Type: String

- MANUFACTURER_CONTACT_CITY
  - Manufacturer Contact City
  - Type: String

- MANUFACTURER_CONTACT_STATE
  - Manufacturer Contact State Code
  - Type: String

- MANUFACTURER_CONTACT_ZIP_CODE
  - Manufacturer Contact Zip Code
  - Type: String

- MANUFACTURER_CONTACT_ZIP_EXT
  - Manufacturer Contact Zip Code Ext
  - Type: String

- MANUFACTURER_CONTACT_COUNTRY
  - Manufacturer Contact Country Code
  - Type: String

- MANUFACTURER_CONTACT_POSTAL
  - Manufacturer Contact Postal Code
  - Type: String

- MANUFACTURER_CONTACT_AREA_CODE
  - Manufacturer Contact Phone No Area Code
  - Type: String

- MANUFACTURER_CONTACT_EXCHANGE
  - Manufacturer Contact Phone No Exchange
  - Type: String

- MANUFACTURER_CONTACT_PHONE_NO
  - Manufacturer Contact Phone No
  - Type: String

- MANUFACTURER_CONTACT_EXTENSION
  - Manufacturer Contact Phone No Ext
  - Type: Integer
  - Level: Nominal

- MANUFACTURER_CONTACT_PCOUNTRY
  - Manufacturer Contact Phone No Country Code
  - Type: String

- MANUFACTURER_CONTACT_PCITY
  - Manufacturer Contact Phone No City Code
  - Type: String

- MANUFACTURER_CONTACT_PLOCAL
  - Manufacturer Contact Phone No Local
  - Type: String

- MANUFACTURER_G1_NAME
  - Manufacturer G1 Name
  - Type: String

- MANUFACTURER_G1_STREET_1
  - Manufacturer G1 Street 1
  - Type: String

- MANUFACTURER_G1_STREET_2
  - Manufacturer G1 Street 2
  - Type: String

- MANUFACTURER_G1_CITY
  - Manufacturer G1 City
  - Type: String

- MANUFACTURER_G1_STATE_CODE
  - Manufacturer G1 State Code
  - Type: String

- MANUFACTURER_G1_ZIP_CODE
  - Manufacturer G1 Zip Code
  - Type: String

- MANUFACTURER_G1_ZIP_CODE_EXT
  - Manufacturer G1 Zip Code Ext
  - Type: String

- MANUFACTURER_G1_COUNTRY_CODE
  - Manufacturer G1 Country Code
  - Type: String

- MANUFACTURER_G1_POSTAL_CODE
  - Manufacturer G1 Postal Code
  - Type: String

- DATE_MANUFACTURER_RECEIVED
  - Date Manufacturer Received
  - Type: Date

- DEVICE_DATE_OF_MANUFACTURE
  - DEVICE_DATE_OF_MANUFACTURE
  - Type: Date

- SINGLE_USE_FLAG
  - Single Use Flag
  - Type: String
  - Values: Y, N, I, *
  - Required

- REMEDIAL_ACTION
  - Remedial Action:  
    RC = Recall  
    RP = Repair  
    RL = Replace  
    RB = Relabeling  
    OT = Other  
    NO = Notification  
    IN = Inspection  
    PM = Patient Monitoring  
    MA = Modification/Adjustment
  - Type: String

- PREVIOUS_USE_CODE
  - Previous Use Code
  - Type: String
  - Values: I, N, R, U
  - Required

- REMOVAL_CORRECTION_NUMBER
  - Removal/Correction Number
  - Type: String

- EVENT_TYPE
  - Event type:  
    D = Death  
    IN = Injury  
    IL = Injury  
    IJ = Injury  
    M = Malfunction  
    O = Other  
    * = No answer provided  
  - Type: String
  - Required

- DISTRIBUTOR_NAME
  - Distributor Name
  - Type: String

- DISTRIBUTOR_ADDRESS_1
  - Distributor Address line 1
  - Type: String

- DISTRIBUTOR_ADDRESS_2
  - Distributor Address line 2
  - Type: String

- DISTRIBUTOR_CITY
  - Distributor City
  - Type: String

- DISTRIBUTOR_STATE_CODE
  - Distributor State Code
  - Type: String

- DISTRIBUTOR_ZIP_CODE
  - Distributor Zip Code
  - Type: String

- DISTRIBUTOR_ZIP_CODE_EXT
  - Distributor Zip Code Ext
  - Type: String

- REPORT_TO_MANUFACTURER
  - Report to Manufacturer
  - Type: String

- MANUFACTURER_NAME
  - Manufacturer Name
  - Type: String

- MANUFACTURER_ADDRESS_1
  - Manufacturer Address line 1
  - Type: String

- MANUFACTURER_ADDRESS_2
  - Manufacturer Address line 2
  - Type: String

- MANUFACTURER_CITY
  - Manufacturer City
  - Type: String

- MANUFACTURER_STATE_CODE
  - Manufacturer State Code
  - Type: String

- MANUFACTURER_ZIP_CODE
  - Manufacturer Zip Code
  - Type: String

- MANUFACTURER_ZIP_CODE_EXT
  - Manufacturer Zip Code Ext
  - Type: String

- MANUFACTURER_COUNTRY_CODE
  - Manufacturer Country Code
  - Type: String

- MANUFACTURER_POSTAL_CODE
  - Manufacturer Postal Code
  - Type: String

- TYPE_OF_REPORT
  - Type of Report
  - Type: String

- SOURCE_TYPE
  - Source Type:  
    00 Other  
    01 Foreign  
    02 Study  
    03 Literature  
    04 Consumer  
    05 Health Professional  
    06 User facility  
    07 Company representation  
    08 Distributor  
    99 Unknown  
    * Invalid data  
  - Type: String

- DATE_ADDED
  - Date Added
  - Type: Date
  - Required

- DATE_CHANGED
  - Date Changed
  - Type: Date
  - Required
