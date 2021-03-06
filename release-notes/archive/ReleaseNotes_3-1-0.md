Release Notes
xTuple ERP
OpenMFG/Standard Edition/PostBooks
Version 3.1.0
October 8, 2008
----------------------------------

This is the Final Release of version 3.1.0. Thanks to all who
have provided valuable feedback and also financial sponsorship
during this entire release cycle.

PLEASE NOTE: The Help Files have been updated to coincide with
the final release.

----------------------------------

The following features and bug fixes have been added to the
application since the RC release. Additional detail for each
item listed below may be found on our community website
(www.xtuple.org). Simply go to the Issue Tracker and select the
Changelog option.


New Features:

* [All] Updated code to make several functions usable by
scripting

Bug Fixes:

* [Accounting] Fixed issue with incorrect qty. during Lot/Location
distribution
* [Accounting] Added error checking to identify internal 
inconsistencies in Invoice Tax information
* [Accounting] Fixed inter Warehouse transfer function to handle
average costed Items correctly
* [Accounting] Fixed issue where in some cases the Tax option was
incorrectly being set to �None� on the Invoice Item screen
* [Accounting] Fixed issue leading to error when inserting into
api.glaccount
* [Accounting] Fixed PostBooks issue where columns were not
aligned correctly in financial trend reports
* [Accounting] Improved error messaging when user attempts to
post an unbalanced G/L series
* [Accounting] Made sure year columns appear correctly when
printing Income Statement annual trend reports
* [CRM] Improved search functionality when selecting Contacts in
CRM and elsewhere
* [CRM] Fixed column sorting inconsistencies in CRM Account,
Contact, and Address search and list screens
* [CRM] Ensured that CRM Account is automatically populated when
a Contact is selected on the New Incident screen
* [Inventory] Fixed issue with Inventory distribution screen not
properly recognizing expiration dates
* [Inventory] Fixed issue where reassignment of Lot/Serial qty.
create duplicate Lot numbers for Lot-controlled Items
* [Inventory] Fixed issue preventing creation of new Average
Costed Item Sites when QOH = 0
* [Inventory] Added extra check to disable manual cost when
reducing Inventory for Average costed Items
* [Inventory] Fixed issue preventing selection of G/L Accounts
if no Company segment in use
* [Inventory] Fixed issue with Lot/Serial Transfer Order
shipments appear as not posted in Inventory history
* [Inventory] Fixed issue preventing creation of new Sites if
no Address defined
* [Inventory] Fixed issue leading to errors when attempting to
ship Transfer Orders having manually-entered TO numbers
* [Manufacture] Fixed Work Order History report so data prints
correctly
* [Products] Fixed issue with Item Cost Summary screen not
displaying information
* [Sales] Fixed issue leading to error when selecting Tax link
on Return Authorization screen
* [Sales] Fixed issue with Contact information not saving
properly when adding a new Customer
* [System] Fixed issue with update script which was leading to
errors

----------------------------------

This is the Release Candidate for version 3.1.0. It is primarily
a bug fix release. Thanks to all in the community who have been
providing valuable feedback during this entire release cycle.
----------------------------------

The following features and bug fixes have been added to the
application since the Beta2 release. Additional detail for each
item listed below may be found on our community website
(www.xtuple.org). Simply go to the Issue Tracker and select the
Changelog option.


New Features:

* [CRM] Added jump link to email and web browser for Contact
email address and web address
* [Inventory] Created API views for Miscellaneous Count Tags
* [Purchase] Added "Search for" functionality to Item Source
list
* [System] Rounded out Package Manager functionality


Bug Fixes:

