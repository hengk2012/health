# RxNorm Term Types for Normalized Names

## Summary
RXNORM source uses term types (TTYs) to indicate generic and branded drug names at different levels of specificity. This dataset includes the full list of term types, where source provider is RXNORM.

## Description
RxNorm provides normalized names for clinical drugs and links its names to many of the drug vocabularies commonly used in pharmacy management and drug interaction software, including those of First Databank, Micromedex, MediSpan, Gold Standard Drug Database, and Multum. By providing links between these vocabularies, RxNorm can mediate messages between systems not using the same software and vocabulary.

Each RXNORM normalized name follows a simple pattern using the ingredient, strength, and dose form. For branded drugs, RXNORM normalized name includes the brand name, and for packs of drugs, RXNORM normalized name includes the quantities of each drug.

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
 - RXNorm normalized name
 - RXNORM term types
- Other Titles
 - TTYs
 - Term Types

## Schema
- Code_TTY
  - Code for Term Type
  - Type: String
  - Required
  - Maximum Length : 8
  
- Name
  - Name for Term Type
  - Type: String
  - Maximum Length : 50

- Description
  - Detailed description of Term Type
  - Type: String
  - Maximum Length : 3000
