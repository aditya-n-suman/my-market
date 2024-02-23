# User App
It contains everything related to user app MyMarket
## Functionalities
It contains all the functionalities provided by this app
### Listings of
- Vegetables
- Fruits
- Dairy products & Confectioneries
### Offers/Discounts on
- individual items
- item categories
- item variants
## UI Details
### Products List
- Image
- name
- short description
- rate
- quantifier
- quantity 
- quantity selector buttons
### Cart
- **Product List**, where each product will contain
  - image
  - name
  - quantity
  - actual rate
  - discounted rate
  - quantity selector buttons
- Price Breakup
  - total price of products
  - discount total
  - GST
  - total amount to be paid
- Link to select/add address details
- Lint to **Payment Portal**
### Select/Add/Edit address
- contains
  - addressType/tag
  - name [editable]: picks account name as default
  - pincode
  - country: `india` as default
  - state
  - detail: multiliner
  - contact no.: picks account's phone as default
  - longitude: captured `by GPS`
  - latitude: captured `by GPS`
- All fields should be mandatory except GPS location
- opened through `edit` option:
  - all fields should be editable
- saving takes one step back in navigation history
### Payment Portal
- payment options to select from
  - list of cards added
  - list of UPI addresses added
- button to add new payment method
- Pay button
- if successful redirects to home page, else to the cart
### Recent Orders
- contains list of order with
  - Date/timestamp
  - order summary: e.g. Cabbage, Spinach and 8 more
  - Amount spent
  - status
    - ordered
    - en-ruote
    - delivered
    - cancelled
- clicking on any list item should
  - take to order summary page with
    - order item list similar to cart [non_editable]
    - amount details
    - `Get help` with current order action
  - going back takes to recent order list
### Account Details
- Account creation
  - All details needed for account (listed below)
  - can be opened after signup
  - should open after login if details are missing
  - should be skippable
  - should be completed BTS from shipping details if something is missing
- contains
  - Name
  - Email
  - Phone
  - default address
### Login/signup
- takes
  - Email/phone number
  - password
  - forgot password, request otp 
  - if forgot password clicked
    - password input disables
    - otp status appers
    - OTP input appears
  - submit button
- signup success
  - lands on profile creation page
  - if skips creation lands on home page
- login success
  - lands on home page
