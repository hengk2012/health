# RxNorm Data Elements and Attributes Names

## Summary
This dataset provides a brief explanation of the names and values for the data elements and attributes in RxNorm and the UMLS.

## Description
RxNorm provides normalized names for clinical drugs and links its names to many of the drug vocabularies commonly used in pharmacy management and drug interaction software, including those of First Databank, Micromedex, MediSpan, Gold Standard Drug Database, and Multum. By providing links between these vocabularies, RxNorm can mediate messages between systems not using the same software and vocabulary.

There is exactly one row in this table for each allowed value of selected data elements or attributes that have a finite number of abbreviations as allowed values. Examples of such data elements include TTY, ATN, TS, STT, REL, RELA.

## Facts
- Date Created: 2004-11
- Date Modified: 2016-06-06
- Version: 2016.06
- Update Frequency: Monthly
- Temporal Coverage: N/A
- Spatial Coverage: United States
- Source: National Library of Medicine (NLM)
- Source License URL: https://uts.nlm.nih.gov/license.html
- Source License Requirements: Reporting Requirements
- Source Citation: N/A
- Keywords: 
 - Abbreviated Values
 - Data elements
 - Attributes
- Other Titles
 - RXNDOC
 - Metathesaurus MRDOC 
 - UMLS MRDOC 
 - Values associated with a specific Data element/attribute

## Schema
- Data_Name
  - Data element or attribute
  - Type: String
  - Required
  - Maximum Length : 50
  
- Data_Value
  - Abbreviation that is one of its values
  - Type: String
  - Maximum Length : 1000

- Data_Type_Explanation
  - Type of information in Explanation column
  - Type: String
  - Required
  - Maximum Length : 50

- Data_Value_Explanation
  - Explanation of Data_Value
  - Type: String
  - Maximum Length : 1000
