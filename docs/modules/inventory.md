# Inventory module

Owner: dulaakalanka2002-arch · Branch: feature/resources

## Covers
Inventory items, check-out and return, low-stock alerts, quantity history, bulk import and the public QR item page.

## Tables
inventory, inventory_assignments

## How to test
1. Import the inventory CSV and check the items appear in the list.
2. Check an item out to a teacher, then return it.
3. Lower an item's quantity below its minimum and check the low-stock alert.
4. Open an item's QR page (/item/[token]).
