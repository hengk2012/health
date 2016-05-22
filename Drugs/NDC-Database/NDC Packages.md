# NDC Packages

## Summary
The Drug Listing Act of 1972 requires registered drug establishments to provide the Food and Drug Administration (FDA) with a current list of all drugs manufactured, prepared, propagated, compounded, or processed by it for commercial distribution.  (See Section 510 of the Federal Food, Drug, and Cosmetic Act (Act) (21 U.S.C. § 360)). Drug products are identified and reported using a unique, three-segment number, called the National Drug Code (NDC), which serves as a universal product identifier for drugs. FDA publishes the listed NDC numbers and the information submitted as part of the listing information in the NDC Directory which is updated daily.

## Description
The NDC Directory contains ONLY information on final marketed drugs submitted to FDA in SPL electronic listing files by labelers. (A labeler may be either a manufacturer, including a repackager or relabeler, or, for drugs subject to private labeling arrangements, the entity under whose own label or trade name the product will be distributed.) Inclusion of information in the NDC Directory does not indicate that FDA has verified the information provided. The content of each NDC Directory entry is the responsibility of the labeler submitting the SPL file. Assignment of an NDC number does not in any way denote FDA approval of the product. Any representation that creates an impression of official approval because of possession of an NDC number is misleading and constitutes misbranding. (21 CFR 207.39) 

## Facts
- Date Created: 2012
- Date Modified: 2016-05-20
- Version: 2016.05
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
 - NDC Packages
- Other Titles
 - National Drug Code Directory
 - NDC codes, NDC packages

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

- NDC_PACKAGE_CODE
  - The labeler code, product code, and package code segments of the National Drug Code number, separated by hyphens. Asterisks are no longer used or included within the product and package code segments to indicate certain configurations of the NDC.
  - Type: String
  - Required
  - Maximum Length : 12
  
- PACKAGE_DESCRIPTION
  - A description of the size and type of packaging in sentence form. Multilevel packages will have the descriptions concatenated together.  For example: 4 Bottles in 1 Carton/100 Tablets in 1 Bottle.
  - Type: String
  - Required
