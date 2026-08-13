# Portfolio Data Model

This document describes the operational entities used by the CCS Stores Factory Operations Assistant. It intentionally excludes live spreadsheet IDs, private customer data and credentials.

## Product & Inventory

Typical fields:

- Product
- Opening stock
- Quantity in
- Quantity out
- Current balance
- Unit
- Last updated

## Production Records

Typical fields:

- Date/time
- Product / output type
- Quantity
- Unit
- Source message / reference
- Notes

For PKO operational estimates, settled 200-litre drums can be converted using the factory rule of approximately **6 settled drums = 1 ton**.

## Sales Records

Typical fields:

- Sale ID
- Date
- Buyer
- Product
- Quantity
- Unit price
- Total amount
- Amount received
- Outstanding balance
- Payment status

## Expenses Records

Typical fields:

- Expense ID
- Date
- Category
- Description
- Amount
- Paid to
- Payment method
- Receipt available

## Payment Records

Typical fields:

- Payment ID
- Sale ID
- Buyer
- Amount paid
- Date
- Payment method
- Remaining balance

## Delivery Records

Typical fields:

- Delivery ID
- Related sale / purchase ID
- Customer / supplier
- Destination
- Status
- Delivery fee
- Date

## Buyers Records

Typical fields:

- Buyer ID
- Buyer / company name
- Contact details
- Products purchased
- Location
- Notes

## Raw Materials Inventory

Typical fields:

- Purchase ID
- Supplier
- Kernel quantity
- Unit / weight
- Purchase price
- Transport cost
- Amount paid
- Outstanding amount
- Delivery status

## Farm Feed Usage

Typical fields:

- Date
- Feed type
- Quantity used
- Unit
- Farm / destination
- Inventory deduction

PKC usage for the pig farm reduces the main PKC inventory and is also stored in the Farm Feed Usage log.

## Pig Farm Records

Typical fields:

- Date
- Event type: Birth / Death / Purchase
- Quantity
- Notes
- Updated livestock balance
