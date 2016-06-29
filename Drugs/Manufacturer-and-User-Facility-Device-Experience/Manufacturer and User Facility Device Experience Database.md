# Manufacturer and User Facility Device Experience Database

## Summary
MAUDE data represents Reports of adverse Events involving medical Devices the datasets consist of voluntary Reports since June 1993, User facility Reports since 1991, Distributor Reports since 1993, and Manufacturer Reports since August 1996.

## Description
Manufacturer and User Facility Device Experience Database represents Reports of adverse Events involving medical Devices.  
The dataset contains 75 fields including a MDR Report key,the Report Number and and the Date of the Event.

## Facts
- Date Created: 2010
- Date Modified: 2016-06-01
- Version: 2016.06.28
- UpDate Frequency: Weekly
- Temporal Coverage: 1991 to 2016-06-01
- Spatial Coverage: USA
- Source: U.S. Food and Drug Administration (FDA)
- Source License URL: N/A
- Source License Requirements: Open for commercial Use
- Source Citation: N/A 
- Keywords: 
 - Maude
 - Device Experience 
- Other Titles
 - Medical Devices adverse Events
 - FDA MAUDE Dataset

## Schema
- MDR_Report_Key
  - MDR Report Key
  - Type: String
  - Required

- Event_Key
  - Event Key
  - Type: String

- Report_Number
  - Report Number
  - Type: String
  - Required

- Report_Source_Code
  - Report Source Code
  - Type: String
  - Values: D, M, P, U
  - Required

- Is_Manufacturer_Link_Flag_
  - Manufacturer Link Flag (internal information Flag)
  - Type: Boolean
  - Required

- Number_Devices_In_Event
  - Number Devices in Event
  - Type: String

- Number_Patients_In_Event
  - Number Patient in Event
  - Type: String

- Received_Date
  - Received Date
  - Type: Date
  - Required

- Is_Adverse_Event_Flag
  - Adverse Event Flag
  - Type: Boolean

- Is_Product_Problem_Flag
  - Product Problem Flag
  - Type: Boolean

- Date_Report
  - Report Date
  - Type: Date

- Event_Date
  - Date of Event
  - Type: Date 

- Reprocessed_And_Reused_Flag
  - Single Use Flag (Reprocessor Flag)
  - Type: String
  - Values: Y, N, I, *

- Reporter_Occupation_Code
  - Reporter Occupation Code
  - Type: String

- Health_Professional
  - Health Professional
  - Type: String
  - Values: Y, N, I, *

- Initial_Report_To_FDA
  - Initial Report to FDA
  - Type: String
  - Values: Y, N, I, *, U

- Date_Facility_Aware
  - Date Facility Aware 
  - Type: String

- Report_Date
  - Report Date
  - Type: Date

- Report_To_FDA
  - Report to FDA
  - Type: String
  - Values: Y, N, I, *
  - Required

- Date_Report_To_FDA
  - Date Report to FDA
  - Type: Date

- Event_Location
  - Event Location Code Key
  - Type: String
  - Required

- Date_Report_To_Manufacturer
  - Date Report to Manufacturer
  - Type: Date

- Manufacturer_Contact_T_Name
  - Manufacturer Contact Title Name
  - Type: String

- Manufacturer_Contact_F_Name
  - Manufacturer Contact Title First Name
  - Type: String

- Manufacturer_Contact_L_Name
  - Manufacturer Contact Title Last Name
  - Type: String

- Manufacturer_Contact_Street_1
  - Manufacturer Contact Street 1
  - Type: String

- Manufacturer_Contact_Street_2
  - Manufacturer Contact Street 2
  - Type: String

- Manufacturer_Contact_City
  - Manufacturer Contact City
  - Type: String

- Manufacturer_Contact_State
  - Manufacturer Contact State Code
  - Type: String

- Manufacturer_Contact_Zip_Code
  - Manufacturer Contact Zip Code
  - Type: String

- Manufacturer_Contact_Zip_Ext
  - Manufacturer Contact Zip Code Ext
  - Type: String

- Manufacturer_Contact_Country
  - Manufacturer Contact Country Code
  - Type: String

