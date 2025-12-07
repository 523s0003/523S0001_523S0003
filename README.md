[readme.txt](https://github.com/user-attachments/files/24015215/readme.txt)
AWE Electronics – Final Project Software Engineering – Semester 1 (2025–2026)

=====================================================
Team Members
=====================================================
1. Nguyen Tien Khoa – 523S0003
2. Phu Quang An – 523S0001

=====================================================
GitHub Repository Link
=====================================================
https://github.com/523s0003/523S0001_523S0003

(Note: The GitHub repository is used only for project reference as required in the assignment. 
The full source code and database are included inside the submission .zip file.)

=====================================================
Development Environment
=====================================================
IDE:
  • Microsoft Visual Studio 2022 (ASP.NET MVC Framework)

Programming Language:
  • C# (ASP.NET MVC 5)
  • Razor Views (.cshtml)
  • HTML5, CSS3, JavaScript
  • LINQ

Frameworks / Libraries:
  • ASP.NET MVC 5
  • ADO.NET (for database interaction)
  • Bootstrap 5.3 (UI components and layout)
  • FontAwesome (icons)
  • jQuery (DOM interaction)

Database:
  • Microsoft SQL Server LocalDB / SQL Server Express

=====================================================
How to Run / Compile the Source Code
=====================================================

1. Extract the submission .zip file.
   Folder structure should look like:
   - /SourceCode/
   - database.sql
   - readme.txt
   - Report.pdf
   - SE_Rubrics_TeamContribution.xlsx
   - Presentation.pptx
   - Demo.mp4

2. Open the project:
   - Launch Visual Studio 2022
   - Click **"Open a project or solution"**
   - Select the file: **AWE_Agent_WebApp.sln**

3. Restore Packages:
   - Visual Studio will automatically restore required NuGet packages when the project loads.

4. Configure the Database:
   - Open SQL Server Management Studio (SSMS)
   - Create a new database (e.g. AWE_Electronics)
   - Run the provided **database.sql** file to create tables and insert sample data

5. Update the Database Connection String:
   - Go to **Web.config**
   - Find `<connectionStrings>`
   - Update:
        ```
        <add name="AWEConnection"
             connectionString="Data Source=YOUR_SERVER_NAME;Initial Catalog=AWE_Electronics;Integrated Security=True;"
             providerName="System.Data.SqlClient" />
        ```

6. Run the Application:
   - Press **F5** or click **Start Debugging**
   - The home page will open at:
        https://localhost:xxxx/Home/Index

=====================================================
Project Features
=====================================================
✔ Homepage with categories, banner, hover effects  
✔ Category pages (Apple, Laptops, Cellphones, etc.)  
✔ Product details page  
✔ Shopping Cart (Add, Remove, Update quantity)  
✔ Checkout page (shipping information + order summary)  
✔ Payment confirmation page  
✔ Login page (UI only)  
✔ MVC architecture (Models, Views, Controllers)  

=====================================================
Notes
=====================================================
- All images used in the project are placed under /Images folder.
- The project follows the required MVC structure.
- This readme.txt contains all information required by the assignment rubric.

=====================================================
End of Document
=====================================================
