<h1 align="center">✂ Barber POS</h1> <p align="center"> <b>A fast, offline-first point of sale for barber shops.</b><br> Built with Flutter, Drift (SQLite) and Material 3. </p> <p align="center"> <img width="196" height="400" alt="Sale screen" src="https://github.com/user-attachments/assets/02d24e62-3f10-4ba5-9374-436ca6764cca" /> <img width="196" height="400" alt="Reports screen" src="https://github.com/user-attachments/assets/b883c50a-c8b9-4fd6-86a2-e7888dc1c72a" /> </p>
✨ Features
One-tap sales: tap service tiles in a responsive grid and watch the total update.
Cash & Whish payments: every order records how it was paid.
Receipts: on-screen receipt after each sale, with print or save as an A6 PDF.
Service manager: add, edit and price services; toggle a service off to hide it without losing history.
Live reports: daily and monthly totals, order counts and the cash vs Whish split, updating in real time.
CSV export: export the selected day or month (saved to app storage on Android, share sheet on iOS).
Google Drive backup & restore: back up the database and restore it on a new device; last backup time shown in Settings.
Offline-first: all data is stored locally in SQLite.
📱 Screenshots
<table align="center"> <tr> <td align="center"><b>Sale</b></td> <td align="center"><b>Services</b></td> <td align="center"><b>Reports</b></td> </tr> <tr> <td align="center"><img width="196" height="400" alt="Sale" src="https://github.com/user-attachments/assets/e5af52dc-caf2-4d62-840a-e68d2c49b9b3" /></td> <td align="center"><img width="196" height="400" alt="Services" src="https://github.com/user-attachments/assets/a7938fc4-19ed-45e9-abc5-786dd32869c5" /></td> <td align="center"><img width="196" height="400" alt="Reports" src="https://github.com/user-attachments/assets/aadc23f4-cd0e-478b-b1d6-1e86074531ae" /></td> </tr> </table>
🧭 How it works
Sale: select the services the customer wants.
Pay: choose Cash or Whish; the order and its items are saved in one transaction.
Receipt: review, then print or save a PDF.
Reports & backup: check daily/monthly totals, export CSV and back up to Google Drive.
🗂 Project structure
lib/
├── main.dart
├── core/
│   ├── backup/        # Google Drive backup & restore
│   ├── database/      # Drift database and tables
│   └── export/        # CSV export and file saving
└── features/
    ├── home/          # Bottom navigation
    ├── sales/         # Sales screen, receipt screen, receipt PDF
    ├── services/      # Services list and add/edit dialog
    ├── reports/       # Daily and monthly reports
    └── settings/      # Backup and restore controls
