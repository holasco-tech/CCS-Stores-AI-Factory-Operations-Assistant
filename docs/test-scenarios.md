# Test Scenarios

## Production

**Input:** `We produce 2 drums of hot oil today.`  
**Expected:** A production record is created and the user receives a success acknowledgement.

## Farm feed

**Input:** `Farm Feed: 1 bag of PKC was used for the pig farm today.`  
**Expected:** Farm Feed Usage is recorded and PKC inventory is reduced by one bag.

## Expense

**Input:** Record a ₦15,000 diesel/fuel factory expense paid by bank transfer.  
**Expected:** Expense is saved with category, description, payee, payment method and receipt status.

## Sale + part payment

**Input:** Sell 1 bag of PKC to Bisi Farms for ₦12,000; receive ₦5,000.  
**Expected:** Sales record shows ₦12,000 total, ₦5,000 paid and ₦7,000 outstanding.

## Remaining payment

**Input:** Bisi Farms pays the remaining ₦7,000 for `SALE-20260805-124251`.  
**Expected:** Payment is recorded and the related sales balance is updated.

## Kernel purchase

**Input:** Purchase and receive 1,000 kg of palm kernel nuts; record supplier/payment details.  
**Expected:** Raw-material purchase is created with a unique purchase ID and delivery status.
