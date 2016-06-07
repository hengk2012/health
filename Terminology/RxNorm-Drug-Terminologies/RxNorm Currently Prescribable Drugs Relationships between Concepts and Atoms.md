# RxNorm Currently Prescribable Drugs Relationships between Concepts and Atoms
 
## Summary
This data contains all of the relationships that exist between atoms and between concepts for currently prescribable drugs. This includes source-provided relationships and relationships between RXNORM source-provided drug names.
 
## Description
RxNorm provides normalized names for clinical drugs and links its names to many of the drug vocabularies commonly used in pharmacy management and drug interaction software, including those of First Databank, Micromedex, MediSpan, Gold Standard Drug Database, and Multum. By providing links between these vocabularies, RxNorm can mediate messages between systems not using the same software and vocabulary.

This dataset is a subset of currently prescribable drugs found in RxNorm. NLM intends it to be an approximation of the prescription drugs currently marketed in the US. The subset also includes some frequently-prescribed over-the-counter drugs.  

The subset includes only the active RxNorm normalized names, codes (RxCUIs), attributes, and relationships, as well as the FDA structured product label drugs and ingredients and the small set of CMS data. Hence it includes the Source_Abbreviation=RXNORM, MTHSPL, MTHCMSFRF data only; no other source provider data.  It does not contain any suppressed or obsolete data.  
 
RXNORM provided relationships exist between atoms and between concepts, while source-provided relationships only exist between atoms from that source.  
 
Relationships in this dataset connect RXAtom_AUI_IDs or RXConcept_CUI_IDs. The corresponding drug names for these RXAtom_AUI_IDs and RXConcept_CUI_IDs are found in “RxNorm Drugs Names and Identifiers” dataset.  
 
For asymmetrical relationships there is one row for each direction of the relationship. 
 
Direction of relationship: the relationship which the SECOND concept or atom (with RXConcept2_CUI_ID and RXAtom2_AUI_ID) HAS TO the FIRST concept or atom (with RXConcept1_CUI_ID and RXAtom1_AUI_ID).  
 
A relationship will exist between the base atom and its duplicate atoms with "includes" and "included_in" (Relationship_Attribute_RELA). This relationship will carry the Source_Abbreviation=RXNORM.  
 
Specified (with quantity factor) and unspecified (without quantity factor) versions of extended release products are connected by the "has_quantified_form" and "quantified_form_of" reciprocal relationship attributes (Relationship_attribute_RELA)
 
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
 - Currently prescribable drugs 
 - Source-provided relationships
- Other Titles
 - prescribe/RXNREL
 - Relationships
 - Currently prescribable related concepts and atoms
 - Related Concepts analytics
 - Related Atoms analytics
 
## Schema
- RXConcept1_CUI
  - Unique identifier of first concept
  - Type: String
  - Maximum Length : 8
 
- RXAtom1_AUI
  - Unique identifier for first atom
  - Type: String
  - Maximum Length : 8
  
- Relation_Source1_Type_STYPE1
  - The name of the column in “RxNorm Drugs Names and Identifiers” that contains the identifier used for the first concept or first atom in source of the relationship (e.g., 'AUI' or 'CUI').
  - Type: String
  - Maximum Length : 50 
  
- Relationship_Code_REL
  - Relationship code of second concept or atom to first concept or atom
  - Type: String
  - Maximum Length : 4
  
- RXConcept2_CUI
  - Unique identifier of second concept
  - Type: String
  - Maximum Length : 8
 
- RXAtom2_AUI
  - Unique identifier for second atom
  - Type: String
  - Maximum Length : 8
  
- Relation_Source2_Type_STYPE2
  - The name of the column in “RxNorm Drugs Names and Identifiers” that contains the identifier used for the first concept or first atom in source of the relationship (e.g., 'AUI' or 'CUI').
  - Type: String
  - Maximum Length : 50 
  
- Relationship_Attribute_RELA
  - Additional (more specific) relationship label  
  ((optional))
  - Type: String
  - Maximum Length : 100
  
- Relationship_RUI
  - Unique identifier for relationship
  - Type: String
  - Maximum Length : 10
  
- Source_Asserted_Relationship_SRUI
  - Source asserted relationship identifier, if present  
  [no value provided]
  - Type: String
  - Maximum Length : 50  
 
- Source_Abbreviation
  - Source abbreviation
  - Type: String
  - Required
  - Maximum Length : 20
  
- Source_of_Relationship_Text
  - Source of relationship labels   
  (no value provided) 
  - Type: String
  - Maximum Length : 1000  
  
- Source_Asserted_Direction
  - Source asserted directionality flag.  
  - Type: Number
  - Level: Nominal
  - Format: short
  
- Machine_Generated_RG
  - Machine generated and unverified indicator  
  (optional)
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