* [All] Prevented users from creating empty CRM master
information records
* [All] Fixed issue where itemsite_freeze column in database
API view "api.itemsite" was not being set properly
* [Accounting] Fixed issues with column headings for trend
versions some financial reports not displaying properly
* [Accounting] Fixed issue where Standard Journal items were
getting deleted on save
* [Accounting] Allowed external company credentials to be
editable
* [Accounting] Added check to make sure Invoices have line
items before they can be saved
* [Accounting] Modified the currency conversion effective
date so AR Aging recognizes exchange rates properly
* [Accounting] Enforced saving of more header information on
Cash Receipt
* [Accounting] Reformatted A/R Workbench layout
* [Accounting] Prevented creation of empty Standard Journals
* [Accounting] Enforced selection of Bank Account on Post
Checks screen
* [Accounting] Fixed issue preventing editing of GL Accounts
* [Accounting] Fixed Print Invoice windows so numbers appear
in correct sequence
* [Accounting] Changed Invoice to pass the Invoice date to
the Invoice Item for calculating the Exchange Rate
* [CRM] Improved Contact search in CRM Incident window to
filter properly
* [CRM] Fixed issue leading to error when unchecking the
"Show Types" option in the Order Activity by Project screen
* [CRM] Widened Contact information fields on Mac
* [CRM] Reformatted layout of To-Do list item screen
* [Inventory] Fixed issue where global unit of measure ratio
changes were not being propagated correctly
* [Inventory] Fixed issue where sufficient quantity on Issue
to Shipping screen was checing Inventory qty to S/O line
balance, not issue amount
* [Inventory] Enforced requirement that CRM Account have
primary Contact before issuing qty. from Item Site having
auto-registration specified
* [Inventory] Cleaned up Issue to Shipping screen
* [Inventory] Enforced closing of Transfer Orders when qty.
is shipped/received complete
* [Inventory] Added costing information to Expired Inventory
report
* [Inventory] Prevented shipping orders if no stock has been
issued to shipping
* [Inventory] Fixed issue leading to error when closing
receipts
* [Inventory] Fixed issue preventing cancellation of
Inventory receipts
* [Inventory] Updated  itemtaxtype api view to accept
inserts/updates when taxauth is "Any"
* [Inventory] Made Lot/Serial # field larger on the Create
Lot/Serial screen
* [Inventory] Changed default control method for new Item
Sites to be "Regular"
* [Inventory] Fixed issue preventing reassignment of
non-perishable Lot qty.
* [Inventory] Reformatted layout for Receipt Item screen
* [Inventory] Fixed problems with QOH handling in Transfer
Order processing
* [Manufacture] Fixed issue where firming a Planned Order
changed the Order type
* [Manufacture] Fixed issue leading to error when
over-posting production
* [Manufacture] Added Check in copy Item process to issue a
warning when the Item Type is changed to Kit and a BOM Item
(on the active Rev) is not marked as Sold
* [Manufacture] Fixed issue on BOO Item screen where run and
setup times were not being displayed correctly
* [Manufacture] Fixed issue preventing the copying of BOMs
for Outside Process Items
* [Products] Reformatted BOO Item screens
* [Products] Removed BOO button from Item master screen in
PostBooks
* [Products] Fixed issue leading to SQL error on Costed
Indented BOM screen
* [Products] Removed invalid line # for this-level costs
in Costed Single Level BOM screen
* [Products] Fixed MOVE UP/MOVE DOWN buttons on BOO screen
so they operate correctly
* [Purchase] Prevented PO maintenance without the privilege
* [Purchase] Prevented over-distribution to single costing
element on Voucher item screen
* [Sales] Reformatted Select Order for Billing screen
* [Sales] Fixed issue leading to error when selecting to
create a new Ship-to Address
* [Sales] Fixed issue where user was asked unnecessarily to
re-enter a Lot/Serial # on the RA screen
* [Sales] Fixed issue leading to error when purging Invoices
* [Sales] Updated Invoice report to include Tracking # for
all shipments where appropriate
* [Sales] Fixed Customer Workbench to display Cash Receipt
dates properly
* [Sales] Removed PO requirement on Quote for Customers
because this is premature
* [Sales] Fixed issue leading to error when selecting
"Show W/O" option on Inventory Availability by Customer Type
screen
* [Schedule] Reformatted Work Center screen
* [System] Cleaned up CRM privileges for clarity
* [System] Added Exchange Rate report definition to database
* [System] Fixed issue where selecting CANCEL created a new
group in Maintain Groups screen
* [System] Fixed issue where TO generation configuration
incremented in wrong direction

----------------------------------
Release Notes
xTuple ERP
OpenMFG/Standard Edition/PostBooks
Version 3.1.0Beta2
August 28, 2008
----------------------------------

This is the second Beta release of version 3.1.0. Thanks to all our
beta testers who have been sending us valuable feedback! Please keep
up your efforts.

NOTE: For users migrating their databases forward to 3.1.0Beta2, a
new version of the Updater tool is required to complete this upgrade
successfully. All users migrating to 3.1.0Beta2 should download and
use updater2.0.0beta2.

