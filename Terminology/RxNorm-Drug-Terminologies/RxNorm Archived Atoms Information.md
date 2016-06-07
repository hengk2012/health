# RxNorm Archived Atoms Information 

## Summary
This dataset includes history information about RxNorm atoms. It contains information about SAB=RXNORM atoms that are no longer in “RxNorm Drugs Names and Identifiers”.

## Description
RxNorm provides normalized names for clinical drugs and links its names to many of the drug vocabularies commonly used in pharmacy management and drug interaction software, including those of First Databank, Micromedex, MediSpan, Gold Standard Drug Database, and Multum. By providing links between these vocabularies, RxNorm can mediate messages between systems not using the same software and vocabulary.

The dataset contains data about RxNorm Source provider (atoms) that are no longer a part of the RxNorm database because the drug data source provider is no longer providing this name to RxNorm. 

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
 - Data history
 - Archived atoms
- Other Titles:
 - RXNATOMARCHIVE
 - Archive Data
 - Archived Drugs analytics

## Schema
- RXAtom_AUI
  - RxNorm Unique identifier for atom (RxNorm Atom ID)
  - Type: String
  - Required
  - Maximum Length : 8
 
- MTH_AUI
  - Metathesaurus Unique identifier for atom
  - Type: String
  - Maximum Length : 10
 
- Drug_String
  - Drug name
  - Type: String
  - Required
  - Maximum Length : 4000
 
- Atom_Archived_Timestamp
  - Date/Time Archived
  - Type: Date & Time
  - Required
  - Format : Date & Time
 
- Atom_Created_Timestamp
  - Date/Time Created in this version of RxNorm
  - Type: Date & Time
  - Required
  - Format : Date & Time
 
- Atom_Updated_Timestamp
  - Date/Time Updated in this version of RxNorm
  - Type: Date & Time
  - Required
  - Format : Date & Time

- Most_Useful_Source_CODE
  - "Most useful" source asserted identifier (if the source vocabulary has more than one identifier), or RxNorm-generated source entry identifier (if the source vocabulary has none.)  
These are the FDA generated unique ingredient identifiers (UNIIs) for Source_Abbreviation =MTHSPL and Term_Type_In_Source=SU atoms.
  - Type: String
  - Maximum Length : 50
 
- Is_Brand
  - Branded data flag  
  (not used)
  - Type: Boolean
 
- Language
  - Language of Term
  - Type: String
  - Maximum Length : 3 
 
- Atom_Last_Released_Date
  - Date this name (atom) was last released from RxNorm
  - Type: Date
  - Format : Date
 
- Source_Asserted_Atom_SAUI
  - Source asserted atom identifier  
  [optional]
  - Type: String
  - Maximum Length : 50  
 
- Version_Source_Abbreviation
  - Versioned Source Abbreviation
  - Type: String
  - Maximum Length : 40 
 
- RXConcept_CUI
  - RxNorm Unique identifier for concept (concept ID)
  - Type: String
  - Maximum Length : 8
 
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
 
- Merged_To_RXConcept_CUI
  - RxNorm Unique identifier for concept (concept ID) which name (atom) was merged into
  - Type: String
  - Maximum Length : 8
