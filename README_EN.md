# CarePoint Pharmacy Demo

A standalone, browser-based demo for exploring pharmacy inventory, billing, supplier requests, daily reports, and backups. This is a demonstration project only; it is not suitable for real pharmacy operations or real patient data.

## Start the demo

1. Open `portfolio.html` to view the project portfolio.
2. Open `carepoint-pharmacy-demo-reviewed.html` in a modern browser to try the demo.
3. Sign in with one of the built-in demo accounts:

| Role | Username | Password |
|---|---|---|
| Super Admin | `superadmin` | `super123` |
| Admin | `admin` | `admin123` |
| Cashier | `cashier` | `cashier123` |

The section menu changes according to the signed-in role. Super Admin can create staff accounts. Newly created staff accounts start with password `123`.

## Features

### Inventory and medicines

- Record stock items, quantities, expiry dates, medicine names, retail prices, and supplier details.
- Review expiry alerts and current inventory.
- Create and edit medicine catalogue entries.

### Billing

- Add one or more medicines to a bill and record a sale.
- Complete and print a receipt. Patient name, age, and sex are optional demo fields.
- Sales reduce the recorded inventory quantity.

### Suppliers and requests

- Save supplier contact details, including an email address.
- Record wholesale purchases; a saved purchase increases stock.
- Prepare a request for one or more drugs and open it as an email draft with **Share by email**. The app does not send the email automatically.
- Use **Generate PDF**, then choose **Save as PDF** in the browser print dialog.

### Daily business and drug ledger

- Choose a date to review recorded sales, bill count, units sold, purchases, and expenses.
- Record business expenses with a description, amount, and date.
- Review a selected drug's transaction ledger over all time, the last 7, 30, or 90 days, or the last year.
- The daily net figure subtracts recorded purchases and expenses from recorded sales. It is an estimate, not profit or a bank balance; the demo does not handle all costs, refunds, taxes, or payment settlement.

### Daily stock reports

- Any signed-in role can save today's inventory snapshot and download saved reports as CSV.
- Reports contain the stock item name, quantity, expiry, price, and supplier fields available in the demo.
- The latest 60 daily reports are kept in this browser. Automatic daily stock snapshots are captured with the nightly backup when the page is open.

### Backup and restore

- Any signed-in role can download a full JSON backup or save an internal snapshot.
- Automatic snapshots run at **11:59 PM local time** while the page is open. If there are newer changes when closing the page, the browser asks for confirmation; after confirming, the demo attempts to save an internal snapshot.
- Internal snapshots are stored in this browser and the latest five are kept. They are not a substitute for downloading a backup file to another safe location.
- Only Super Admin can restore a JSON or internal backup. Restore replaces the current demo data; a safety snapshot is attempted first.
- Full backups can contain staff account records and passwords. Store backup files privately and restore only trusted files.

## Before using this demo

This is a practice/demo tool. Do not enter real patient details, real staff passwords, or live pharmacy records. Demo records stay in the browser profile used on this device. Download backups regularly and keep them private. The built-in logins and roles are for trying the demo only; they are not safe for a real pharmacy.

## Pharmacy staff tutorial: daily workflow

### 1. Sign in with your role

Use the demo account provided for your role. Cashiers mainly use **Billing**. Admins manage medicines, suppliers, purchases, daily business, and the drug ledger. Super Admin can also manage staff accounts and restore backups. Every signed-in role can save or download stock reports and download a full backup.

### 2. Set up medicines and check stock

1. Open **Medicine catalogue** to add a medicine that can be sold. Enter its name, selling price, starting quantity, and expiry date, then save it.
2. Open **Inventory & expiry** to review quantities and expiry warnings, or add a stock item that is not in the sale catalogue.
3. Check that the medicine name, quantity, price, and expiry are correct before billing.

### 3. Add a supplier and request medicines

1. Open **Suppliers, requests & purchases**.
2. Add the supplier's company name and email. Contact person and phone are optional.
3. Under **Request drugs from a supplier**, enter each drug/product and requested quantity. Add a note for details such as strength, brand, or delivery instructions.
4. Choose **Share by email** to open a prepared email draft. Review it and send it from your email app.
5. Choose **Generate PDF** and then **Save as PDF** in the browser print window if you need a printable copy.

A request only asks the supplier for stock; it does not add anything to inventory. When stock arrives, use **Record wholesale purchase**. Select the supplier and medicine, enter the quantity and unit cost, then save. The purchase increases the stock quantity.

### 4. Make a sale and print a receipt

1. Sign in as Cashier, Admin, or Super Admin and open **Billing**.
2. Select a medicine, enter the quantity, and choose **Add**. Repeat for other items in the same bill.
3. Patient name, age, and sex are optional. Choose the payment method.
4. Choose **Complete & print bill**. Check the receipt, then print it if needed. Completing the bill records the sale and reduces stock.
5. If the app reports that stock is too low, ask an Admin to record received stock before completing the bill.

### 5. Review the drug ledger

Open **Drug ledger**, choose a medicine, then choose the period: all time, last 7, 30, or 90 days, or last year. The ledger lists recorded purchases and sales with the balance shown after each entry.

### 6. Check the day's business and record expenses

1. Admins can open **Daily business** and choose the business date.
2. Review recorded sales, bill count, units sold, supplier purchases, and expenses.
3. To record an expense, enter a description, amount, and date, then save it.
4. The net figure subtracts recorded purchases and expenses from sales. Treat it as a quick estimate, not profit or a bank balance.

### 7. Save a daily stock report

Open **Daily stock reports** and choose **Save today's stock report**. The report saves a snapshot of the current inventory. Use **Download CSV** beside a saved report to keep or share a spreadsheet copy. Automatic stock snapshots are also saved with the 11:59 PM backup when the page is open.

### 8. Back up the demo data

1. Any signed-in role can open **Backup & restore** and choose **Download backup JSON** to save a full copy outside the browser.
2. You can also choose **Save snapshot now** to keep an internal snapshot in this browser.
3. The app attempts an automatic internal backup at 11:59 PM while the page is open. If you close the page after making changes, the browser asks you to confirm leaving and then the app attempts to save an internal snapshot.
4. Keep downloaded JSON files private. They may include staff account records and passwords.
5. Only Super Admin can restore a backup. Restore replaces the current demo data, so select a trusted file and confirm carefully.

### 9. Sign out

Choose **Sign out** when you finish, especially on a shared computer. Signing out hides the app until the next login; it does not delete the saved demo records.

## Contact

Replace these placeholders with the project owner's preferred contact details:

- **Name / business:** Wikum
- **Phone / WhatsApp:** +94706863275
- **Email:** wikumchath@gmail.com
- **Address or website (optional):** [Add your address or website]