----------------------------------
The following features and bug fixes have been added to the applications
since the release of the first Beta. Additional detail for each item
listed below may be found on our community website (www.xtuple.org).
Simply go to the Issue Tracker and select the Changelog option.


New Features:

* [A/P] Made AP checks print in alphabetical order
* [A/R] Added link to Invoice Detail in A/R Open Items and A/R Open Items
by Customer
* [A/R] Changed A/R Workbench menu options to be consistent with A/R Open
Items screen
* [Accounting] Cleaned up layout on A/R Open and A/P Open windows
* [Accounting] Cleaned up layout on Cash Receipt Window
* [Accounting] Cleaned up Credit Memo window
* [Accounting] Made Misc. Voucher Window the same as standard Voucher
window
* [Accounting] Added ability to void AP Credit Memos; also, prevented
users from using voided Credit Memos
* [Accounting] Added regular expression support to Check # field on Check
Register
* [Inventory] Cleaned up Transfer Order window
* [Inventory] Added Warehouse Code to Order select widget and Enter
Receipts screen
* [P/D] Added colors to BOM
* [Products] Added "Only show Items where Actual and Standard Costs are
different" to Item Cost by Class Code display
* [Sales] Added Customer Name to List Pricing Schedule Assignments
* [System] Added the ability to store and run metaSQL queries from the
database
* [System] Created Screen Control widget that allows for "codeless"
screens to be created


Bug Fixes:

*  [All] Fixed issue with screens redrawing too slowly
* [All] Fixed search functionality to work in Order cluster
* [All] Fixed problems with api.bomitem view
* [A/P] Prevented deletion of Expense Categories in use
* [A/P] Made formatting functions consistent between database and
application
* [A/P] Fixed issue leading to empty Tax Authority drop down list
* [A/P] Fixed issue leading to error when selecting Vendor Type in
Aging
* [A/P] Improved currency logic to use the selected Bank Account to
determine the open A/P items to be listed and selected on Select Payments
screen
* [A/P] Fixed issue preventing correct receiving of inventory Items
* [A/P] Fixed issue leading to error when selecting to cancel creation
of Misc Credit/Debit Memos
* [A/P] Fixed issue where "error" was displaying as document when
selecting to print an Invoice against which a Cash Deposit was applied
* [A/R] Modified A/R Aging printed report comment to read "base amounts
calculated from document date"
 * [A/R] Changed the araging function so now 1) the aropen_amount is
