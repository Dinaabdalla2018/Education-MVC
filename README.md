# Student Management System

This is a web application for managing students and grades that allows instructors and admins to add, edit, and delete students, view grades, and search by name and date. The application provides two types of users, Instructor and Admin. The application is built using ASP.NET Core MVC, and provides authentication and authorization to ensure secure access to the functionalities.

## Prerequisites 

- Visual Studio 2020
- .NET Core 7
- SQL Server 2019 or later

## Getting Started

1. Clone the repository to your local machine.
2. Open the solution file `Education.sln` in Visual Studio.
3. Open the `appsettings.json` file in the `Education.Web` project and replace the database connection string with your own.
4. Open the Package Manager Console in Visual Studio and run the following command to create the database tables:

```
Update-Database
```

5. Build and run the solution in Visual Studio. This will launch the application on `http://localhost:5000`.

## Features

### Instructor

The instructor can perform the following actions:

- Login to the application.
- Add, edit, and delete students as requested by the admin.
- View grades of students and search by name and date.
- View their own lesson and all lessons.

### Admin

The admin can perform the following actions:

- Login to the application.
- Add, edit, and delete students and instructors.
- Accept or reject requests of instructor.
- View grades of students and search by name and date.
- View their own lesson and all lessons.

## Authentication and Authorization

The application provides authentication and authorization to ensure secure access to the functionalities. The authentication process is implemented using ASP.NET Core Identity, and the authorization is implemented using roles. When a user logs in, the server generates a cookie that contains the user's session data. On subsequent requests to the server, the server verifies the cookie and grants or denies access to the requested resource based on the user's role and permissions.

## Built With

- ASP.NET Core MVC - A back-end web application framework.
- SQL Server - A relational database management system.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
