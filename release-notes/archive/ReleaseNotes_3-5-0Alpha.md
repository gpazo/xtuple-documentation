Release Notes
xTuple ERP
PostBooks, Standard, and Manufacturing Editions
Version 3.5.0Alpha
January 29, 2010
----------------------------------

This is the alpha release of version 3.5.0. This release is
packed with lots of new features, and more still to come in the
next stage of the release cycle. As always, we are looking for
feedback from alpha testers. But testers please note: the
purchasing module should be avoided, since extensive changes to
support drop shipping are not yet complete.

Here's an overview of new features in this release:

Expanded Pricing Effectivity Support
  * More info: http://www.xtuple.org/issuetracker/view.php?id=9603

Embedded MetaSQL Editor
  * More info: http://www.xtuple.org/issuetracker/view.php?id=7732

Tooling Management
  * Full spec: http://www.xtuple.org/node/2197

Also of note:
  * Automatic A/R Discounts
  * Improved Lot/Serial Support
  * Support for Postgres 8.4

----------------------------------

The following features and bug fixes have been added to the
applications since the release of 3.4.0. Additional detail for each
item listed below may be found on our community website
(www.xtuple.org). Simply go to the Issue Tracker and select the
"Changelog" option.


New Features:

* [Accounting] Reconcile Bank Accounts by Credit Card
* [Accounting] Add support for A/R discounts to Cash Receipt
* [Accounting] Add the ability to select by customer group in to
the A/R aging display and the printed report
* [Accounting] Add pricing effectivity options to sales order
* [Accounting] Selection hold button on Payables Workbenc
* [Accounting] Provide color emphasis on credit type columns on
Open Receivables display
* [Accounting] "Apply line bal." button within the "Apply A/R
Credit Memo" screen
* [Accounting] Tooling issue and return
* [Accounting] Calculate freight on Returns using freight
pricing schedules
* [Accounting] The ship order window should use the freight
calculation algorithm
* [Accounting] Add radio buttons to the Print Packlist Form
window to explicitly choose whether to print Picklist
* [Accounting] Bank rec history label should refer to date
range
* [Architectural] Embed MetaSQL editor into xTuple ERP
application and add some enhancements
* [Architectural] Adding index on arapply to improve
performance
* [Architectural] Added First Group field to api.itemsite vie
* [Architectural] Capture and log qWarning/qDebug output to
window accessible from application
* [Architectural] Remove dependency on curl for credit card
processing
* [CRM] Prompt "are you sure" when deleting a Contact
* [Inventory] Serialized Job Items
* [Inventory] Automatically generate Serial Numbers
* [Inventory] Preserve lot # during Inter-Warehouse Transfer
* [Inventory] Ability to add back into inventory previously
scrapped or expensed items
* [Inventory] Auto populate Lot/Serial
* [Manufacture] Add the ability to set W/O item cost recognition
defaults at the item site level
* [Purchase] Increase price precision
* [Purchase] Add a notes field to voucher distributions
* [Sales] Move sales order reschedule feature to the Sales Order
Window
* [Sales] Price Schedule enhancement pack
* [Sales] Add option to recalculate pricing on a sales order
when the shipto is changed
* [Sales] Add "Scheduled Date Range" criteria to the Print
Packing List by Ship Via window
* [Sales] Remove freight charge on Back Order Invoices
* [System] Rename user "groups" to "roles"; add column to List
Users

Bug Fixes:

* [All] Idle timeout does not roll back partial transactions
* [All] Blocks on db when certain screens are open
* [All] Distribution screen holds Postgres
* [Accounting] Return work order material revalues WIP
incorrectly on average cost
* [Accounting] Return Stock to Shipping for Lot/Serial MLC
items can miss distribution history
* [Accounting] reloading some api view definitions gives sql
errors on tax fields
* [Accounting] List Price UOM on item master is misleading
* [Architectural] Type setting of the XComboBox not being set
correctly to type "Adhoc"
* [Batch Manager] Update buffers status by planner code returns
query error
* [CRM] Sticky options not remembering settings
* [CRM] Cannot Delete CRM Account w/ Primary and/or Secondary
Contacts
* [CRM] when you detach a Primary/Secondary Contact from a CRM
Account, it's still there
* [Inventory] Only one item site for any item may ship at any
time
* [Inventory] Incomplete Lot/Serial transaction leaves orphaned
itemlocdist entries
* [Manufacture] Standard Operation data not available when
adding operations
* [Manufacture] BOO Instructions not in display
* [Products] Qty Per limits to Qty decimal precision on BOM
item
* [Sales] Deleting sales orders and SO line items slow
* [Sales] Performance issue with Sales -> List Quotes
* [Sales] Tax and freight not displayed in Billing Edit list
* [Sales] System Hangs on Credit Memo Line Item when item
number entered (after turning items to Exclusive)
* [System] Maintaining others preferences
* [System] XML import automatically prepends api. to all views