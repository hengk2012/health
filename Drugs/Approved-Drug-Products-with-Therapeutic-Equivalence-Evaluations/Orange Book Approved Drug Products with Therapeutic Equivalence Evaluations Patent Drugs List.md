# Orange Book Approved Drug Products with Therapeutic Equivalence Evaluations Patent Drugs List

## Summary
This data set is also called Orange Book. The data set contains drug ingredient, dosage form, route, product number, therapeutic equivalence code, whether or not it is reference listed drug etc.

## Description
The publication Approved Drug Products with Therapeutic Equivalence Evaluations (the List, commonly known as the Orange Book) identifies drug products approved on the basis of safety and effectiveness by the Food and Drug Administration (FDA) under the Federal Food, Drug, and Cosmetic Act (the Act). 
The Approved Drug Products list first appeared as a print publication in October 1980. With the 25th edition (2005), Portable Document Format (PDF) versions of the Annual Edition and the Cumulative Supplement became available.
The Orange Book Search was added to the FDA website October 31, 1997.

## Facts
- Date Created: 1981
- Date Modified: 2016-04-01
- Version: 2016.04
- Update Frequency: Monthly
- Temporal Coverage: 1981 to 2016-04
- Spatial Coverage: United States
- Source: U.S. Food and Drug Administration
- Source License URL: N/A
- Source License Requirements: N/A
- Source Citation: http://www.fda.gov/Drugs/InformationOnDrugs/ucm129689.htm
- Keywords:
  - Approved drug
  - Therapeutic equivalence
  - Patent
  - Book FDA
  - Drug Book
  - Orange Book
  - Generic Drug Products
  - Drugs List
- Other titles:
  - Ingredient of newly approved drug
  - Dosage of approved drug product
  - Product number of drugs with therapeutic equivalence
  - Reference listed drugs
  - Approved Drug Products with Therapeutic Equivalence Evaluations Patent Book FDA
  - Approved Drug Book Products with Therapeutic Equivalence Evaluations Patent
  - Approved Orange Book Drug Products with Therapeutic Equivalence Evaluations Patent
  - Approved Generic Drug Products with Therapeutic Equivalence Evaluations Patent
  - Approved Drug Products with Therapeutic Equivalence Evaluations Patent Drugs List
  
## Schema
- Application_Type
  - The type of new drug application approval. New Drug Applications (NDA or innovator) or Abbreviated New Drug Applications (ANDA or generic).
  - Type: String
  - Required
- Application_No
  - o	New Drug Application (NDA) Number. The FDA assigned number to the application.
  - Type: Integer
  - Level: Nominal
  - Required
- Product_No
  - The FDA assigned number to identify the application products. Each strength is a separate product.  May repeat for multiple part products.
  - Type: Integer
  - Level: Nominal
  - Required
- Patent_No
  - Patent numbers as submitted by the applicant holder for patents covered by the statutory provisions.  May repeat for multiple applications and multiple products. Includes pediatric exclusivity granted by the agency.
  - Type: String
  - Required
- Patent_Expire_Date
  - The date the patent expires as submitted by the applicant holder including applicable extensions.
  - Type: Date
  - Required
- Drug_Substance_Flag
  - Patents submitted on FDA Form 3542 and listed after August 18, 2003 may have a drug substance flag indicating the sponsor submitted the patent as claiming the drug substance.
  - Type: String
- Drug_Product_Flag
  - Patents submitted on FDA Form 3542 and listed after August 18, 2003 may have a drug product flag indicating the sponsor submitted the patent as claiming the drug product.
  - Type: String
- Patent_Use_Code
  - Code to designate a use patent that covers the approved indication or use of a drug product.  May repeat for multiple applications, multiple products and multiple patents.
  - Type: String
- Delist_Flag
  - o	Patent Delist Request Flag. Sponsor has requested patent be delisted.  This patent has remained listed because, under Section 505(j)(5)(D)(i) of the Act, a first applicant may retain eligibility for 180-day exclusivity based on a paragraph IV certification to this patent for a certain period.  Applicants under Section 505(b)(2) are not required to certify to patents where this flag is set to Y.
  - Type: String
