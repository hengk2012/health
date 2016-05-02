# RxNorm Source Provider Information

## Summary
This data set contains contact information for source providers, available term types and attributes, and other information related to each RxNorm source.

## Description
RxNorm provides normalized names for clinical drugs and links its names to many of the drug vocabularies commonly used in pharmacy management and drug interaction software, including those of First Databank, Micromedex, MediSpan, Gold Standard Drug Database, and Multum. By providing links between these vocabularies, RxNorm can mediate messages between systems not using the same software and vocabulary.

RxNorm receives drug names from 14 source terminologies. In addition to the 14 data sources, the derived RxNorm normalized drug names become a terminology. 
RxNorm reflects and preserves the meanings, drug names, attributes, and relationships from its sources. There is one row in this file for every source in RxNorm.

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
  - RXNorm data sources
  - drug terminologies
  - pharmacy knowledge base systems
- Other Titles
 - RXNSAB
 - Source Terminologies
 - Drug Vocabularies
 - Source Abbreviation
 - Source Provider Analytics

## Schema
- Source_Concept_VCUI
  - Concept unique identifier of the versioned source concept for a source
  - Type: String
  - Maximum Length : 8
  
- Root_Source_Concept_RCUI
  - Concept unique identifier of the root source concept for a source
  - Type: String
  - Maximum Length : 8

- Versioned_Source_Abbreviation
  - The versioned source abbreviation for a source
  - Type: String
  - Maximum Length : 40

- Root_Source_Abbreviation
  - The root source abbreviation, for a source
  - Type: String
  - Required
  - Maximum Length : 20
  
- Official_Name
  - The official name for a source
  - Type: String
  - Maximum Length : 3000
  
- Source_Family
  - The Source Family for a source
  - Type: String
  - Maximum Length : 20

- Version
  - The source version
  - Type: String
  - Maximum Length : 20
  
- Start_Date
  - The date a source became active
  - Type: Date
  - Format: Date
  
- End_Date
  - The date a source ceased
  - Type: Date
  - Format: Date
  
- Meta_Insert_Version
  - The version of the Metathesaurus a source first appeared
  - Type: String
  - Maximum Length : 10

- Meta_Remove_Version
  - The version of the Metathesaurus a source was removed
  - Type: String
  - Maximum Length : 10
  
- Source_License_Contact
  - The source license contact information.  
  A semi-colon separated list containing the following fields: Name; Title; Organization; Address 1; Address 2; City; State or Province; Country; Zip or Postal Code; Telephone; Contact Fax; Email; URL
  - Type: String
  - Maximum Length : 1000
  
- Source_Content_Contact
  - The source content contact information.  
  A semi-colon separated list containing the following fields: Name; Title; Organization; Address 1; Address 2; City; State or Province; Country; Zip or Postal Code; Telephone; Contact Fax; Email; URL
  - Type: String
  - Maximum Length : 1000

- Source_Restriction_Level_SRL
  - License Agreement level   
Sources with SRL=0 follow the general terms of the license. All other values in SRL, have some restrictions outlined in section 12 of the UMLS license agreement
  - Type: Integer
  - Level: Ordinal
  
- Term_Frequency
  - The number of terms for this source in “RxNorm Drugs Names and Identifiers”   
  (not implemented yet)
  - Type: Integer
  - Level: Ratio
  - Format: int

- CUI_Frequency
  - The number of concept identifier associated with this source   
  (not implemented yet)
  - Type: Integer
  - Level: Ratio
  - Format: int

- Context_Type_CXTY
  - The type of relationship label 
  - Type: String
  - Maximum Length : 50

- Term_Type_List_TTYL
  - Term type list from source
  - Type: String
  - Maximum Length : 300
  
- Attribute_Name_List_ATNL
  - The attribute name list
  - Type: String
  - Maximum Length : 1000

- Language
  - The language of the terms in the source
  - Type: String
  - Maximum Length : 3
  
- Character_Encoding
  - Character set as specified by the IANA official names for character assignments 
  - Type: String
  - Maximum Length : 20

- Is_Current_Version
  - A true or false flag indicating whether or not this row corresponds to the current version of the named source
  - Type: Boolean

- Is_Source_In_Subset
  - A true or false flag indicating whether or not this row is represented in the current MetamorphoSys subset.   
  Initially always true where Is_current_version is true
  - Type: Boolean

- Source_Short_Name
  - The short name of a source as used by the NLM Knowledge Source Server
  - Type: String
  - Maximum Length : 3000
  
- Source_Citation
  - Citation information for a source.   
  A semi-colon separated list containing the following fields: Author(s); Author(s) address; Author(s) organization; Editor(s); Title; Content Designator; Medium Designator; Edition; Place of Publication; Publisher; Date of Publication/copyright; Date of revision; Location; Extent; Series; Availability Statement (URL); Language; Notes
  - Type: String
  - Maximum Length : 4000
