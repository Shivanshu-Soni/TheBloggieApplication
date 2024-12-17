Bloggie Application

A fully functional blogging platform built using .NET Core 7, leveraging ASP.NET Core Identity for authentication and Entity Framework Core for database interactions.

Features
User Authentication
Secure user registration, login, logout, and role-based access using ASP.NET Core Identity.
Blog Management
Create, read, update, and delete blog posts.
Rich content editing with tags and categories.
Database Integration
Database management with Entity Framework Core and code-first migrations.
Responsive Design
User-friendly interface optimized for mobile and desktop users.
Admin Dashboard
Admin access for managing blogs, users, and roles.
Tech Stack
Backend: ASP.NET Core 7 (C#)
Authentication: ASP.NET Core Identity
Database: SQL Server (Entity Framework Core 7)
Frontend: Razor Pages / MVC Views, Bootstrap
IDE: Visual Studio Code / Visual Studio 2022
Version Control: Git
Getting Started
Prerequisites
Ensure you have the following installed:

.NET 7 SDK
SQL Server or any compatible database.
Visual Studio Code or Visual Studio 2022
Git
Setup Instructions
Clone the Repository


git clone https://github.com/yourusername/bloggie-application.git
cd bloggie-application
Restore Dependencies
Run the following command to restore NuGet packages:


dotnet restore
Set Up the Database

Update your appsettings.json with your database connection string:


"ConnectionStrings": {
    "DefaultConnection": "Server=.;Database=BloggieDb;Trusted_Connection=True;MultipleActiveResultSets=true"
}
Apply migrations to create the database schema:

dotnet ef database update
Run the Application
Use the following command to start the project:


dotnet run
Access the Application
Open a browser and navigate to:




Add a new migration:


Copy code
dotnet ef migrations add MigrationName
Update the database:


Copy code
dotnet ef database update
