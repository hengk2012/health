# RxNorm Changed Atoms and Concepts from Last Release

## Summary
This dataset contains information on atoms that have changed concepts from the previous release to the current release. It only provides data about changes since the last release of RxNorm, it is not cumulative.

## Description
RxNorm provides normalized names for clinical drugs and links its names to many of the drug vocabularies commonly used in pharmacy management and drug interaction software, including those of First Databank, Micromedex, MediSpan, Gold Standard Drug Database, and Multum. By providing links between these vocabularies, RxNorm can mediate messages between systems not using the same software and vocabulary.

The dataset provides information about changes to the concept_id (RXCUI) for atoms in RxNorm from release to release. For source asserted atoms, all data fields will be populated. For RXCUI changes to RxNorm forms that have been archived, only the Source_Abbreviation, Old_RXConcept_CUI, and Old_RXConcept_CUI will be provided. Full information about RxNorm forms that have been archived can be found in the “RxNorm Archived Atoms Information” dataset.
## Facts
- Date Created: 2004-11
- Date Modified: 2016-05-02
- Version: 2016.05.02
- Update Frequency: Monthly
- Temporal Coverage: N/A
- Spatial Coverage: United States
- Source: National Library of Medicine (NLM)
- Source License URL: https://uts.nlm.nih.gov/license.html
- Source License Requirements: Reporting Requirements
- Source Citation: This release of RxNorm is consistent with the 2015AB UMLS Metathesaurus release.
- Keywords: 
 - Concept Changes
 - Data history
- Other Titles
 - RXNCUICHANGES
 - Concept changes analytics
 - Concepts changed for a specific source provider

## Schema
- RXAtom_AUI
  - RxNorm Unique identifier for atom (RxNorm Atom ID)
  - Type: String
  - Maximum Length : 8
  
- Most_Useful_Source_CODE
  - "Most useful" source asserted identifier (if the source vocabulary has more than one identifier), or RxNorm-generated source entry identifier (if the source vocabulary has none.)  
These are the FDA generated unique ingredient identifiers (UNIIs) for Source_Abbreviation =MTHSPL and Term_Type_In_Source=SU atoms.
  - Type: String
  - Maximum Length : 50

- Source_Abbreviation
  - Source abbreviation
  - Type: String
  - Maximum Length : 20

- Term_Type_In_Source_TTY
  - Term type in source  
   Refer “RxNorm Term Types for Normalized Names” for RxNorm source
  - Type: String
  - Maximum Length : 20
  - Reference: RxNorm Term Types for Normalized Names
  
- Drug_String
  - Drug name
  - Type: String
  - Maximum Length : 3000
  
- Old_RXConcept_CUI
  - Old RxNorm Unique identifier for concept (concept ID)
  - Type: String
  - Required
  - Maximum Length : 8
  
- New_RXConcept_CUI
  - New RxNorm Unique identifier for concept (concept ID)
  - Type: String
  - Required
  - Maximum Length : 8
