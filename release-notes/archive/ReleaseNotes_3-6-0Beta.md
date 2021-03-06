Release Notes
xTuple ERP
PostBooks, Standard, and Manufacturing Editions
Version 3.6.0Beta
September 20, 2010
----------------------------------

This is the beta release of version 3.6.0.

----------------------------------

The following features and bug fixes have been added to the
applications since the release of 3.5.4. Additional detail for
each item listed below may be found on our community website
(www.xtuple.org). Simply go to the Issue Tracker and select the
"Changelog" option.


New Features:

* [Accounting] Add ability to record Purchase Price Variance
upon Receipt
* [Accounting] Provide the ability to "delete" g/l transaction
* [Accounting] Allow users to edit posted Journal Entries
* [Accounting] Warning message when adding wrong "type" account
to account assignment
* [Accounting] Add Sub Ledger to Accounting
* [Accounting] Add the ability for Credit Memos to be applied
to Cash Receipts
* [Architectural] Consolidate Setup screens
* [Architectural] Convert "display" queries to MetaSQL stored
in the database
* [Architectural] Sub class Work Order Cluster to Virtual
Cluster
* [Architectural] Sub class Vendor Cluster to Virtual Cluster
* [Architectural] Remove Transfer Order Cluster
* [Architectural] Remove Sales Order Cluster
* [Architectural] Sub class Planned Order Cluster to Virtual
Cluste
* [Architectural] Sub class G/L Cluster to Virtual Cluster
* [Architectural] Sub class Customer Cluster to Virtual Cluster
* [Architectural] Remove Purchase Order Cluster
* [Architectural] Create a user preference to set lists to
alternating colors
* [Architectural] Remove user preference to show clusters as
buttons
* [Architectural] Expand subclassing of virtualcluster and
virtualclusterlineedit
* [CRM] Add parameter widget to Search Accounts screen
* [CRM] Add Parameter Widget to Search Contacts scree
* [CRM] Add Parameter Widget to Opportunity workbench
* [Inventory] Break information on Shipping Information screen
into tabs
* [Reports] Print Preview
* [Sales] Add an option to not delete Quotes when they are
converted to Sales Orders
* [Sales] Customer workbench--visual indication to show
customers on credit hold or warn

Bug Fixes:

