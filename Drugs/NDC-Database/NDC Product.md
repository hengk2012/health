# NDC Product

## Summary
The Drug Listing Act of 1972 requires registered drug establishments to provide the Food and Drug Administration (FDA) with a current list of all drugs manufactured, prepared, propagated, compounded, or processed by it for commercial distribution.  (See Section 510 of the Federal Food, Drug, and Cosmetic Act (Act) (21 U.S.C. § 360)). Drug products are identified and reported using a unique, three-segment number, called the National Drug Code (NDC), which serves as a universal product identifier for drugs. FDA publishes the listed NDC numbers and the information submitted as part of the listing information in the NDC Directory which is updated daily.

## Description
The NDC Directory contains ONLY information on final marketed drugs submitted to FDA in SPL electronic listing files by labelers. (A labeler may be either a manufacturer, including a repackager or relabeler, or, for drugs subject to private labeling arrangements, the entity under whose own label or trade name the product will be distributed.) Inclusion of information in the NDC Directory does not indicate that FDA has verified the information provided. The content of each NDC Directory entry is the responsibility of the labeler submitting the SPL file. Assignment of an NDC number does not in any way denote FDA approval of the product. Any representation that creates an impression of official approval because of possession of an NDC number is misleading and constitutes misbranding. (21 CFR 207.39)

## Facts
- Date Created: 2012
- Date Modified: 2016-06-01
- Version: 2016.06.30
- Update Frequency: Daily
- Temporal Coverage: N/A
- Spatial Coverage: United States
- Source: US Food and Drug Administration (FDA)
- Source License URL: N/A
- Source License Requirements: Open for commercial use
- Source Citation: N/A
- Keywords: 
 - National Drug Code
 - NDC
 - NDC Products
- Other Titles
 - National Drug Code Directory
 - NDC codes, NDC Products

## Schema
- PRODUCT_ID
  - ProductID is a concatenation of the NDCproduct code and SPL documentID. It is included to help prevent duplicate rows from appearing when joining the product and package files together.  It has no regulatory value or significance.
  - Type: String
  - Required

- PRODUCT_NDC
  - The labeler code and product code segments of the National Drug Code number, separated by a hyphen. Asterisks are no longer used or included within the product code segment to indicate certain configurations of the NDC.
  - Type: String
  - Required
  - Maximum Length : 10 

- PRODUCT_TYPE_NAME
  - Indicates the type of product, such as Human Prescription Drug or Human OTC Drug. This data element corresponds to the “Document Type” of the SPL submission for the listing.
  - Type: String
  - Required

- PROPRIETARY_NAME
  - Also known as the trade name. It is the name of the product chosen by the labeler.
  - Type: String
 
- PROPRIETARY_NAME_SUFFIX
  - A suffix to the proprietary name, a value here should be appended to the ProprietaryName field to obtain the complete name of the product. This suffix is often used to distinguish characteristics of a product such as extended release (“XR”) or sleep aid (“PM”). Although many companies follow certain naming conventions for suffices, there is no recognized standard
  - Type: String

- NONPROPRIETARY_NAME
  - Sometimes called the generic name, this is usually the active ingredient(s) of the product.
  - Type: String

- DOSAGE_FORM_NAME
  - The translation of the Dosage Form Code submitted by the firm. The complete list of codes and translations can be found www.fda.gov/edrls under Structured Product Labeling Resources.
  - Type: String
  - Required

- ROUTE_NAME
  - The translation of the Route Code submitted by the firm, indicating route of administration. The complete list of codes and translations can be found at www.fda.gov/edrls under Structured Product Labeling Resources
  - Type: String

- START_MARKETING_DATE
  - This is the date that the labeler indicates was the start of its marketing of the drug product
  - Type: Date

- END_MARKETING_DATE
  - This is the date the product will no longer be available on the market. If a product is no longer being manufactured, in most cases, the FDA recommends firms use the expiration date of the last lot produced as the End Marketing Date, to reflect the potential for drug product to remain available after manufacturing has ceased. Products that are the subject of ongoing manufacturing will not ordinarily have any End Marketing Date. Products with a value in the End Marketing Date will be removed from the NDC Directory when the End Marketing Date is reached.
  - Type: Date
  - Required

- MARKETING_CATEGORY_NAME
  - Product types are broken down into several potential Marketing Categories, such as NDA/ANDA/BLA, OTC Monograph, or Unapproved Drug. One and only one Marketing Category may be chosen for a product, not all marketing categories are available to all product types. Currently, only final marketed product categories are included.  The complete list of codes and translations can be found at www.fda.gov/edrls under Structured Product Labeling Resources.
  - Type: String
  - Required

- APPLICATION_NUMBER
  - This corresponds to the NDA, ANDA, or BLA number reported by the labeler for products which have the corresponding Marketing Category designated. If the designated Marketing Category is OTC Monograph Final or OTC Monograph Not Final, then the Application number will be the CFR citation corresponding to the appropriate Monograph (e.g. “part 341”). For unapproved drugs, this field will be null.
  - Type: String
  - Maximum Length : 11
 
- LABELER_NAME
  - Name of Company corresponding to the labeler code segment of the Product NDC
  - Type: String
  - Required

- SUBSTANCE_NAME
  - This is the active ingredient list. Each ingredient name is the preferred term of the UNII code submitted
  - Type: String

- ACTIVE_NUMERATOR_STRENGTH
  - These are the strength values (to be used with units below) of each active ingredient, listed in the same order as the Substance Name field above.
  - Type: String

- ACTIVE_INGRED_UNIT
  - These are the units to be used with the strength values above, listed in the same order as the Substance Name and Substance Number.
  - Type: String

- PHARM_CLASSES
  - These are the reported pharmacological class categories corresponding to the Substance Names listed above.
  - Type: String

- DEA_SCHEDULE
  - This is the assigned Drug Enforcement Administration Schedule number as reported by the labeler.
  - Type: String
  - Values: CI, CII, CIII, CIV
  - Maximum Length : 4