normalized to base Currency using the aropen_docdate and 2) since
aropen_paid was not being normalized, changed it to use aropen_curr_id
and aropen_docdate
* [A/R] Fixed Customer Info Workbench to associate document types
correctly under the A/R History tab
* [A/R] Updated Invoice report to show Cash Receipts received as
payments
* [G/L] Prevented duplicate Sub Account numbers
* [G/L] Prevented duplicate Profit Center Numbers
* [G/L] Enabled multi-currency amounts in GL Series Item
* [Accounting] Fixed error resulting when selecting to enter an
invalid date in Fiscal Year displays
* [Accounting] Prevented users from re-reconciling dates when doing
Bank Reconciliations
* [Accounting] Fixed missing Vendor Number validation on Misc. Check
screen
* [Accounting] Changed A/R Workbench to 1) convert A/R Open Items to
metaSQL and fix any currency conversion problems and 2) change total
Open Items to display total in base Currency for consistency
* [Accounting] Fixed Check Run screen to disable POST CHECK button
after posting a Check
* [Accounting] Added checks for duplicates before saving a Company
segment value
* [Accounting] Fixed cast type error when reprinting Invoices in
PostBooks
* [Accounting] Enforced conversion to base Currency for multi-currency
Debit Memos
* [Accounting] Added Currency symbol to A/R Open Item and A/R
Applications screens
* [Accounting] Enforced dates to be recognized when re-querying AR
Applications screen
* [Accounting] Added check to ensure that at least one period is
selected before generating the Budget table
* [Accounting] Fixed issue leading to error when selecting to create
a Standard Journal
* [Accounting] Added terms due date checks to Misc AP and AR Credit
Memos
* [CRM] Fixed issue preventing the parent window of the CRM Account
screen from closing when CRM Account screen is closed/saved
* [CRM] Removed blank column in Incidents by CRM Account screen
* [CRM] Fixed tab order in Incident screen
* [CRM] Allowed newly-created Customer records to be merged with
existing CRM Accounts; but this is not possible for already-existing
Customer records
* [CRM] Prevented improper incrementing of Incident Numbers
* [CRM] Fixed issue preventing creation of new Incidents
* [CRM] Fixed issue preventing creation of Master Information for
Incidents
* [I/M] Disabled Misc. Adjustment for Breeder Items
* [I/M] Changed function postTransformTrans to delete empty itemloc
records
* [S/R] Added Vendor name to search list at PO Receipt
* [Inventory] Allowed shipping an RA order without requiring the
privilege for maintaining RAs
* [Inventory] Fixed issue leading to error when searching for and
Order at receiving
* [Inventory] Fixed issue preventing users from adding line items
to Transfer Orders when Order number generation is manual
* [Inventory] Fixed query that determines if warranty date is
required
* [Inventory] Fixed issue leading to error when receiving RAs with
only receiving privileges
* [Inventory] Fixed issue leading to error when reassigning
Lot/Serial qty.
* [Inventory] Added posted value option to Expired Inventory report
* [Inventory] Fixed Packing List Batch to print with data and without
error
* [Inventory] Fixed issue where error was received when selecting
Warehouse on Transfer Order screen if number generation method was
configured to be manual
* [Inventory] Fixed issue leading to errors when receiving
non-Inventory items against POs
* [Inventory] Fixed issue leading to error when printing labels by
Invoice
* [Inventory] Fixed issue leading to error when running Summarized
Transaction History
* [W/O] Added regular expression support  to W/O History by W/O
screen
* [W/O] Fixed issue preventing setup time flag from clearing when
posting Operations corrections
* [Manufacture] Fixed issue leading to error when printing BOO
* [Manufacture] Fixed issue leading to error when printing Labor
Variance by BOO items screen
* [Manufacture] Updated Lot/Serial assignment screen to display "N/A"
instead of 01/01/1970 if the Item does not expire or has no waranty
* [Products] Fixed issue preventing creation of aliases for
newly-created Items
* [Products] Changed the indented, sequenced, single, and summarized
BOM reports to disable Revision widget until a valid Item is entered
* [Products] Changed Item look up list to use terms "Make" and "Buy"
* [Products] Changed BOO List to work the same as BOM List�namely,
DELETE button is enabled/disabled based on revision control
* [Products] Fixed screen sizing problem on Operations By Work
Center screen
* [Products] Fixed problem where Kit Item Type not enabled unless
Breeder BOMs enabled
* [Products] Fixed BOO so revision date and location are saved
correctly
* [Products] Fixed issue leading to error when selecting a UOM on
the Item master
* [Products] Fixed issue preventing deletion of BOMS for Outside
Process Items
* [Products] Fixed issue leading to error when printing Kit Item
masters
* [Products] Fixed issue preventing addition of Tax Types to new
Items
* [Products] Renamed screen title to correctly specify Registration
Characteristics
* [Products] Disabled Item Lot/Serial information on Registration
screen
* [Products] Strengthened links between CRM, SO, and Shipment to
improve validation of information
* [Products] Fixed Registration screen to not request re-entry of
already known Lot/Serial number
* [P/O] Prevented creation of duplicate Vendor Types
* [P/O] Fixed inconsistent exchange rate information displays on
Item Source screen
* [Purchase] Tightened relationship between Locales and date
formats in the application
* [Purchase] Fixed unnecessary incrementing of P/R# if planned P/O
release is canceled
* [Purchase] Fixed issue leading to error when creating a Purchase
Order if the PO number generation method is manual
* [Reports] Removed depreciated item_invuom field from reports
* [Reports] Changed backlog, bookings, and sales history reports to
normalize prices to base Currency using the Currency Exchange Rate
effective on either the order date (backlog and bookings) or the
invoice date (sales history)
* [S/O] Prevented duplicate Customer Form Assignments
* [S/O] Removed Item joins in selectUninvoicedShipments
* [S/O] Fixed issue leading to conflicts from overlapping SO/Quote
numbers
* [S/O] Changed sequence of populate so that Sale Price is populated
before Net Unit Price and Discount % from Sale calculation
* [S/O] Made sure Characteristics are reset properly when clearing
for new line items on Sales Order
* [Sales] Removed unnecessary request to save Sales Order line items
when no details have been changed
* [Sales] Fixed PackingList-Shipment report to work with Kit Items
* [Sales] Fixed Item list screen to include Kit Items
* [Sales] Fixed wrong usage of function for coitem line numbers in
the PickingListSOLocsNoClosedLines.xml report
* [Sales] Added edit to require at least one line item before you can
save an RA
* [Sales] Added hard edit to disallow receiving more than RA
authorized
* [Sales] Added 2 edits for Credit Memo numbers: 1) cannot be blank
and 2) cannot already be in use
* [Sales] Prevented users from overriding prices on Sales Orders if
they don't have the  privilege
* [Sales] Changed Sales Order and Sales Order Item to disable all
widgets when in View mode to preclude unnecessary "Save" message
* [Sales] Fixed issue leading to error when printing Billing Edit
list
* [Sales] Allowed assignment to future Pricing Schedule Assignments;
however, expired schedules are not allowed
* [Sales] Fixed issue preventing creation of RA
* [Sales] Fixed margin calculation on Quote screen to handle multiple
Currencies correctly
* [Sales] Fixed issue preventing editing of Sales Order line items
* [Sales] Fixed overly detailed price precision on Summarized Backlog
by Warehouse screen
* [Sales] Fixed issue leading to error when printing Sales Order form
* [Sales] Removed the duplicate unique constraint on the ipsitem table
* [Sales] Improved multi-currency support in Sales Analysis reports
* [M/S] Prevented duplicate Warehouse Calendar Exceptions
* [M/S] Fixed issue leading to error when changing qty. at Firm
Planned Order
* [Schedule] Prevented Planned Orders for inactive Items
* [System] Required username and password on User Information screen
* [System] Fixed problem with tool bar positions not being remembered
properly
* [System] Fixed issue leading to error when canceling a Quote if
number-generation method is set to manual
* [System] Enforced use of default values for Event fence days


