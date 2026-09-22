# PROFESSIONAL RETAIL POS APPLICATION — MASTER BUILD PROMPT

I want you to help me BUILD a complete professional POS (Point of Sale) application for a retail shop.

I will manage the project using Git/GitHub and I will use your help throughout development.

IMPORTANT: Do not only give me an architecture or tutorial. I want you to ACTUALLY BUILD the application with complete working code, step by step.

Later, I may upload the complete project as a ZIP file. When I do that, you must audit the entire project against this exact specification and identify every missing, incomplete, broken, insecure, or incorrectly implemented feature.

---

# 1. TECHNOLOGY STACK

Use this stack:

* PHP
* Laravel
* SQLite
* HTML
* CSS
* Vanilla JavaScript
* Blade templates

Do NOT use:

* React
* Vue
* Angular
* Node.js
* Next.js
* MongoDB
* Firebase
* unnecessary external frameworks

Bootstrap/Tailwind should not be required unless there is a very strong reason. Prefer custom CSS and Vanilla JavaScript.

The application must work locally on Windows.

---

# 2. DEVELOPMENT STYLE

I will use Git.

Therefore:

* Keep the project structure clean.
* Make changes in logical stages.
* Do not randomly rewrite working files.
* Do not remove existing features when adding new ones.
* Keep database migrations organized.
* Keep controllers/models/services organized.
* Keep JavaScript and CSS maintainable.
* Make every feature Git-friendly.

For every development stage:

1. Explain what you are building.
2. Show the files that will be created/modified.
3. Give complete code.
4. Give exact commands.
5. Explain how I can test it.
6. Do not use fake placeholder code.
7. Do not write "same as above".
8. Do not write "// rest of code".
9. Do not silently remove previous functionality.

If the response becomes too long, continue in the next response from the exact point where you stopped.

---

# 3. MAIN GOAL

Build a modern, professional, highly animated, fast and fully responsive retail POS application.

It must feel like real commercial POS software, not a basic student CRUD project.

The application must prioritize:

* Speed
* Easy operation
* Minimal typing
* Barcode-first workflow
* Simple navigation
* Professional UI
* Security
* Accurate stock
* Accurate financial calculations
* Responsive design

---

# 4. RESPONSIVE DESIGN

The application MUST work properly on:

* Desktop PC
* Laptop
* Tablet
* Mobile phone

Do not simply shrink the desktop interface.

Create proper responsive layouts.

### Desktop

* Full sidebar
* Dashboard cards
* Large POS layout
* Product grid
* Cart panel

### Tablet

* Responsive columns
* Touch-friendly buttons
* Collapsible navigation

### Mobile

* Hamburger menu
* Mobile-friendly POS
* Responsive cart
* Touch-friendly controls
* Responsive tables
* Responsive forms
* Responsive reports

---

# 5. ANIMATED UI

The application must be highly animated but professional.

Use smooth animations for:

* Login
* Dashboard
* Sidebar
* Buttons
* Cards
* Product cards
* Cart
* Modals
* Dropdowns
* Notifications
* Page transitions
* Loading states
* Charts
* Success messages
* Error messages

Use animations carefully so the POS remains fast.

Do NOT create unnecessary animations that slow down normal shop operations.

---

# 6. THEME SYSTEM

Create a proper theme system.

At minimum:

* Light Mode
* Dark Mode

The selected theme must persist after closing/reopening the application.

Use CSS variables where appropriate.

Theme must apply to:

* Login
* Dashboard
* Sidebar
* POS
* Products
* Tables
* Forms
* Modals
* Reports
* Settings
* Notifications
* Invoice preview

---

# 7. SECURITY

Security is very important.

Use Laravel's proper security mechanisms.

Implement:

* Secure authentication
* Password hashing
* Session security
* CSRF protection
* Server-side validation
* Authorization
* Role-based access control
* Permission checks
* Route protection
* Input validation
* Safe database queries
* Proper error handling
* Login rate limiting/protection where appropriate
* Activity logging

