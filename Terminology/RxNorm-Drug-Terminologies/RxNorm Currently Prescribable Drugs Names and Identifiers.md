# RxNorm Currently Prescribable Drugs Names and Identifiers

## Summary
This data contains all Currently Precribable drug and ingredient names and codes. Every string or concept name in RxNorm appears in this file, connected to its language, source vocabularies, and its concept identifier.

## Description
RxNorm provides normalized names for clinical drugs and links its names to many of the drug vocabularies commonly used in pharmacy management and drug interaction software, including those of First Databank, Micromedex, MediSpan, Gold Standard Drug Database, and Multum. By providing links between these vocabularies, RxNorm can mediate messages between systems not using the same software and vocabulary.

This dataset is a subset of currently prescribable drugs found in RxNorm. NLM intends it to be an approximation of the prescription drugs currently marketed in the US. The subset also includes some frequently-prescribed over-the-counter drugs.  

The subset includes only the active RxNorm normalized names, codes (RxCUIs), attributes, and relationships, as well as the FDA structured product label drugs and ingredients and the small set of CMS data. Hence it includes the Source_Abbreviation=RXNORM, MTHSPL, MTHCMSFRF data only; no other source provider data.  It does not contain any suppressed or obsolete data.

Concepts are collections of synonyms at a given level of abstraction. Each concept receives an RX_Concept_CUI, which is unique to that concept. An RX_Concept_CUI is essentially the "name" of a concept that computers read and understand. Each drug name carries additional characteristics, including its source, its code (the unique identifier assigned by its source), and its term type. An atom is a drug name plus these additional characteristics. Each atom within a concept receives an atom unique identifier, an RX_Atom_AUI.

Each row in this file represents a single atom, and the RXAtom_AUI value is unique for each row. Essentially, the row is the atom. Because a given concept may include multiple atoms, there may be multiple rows with a given RXConcept_CUI.

RxNorm is creating duplicates of source asserted atoms, which carry multiple meanings. When an atom is duplicated, the original source atom is considered to be a 'Base' atom. The duplicate atoms' strings are created by appending '_#N' to the Base atom string where 'N' is a number from 1 to N number of duplicates for this base atom. The duplicate atom's ‘Term_Type_in_Source_TTY’ will be created by prepending 'MTH_RXN_' to the base atom's term type.

## Facts
- Date Created: 2004-11
- Date Modified: 2016-04-04
- Version: 2016.04.04
- Update Frequency: Monthly
- Temporal Coverage: N/A
- Spatial Coverage: United States
- Source: National Library of Medicine (NLM)
- Source License URL: https://uts.nlm.nih.gov/license.html
- Source License Requirements: Reporting Requirements
- Source Citation: This release of RxNorm is consistent with the 2015AB UMLS Metathesaurus release.
- Keywords:
 - Over-the-counter drugs names
 - Currently prescribable drugs names
 - Frequently prescribed drugs names
 - RxNorm normalized names
- Other Titles
 - prescribe/RXNCONSO
 - Concept Names and Sources
 - Drugs names and unique identifiers
 - Currently Prescribable drugs names analytics
 - Synonymous drugs names with the same concept
 - Normalized name for a concept (source_abbreviation = RXNORM)
 - Normalized drugs names (source_abbreviation = RXNORM)
 - Duplicated Drugs analytics

## Schema
- RXConcept_CUI
  - RxNorm Unique identifier for concept (concept ID)
  - Type: String
  - Required
  - Maximum Length : 8

- Language
  - Language of Term
  - Type: String
  - Values: ENG
  - Maximum Length : 3 
  
- Term_Status_TS
  - Term status  
  (no value provided)
  - Type: String
  - Maximum Length : 1
  
- Term_LUI
  - Unique identifier for term  
  (no value provided)
  - Type: String
  - Maximum Length : 8
  
- String_Type_STT
  - String type  
  (no value provided)
  - Type: String
  - Maximum Length : 3
  
- String_SUI
  - Unique identifier for string
  (no value provided)
  - Type: String
  - Maximum Length : 8
 
- Is_Preferred
  - Atom status - preferred (true) or not (false) for this string within this concept  
  (no value provided)
  - Type: Boolean
  
- RXAtom_AUI
  - RxNorm Unique identifier for atom (RxNorm Atom ID)
  - Type: String
  - Required
  - Maximum Length : 8
  
- Source_Asserted_Atom_SAUI
  - Source asserted atom identifier  
  [optional]
  - Type: String
  - Maximum Length : 50  

- Source_Asserted_Concept_SCUI
  - Source asserted concept identifier   
  [optional]
  - Type: String
  - Maximum Length : 50  
  
- Source_Asserted_Descriptor_SDUI
  - Source asserted Descriptor identifier   
  [optional]
  - Type: String
  - Maximum Length : 50  
  
- Source_Abbreviation
  - Source abbreviation
  - Type: String
  - Required
  - Maximum Length : 20
  
- Term_Type_In_Source_TTY
  - Term type in source  
   Refer “RxNorm Term Types for Normalized Names” for RxNorm source
  - Type: String
  - Required
  - Maximum Length : 20
  - Reference: RxNorm Term Types for Normalized Names 
  
- Most_Useful_Source_CODE
  - "Most useful" source asserted identifier (if the source vocabulary has more than one identifier), or RxNorm-generated source entry identifier (if the source vocabulary has none.)  
These are the FDA generated unique ingredient identifiers (UNIIs) for Source_Abbreviation =MTHSPL and Term_Type_In_Source=SU atoms.
  - Type: String
  - Required
  - Maximum Length : 50
  
- Drug_String
  - Drug name
  - Type: String
  - Required
  - Maximum Length : 3000
  
- Source_Restriction_Level_SRL
  - Source Restriction Level  
  (no value provided)
  - Type: String
  - Maximum Length : 10 

- Suppressible_Flag_SUPPRESS
  - Suppressible flag.  
  N - not suppressible.  
  O - Specific individual names (atoms) set as Obsolete because the name is no longer provided by the original source.  
  Y - Suppressed by RxNorm editor.  
  E - unquantified, non-prescribable drug with related quantified, prescribable drugs.  
  NLM strongly recommends that users not alter editor-assigned suppressibility.
  - Type: String
  - Values:  N, O, Y, E
  - Maximum Length : 1
  
- Content_View_Flag
  - Content view flag. RxNorm includes one value, '4096', to denote inclusion in the Current Prescribable Content subset.  
  All rows with value '4096' can be found in the subset.
  - Type: String
  - Maximum Length : 50
