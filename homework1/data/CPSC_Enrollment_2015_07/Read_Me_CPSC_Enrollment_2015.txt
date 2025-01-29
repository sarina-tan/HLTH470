Contract/Plan/State/County Package

CPSC_enrollment_YYYY_MM.zip
The State/County/Contract/Plan (CPSC) Enrollment Data package is a compressed file (using WinZip) 
consisting of the following files:

Read_Me_CPSC_Enrollment_2015.txt - this file
CPSC_Contract_Info_YYYY_MM.csv - data file (where YYYY = year and MM = month)
CPSC_Enrollment_Info_YYYY_MM.csv - data file (where YYYY = year and MM = month)

The CPSC_Contract_Info_YYYY_MM.csv file is a comma separated value (csv) text file
containing descriptive attributes for every contract/plan combination that appears
in the CPSC_Enrollment_Info_YYYY_MM.csv file.

The CPSC_Enrollment_YYYY_MM.csv file is a comma separated value (csv) text file 
contains the enrollment data for the month and year described in the file name for
every contract/plan in every state/county.

Text values in the data files are surrounded by double a quote (") so that commas that 
are part of an organization name could be included. The data type of each column is 
shown in brackets ([]) below. The columns in each data file are described below, the
column names are included as the first row of data:

CPSC_Contract_Info_YYYY_MM.csv Columns
  Contract ID - [text] - The contract identifier 
  Plan ID - [text] - The plan identifier
  Organization Type - [text] - The type of contract held by the organization with CMS 
  Plan Type  - [text] - The type of plan offered to beneficiaries
  Offers Part D - "Yes" = offers Part D benefit, "No" = does not offer Part D benefit
  SNP Plan - "Yes" = Special Needs Plan, "No" = not a Special Needs Plan
  EGHP - "Yes" = Employer Group Health Plan, "No" = not an Employer Group Health Plan
  Organization Name - [text] - The name of the organization
  Organization Marketing Name - [text] - The name of the organization markets to beneficiaries
  Plan Name - [text] - The name of the plan created by the organization
  Parent Organization - [text] - the name of the parent organization for this contract
  Contract Effective Date - the data the contract began with CMS

CPSC_Enrollment_YYYY_MM.csv Columns
  Contract ID - [text] - The contract identifier 
  Plan ID - [text] - The plan identifier
  SSA Code - [text] - The Social Security state/county code
  FIPS Code - [text] - The Federal Information Processing Standard state/county code
  State - [text] - The two letter postal code for the state
  county - [text] - The name of the county
  Enrolled - [numeric] - Number of beneficiaries enrolled in the contract/plan in the state/county

These files contain data for the following organization types (where there are active contracts): 

  Local CCP
  Regional CCP
  MSA 
  PFFS 
  Demonstrations 
  National PACE 
  1876 Cost 
  HCPP - 1833 Cost
  Employer Sponsored PDP
  PDP

Special Notes:

  (1) The privacy laws of HIPAA have been interpreted to prohibit publishing 
  enrollment data with values of 10 or less. Consequently some enrollment data
  in this file have been set to blank because the enrollment was 10 or less. 

  (2) The enrollment data file contains more than 65,536 rows of data. This means 
  that Microsoft Excel will not be able to import all of the data for viewing. All 
  of the data can be viewed in Microsoft Access or in a statistical package, such 
  as SAS. 
 
  (3) The enrollment data file lists enrollees by their legal state and county of 
  residence; this is the county used for payment purposes. For example, an individual 
  who moved from Baltimore to Los Angeles and enrolled in XYZ Insurance company of 
  California would be paid at the Baltimore rate until the change of address was 
  recorded in the Social Security system. Consequently, the XYZ enrollment records 
  will include both the California counties in its approved contract service area as 
  well as the counties throughout the United States where XYZ has enrollees. 

  Please note that enrollment in these out of service area counties is very often under
  10, which leads to the suppression of the numbers.  This file does not indicate which 
  counties belong to the approved contract service area of a Medicare Advantage 
  organization and which counties are outside of its service area. You may refer to 
  the Medicare Advantage county service area file, which is available as a separate 
  download, to identify the approved contract service areas for these organizations.  

  (4) Pilot contracts are excluded from this file. The aggregate enrollment for these 
  contracts is available in the Monthly Contract and Enrollment Summary Report.