NEVER store passwords as plain text.

NEVER rely only on JavaScript for permission/security.

All sensitive actions must be checked on the Laravel backend.

---

# 8. ADMIN AND CASHIER SYSTEM

Create a proper user/role/permission system.

## ADMIN

Admin can:

* Add cashier
* Edit cashier
* Delete cashier
* Disable cashier
* Enable cashier
* Reset cashier password
* View cashier information
* Manage permissions
* View activity logs
* Manage products
* Manage categories
* Manage brands
* Manage barcode
* Manage purchases
* Manage sales
* Manage returns
* Manage customers
* Manage suppliers
* Manage expenses
* View reports
* Manage settings
* Backup database
* Restore database

## CASHIER

Cashier permissions must be configurable by Admin.

Example:

Allowed:

* POS
* New Sale
* Customer
* Invoice
* Sales History

Restricted:

* Delete Product
* Delete User
* Backup
* Restore
* Settings
* Profit Report
* User Management

Admin must be able to change permissions.

A cashier must NOT be able to bypass permissions by manually typing a URL.

---

# 9. DASHBOARD

Create a professional animated dashboard.

Show:

* Today's sales
* Today's profit
* Today's purchases
* Today's expenses
* Total products
* Total stock
* Total customers
* Total suppliers
* Customer due
* Supplier due
* Low-stock products
* Out-of-stock products
* Recent sales
* Recent invoices

Charts:

* Daily sales
* Weekly sales
* Monthly sales
* Profit
* Purchase
* Expense
* Category-wise sales

Charts should support date filtering.

---

# 10. POS / SALES SCREEN

Create a fast POS screen.

Features:

* Product search
* Barcode scan
* Product category filter
* Product cards
* Product image
* Add to cart
* Remove from cart
* Increase quantity
* Decrease quantity
* Manual quantity input
* Discount
* VAT/tax
* Subtotal
* Grand total
* Customer selection
* Cash payment
* Due payment
* Change calculation
* Payment method
* Hold bill
* Resume bill
* Clear cart
* Cancel sale
* Complete sale
* Print receipt

The POS must be optimized for real shop usage.

---

# 11. BARCODE SYSTEM — VERY IMPORTANT

Create a professional barcode system.

USB barcode scanners should work.

Barcode scanner input should be handled using Vanilla JavaScript.

Support:

* Barcode scanning
* Barcode searching
* Barcode generation
* Barcode printing
* Barcode validation
* Duplicate barcode prevention
* Multiple barcodes for one product
* Bulk barcode entry

## IMPORTANT REAL-WORLD REQUIREMENT

Suppose I have:

Product:

A Company Oil 1L

I have 100 bottles.

Every bottle may have a different barcode.

I DO NOT want to create the product 100 times.

I want:

Product created ONE time:

A Company Oil 1L
Brand: A Company
Purchase Price: 150
Selling Price: 180
Stock: 100

Then I want to attach 100 different barcodes to this SAME product.

Example:

890000001
890000002
890000003
...
890000100

Create a Bulk Barcode Entry screen.

Workflow:

Select Product
→ Scan barcode
→ Barcode automatically added
→ Scan next barcode
→ Automatically added
→ Continue

The product name, price, category and other information must NOT need to be entered repeatedly.

When any assigned barcode is scanned in POS:

Barcode
→ Find associated product
→ Add product to cart

Prevent duplicate barcode assignment.

---

# 12. PRODUCT MANAGEMENT

Product fields:

* Product name
* SKU/Product code
* Multiple barcodes
* Category
* Brand
* Unit
* Purchase price
* Selling price
* Wholesale price
* Current stock
* Minimum stock
* Product image
* Description
* Status
* Created date
* Updated date

Features:

