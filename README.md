# 📚 BookDepo

## Project Overview
BookDepo is an online Book shop that provides a web-based platform for purchasing and managing books. Users can browse through available books, view details, and place orders, while admins have the ability to manage books and their associated categories.

## Features

### User Features
- **Browse Books**: Customers can view all available books along with details like title, author, price, and category.
- **Order Books**: Users can place orders for the books they wish to purchase.
  
### Admin Features
- **Manage Books**: Admins can add, edit, and delete books. While creating a book, admins can assign it to a category.
- **Manage Categories**: Admins can add and edit book categories to organize the books efficiently.

## Tech Stack
- **Backend**: ASP.NET Core MVC
- **Database**: Microsoft SQL Server
- **ORM**: Entity Framework Core

## Installation & Setup

### Prerequisites
- Visual Studio 2022 (with .NET 8.0 SDK installed)
- SQL Server (local or cloud-based)

### Required NuGet Packages
- `Microsoft.EntityFrameworkCore`
- `Microsoft.EntityFrameworkCore.SqlServer`
- `Microsoft.EntityFrameworkCore.Tools`
- `Microsoft.AspNetCore.Identity.EntityFrameworkCore`

### Steps to Run in Visual Studio

1. **Clone the repository**:

    ```bash
    git clone https://github.com/Yashgabani845/BookDepo.git
    ```

2. **Open the solution**: Open the `.sln` file in Visual Studio.

3. **Set up the database connection**: 
   - In the `appsettings.json` file, update the connection string to match your local SQL Server configuration:
   
   ```json
   "ConnectionStrings": {
     "DefaultConnectionString": "Server=YOUR_SERVER_NAME;Initial Catalog=bookdepo;Integrated Security=True;Connect Timeout=30;"
   }
   ```

4. **Run migrations**: Open the NuGet Package Manager Console and run the following commands to create the database:
   
   ```bash
   update-database
   ```

5. **Run the project**: Start the application by running it with or without debugging.

---