----------------------------------
Release Notes
xTuple ERP
OpenMFG/Standard Edition/PostBooks
Version 3.1.0Beta
August 08, 2008 (i.e., 08/08/08)
----------------------------------

This is the Beta release of version 3.1.0. Thanks to all in the
community who contributed valuable patches and feedback during the
Alpha cycle! Please keep up the effort on this Beta. We are eager
to hear from as many of you as possible.

In addition to the functionality highlighted for special testing
in the 3.1.0Alpha Release Notes, we are also interested in feedback
on the following feature which appears for the first time in this
Beta release:

Kit Item Type
  * Full spec: http://wiki.xtuple.org/SalesOrderKitting

Once again, here are the areas of new functionality we added for
the Alpha release. If you have not tested these new features
yet, please do so and send us any feedback you have:

Multi-Company Financial Consolidation
  * Full spec: http://wiki.xtuple.org/MultiCompanyConsolidation

Average Costing
  * Full spec: http://wiki.xtuple.org/AverageCosting

Package Manager
  * Full spec: http://wiki.xtuple.org/PackageManager
  * NOTE: Must use the 2.0.0Beta updater, not the old 1.0/1.1 updater

Sales Order Reservations by Location
  * Full spec: http://wiki.xtuple.org/SalesReservationsByLocation

Purchase of Manufactured Items
  * Manufactured Items may now be purchased


----------------------------------
The following features and bug fixes have been added to the applications
since the release of version 3.0.1Alpha. Additional detail for each item
listed below may be found on our community website (www.xtuple.org).
Simply go to the Issue Tracker and select the Changelog option.


New Features:

* [Accounting] Created API view for Incident
* [Purchase] Created API view for Vendor
* [Sales] Create Kit Item Type
* [System] Added support for Site (i.e, Warehouse) level security


Bug Fixes:

