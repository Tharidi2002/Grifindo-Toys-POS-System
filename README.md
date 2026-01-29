# Grifindo Toys — POS System (Summary)

A compact C# WinForms Point-of-Sale (POS) desktop application for toy retail (Grifindo Toys). Manage products, users, sales, receipts and images. Supports MS Access or MySQL as the backend.

## Quick facts
- Platform: Windows (C# WinForms)
- Database: MS Access (default) or MySQL (configurable)
- Notable features: product/user management, image upload (local images/ folder), SHA256 password hashing, soft-delete, receipt template, weekly sales chart (LiveCharts), data backup.

## Quick setup
1. Clone: `git clone https://github.com/Tharidi2002/Grifindo-Toys-POS-System.git`
2. Open the solution in Visual Studio (restore NuGet packages if prompted).
3. Configure DB in `App.config`:
   - Set `DbProvider` to `MSACCESS` or `MYSQL`
   - Update connection string for MySQL if used (tested with MySQL 8)
4. Build and run (F5). Create/seed database tables if required.

## Important notes
- Images: product/user images are copied into a local `images/` directory; backups use `.bak` files.
- Security: passwords hashed with SHA256 (`Util.GetHashSHA256`).
- Soft delete: `IsDeleted` flag is used for products/users; there are helper methods to list deleted items.
- Receipts: template placeholders include `<Orders/>`, `<Total/>`, `<Cash/>`, `<Change/>`, `<Id/>`, `<Cashier/>`, `<Date/>`.

## Screenshots / Application images
Below are all screenshots included in the repository:

![Screenshot (69)](https://github.com/user-attachments/assets/751bae79-6005-4d74-b3e8-ab57e888a292)
![Screenshot (70)](https://github.com/user-attachments/assets/6c48bfd4-17ba-4553-8d75-625a707685f7)
![Screenshot (71)](https://github.com/user-attachments/assets/75748b48-c694-4438-bc6d-a39d590a1f61)
![Screenshot (72)](https://github.com/user-attachments/assets/fb39a50e-bb11-4027-8b3e-745dc1102105)

![Screenshot (73)](https://github.com/user-attachments/assets/251063dd-60a8-4a69-9b50-0b98be99b0d8)
![Screenshot (74)](https://github.com/user-attachments/assets/baa49328-c038-4be4-bf62-2f1f6745b65c)
![Screenshot (78)](https://github.com/user-attachments/assets/5d3f26da-bf95-4a8c-a0b4-b23f9c15a408)
![Screenshot (79)](https://github.com/user-attachments/assets/a2d5a4fa-373b-40e8-8c02-9b089f46047b)

![Screenshot (80)](https://github.com/user-attachments/assets/d96f77aa-10b5-4fdd-80df-f25a50238f2f)
![Screenshot (81)](https://github.com/user-attachments/assets/2813a14d-1f53-49c8-9385-114cf8d18a46)
![Screenshot (82)](https://github.com/user-attachments/assets/3a9c1a20-4617-492c-830a-c396712799ea)
![Screenshot (86)](https://github.com/user-attachments/assets/56fa4848-b895-49c9-b611-70f05d7c525f)

![Screenshot (87)](https://github.com/user-attachments/assets/611c811b-2a5f-46ea-9874-0e6766582cf6)
![Screenshot (88)](https://github.com/user-attachments/assets/af980677-831e-4dd1-8fc6-fd1c365eebdd)
![Screenshot (89)](https://github.com/user-attachments/assets/11744bb0-1ed6-4384-8922-9102611214fc)