* Add
* Edit
* View
* Search
* Archive/Delete
* Disable
* Product history

Do not permanently delete products if doing so would break old invoices or transaction history.

Use archive/soft-delete where appropriate.

---

# 13. CATEGORY MANAGEMENT

Support:

* Add category
* Edit category
* Archive/delete category
* Search category
* Category-wise products

---

# 14. BRAND MANAGEMENT

Support:

* Add brand
* Edit brand
* Archive/delete brand
* Search brand
* Brand-wise products

---

# 15. PURCHASE MANAGEMENT

Create purchase management.

Workflow:

Supplier
→ Product
→ Quantity
→ Purchase Price
→ Save Purchase

After completing purchase:

Stock must automatically increase.

Example:

Old stock = 20
Purchase = 50
New stock = 70

Store complete purchase history.

---

# 16. SALES MANAGEMENT

After completing a sale:

Stock must automatically decrease.

Example:

Stock = 70
Sold = 3
Remaining = 67

Use database transactions for sales and stock changes.

---

# 17. RETURN SYSTEM

Create sales return functionality.

Support:

* Select invoice
* Select product
* Return quantity
* Return reason
* Refund amount
* Stock adjustment
* Return history

Do not allow invalid return quantities.

---

# 18. CUSTOMER MANAGEMENT

Customer fields:

* Name
* Phone
* Address
* Email
* Total purchase
* Paid
* Due
* Status

Features:

* Add customer
* Edit customer
* Search customer
* View purchase history
* View due
* Receive payment
* Payment history

---

# 19. CUSTOMER DUE

Example:

Total = 5000
Paid = 3000
Due = 2000

Later:

Customer pays 1000

Remaining due = 1000

Maintain complete payment history.

---

# 20. SUPPLIER MANAGEMENT

Supplier fields:

* Name
* Phone
* Address
* Email
* Company
* Due

Features:

* Add supplier
* Edit supplier
* Search supplier
* Purchase history
* Supplier due
* Supplier payment history

---

# 21. EXPENSE MANAGEMENT

Support expenses:

* Electricity
* Rent
* Transport
* Salary
* Repair
* Other

Fields:

* Category
* Amount
* Date
* Note
* Created by

Use expenses in net profit calculations.

---

# 22. INVOICE / RECEIPT

Create professional invoices.

Invoice should include:

* Shop logo
* Shop name
* Address
* Phone
* Invoice number
* Date
* Time
* Cashier
* Customer
* Product
* Quantity
* Unit price
* Discount
* VAT/tax
* Subtotal
* Total
* Paid
* Due
* Change

Support:

* Print
* Reprint
* Invoice history

Create layouts for:

* 58mm thermal printer
* 80mm thermal printer
* Normal printer/A4 invoice

---

# 23. PRINT SYSTEM

Use print-friendly CSS.

When printing receipt:

Only the receipt should print.

Do not print the dashboard/sidebar.

Support browser/local printer workflow.

---

# 24. SALES REPORT

Create:

* Daily sales
* Weekly sales
* Monthly sales
* Custom date range
* Product-wise sales
* Cashier-wise sales
* Customer-wise sales

Show:

* Total sales
* Total transactions
* Discount
* VAT
* Paid
* Due
* Profit

---

# 25. PURCHASE REPORT

Show:

* Total purchases
* Purchase amount
* Supplier
* Product
* Quantity
* Date
* Payment
* Due

---

# 26. PROFIT REPORT

Calculate:

Selling price - purchase cost = gross profit

Then:

Gross profit - expenses = net profit

Show clearly:

* Gross sales
* Cost of goods
* Gross profit
* Expenses
* Net profit

Do not mix revenue and profit.

---

# 27. STOCK REPORT

Show:

* Product
* Current stock
* Minimum stock
* Low stock
* Out of stock
* Stock movement

Stock history should include:

* Purchase
* Sale
* Return
* Adjustment

---