* [A/P] Fixed issue with Document Numbers not displaying in the Billing
Selections screen
* [A/P] Fixed error received when vouchering a PO having a Return
* [A/P] Renamed columns in Expense Categories selection window to have
correct values
* [A/P] Fixed issue with Check Numbers not incrementing correctly when
creating new miscellaneous Checks
* [A/P] Added drill-down detail in G/L Transaction screen for
miscellaneous distributions entered on Vouchers
* [A/R] Added $0 invoices to Customer History screen
* [Accounting] Enabled billing Terms to remain with Document records
even after Terms themselves are disabled at master information level
* [Accounting] Removed text box displaying Check Number on Prepare Check
Run screen because it enabled duplicate Check Numbers and was unnecessary
* [Accounting] Enabled entry of negative miscellaneous distributions on
Cash Receipt screen
* [Accounting] Fixed screen resizing problem on Check Register screen
* [Accounting] Fixed issue preventing issuance of Credit Memos for P/O
Returns
* [CRM] Fixed issue where CRM Addresses were not being handled correctly
if shared by more than one CRM Account Contact
* [CRM] Enabled Customer to be merged with existing CRM Account
* [CRM] Fixed CRM Account fill list so pre-existing CRM Account Numbers
are recognized better
* [I/M] Disabled DISTRIBUTE button on inventory distribution screen
unless a line item is selected for distribution first
* [S/R] Fixed issue where $ value was not saved when editing RMA Line
Items
* [Inventory] Fixed issue leading to error when printing Packing List
from Summarized Backlog screen
* [Inventory] Fixed error received when reassigning Lot/Serial quantity
* [Inventory] Fixed screen resizing issue on Slow Moving Inventory By
Class Code screen
* [Inventory] Fixed screen resizing issue on Substitute Availability By
Item screen
* [Inventory] Moved data which was displaying in wrong columns on Enter
PO Receipt screen
* [Inventory] Fixed issue with Unbalanced QOH utility not working
properly
* [Inventory] Changed Packing List print screen to accept SO and TO in
same widget
* [Inventory] Fixed issue preventing reassignment of Lot/Serial qty. for
Item Site changed from regular control method to Lot control method
* [Inventory] Added timestamp for relocate Inventory transactions
* [Inventory] Added timestamp for Site Transfer transactions
* [Inventory] Fixed issue leading to error when posting Count Tags
* [Inventory] Updated Item Site to show "None" as disabled control method
for Reference and Job Item Types
* [Inventory] Changed External Shipping maintenance screen to look, feel,
and work like other screens
* [Inventory] Allowed Location to be selected from list when default is
checked and MLC is not on Item Site screen
* [Inventory] Fixed ability to view document number for Inventory
transfers in Inventory history screens
* [Inventory] Fixed combo boxes so data available for selection on Transit
Site masters
* [Manufacture] Fixed issue where some materials were not being issued to
Work Orders
* [Manufacture] Fixed issue leading to error when correcting Operations
posting
* [Manufacture] Fixed issue causing qty. values not to be updated
correctly when posting Operations corrections
* [Products] Fixed PRINT button on View Costing Detail screen
* [Products] Fixed screen resizing issue on Standard Operations By Work
Center screen
* [Products] Fixed multiple Product reports which were printing with no
data
* [Products] Updated SO Item screen to update Price UOM whenever Qty.
UOM is changed
* [Purchase] Fixed issue leading to error when adding Item Source Price
for "make" Items
* [Purchase] Fixed misnamed column header in PO Item displays
* [Purchase] Updated Voucher due date calculation for proximo terms to
be based on Invoice Date instead of system date
* [Sales] Updated Billing Selections screen to perform subtotaling using
correct input values
* [Sales] Fixed issue leading to error when selecting "X" button in the
empty Sales Order screen
* [Sales] Included Misc. Invoice items in tax calculation on Summarized
Taxable Sales report
* [Sales] Fixed issue leading to error when selecting to create a Quote
using a Prospect as a Customer
* [Sales] Fixed issue preventing display and saving of Characteristics on
Quote Item screen
* [Sales] Fixed RMA numbers to increment correctly
* [Sales] Fixed screen resizing problem on Customer Information Workbench
* [System] Moved several security privileges from Sales Module to
Accounting Module, including MaintainTerms, PostARDocuments, and
PrintInvoices
* [System] Standardized all stock reports to use only Arial or Helvetica
fonts
* [System] Removed duplicate EnableBatchManager values in PostBooks
metric table


----------------------------------
Release Notes
xTuple ERP
OpenMFG/Standard Edition/PostBooks
Version 3.1.0Alpha
July 25, 2008
----------------------------------

This is the Alpha release of version 3.1.0. We are especially eager
to hear feedback from alpha testers on the following new areas of
functionality:

Multi-Company Financial Consolidation
  * Full spec: http://wiki.xtuple.org/MultiCompanyConsolidation

Average Costing
  * Full spec: http://wiki.xtuple.org/AverageCosting

Package Manager
  * Full spec: http://wiki.xtuple.org/PackageManager

Sales Order Reservations by Location
  * Full spec: http://wiki.xtuple.org/SalesReservationsByLocation

Purchase of Manufactured Items
  * Manufactured Items may now be purchased

