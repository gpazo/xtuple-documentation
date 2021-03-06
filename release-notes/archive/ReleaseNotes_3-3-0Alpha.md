Release Notes
xTuple ERP
PostBooks, Standard, and Manufacturing Editions
Version 3.3.0Alpha
June 03, 2009
----------------------------------

This is the Alpha release of version 3.3.0. We are especially eager
to hear feedback from alpha testers on the following new areas of
functionality:

Distribution Resource Planning (DRP)
  * Full spec: http://www.xtuple.org/DistributionResourcePlanning

Improved VAT and international tax support
  * Full spec: http://www.xtuple.org/EnhancedTaxInternationalization

Multiple Accounting features
  * Re-allocation of AR applications
  * Automated forward-updating
  * Reverse Cash Receipts
  * Printing AR Memos
  * And more....

EDI Profiles Revision
  * Full spec: http://www.xtuple.org/EDIProfilesRevision
  * PLEASE NOTE: This spec is partially-implemented only
  * For a preview, see
       - Sales > Customer > Customer Master > Transmission Tab
	 - Sales > Forms > E-mail Sales Order Form

Translation
  * Support for translating extension packages

----------------------------------

The following features and bug fixes have been added to the applications
since the release of version 3.2.2. Additional detail for each item
listed below may be found on our community website (www.xtuple.org).
Simply go to the Issue Tracker and select the Changelog option.


New Features:

* [All] Add "Copy to Clip Board" to XTreeWidget default Context Menu
* [All] Application has hard-coded shortcut keys
* [All] Integrate xTuple user and PostgreSQL users
* [All] Need to determine translation mechanism for screen builder 
extensions
* [All] Updated menus to be more memory efficient and to address some 
issues related to rescanning privileges
* [Accounting] Add ability to filter out trial balances with no balance
or activity.
* [Accounting] Change or Remove the automatic forward account balances
capability in Accounting
* [Accounting] Add option to make forward updating accounts fully
automatic
* [Accounting] Enable reversing of Cash Receipt postings
* [Accounting] Adjustment Types description column show name value
* [Accounting] Enable re-allocation of AR applications
* [Accounting] Need to do a negative cash receipt
* [Accounting] Display Cash Receipt subtotals
* [Accounting] Preserve cash receipt info in arapply, credit memos,
and cash deposits
* [Accounting] Enhance Expense Cat Master List to Show G/L Accounts
* [Accounting] Invoice: Add Due Date and Discount Date
* [Accounting] Cannot control Customer's Check Date
* [Accounting] Reference and Notes for Vouchers
* [Accounting] Printing Debit Memos or Credit Memos
* [Accounting] Voiding vouchers does not undo distributions
* [Accounting] Change Reprint Invoices to allow selection by Balance
Due
* [Batch Manager] "Make "Submit Action to ..." Send Email
* [CRM] Add email to searchable fields on CRM Search for Contact
* [CRM] Improve visibility to prior comments on Incident Workbench
* [CRM] Need ability to edit comments
* [CRM] Create Jump To field for incident number
* [CRM] Comments for To-Do's and Tasks
* [Inventory] In Built Inventory Availablity by...
* [Inventory] ABC Classcode and Cycle Count Frequency added to
dspItemSitesByParameterList.cpp
[Inventory] Add an ability to set Location Default whilst Posting
to Inventory
* [Products] Create Item Site by Class Code Util - Needs First
Group field
* [Purchase] Purchase Order Items Window - Prices Tab
* [Purchase] Enhance PO Report Def - Alt Address Prints as Ship To
* [Schedule] Add Distribution Resource Processing (DRP) capability
to Standard Edition
* [Sales] Reorganize and consolidate customer information
* [Sales] Add button to Return Authorization workbench to create a
NEW RA
* [Sales] Rcv site in RA header doesn't affect sites in RA items
- P/R Column
* [Sales] Add Function getpacklistitemlotserialqty()
* [Sales] Explode Kits on Return Authorizations same as Sales Orders
* [Sales] Allow Kit components to inherit COS from Kit parent
* [System] Change default script extension to .js
* [System] Add support on lists (xtreewidget) for export to CSV, ODF
and HTML file formats
* [System] Expose method to add right click menu on xtreewidget and
xtreeview via scripting
* [System] Provide method to open core xTuple screens from other
screen builder screens
* [System] Rework layouts on windows using parameterGroup and
warehouseGroup to use "natural" layouts
* [System] Additional alert functionality when cost exceeds max cost
* [System] Enable incident emails by category setting
* [System] Add the ability to purge sales orders
* [System] Reason Codes assigned to documents
* [System] Add "sticky" memory to grid sorting on xtreewidget
* [System] Add DB Configuration Option to Disallow All User Logons
* [System] Add command line arguments for specifying Enhanced Auth
and SSL boolean
* [System] add include facility to scripting


Bug Fixes:

*  [All] Date Time Stamp in comment change log displays time as
12:00:00 AM
* [All] Remove Schedule Backup menu option
* [All] Obsolete macro in widgets library
* [All] some tables have user ids but should have user names
* [All] Missing return from Screen::submit()
* [Accounting] Tax liability note on G/L transactions causes G/L
series not to group properly
* [Accounting] Post zero amount invoices to aropen, simplify AR
Open query
* [Accounting] Accounting menus inconsistent
* [Accounting] possible to have a closed aropen item with no
aropen_closedate
* [Accounting] Customer Information Workbench missing previously
available information
* [Accounting] Privilege Hole in Sales Order
* [Accounting] Viewing Unposted Invoices
* [Accounting] Sales Order Lookup - Pattern Matching Not Working
* [Accounting] Inactive Vendors not controlled in miscellaneous
voucher entry
* [Accounting] Rescan privileges ignores initMenu script
* [Accounting] Right click drill down results on A/R aging are
incorrect
* [Accounting] GL Trans Report for Doc Type 'IN' does not display
Customer Name
* [Accounting] CR notes not carried forward
* [Accounting] Need to do a negative cash receipt
* [Accounting] Negative cash receipts
* [Schedule] MRP - Grouping Adds Extra Day
* [Accounting] Possible rounding errors when vouchering/processing
in multiple currencies different from base
* [Accounting] Able to save and 'post' a blank Cash Receip
* [Accounting] Deposit Registry does not total Base Balance
* [Accounting] Cash Receipts missing Base Amount column and
total
* [Accounting] Cannot load CSV credit card information to
custcreditcard view
* [Accounting] Cannot load CSV G/L Accounts from glaccount view
* [Accounting] Financial reports printing zeros by group headers
* [Accounting] Post Check generates "Check does not balance"
error message
* [Accounting] Fix Serial Columns screen Fix button produces
error
* [Accounting] Db error posting misc. check with debit memo
* [Accounting] Menu Item Tool-tips non-translatable
* [Accounting] API view glaccount incorrectly defaults profit_center
and sub_account to '1'
* [Batch Manager] creating an edi profile gives missing
ediprofile_emailhtml error
* [CRM] User is able to edit 'Use of Contacts' in Contact's
view mode
* [CRM] Special characters problem on incident workbench?
* [CRM] Tab order incorrect in Task Window
* [CRM] Can not double click opportunity
* [CRM] Contact not opening on double-click
* [CRM] Text > Integer issue
* [CRM] saveAddr() uses wrong comparison technique
* [CRM] tab order in ToDo item entry skips "owner" and "assigned
to"
* [Inventory] Detail Inv Hist by detail Date range do not
deactivate
* [Inventory] error message on delete site location is misleading
* [Inventory] Inventory UOM vs Vendor UOM on Receiving screen.
* [Inventory] Print Shipping Form screen -- Remove shipping
charges
* [Inventory] Multiple Issue Stock to Shipping cause Packing List
to report incorrect Qty Shipped
* [Inventory] Post Count Tag Difference can create multiple
entries for same location, same item
* [Inventory] Update ABC class generates DB log error
* [Inventory] Able to create blank Site type record
* [Inventory] Deleting Site type record generates DB log error
* [Inventory] Transfer Order does not expand list correctly
* [Manufacture] Return W/O Mat. Batch -- Commit executed
erroneously after error
* [Manufacture] Disassembly Work Orders Should not check Order
Parameters
* [Products] Copy BOO doesn't copy closewo flag
* [Products] Canceling to create a new item group member displays
mismatched message
* [Products] Delete does not refresh list in Class codes
* [Purchase] Purchaseorder api allows import of leading zeros
* [Purchase] Characteristics not printed on PO
* [Purchase] User is allowed to post comments while viewing
Purchase Order details
* [Purchase] Purchase Request by Planner Code does not expand
list correctly
* [Reports] Backlog by Customer mixing information
* [Reports] Financial Report Grade 0 errors
* [Reports] SO Picklist - Wrong Use of Line Function
* [Sales] Can not issue credit on credit card processor from
script
* [Sales] UPC does not show up on Item search scree
* [Sales] Credit Memo Item Search error when Item UPC Code checked
* [Sales] Update ship via on invoice and packing list when SO is
saved
* [Sales] Kits do not delete from SO
* [Sales] Negative customer discount was removed
* [Sales] Error importing to api.salesline
* [Sales] Update Prices does not update Characteristic Prices
* [Sales] Credit memo item lookup (ctrl-L) fails due to lack of
explicit type casts in PostgreSQL 8.3.X
* [Sales] Sales order contact information is missing from
api.salesorder
* [Sales] api.salesorder should allow for manually set number even
when numbering is set to automatic
* [Sales] SO and Invoice not honoring default UOM in pricing
* [Sales] SO Ship To Phone Number does not write to invchead table
* [Sales] RA Workbench: Print RA with selected customer type
generates DB log
* [Sales] Packing List Batch: Selecting 'x' button to add SO
generates DB log error
* [Sales] creditCard.cpp compiler warning
* [Sales] Customer Information Workbench does not check for
privilege
* [Sales] Quote for Prospect does not filter contact list to
selected CRM account
* [Sales] Newly created invoices are not displayed in Customer
Workbench
* [Sales] Summarized Sales By Customer By Item - Average Price
Calculation is Wrong
* [Sales] Sales History by Customer link to Invoice Information
does not work
* [Sales] Selecting disposition as 'Credit' and credit by as
'None' displays database error
* [System] Free floating windows don't close when application
closes
* [System] Images list unusuable over slow remote links
* [System] locale - timestamp format issue
* [System] Change parameterGroup and warehouseGroup to layout
and size naturally
* [System] Edit User cancel button does not wor
* [System] Add command line arguments for specifying Enhanced
Auth and SSL boolean
* [System] schedule server backup or server maintenance with
time but no date gives sql error
* [System] empty default credit limit causes an error importing
sales order xml
* [System] replace OpenMFG with Manufacturing
* [System] add include facility to scripting
* [System] User is allowed to add/revoke privileges to a group
in view mode
* [System] Exchange Rates: Overlapping of date ranges generates
DB log error
* [System] api.creditmemo - cust_number Not Defaulting Bill-To
Info
* [System] Qt designer (external) gives driver errors when
opening
