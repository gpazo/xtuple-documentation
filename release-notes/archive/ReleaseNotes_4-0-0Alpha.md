Release Notes
xTuple ERP
Version 4.0.0Alpha
March 30, 2012
----------------------------------

This is the alpha release of version 4.0.0. This release includes
several new features and bug fixes. As always, we are looking for
feedback from alpha testers. However, if you do test the alpha, 
please be reminded alpha software should not be used in live
production.

Information about compatibility issues related to this software
version can be found on the xTuple Compatibility Matrix at the
following address: www.xtuple.org/compatibility-matrix.

Here's an overview of notable new features in this release:

Added tabs to desktop
  * Converted "inside the desktop" view to use tabs for every 
    open screen 

Enhanced Job Costing functionality 
  * Purchase-to-Job
  * Automatic issue of Purchased Items to Work Orders
  * Job Costing for child Work Orders

Multiple Project updates
  * Ability to copy Projects
  * And more

----------------------------------

The following features and bug fixes have been added to the
applications since 3.8.0. Additional detail for each item listed below
may be found on our community website under the Issue Tracker.

New Features:

* Change Workspace mode to used tabbed MDI Area [16319]
* Update Unposted Invoices to use display class [16383]
* Posting Bank Adjustment [16571]
* Enhance Operation Buffer Status report [16602]
* Add Purchase-to-Job and automatic issue capability for purchased items [16604]
* Add Costing over-ride on the Bill of Materials [16605]
* Add job costing capability for child work orders [16606]
* Incidents should be enhanced to be filterable on Item and Lot/Serial numbers [16607]
* CRM Account and Contact should be added as standard associations for Project [16609]
* Add additional filters to Project List [16610]
* The assigned date should automatically populate on a Project or Project Task when the document is assigned [16611]
* The completed date should automatically populate on a Project or Project Task when the document status is changed to completed [16612]
* Project and Project Task should be modified to be able to keep track of date changes by whom and when [16613]
* A/R Credit Memo does not release number [11573]
* schema_path search [13211]
* Config option on license manager [15451]
* Add WEIGHTSCALE to format options [15851]
* Add costs and BOM data on the item master window [16315]
* Add the ability to copy Projects [16615]
* Add support for recursive lot tracing for items posted through Misc. Production Posting [16616]
* Make gltrans and sltrans share the same id sequence [17083]
* Make ship form not mandatory in the application [17085]
* Toggle of bankrecitem to uncleared should delete the bankrecitem [17086]
* Create additional transaction type default locations with automatic distribution [17112]
* Reimplement order sequence numbering to prevent number gaps and collisions [17119]


Bug Fixes:

* X-ing out of the application with new RA screen open creates orphaned entries. [8562]
* Posting authorized credit card does not process transaction [8864]
* Empty trialbal column header options confusing [9280]
* Summarized sales displays and reports skew averages incorrectly if misc credit memos have been posted [9458]
* It is possible to delete a Return leaving orphaned work orders [9866]
* PO#'s being skipped [11711]
* Existing line items not displayed while creating RA if manual numbering [12290]
* Transfer order contact change is not handled correctly when reopening transfer order [15900]
* Print report of Pricing Schedule Assignments displays incorrect details [16163]
* Observation: It is possible to create an invoice with no line items [16207]
* Incorrect behavior is observed on clicking "Yes" button in cancellation of a Role [16210]
* The definition of api.purchaseline is incorrect - duplicate PO Lines are returned because the view includes information from work order [16284]
* Financial report tool accepts bad data [16295]
* Selecting to delete a sales order doesn't delete the Purchase order linked to the Sales order line item sub component [16303]
* Blank tax code is created on cancelling the creation of a Tax code [16321]
* UI on detailed inventory history by Lot/Serial needs clean up [16394]
* Create Item Site Utility not functional with InterfaceToGL metric disabled [16409]
* Empty locale is created on selecting to cancel the creation of a new locale [16420]
* Expired Inventory print report doesn't honor the options selected [16458]
* Cost values are printed irrelevantly in the print report of Work Order history by Class code screen [16472]
* Irrelevant dialog is displayed on selecting to re-open Work Order History by Item screen [16473]
* Cancel button does not work in Production Plan window [16485]
* BOM [16498]
* Incorrect behavior is observed in Print Invoice screen when copies decreased to less than 1 [16500]
* Item Costs by Class Code [16513]
* Selecting to copy a sales order doesn't generate Purchase Request linked to the sales order line item [16533]
* Un-expected behavior is observed on selecting a non-working day as the schedule date for a sales order line item [16535]
* Pending availability [16556]
* Quote with scheduled date that is not a working day allows creation of line items on non-working days without warning [16561]
* itemcomment and itemsitecomment api views aren't accessible [16587]
* Pricing schedule of type "Freight" assigned to a Customer Ship-To is not functional [16681]
* Qty per on bom does not reflect locale [16696]
* "Deactivate" option is not available on right click of an Opportunity [16702]
* It is possible to save a Sales Order with blank Sales Order Number [16704]
* DB log error is generated on selecting to print Time-Phased Bookings screen [16719]
* AP aging report not showing correct amounts on aging columns [16724]
* QDir.homePath() script exposure returns JavaScript undefined [16735]
* Error message is displayed on scheduling 'Run MPS' using xtConnect [16746]
* Summarized BOM [16748]
*  It is possible to edit a Purchase Order even after revoking the necessary privileges [16762]
* Add date range filter to customer workbench, sales tab [16763]
* Able to reserve qty. with no QOH [16770]
* Return not reflected on Item Availability Workbench [16802]
* issueWoMaterialItem screen - unused component description2 field [16811]
* Faulty logic in Invoice Item [16824]
* Item Availability Workbench - Where-Used tab rounds qty-per values for non-fractional items [16840]
* As of Date on Customer Statement does not work [16875]
* Posted invoice entries are displayed under incorrect date in the Invoice Register screen [16882]
* It is possible to create a purchase order for an itemsite with no work week defined [16896]
* Lack of index on xtmfg.booitem results in severely degraded MRP performance [16919]
* Item privileges not implemented [16969]
* Item Types filter not working [16990]
* Count Tag Edit List only shows variance values for posted count slips [16994]
* Opportunities vs Customer [17010]
* Tax Registrations requires chart of accounts privilege [17027]
* When Creating New Contact, Default Owner Should be Creator [17032]
* Duplicate accounts utility shows project accounts when it shouldn't [17105]
* Selecting to create a New item crashes the application [17188]
* It is not possible to create WH1 site in Postbooks empty database [17192]