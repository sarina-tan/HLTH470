Medicare Advantage County Service Area Data

The Medicare Advantage (MA) organization county (Cnty) service area (SA) data package
is a compressed file (using WinZip) consisting of the following files:

Read_Me_MA_Cnty_SA_2015.txt - this file
MA_Cnty_SA_YYYY_MM.csv - data file (where YYYY = year and MM = month)

The MA_Cnty_SA_YYYY_MM.csv file is a comma separated value (csv) text file containing
approved service area information for the month and year described in the file name.
Text values in the file are surrounded by a double quote (") so that commas that are
part of an organization name could be included. The data type of each column is shown 
in brackets ([]) below. The file contains the following columns (these column names 
are included as the first row of data):

  Contract ID - [text] - The contract identifier 
  Organization Name - [text] - The name of the organization
  Organization Type - [text] - The type of contract held by the organization with CMS 
  Plan Type - [text] - The type of plan offered to beneficiaries
  Partial - [text] - Asterisk (*) when only part of the county is covered
  EGHP - [text] - Asterisk (*) when only Employer Group Plans are offered 
  SSA Code - [text] - The Social Security state/county code
  FIPS Code - [text] - The Federal Information Processing Standard state/county code
  County - [text] - The name of the county
  State - [text] - The two letter postal code for the state
  Notes - [text] - Contains additional information about some rows of data

This file contains data for the following organization types (where there are active contracts): 

  Local CCP
  Regional CCP
  MSA 
  PFFS 
  Demonstrations 
  National PACE 
  1876 Cost 
  HCPP - 1833 Cost


Special Notes: 

  (1) The service area for HCPP - 1833 Cost organizations is the entire United States.
  CMS systems have not traditionally stored the 3300 plus rows of data to to define
  each and every state and county for this organization type. This file continues
  this tradition because to expand out these contracts would add close to 30,000
  rows of data. These specific contracts have information in the notes column. 

  (2) The data file contains more than 65,536 rows of data. This means that Microsoft
  Excel will not be able to import all of the data for viewing. All of the data 
  can be viewed in Microsoft Access or in a statistical package, such as SAS. 

  (3) Pilot contracts are excluded from this file.