Warehouse Changed to "Site"
  * Makes solution more accessible for retailers and other types of
    businesses
  * Use new "Site Types" to define Sites as Store, Warehouse, etc.

----------------------------------

The following features and bug fixes have been added to the applications
since the release of version 3.0.1. Additional detail for each item
listed below may be found on our community website (www.xtuple.org).
Simply go to the Issue Tracker and select the Changelog option.


New Features:

* [All] Disallow users from using wrong GUI version on database
* [All] Database API View "api.itemsite" and itemsite_freeze column
* [Accounting] Spell out A/E/L/Q/R and show sub-type in COA display
* [Accounting] Display Sub-Acct Code & Sub-Acct Code Description in
display of ACCOUNTING - ACCOUNT - CHRT ACCTS
* [Accounting] Add additional parameters to the Check Register
* [Accounting] Add ability to have the default billing date the
current date
* [Accounting] Create API view for Cash Receipt
* [Accounting] Create an API view for Incident
* [Accounting] Print Credit Card Receipts
* [Accounting] Multi-Database Financial Report Engine Consolidation
* [A/R] POST button needed on Cash Receipt
* [CRM] Add button/link from right click on To-Do list to customer
workbench (if applicable)
* [CRM] The system shall allow revenue to be reconciled, and
disputed
* [CRM] Add middle initial and suffix to contact
* [Inventory] Allow sales reservations to be made at the location
level
* [Inventory] Add average costing as a cost method
* [Inventory] Create API view for Site (Warehouse)
* [Products] Transformations between Manufactured Type Item and
Job Type Item
* [Purchase] Permit Purchase of Manufactured Items
* [Sales] Add information about To-Do data to customer workbench
* [Sales] Add Customer Type API view
* [Sales] Add the ability to print a customer statement from the
Customer Information Workbench
* [Sales] Add columns to Summarized Backlog
* [Sales] Create API view for Sales History
* [Schedule] Allow planned work orders to be changed to planned
purchase orders and vice versa
* [System] Change "Warehouse" nomenclature to "Site"
* [System] Allow access to Hotkeys independent of preferences
* [System] Event Created When Database Log Generated

Bug Fixes:

* [All] api.itemsrc and api.itemscrp View Rules Attached
* [Accounting] Changing the company code does not change chart of
accounts
* [Accounting] List views center align "Category" column. Should
be Left Justified
* [Accounting] Funds Type no longer includes credit card in Cash
Receipts
* [Accounting] Can't edit Misc Checks after creation
* [A/R] Customer History incomplete
* [A/R] Araging function is miscalculating the formatted current
amount
* [G/L] Duplicate Company Numbers are Possible
* [Inventory] Serial number quantities show total for the location
when distributing
* [Inventory] 8.3 typecast error
* [Inventory] Serialized items can not receive qty greater than 2
at a time
* [Inventory] Job and reference items allowed in Inv Trans lookups
* [Inventory] Update Lead Time functionality doesn't work
* [Inventory] Document number does not show up in inventory
transaction screen
* [Inventory] Cannot distribute qtys from MLC warehouse
* [Inventory] Lot/Serial info not displaying in Inventory History
* [Inventory] Items may only be purchased or manufactured or
Breeder
* [Inventory] Upgrade Script Does Not Set itemloc_ls_id
* [Inventory] Lot/Serial info not displaying in multiple inventory
screens
* [I/M] TW trans allowed for NONE Item Site
* [Manufacture] Disassembly production entries w/ immediate
transfer to warehouse
* [Manufacture] Work Order Explosion does do UOM conversion for
child work orders
* [Products] Selecting to view inventory History displays an
irrelevant date selection dialog
* [Products] When creating a lot/serial registration, SQL error
returned if no account selected
* [P/O] "Average Cost" Posting when Vouchering
* [Sales] Selecting to convert multiple quotes causes the
application to crash
* [Sales] On deleting RA's from the list gives an SQL error
* [Sales] Creating Sales Orders with API view slow on a large
database
* [S/O] Duplicate Shipform names may be entered
* [S/O] Credit Card - Delete Charged SO - No Warning or Credit
* [System] Use QTextBrowser object to define e-mail text body
* [System] Std. Edition gives error boohead error
* [System] Duplicate Characteristics may be entered
* [System] Duplicate Comment Types may be entered.
* [System] Hard Code "mfgadmin" As the Logon User in Updater
* [System] Duplicate users by using New Employee function
* [System] User details not saved while defining employee as User
