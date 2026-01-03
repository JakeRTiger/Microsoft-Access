# Microsoft-Access
Access Databases created for Clients on Upwork.  See GRUENE CRM SCREENSHOTS.doc
Greune CRM - Custom Built Custmer Relationship Management (CRM) Microsoft Access Database to manage promotions and track customers.
How the project started:
Given an Excel file that contains hundreds of thousands of records that contained tens of thousands of duplicated records
Created a relational database consisting of three tables:
Customer Address (ID, city, state, zip code, address)
TblNames (IDName,IDCust, email, first name, last name, alt email, date updated
TblPromo (idPromo, idName, PromoID)
Any Address can have multiple Names (first name, last name, email, alt email) and any name can be assigned ne or more promotions
There is a Customer screen that contains three forms:
Main form showing the adress, city, state, zip code
Sub form containg the names (first name, last name, email, alt email) linked by the ID in the Main form to the idCust in the sub form
2nd sub form containing the promotions each name has been assigned linked by the idname in the sub form containing Name  to tjhe idname in the TblPromo
Basically think of it as a stack with address on top followed by Name followd by Promo
The Customer address table has keys for City, State, Zip Code, and Address
The TblNames  has keys for idCust, first name and last name
TblPromo has keys for idName and PromoID

Features of the CRM
Import Excel files.  A template of the Excel file can be obtained by exporting data from the search screen (described below) if needed
The user will select a promo code, then import the filled out Excel file contains all the fields described above in the Customer address and tblNames tables

Filter screen
This screen has a list box of all promo codes  and seperate fields for First nme, Last Name, Address, City, Email zip code or zip code ranges.
Once the Perform Search button is pressed. say Promo code GHTB was selected in the multi-select list box and San Antonio entered in the City text box
Once the Perform Search button is pressed the results will appear in a new form called Filter Results.  In this example the search found 14,768 records.
The Filter Results screen contains a hyper link on the ID that will take the user to the Customer Screen (handy feature).  This screen is very powerful.  Edits can
be done directly on the screen to remove records or update, by pressing the Update CRM button the changes are submitted.  There is also a feature to output to Excel
and/or delete records,  This form also contains a sub form of the promo codes assigned to each records.  Its a very useful screeen.
Import Functionality
The Filter Results screen as mentioned can export to Excel and also delete the records in the database if desired.  As a test I filtered all San Antonio records and there were over 38000 records.  I exported the records to Excel and also deleted the records.  Opened the Excel file, made a change to two random records,saved the Excel file and re-imported and all the records including the changes we uploaded back into the database and it was done very fast under one minute.  Not bad considering that each records can have multiple promo codes and the fact that the records are being added to three tables.  Again Very powerful.

Chiropractic Continuing Education Database  Seminar Planning













