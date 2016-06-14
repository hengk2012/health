# RxNorm Semantic Types for Concepts

## Summary
It contains the semantic types, or broad subject categories, assigned to each concept. Every concept receives at least one semantic type.

## Description
RxNorm provides normalized names for clinical drugs and links its names to many of the drug vocabularies commonly used in pharmacy management and drug interaction software, including those of First Databank, Micromedex, MediSpan, Gold Standard Drug Database, and Multum. By providing links between these vocabularies, RxNorm can mediate messages between systems not using the same software and vocabulary.

All RxNorm concepts have at least one entry in this file. Many have more than one entry. Eighty percent of RxNorm drug concepts have the semantic type 'Clinical Drug'. This dataset associates semantic type data with RXConcept_CUI_IDs. The corresponding drug names for these RXConcept_CUI_IDs are found in “RxNorm Drugs Names and Identifiers” dataset.

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
- Source Citation: N/A
- Keywords: 
 - Semantic type
 - Concept
 - Subject categories
 - Semantic network
- Other Titles
 - RXNSTY
 - Semantic Types
 - MRSTY
 - Categories name assigned to each concept
 - Current Prescribable Content subset (all rows with value '4096')

## Schema
- RXConcept_CUI
  - RxNorm Unique identifier for concept (concept ID)
  - Type: String
  - Required
  - Maximum Length : 8
  
- Semantic_Type_TUI
  - Unique identifier of Semantic Type
  - Type: String
  - Maximum Length : 4

- Semantic_Type_Tree_Number_STN
  - Semantic Type tree number
  - Type: String
  - Maximum Length : 100

- Semantic_Type_Value_STY
  - Semantic Type Values
  - Type: String
  - Maximum Length : 50

- Attribute_ATUI
  - Unique identifier for attribute  
  (no value provided)
  - Type: String
  - Maximum Length : 11
  
- Content_View_Flag
  - Content view flag. RxNorm includes one value, '4096', to denote inclusion in the Current Prescribable Content subset.  
  All rows with value '4096' can be found in the subset.
  - Type: String
  - Maximum Length : 50
