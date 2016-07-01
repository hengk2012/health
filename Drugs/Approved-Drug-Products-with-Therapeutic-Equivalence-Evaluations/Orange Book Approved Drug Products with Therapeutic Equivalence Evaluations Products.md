# Orange Book Approved Drug Products with Therapeutic Equivalence Evaluations Products

## Summary
This data set is also called Orange Book. The data set contains drug ingredient, dosage form, route, trade name, strength, product number, therapeutic equivalence code etc. for approved drug products with therapeuti equivalence.

## Description
The publication Approved Drug Products with Therapeutic Equivalence Evaluations (the List, commonly known as the Orange Book) identifies drug products approved on the basis of safety and effectiveness by the Food and Drug Administration (FDA) under the Federal Food, Drug, and Cosmetic Act (the Act). 
The Approved Drug Products list first appeared as a print publication in October 1980. With the 25th edition (2005), Portable Document Format (PDF) versions of the Annual Edition and the Cumulative Supplement became available.
The Orange Book Search was added to the FDA website October 31, 1997.

## Facts
- Date Created: 1981
- Date Modified: 2016-06-15
- Version: 2016.6
- Update Frequency: Monthly
- Temporal Coverage: 1981 to 2016-05
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
  - Generic Drug Products
  - Drugs List
- Other titles:
  - Newly approved drug with therapeutic equivalence
  - Product Number of approved drug product
  - Trade names of drugs with therapeutic equivalence
  - Approved with Therapeutic Equivalence Evaluations Book FDA  Drug Products
  - Approved with Therapeutic Equivalence Evaluations Drug Book Products
  - Approved Generic Drug Products with Therapeutic Equivalence 
  
## Schema
- Ingredient
  - The active ingredient(s) for the product. Multiple ingredients are in alphabetical order, separated by a comma.
  - Type: String
  - Required
- Dosage_Form_Route
  - The product dosage form and route separated by a comma.
  - Type: String
  - Required
- Trade_Name
  - The trade name of the product as shown on the labeling.
  - Type: String
  - Required
- Applicant
  - The firm name holding legal responsibility for the new drug application.  The firm name is condensed to a maximum twenty character unique string.
  - Type: String
  - Required
- Strength
  - The potency of the active ingredient.  May repeat for multiple part products.
  - Type: String
  - Required
- Application_Type
  - The type of new drug application approval.  New Drug Applications (NDA or innovator) or Abbreviated New Drug Applications (ANDA or generic).
  - Type: String
  - Required
- Application_No
  - New Drug Application (NDA) Number. The FDA assigned number to the application.
  - Type: Number
  - Level: Nominal
  - Required
- Product_No
  - The FDA assigned number to identify the application products. Each strength is a separate product.  May repeat for multiple part products.
  - Type: Number
  - Level: Nominal
  - Required
- Therapeutic_Equivalence_Code
  - Therapeutic Equivalence (TE) Code. The TE Code indicates the therapeutic equivalence rating of generic to innovator Rx products
  - Type: String
- Approval_Date
  - The date the product was approved as stated in the FDA approval letter to the applicant.  The format is yyyy-mm-dd.  Products approved prior to the January 1, 1982 contain the phrase: "Approved prior to Jan 1, 1982".
  - Type: Date
  - Required
- Is_Reference_Listed_Drugs
  - Reference Listed Drug (RLD). The pioneer or innovator of the drug.  The RLD identifies the product Abbreviated New Drug Applications (ANDA) use as a reference.  Format is true or false.
  - Type: Boolean
  - Required
- Type
  - The group or category of approved drugs.  Format is RX, OTC, DISCN.
  - Type: String
  - Required
- Applicant_Full_Name
  - The full name of the firm holding legal responsibility for the new drug application.
  - Type: String
  - Required