- Manufacturer_Contact_Postal
  - Manufacturer Contact Postal Code
  - Type: String

- Manufacturer_Contact_Area_Code
  - Manufacturer Contact Phone No Area Code
  - Type: String

- Manufacturer_Contact_Exchange
  - Manufacturer Contact Phone No Exchange
  - Type: String

- Manufacturer_Contact_Phone_No
  - Manufacturer Contact Phone No
  - Type: String

- Manufacturer_Contact_Extension
  - Manufacturer Contact Phone No Ext
  - Type: Integer
  - Level: Nominal

- Manufacturer_Contact_PCountry
  - Manufacturer Contact Phone No Country Code
  - Type: String

- Manufacturer_Contact_PCity
  - Manufacturer Contact Phone No City Code
  - Type: String

- Manufacturer_Contact_PLocal
  - Manufacturer Contact Phone No Local
  - Type: String

- Manufacturer_G1_Name
  - Manufacturer G1 Name
  - Type: String

- Manufacturer_G1_Street_1
  - Manufacturer G1 Street 1
  - Type: String

- Manufacturer_G1_Street_2
  - Manufacturer G1 Street 2
  - Type: String

- Manufacturer_G1_City
  - Manufacturer G1 City
  - Type: String

- Manufacturer_G1_State_Code
  - Manufacturer G1 State Code
  - Type: String

- Manufacturer_G1_Zip_Code
  - Manufacturer G1 Zip Code
  - Type: String

- Manufacturer_G1_Zip_Code_Ext
  - Manufacturer G1 Zip Code Ext
  - Type: String

- Manufacturer_G1_Country_Code
  - Manufacturer G1 Country Code
  - Type: String

- Manufacturer_G1_Postal_Code
  - Manufacturer G1 Postal Code
  - Type: String

- Date_Manufacturer_Received
  - Date Manufacturer Received
  - Type: Date

- Device_Date_Of_Manufacture
  - Device_Date Of Manufacture
  - Type: Date

- Single_Use_Flag
  - Single Use Flag
  - Type: String
  - Values: Y, N, I, *
  - Required

- Remedial_Action
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

- Previous_Use_Code
  - Previous Use Code
  - Type: String
  - Values: I, N, R, U
  - Required

- Removal_Correction_Number
  - Removal/Correction Number
  - Type: String

- Event_Type
  - Event Type:  
    D = Death  
    IN = Injury  
    IL = Injury  
    IJ = Injury  
    M = Malfunction  
    O = Other  
    * = No answer provided  
  - Type: String
  - Required

- Distributor_Name
  - Distributor Name
  - Type: String

- Distributor_Address_1
  - Distributor Address line 1
  - Type: String

- Distributor_Address_2
  - Distributor Address line 2
  - Type: String

- Distributor_City
  - Distributor City
  - Type: String

- Distributor_State_Code
  - Distributor State Code
  - Type: String

- Distributor_Zip_Code
  - Distributor Zip Code
  - Type: String

- Distributor_Zip_Code_Ext
  - Distributor Zip Code Ext
  - Type: String

- Report_To_Manufacturer
  - Report to Manufacturer
  - Type: String

- Manufacturer_Name
  - Manufacturer Name
  - Type: String

- Manufacturer_Address_1
  - Manufacturer Address line 1
  - Type: String

- Manufacturer_Address_2
  - Manufacturer Address line 2
  - Type: String

- Manufacturer_City
  - Manufacturer City
  - Type: String

- Manufacturer_State_Code
  - Manufacturer State Code
  - Type: String

- Manufacturer_Zip_Code
  - Manufacturer Zip Code
  - Type: String

- Manufacturer_Zip_Code_Ext
  - Manufacturer Zip Code Ext
  - Type: String

- Manufacturer_COUNTRY_Code
  - Manufacturer Country Code
  - Type: String

- Manufacturer_Postal_Code
  - Manufacturer Postal Code
  - Type: String

- Type_Of_Report
  - Type of Report
  - Type: String

- Source_Type
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

- Added_Date
  - Date Added
  - Type: Date
  - Required

- Changed_Date
  - Date Changed
  - Type: Date
  - Required
