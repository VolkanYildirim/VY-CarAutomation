# 🚘 VY-CarAutomation

![C#](https://img.shields.io/badge/C%23-239120?style=for-the-badge&logo=c-sharp&logoColor=white)
![Database](https://img.shields.io/badge/Database-MS_Access-blue?style=for-the-badge)
![Status](https://img.shields.io/badge/Status-Refactoring_Required-orange?style=for-the-badge)

A comprehensive desktop application built with C# and Microsoft Access Database for vehicle management and tracking automation. 

### ⚠️ Development Status: Architecture Refactoring
**Known Issue:** The current legacy version (`v1.0`) contains a 32-bit (x86) Microsoft Access OLEDB driver dependency (`Microsoft.ACE.OLEDB.12.0`). This currently conflicts with modern 64-bit (x64) execution environments like Visual Studio 2022, throwing a `System.InvalidOperationException`.
*Next Steps:* An architecture refactoring loop (forcing x86 execution or database migration) is scheduled to resolve this environment mismatch.

### ⚙️ Security & Privacy (Secure by Design)
- **Local Database Isolation:** All vehicle and user operations are strictly stored locally within the `.mdb` file. 
- **Zero Cloud Exposure:** No external API dependencies or cloud synchronization, eliminating the risk of unauthorized external access to the vehicle database.

### 🔧 Build & Audit
1. Open `Proje1.sln` using Visual Studio.
2. *Note for Auditors:* Attempting to run this on a pure 64-bit environment without the 32-bit Access Database Engine will trigger the known provider error mentioned above.
