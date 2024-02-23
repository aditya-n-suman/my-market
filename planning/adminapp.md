# Admin app

### Login
  - use one of admin emails
  - enter otp
  - lands on welcome screen

**_No signup option_**
### Welcome screen
  - shows welcome message
  - show suggested actions
  - show today's sell chart

### Action: Add an item
  - select category
    - fruits
    - vegetables
    - dairy/confectioneries
  - image
  - name
  - short description
  - rate
  - discount on item
  - number of items
  - variations, if any
    - image [optional]
    - name [optional]
    - rate [optional]
    - additional discount [optional]
    - discount [optional]
    - number of items
### Action: Add discount
  - select discount type
    - on category
    - on item
    - on variation
  - select category
  - **case**: on item/ on variation
    - select item
  - **case**: on variation
    - select variation
    - select variation discount type
      - discount
      - additional discount
  - enter discount
  - apply discount
  - toast shows status of this action
### Action: Add item in bulk
  - select category of datas
  - upload csv data
  - **case**: no category selected
    - csv should have category field
  - **case**: category selected
    - all data will be considered for this category
### Action: show transactions
  - lands on transaction list page sorted with most recent at top
  - each transaction list item shows:
    - time of transaction
    - mode of transaction
    - amount
### Action: see inventory
  - shows list of items available
  - filterable by:
    - category
  - sortable by:
    - quantity
  - supports pagination, by default
  - number of items shown at once can be choosen
