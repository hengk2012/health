# RxNorm Attributes Data for Concepts and Atoms

## Summary
This dataset contains all of the attribute data.  
This includes RXNORM provided attributes, such as normalized 11-digit NDCs, UNII codes, and human or veterinary usage markers, and source-provided attributes, such as labeler, definition, and imprint information. Each attribute has an 'Attribute Name' (ATN) and 'Attribute Value' (ATV) combination. For example, NDCs have an ATN of 'NDC' and an ATV of the actual NDC value.

## Description
RxNorm provides normalized names for clinical drugs and links its names to many of the drug vocabularies commonly used in pharmacy management and drug interaction software, including those of First Databank, Micromedex, MediSpan, Gold Standard Drug Database, and Multum. By providing links between these vocabularies, RxNorm can mediate messages between systems not using the same software and vocabulary.

This dataset associates attributes data with RXAtom_AUI_IDs and  RXConcept_CUI_IDs. The corresponding drug names for these RXAtom_AUI_IDs and RXConcept_CUI_IDs are found in “RxNorm Drugs Names and Identifiers” dataset.  

A base atom can be identified by the existence of an attribute, where the Attribute_Name_ATN='AMBIGUITY_FLAG' and the Attribute_Value_ATV='Base'. Similarly, the duplicate atoms are identified with Attribute_Name_ATN ='AMBIGUITY_FLAG' and Attribute_Value_ATV ='Duplicate'. This attribute will carry the Source_Abbreviation=RXNORM.  

The quantity factor is stored as an attribute as the value of the Attribute_Name_ATN ='RXN_QUANTITY' with Source_Abbreviation=RXNORM. This quantity factor consists of a number followed by a unit measure. The number might represent a strength, a unit of time, or a quantity of dosages depending upon the drug’s dosage form in use at the time.  

## Facts
- Date Created: 2004-11
- Date Modified: 2016-03-07
- Version: 2016.03.07
- Update Frequency: Monthly
- Temporal Coverage: N/A
- Spatial Coverage: United States
- Source: National Library of Medicine (NLM)
- Source License URL: https://uts.nlm.nih.gov/license.html
- Source License Requirements: Reporting Requirements
- Source Citation: This release of RxNorm is consistent with the 2015AB UMLS Metathesaurus release.
- Keywords: 
 - Attributes
 - Source vocabulary attributes
 - Concept attributes
- Other Titles
 - RXNSAT
 - Simple Concepts and Atom Attributes
 - MRSAT
 - All attributes for a specific concept or atom
 - Attribute name value pairs with in a specific source provider
 - Suppressed and non-suppressed attributes analytics
 - The normalized NDCs provided by NLM (Source_Abbreviation='RXNORM' and Attribute_Name_ATN=’NDC’). These normalized NDCs follows the 11 digit, no dashes HIPAA format

## Schema
- RXConcept_CUI
  - RxNorm Unique identifier for concept (concept ID)
  - Type: String
  - Maximum Length : 8

- Term_LUI
  - Unique identifier for term  
  (no value provided)
  - Type: String
  - Maximum Length : 8
  
- String_SUI
  - Unique identifier for string
  (no value provided)
  - Type: String
  - Maximum Length : 8

- RXAtom_AUI
  - RxNorm Unique identifier for atom (RxNorm Atom ID)
  - Type: String
  - Maximum Length : 8
  
- Source_Type_STYPE
  - The name of the column in “RxNorm Drugs Names and Identifiers” or “RxNorm Relationships Between Concepts and Atoms“ that contains the identifier to which the attribute is attached, e.g., <name>_CUI, <name>_AUI.
  - Type: String
  - Maximum Length : 50 
  
  
- Most_Useful_Source_CODE
  - "Most useful" source asserted identifier (if the source vocabulary has more than one identifier), or RxNorm-generated source entry identifier (if the source vocabulary has none.)  
These are the FDA generated unique ingredient identifiers (UNIIs) for Source_Abbreviation =MTHSPL and Term_Type_In_Source=SU atoms.
  - Type: String
  - Maximum Length : 50
  
- Attribute_ATUI
  - Unique identifier for attribute  
  (no value provided)
  - Type: String
  - Maximum Length : 11
  
- Source_Asserted_Attribute_SATUI
  - Source asserted attribute identifier  
  (no value provided)
  - Type: String
  - Maximum Length : 50
  
- Attribute_Name_ATN
  - Attribute name. Possible values appear in “RxNorm Data Elements and Attributes Names” dataset 
  - Type: String
  - Required
  - Maximum Length : 1000
  
- Source_Abbreviation
  - Source abbreviation
  - Type: String
  - Required
  - Maximum Length : 20
  
- Attribute_Value_ATV
  - Attribute value described under specific attribute name. A few attribute values exceed 1,000 characters. Many of the abbreviations used in attribute values are explained in “RxNorm Data Elements and Attributes Names” dataset 
  - Type: String
  - Maximum Length : 4000

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