# 28. NOTIFICATIONS

Create animated toast notifications.

Examples:

Success:
"Sale completed successfully."

Warning:
"Low stock."

Error:
"Barcode already exists."

Info:
"Backup completed."

---

# 29. KEYBOARD SHORTCUTS

Support useful POS shortcuts.

Example:

F1 = New Sale
F2 = Product Search
F4 = Customer
F8 = Payment
Enter = Complete action
Esc = Close modal

Create a shortcut help screen.

---

# 30. HOLD BILL

Support:

* Hold current bill
* Start another sale
* View held bills
* Resume held bill
* Delete held bill

---

# 31. INVOICE HISTORY

Support:

* Search invoice
* Filter by date
* Filter by cashier
* View invoice
* Reprint
* View payment
* View returned products

---

# 32. BACKUP / RESTORE

Admin only.

Support:

* Database backup
* Download backup
* Restore backup
* Backup history if practical

Validate backup before restoring.

Cashiers must not access this.

---

# 33. ACTIVITY LOG

Log important actions:

* Login
* Logout
* Product creation
* Product update
* Product archive/delete
* Purchase
* Sale
* Return
* Expense
* User creation
* User deletion
* Permission change
* Backup
* Restore

Store:

* User
* Action
* Date/time
* Related record if applicable

---

# 34. SETTINGS

Shop Settings:

* Shop name
* Logo
* Address
* Phone
* Email
* Currency

Invoice Settings:

* Invoice prefix
* Receipt size
* Footer
* Logo visibility
* Customer visibility

Tax:

* Enable/disable
* Tax rate

Theme:

* Light
* Dark

System:

* Backup
* Restore
* Other configuration

---

# 35. DATABASE

Use SQLite.

Design a proper relational database.

Expected tables include, but are not limited to:

* users
* roles
* permissions
* role_permissions
* products
* product_barcodes
* categories
* brands
* customers
* suppliers
* purchases
* purchase_items
* sales
* sale_items
* returns
* return_items
* customer_payments
* supplier_payments
* expenses
* expense_categories
* stock_movements
* held_bills
* activity_logs
* settings

Use:

* Foreign keys
* Indexes where useful
* Relationships
* Timestamps
* Database transactions

---

# 36. DATA INTEGRITY

Financial and stock operations must use database transactions.

For example:

SALE:

1. Validate product
2. Validate stock
3. Create sale
4. Create sale items
5. Decrease stock
6. Create stock movement
7. Record payment
8. Commit

If any step fails:

Rollback the entire transaction.

---

# 37. SEARCH

Search by:

* Product name
* SKU
* Barcode
* Customer name
* Customer phone
* Invoice number
* Supplier
* Date

Use pagination where necessary.

---

# 38. UX

Optimize for real shop use.

Important:

* Fast POS
* Minimal typing
* Barcode-first
* Keyboard shortcuts
* Large important buttons
* Clear errors
* Confirmation before destructive actions
* Touch-friendly controls
* Responsive UI

---

# 39. ERROR HANDLING

Do not expose raw technical errors to normal users.

Show friendly messages.

Keep technical errors in logs for debugging.

---

# 40. CODE QUALITY

Use proper Laravel architecture:

* Routes
* Controllers
* Models
* Migrations
* Seeders
* Blade
* Form Requests
* Policies/Gates
* Services where useful

Keep:

* CSS organized
* JavaScript modular
* Database normalized

Do not create one giant file for everything.

---

# 41. DEMO DATA

Create seeders containing:

* 1 Admin
* 2 Cashiers
* Categories
* Brands
* Products
* Multiple barcodes for one product
* Customers
* Suppliers
* Sample purchases
* Sample sales

Provide demo login credentials clearly.

Do not use real credentials.

---

# 42. GIT COMPATIBILITY

The project must be Git-friendly.

Provide:

* Proper `.gitignore`
* `.env.example`
* Clear README
* Meaningful commits suggested for major features

