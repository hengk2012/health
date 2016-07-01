# Orange Book Approved Drug Products with Therapeutic Equivalence Evaluations Exclusivity

## Summary
This data set is also called Orange Book. The data set contains application type, exclusivity code, exclusivity date etc for approved drug products with therapeuti equivalence.

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
  - Exclusivity
  - Drug Book
  - Orange Book
  - Generic Drug Products
  - Drugs List
- Other titles:
  - Exclusivity of newly approved drug
  - Exclusivity of approved drug product
  - Exclusivity of drugs with therapeutic equivalence
  - Drug Book Products with Therapeutic Equivalence Evaluations Exclusivity
  - Drug Products with Therapeutic Equivalence Evaluations Exclusivity Orange Book
  - Generic Drug Products with Therapeutic Equivalence 
  
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
- Exclusivity_Code
  - Code to designate exclusivity granted by the FDA to a drug product.
  - Type: String
  - Required
- Exclusivity_Date
  - The date the exclusivity expires. Format is YYYY-MM-DD.
  - Type: Date
  - Required
