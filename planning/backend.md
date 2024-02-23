# Backend for myMarket
It contains all the details about backend development for MyMarket.
## User service
manages user creation deletion, profile details and profile updation.
### Admins
- email
- role
### Users
- user_id
- emailId/phone
- password
- role
### Account Details
- account_id
- user_id
- name
- email
- phone
### Address Details
- address_id
- user_id
- name
- phone
- tag
- country
- state
- pincode
- detail
- longitude
- latitude

## Inventory service
manages inventory
### Categories
- category_id
- category_name
### Items
if there in no variations, use self details; otherwise give priority to variation's data.
- item_id
- category_id
- images
- name
- description
- rate
- quantifier (per): e.g. packet, 250g, 1kg, family pack
- item_discount
- quantity [override]:with sum of quantities of variations
- variations[optional]: list of variations containing one `default`
### Item Variations
<!-- if discount not set, use item_discount -->
- variation_id
- item_id
- images
- name
- description
- rate
- quantifier (per): e.g. packet, 250g, 1kg, family pack
- discount
- additional_discount
- quantity
## Order Service
manages ordering of items.
### Order
- order_id
- user_id
- order_time
- order_status
- order_items
- total_price
### Order Item
- order_item_id
- price_paid
- inventory_item_id
- quantity
- rate
## Payment Service
It handles everything related to payments and transactions
### Cards Data
- card_id
- card_number
- expiry
- cvv
- balance
- user_id
### UPI Data
- upi_id
- upi_address
- balance
- user_id
### Transaction
- transaction_id
- user_id
- amount
- payment_mode
- pay_through: contains card_id/upi_id depending on payment_mode
- time