* [Accounting] Sub class Ship-To Cluster to Virtual Cluster
* [Accounting] List unposted invoices too slow to be useful
with large volumes of line items
* [Accounting] Inactive Sales Category ignored on invoice
item screen
* [Accounting] Print report of Bank Accounts display irrelevant
type field for Credit Card
* [Accounting] Cannot view voucher qty. history
* [Accounting] Can not save external company records
* [Accounting] Start date on tax registration window cannot be
changed by typing
* [Accounting] Reference field is not populated in GL when you
back flush operations
* [Accounting] Revert Customer deposit creates a Debit Memo
that can't be applied
* [Accounting] Multi-select posting on cash receipts results
in error
* [Accounting] Hide Check/uncheck show running total on
general ledger transactions display
* [Accounting] Desktop, Reload button for G/L accounts doesn't
seem active
* [Accounting] In Desktop, certain accounts show as negative
balances
* [Accounting] In Desktop, GL Monitored Account balances are
incorrect
* [All] Item description text is cut off
* [All] API view of itemsite record does not expose all required
fields for CSVImport
* [CRM] Double-clicking radio button turns all radio buttons
off and shows credit card xtreewidget
* [CRM] Can't save project
* [Reports] Preview of landscape oriented reports doesn't work
correctly
* [CRM] A new Project doesn't get saved with first Save click
* [CRM] Unable to save comments upon creating a new address
* [CRM] �Owner� field on CRM Account form doesn't filter on
active users
* [CRM] Right Click Menu Options not coded correctly
* [CRM] Incident workbench not refreshing
* [CRM] View mode of an incident enables the user to edit/delete
characteristics
* [Inventory] Document number do not show on Inventory history
displays on Site transfer
* [Inventory] Inventory history by order number screen doesn't
show all types of orders
* [Inventory] Omnibus: Maintain Shipping Contents screen
* [Inventory] Create P/R doesn't populate Purchase Request
number
* [Inventory] Error on tax breakdown window
* [Inventory] �Buffer Status as of� field in print report of
Inventory Status by planner code is blank
* [Inventory] QOH of negative magnitude is not added to total
QOH in print report of QOH by class code
* [Manufacture] Error after deleting work center on post
operations
* [Manufacture] Purchase Requests are not created for manually
entered materials
* [Manufacture] Totals on Production Time Clock report
* [Manufacture] WO Material Start Date for Manufacturing
Edition
* [Manufacture] Run Remaining on WO Edi
* [Manufacture] WO Material Requirements screen does not
consider qty. required as fractional
* [Manufacture] System allows to Edit Work Order without
MaintainWorkOrders privilege
* [Manufacture] Entering the details and selecting �Disassembly�
doesn't create a disassembly w/o
* [Manufacture] Post Operations screen doesn't populate Setup
Performed By and Run Performed By username
* [Manufacture] Back-flushing for items w/o item sites
* [Manufacture] Operations button missing in item screen when
type is breeder
* [Manufacture] Work Order screen has grammatical errors in
some error messages
* [Manufacture] Inventory Availability by WO Report doesn't
display the filter headers in consistent with the selected filters
* [Products] Typo in item changelog comments
* [Products] When copying an item, get QT Script Debugger
exception
* [Products] Report definition "inventoryhistorybyitem" cannot
be found
* [Products] System allows to delete item without
DeleteItemMaster priviledg
* [Products] Script debugger catches exception in xtmfg package
* [Products] Using the single quote in characteristics fields
causes an error
* [Products] Empty item number for BOO item
* [Products] Error on importing revisions into xtmfg.api_boo
* [Products] xtmfg.api_booitem does not populate boo_revision
* [Purchase] P/O Items by Screens showing Inv UOM for Qty ordered
by Vendor UOM
* [Purchase] Able to select a new PO for a voucher that already
has distributions against a different PO
* [Purchase] Tax authority isn't displaying within vendor master
record
* [Purchase] Report of Purchase Order Receipts and Returns by
Vendor for Expense items does not print
* [Reports] PickingListSOLocsNoClosedLines - References to
std/mfg only functions in PostBooks causes db Errors
* [Reports] QOH report does not clear from previous query if new
class has no items assigned
* [Sales] Irrelevant labels are displayed on Select Order for
Billing Screen
* [Sales] Selecting to print from the �Print Invoices by Ship Via�
window displays irrelevant dialog
* [Sales] Time phased sales history by customer by item is really
Time phased sales history by customer
* [Sales] Selecting to delete a sales order for kit item displays
error dialog
* [Sales] quitem_id may overlap with soitem_id causing
non-meaningful error message on quote
* [Sales] Price list report does not exclude inactive items
* [Sales] Toggling in and out of edit mode clears the customer
window
* [Sales] Able to create pricing schedule with expires date prior
to effective date
* [Sales] Loss of functionality within return authorization line
item screen
* [Sales] Db error using apply-to on sales credit memo
* [Sales] Comments on Quotes should be preserved when converted
to a Sales Orde
* [Sales] Return Authorization of Kit item does not close properly
* [Sales] Incident Name and description columns show wrong values
on Customer WB
* [Sales] Status column on CRM tab of Customer WB show id letter
and not name
* [Schedule] Time Phased Capacity Load Display not working as
before
* [Schedule] Time Phased Available Capacity Display not working as
before
* [Schedule] �View Parent Sales Order Information� screen doesn't
display details of sales order
* [Schedule] MPS Production Plans have Jumpy-Modal-Window behavior
on Mac
* [Schedule] MRP Creates WO requirement for TO
* [Schedule] Print report of Time Phased Load by Work Center
doesn't display Tooling items
* [Schedule] Planned Revenue/Expenses Report doesn't display the
filter headers in consistent with the selected filters
* [Schedule] Time Phased Rough Cut Capacity Plan by Work Center
Tooling inconsistency
* [Schedule] Tooling items are not displayed in Capacity Buffer
Status screen
* [System] simple license manager
* [System] Default Tax Authority obsolete
* [System] typo on preference screen under the menu tab
* [System] db error when user prints credit memos without the
MaintainCreditMemos priv.
* [System] [Observation]: User is allowed to delete employee
group associated to an employee
* [System] Using international characters on screen designer
label crash client
* [System] grade ignored in duplicate check when changing group
or name of a metasql statement
* [System] date range filter problem
* [System] Editing user preferences
* [System] Quote �Automatic Use S/O#� number generation is not
functional
* [Translation] .ts file for spanish-mexico have field names on
lotSerialRegistration screen
* [Translation] Context taxCode has the word �Never� as a
literal that can't be translated
* [Translation] Word Always is not present in .ts file for context
taxCod
* [Translation] Typo �Venbor type� in APassignmentsMasterList