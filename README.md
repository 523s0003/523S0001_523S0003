[readme.txt](https://github.com/user-attachments/files/24015093/readme.txt)
==============================
AWE Electronics - Final Project
Software Engineering - Semester 1 (2025–2026)

Team Members
1. Nguyen Tien Khoa – 523S0003
2. Phu Quang An – 523S0001
==============================


========================================
1. GitHub Repository Link
========================================

https://github.com/523s0003/523S0001_523S0003

========================================
2. Technologies, Frameworks, and Libraries
========================================
- ASP.NET MVC 5 (Model–View–Controller)	
- .NET Framework 4.8
- C# Programming Language
- Bootstrap 5.3.2 (layout and responsive UI)
- jQuery (basic client-side interactions)
- HTML5, CSS3, JavaScript
- Visual Studio 2022
- IIS Express (local development web server)

NuGet packages (key ones):
- Microsoft.AspNet.Mvc
- Microsoft.AspNet.Razor
- Microsoft.AspNet.WebPages
- jQuery
- Bootstrap


========================================
3. IDE and Development Environment
========================================
- IDE: Microsoft Visual Studio 2022 (Community Edition)
- Target framework: .NET Framework 4.7.2 / 4.8
- Project type: ASP.NET MVC Web Application
- Web server for debugging: IIS Express
- Operating system used for development: Windows 10 / 11


========================================
4. How to Run the Application
========================================

STEP 1 – Clone or Download the Repository
-----------------------------------------
Option 1: Clone with Git

    git clone https://github.com/your-team/awe-electronics-finalproject.git

Option 2: Download ZIP from GitHub and extract it.

The main solution file is:
    AWE_Agent_WebApp.sln


STEP 2 – Open the Solution in Visual Studio
-------------------------------------------
1. Open Visual Studio.
2. Go to: File → Open → Project/Solution.
3. Select: AWE_Agent_WebApp.sln.


STEP 3 – Restore NuGet Packages
-------------------------------
In Visual Studio:
- Right-click on the Solution → “Restore NuGet Packages”.

This will restore Bootstrap, jQuery, and required ASP.NET MVC libraries.


STEP 4 – Build the Project
--------------------------
From the menu:
- Build → Build Solution  (shortcut: Ctrl + Shift + B)

If the build succeeds, there should be **no red errors** in the Error List.


STEP 5 – Run the Application
----------------------------
Press **F5** or click the **Start (▶)** button.

The browser will open at a URL similar to:
    https://localhost:xxxx/Home/Index

Main features:
- Homepage with banner and 6 clickable categories.
- Navigation bar: Menu, Black Friday Deals, Top Deals, Deal of the day, News, Shopping Cart, Gift cards.
- Shopping Cart page with item list and order summary.
- Checkout page (shipping information + order summary).
- Payment page (payment method + card details).
- Simple login page (Account → Login).


========================================
5. How to Compile / Build
========================================
The project is compiled automatically when you:

- Press **Ctrl + Shift + B** (Build Solution), or
- Press **F5** (Start Debugging, which also builds the solution).

If build errors appear:
- Check that all NuGet packages are restored.
- Check that the target framework is .NET Framework 4.7.2 or 4.8.
- Check that image paths under the Images/ folder are correct.
- Check that controller names and action names match the Views and routes.


========================================
6. Database and Data Storage
========================================
For this project, no real SQL database is required.

- The shopping cart is stored in **Session**:
  - `Session["Cart"]` holds a list of `CartItem`.
- Checkout and payment are simulated.
- No persistent data is stored in a database.

(If needed, a separate .sql file can be added later to demonstrate a possible schema.)


========================================
7. Project Structure Overview
========================================

AWE_Agent_WebApp/
│
├── Controllers/
│   ├── HomeController.cs
│   ├── CategoryController.cs
│   ├── ShoppingCartController.cs
│   ├── CheckoutController.cs
│   └── AccountController.cs
│
├── Models/
│   ├── CartItem.cs
│   └── Product.cs    (if used)
│
├── Views/
│   ├── Home/
│   │   └── Index.cshtml
│   ├── Category/
│   │   └── *.cshtml  (category pages)
│   ├── ShoppingCart/
│   │   └── Index.cshtml
│   ├── Checkout/
│   │   ├── Index.cshtml        (Shipping)
│   │   ├── Payment.cshtml      (Payment)
│   │   └── OrderSuccess.cshtml (Confirmation)
│   ├── Account/
│   │   └── Login.cshtml
│   └── Shared/
│       └── _Layout.cshtml
│
├── Images/
│   ├── apple_imac.jpg
│   ├── cat_fridge.jpg
│   ├── cat_game.jpg
│   ├── cat_laptop.jpg
│   ├── cat_phone.jpg
│   ├── cat_tv.jpg
│   └── banner.jpg
│
└── Web.config


========================================
8. Known Issues and Limitations
========================================
- Shopping cart data is stored in Session only, so it is cleared when:
  - the server restarts, or
  - the browser session expires.
- Login is a simple demo (hard-coded email/password). No real authentication or database.
- Payment is simulated; there is no integration with real payment gateways (PayPal, Stripe, etc.).
- No responsive mobile optimization beyond what Bootstrap provides by default.


========================================
9. Credits
========================================
This project is developed as a group assignment for the
Software Engineering course (Semester 1, 2025–2026).

Team:
- Nguyen Tien Khoa – 523S0003
- Phu Quang An – 523S0001

Supervisor / Lecturer:
Pham Thai Ky Trung
========================================
END OF README
========================================