Never commit:

* `.env`
* passwords
* API keys
* secrets
* database files if they contain private production data

---

# 43. DEVELOPMENT PROCESS

Build the application in logical phases.

Suggested phases:

PHASE 1:
Laravel setup + SQLite + base UI

PHASE 2:
Authentication + Admin/Cashier + permissions

PHASE 3:
Responsive animated UI + theme

PHASE 4:
Products + Categories + Brands

PHASE 5:
Multiple Barcode + Bulk Barcode

PHASE 6:
Purchase + Stock

PHASE 7:
POS + Sales + Payment

PHASE 8:
Receipt + Invoice + Printing

PHASE 9:
Customers + Due

PHASE 10:
Suppliers + Due

PHASE 11:
Returns

PHASE 12:
Expenses + Profit

PHASE 13:
Reports + Dashboard charts

PHASE 14:
Hold Bill + Invoice History + Keyboard shortcuts

PHASE 15:
Backup + Restore + Activity Log

PHASE 16:
Security audit

PHASE 17:
Responsive/UI/Animation optimization

PHASE 18:
Final testing and documentation

---

# 44. IMPORTANT — DO NOT LOSE FEATURES

Maintain a master checklist throughout development.

Every time a feature is completed, mark it:

[✓] Completed
[~] Partially completed
[ ] Not completed
[!] Bug/problem found

Never remove a completed feature without explicitly telling me.

When adding a new feature, verify that old features still work.

---

# 45. FUTURE ZIP AUDIT MODE

IMPORTANT:

Later I may upload the entire Laravel POS project as a ZIP file.

When I say:

"AUDIT THIS PROJECT AGAINST THE MASTER POS REQUIREMENTS"

you must inspect the actual project files and compare them against EVERY requirement in this prompt.

Do NOT just give a general review.

Create a detailed audit containing:

## FEATURE AUDIT

For every requirement:

* Status: PASS / PARTIAL / MISSING / BROKEN
* Relevant file(s)
* What is implemented
* What is missing
* What should be changed

Check at minimum:

* Authentication
* Security
* Admin
* Cashier
* Permissions
* Products
* Categories
* Brands
* Multiple barcodes
* Bulk barcode entry
* POS
* Sales
* Purchases
* Stock
* Returns
* Customers
* Customer due
* Suppliers
* Supplier due
* Expenses
* Profit
* Reports
* Invoice
* Receipt
* Printing
* Hold bill
* Keyboard shortcuts
* Backup
* Restore
* Activity log
* Themes
* Animation
* Responsive design
* Database integrity
* Validation
* Git readiness

Also inspect:

* Routes
* Controllers
* Models
* Migrations
* Blade files
* JavaScript
* CSS
* Authentication
* Authorization
* Database relationships
* Security
* Error handling

If a feature exists but is incomplete, mark it PARTIAL.

If a feature exists but does not work correctly, mark it BROKEN.

Do not assume a feature works merely because a button or page exists.

Trace the actual implementation.

---

# 46. ZIP AUDIT — DO NOT CHANGE CODE AUTOMATICALLY

When I upload a ZIP for audit:

First inspect and report.

Do NOT modify the project unless I explicitly ask you to fix the issues.

If I later say:

"FIX ALL ISSUES"

then provide the required modifications in a controlled manner while preserving all existing working features.

---

# 47. START NOW

Do NOT generate the entire application in one giant response.

Start by:

1. Confirming the technology stack.
2. Creating the complete architecture.
3. Creating the database relationship plan.
4. Creating the master feature checklist.
5. Creating the folder structure.
6. Explaining PHASE 1.
7. Then start implementing PHASE 1 with complete working code.

Remember:

I will use Git.

I want the actual application built step by step.

Later I will be able to upload the ZIP and ask you to audit it against this exact specification.

Do not omit any requirement from this prompt.
