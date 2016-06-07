# RxNorm Retired Concept CUIs

## Summary
It contains information on retired concepts. A concept is retired when it:
- Merges into another concept
- Has been renamed as a result of an error
- No longer appears in source vocabulary

## Description
RxNorm provides normalized names for clinical drugs and links its names to many of the drug vocabularies commonly used in pharmacy management and drug interaction software, including those of First Databank, Micromedex, MediSpan, Gold Standard Drug Database, and Multum. By providing links between these vocabularies, RxNorm can mediate messages between systems not using the same software and vocabulary.

When a concept is retired because it was created as the result of an acknowledged error in a source vocabulary, the RX_Concept1_CUI will be shown as synonymous to itself. In other words, the RX_Concept1_CUI was errant and there is no active RX_Concept_CUI that now represents this error

## Facts
- Date Created: 2004-11
- Date Modified: 2016-06-06
- Version: 2016.06.06
- Update Frequency: Monthly
- Temporal Coverage: N/A
- Spatial Coverage: United States
- Source: National Library of Medicine (NLM)
- Source License URL: https://uts.nlm.nih.gov/license.html
- Source License Requirements: Reporting Requirements
- Source Citation: This release of RxNorm is consistent with the 2015AB UMLS Metathesaurus release.
- Keywords: 
 - History information about RxNorm concepts
 - Data history
- Other Titles
 - RXNCUI
 - Retired RXCUI Data
 - Retired RX_Concept_CUI analytics

## Schema
- RXConcept1_CUI
  - Unique identifier of retired concept
  - Type: String
  - Maximum Length : 8
  
- Version_Source_Abbreviation_Start
  - Version Source Abbreviation of the first RxNorm release RXConcept1_CUI appeared in
  - Type: String
  - Maximum Length : 40

- Version_Source_Abbreviation_End
  - Version Source Abbreviation of the last RxNorm release RXConcept1_CUI appeared in
  - Type: String
  - Maximum Length : 40
  
- Number_Of_RXConcept_CUI_Changed
  - The number of RXConcept_CUI that RXConcept1_CUI was moved or split to.
  - Type: Integer
  - Level: Ratio
  - Format : Long
  
- RXConcept2_CUI
  - Unique identifier of synonymous concept for RXConcept1_CUI
  - Type: String
  - Maximum Length : 8
