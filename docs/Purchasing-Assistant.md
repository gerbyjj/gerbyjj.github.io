---
layout: default
title: Purchasing Assistant
nav_order: 1
---

# Purchasing Assistant
<details open markdown="block">
  <summary>
    Table of contents
  </summary>
  {: .text-delta }
- TOC
{:toc}
</details>

## Purchasing Assistant Tabs

#### Search: Search
- Security: Purchase Assist Features: "Can View Search?"
- Keyword search works better when personal preference "Default Search Term" is set to "AND".
- The default search tab can be set on personal preferences under "Purchasing Assistant Profile Settings":
  - Default Purchasing Assistant Tab

#### Search: Ext Whse PRs
- Client 1 only
- Security: Purchase Assist Features: "Can View Ext Whse Demand Items?"
- Items with Material Code will find matches in the Sourcing Panel with same Material Code.
- Items without Material Code can be searched in the Search pane by keyword . 

#### Cart
- No additional security required for access.

#### Quotes
- Security: Purchase Assist Features: "Can Create Quotes?"

#### Documents
- Security: Purchase Assist Features: "Can Access PA Document Search?"

* * *

## Purchasing Assistant Profile

#### Name
- Nickname given to the profile to distinguish between multiple profiles.

#### Issued By & Issued For
- Organizations to be used on resultant documents.
- Organization lists are limited to the user's create privileges for most document types: Rqn, Tender, PO.

#### Delivery Address
- Delivery address to be used on resultant documents.  
- Issued For organization limits this list.

#### Warehouse Document
- Not applicable (default)
  - Material Catalogue will not be an option in Search availability.
- Warehouse - Replenishment

* * *

## Purchasing Assistant Actions

#### Create a Release/SPO
- Security: Purchase Assist Features: "Can Create SPOs?"
- Contract exists in the Master Catalogue.
- The profile's Issued For organization is a permitted user of the Contract.
- Contract items are returned as Sources in the Sourcing Panel under search results.
- Contracts will be limited to XXX when Profile indicates "Warehouse Replenishment".

#### Release against a specific Contract/Standing Offer Item
- Contract item is not defined as generic item presentation.

#### Release against a generic Contract/Standing Offer Item
- Contract item is defined as generic item presentation.
- Search finds the SPO items against the generic Contract item.

#### Punch Out 
- Contract is defined as Punch Out.
- We don't have a way to test this at the moment.

#### Create a Purchase Order
- Security: Purchase Assist Features: "Can Create Purchase Orders (other than SPOs)?"

#### Create a Purchase Order (source is a Purchase Order in the Master Catalogue)
- Purchase Order exists in the Master Catalogue.
- The profile's Issued For organization is XXX.
- Purchase Order items are returned as Sources in the Sourcing Panel under search results.
- When these items are actioned, the source item pricing is retained on the resultant document.

#### Create a Purchase Order (source is a Historical Purchase)
- Source document does not need to exist in the Master Catalogue.
- Purchase Order and SPO items are returned as Historical Purchases under the Sourcing Panel.
- Historical Purchases are provided as reference for Material searches only:
  - All Client 2 searches
  - Search: Ext Whse PRs
  - Search: Search and availability = Material Catalogue
- Historical Purchases are limited by personal preferences under "Purchasing Assistant Profile Settings":
  - Num of Purchase Orders to display
  - Num of Purchase Order Drawdowns to display
  - Num of months to display
- If user does not have these settings, the limits are defined in System Characteristics/ Miscellaneous definitions, under "Purchasing Assistant".
- When these items are actioned, the source item pricing is not retained on the resultant document.

#### Create a Purchase Order (not based on a source)
- No vendor, no pricing is associated with these items in the cart.
- A vendor will be assigned upon document creation.

#### Create a Requisition
- Security: Purchase Assist Features: "Can Create Purchase Requests?"

#### Create a Stores Requisition (ABCD for Client 2)
- Issued For Org is not a Warehouse Owner (Client 2)

#### Create a Print Requisition
- Client 3 only
- Catalogue refer id is like the default print item code (system char)

#### Create a Replenishment Requisition
- Profile indicates "Warehouse Replenishment" (Client 1)
- Issued For Org is a Warehouse Owner (Client 2)

#### Create a Purchasing Requisition
- Profile does not indicate "Warehouse Replenishment" and Search availability = Commodity Catalogue (Client 1)

#### Create a Quick Quote
- Security: Purchase Assist Features: "Can Create Quotes?"

* * *

## Other Features
- Equivalent Item relationship between Master Catalogue items.
- Master Catalogue items are cached.

