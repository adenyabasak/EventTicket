# EventTicket - Event Management System

EventTicket is a modern Event Management System developed using **ASP.NET Core Web API** and **ASP.NET Core MVC**. The project follows a **Backend API + Frontend MVC** architecture, where all data operations are handled by the API and consumed by the MVC application through **HttpClient**.

The application includes an Admin Panel, Dashboard, Reporting System, Authentication, Excel & PDF Export, and a modern responsive user interface.

---

# Project Architecture

```
SQL Server
     │
Entity Framework Core
     │
ASP.NET Core Web API
     │
 REST API
     │
 HttpClient
     │
ASP.NET Core MVC
     │
Modern User Interface
```

---

# Technologies

| Technology | Description |
|------------|-------------|
| ASP.NET Core MVC | Frontend Application |
| ASP.NET Core Web API | Backend Service |
| Entity Framework Core | ORM |
| SQL Server | Database |
| LINQ | Data Query |
| HttpClient | API Communication |
| Bootstrap 5 | Responsive UI |
| Chart.js | Dashboard Charts |
| Session | Authentication |
| ClosedXML | Excel Export |
| iTextSharp | PDF Export |

---

# NuGet Packages

### API

- Microsoft.EntityFrameworkCore
- Microsoft.EntityFrameworkCore.SqlServer
- Microsoft.EntityFrameworkCore.Tools
- Swashbuckle.AspNetCore

### MVC

- ClosedXML
- iTextSharp.LGPLv2.Core
- Microsoft.EntityFrameworkCore.SqlServer

---

# Project Features

- ASP.NET Core Web API
- ASP.NET Core MVC
- SQL Server Database
- Entity Framework Core
- REST API
- CRUD Operations
- HttpClient API Communication
- Session Authentication
- Admin Panel
- User Registration
- User Login
- Dashboard
- LINQ Join Reports
- LINQ GroupBy Reports
- Chart.js Dashboard
- Excel Export
- PDF Export
- Responsive Bootstrap Design

---

# Authentication

The application contains two different login systems.

### Administrator

The administrator account is predefined.

| Username | Password |
|----------|----------|
| admin | 123 |

> **Important:** The username must be entered as **admin** (lowercase).

After logging in successfully, the administrator is redirected to the **Admin Dashboard**.

---

### User

Users can

- Register
- Login
- Browse Events
- Logout

All user information is stored inside SQL Server.

---

# Database Structure

## EventTicketApi

### Event

- Id
- Title
- ImageUrl
- Date
- City

### Ticket

- Id
- Type
- Price
- EventId
- UserName

### Venue

- Id
- Name
- Capacity
- Location

---

## EventTicketMvc

### User

- Id
- FullName
- Username
- Password
- Role

### Booking

Stores reservation information.

### Payment

Stores payment information.

### Event

Consumes event data coming from the Web API.

---

# Home Page

The Home page is the landing page of the application. Users can browse all available events through a modern card-based interface. A dynamic hero section with randomly changing background images creates a modern user experience.

<img src="https://raw.githubusercontent.com/adenyabasak/EventTicket/master/images/home.png" width="100%">

---

# Login Page

The Login page allows both administrators and users to access the application.

- User Authentication
- Admin Authentication
- Session Management
- Secure Login

<img src="https://raw.githubusercontent.com/adenyabasak/EventTicket/master/images/girisyap.png" width="100%">

---

# Register Page

The Register page allows new users to create an account.

After registration, user information is stored in SQL Server and users can immediately log into the application.

<img src="https://raw.githubusercontent.com/adenyabasak/EventTicket/master/images/kayitol.png" width="100%">

---

# Event List

The Event List page displays all available events.

Administrators can

- View Events
- Update Events
- Delete Events
- View Event Details

All operations communicate with the Web API.

<img src="https://raw.githubusercontent.com/adenyabasak/EventTicket/master/images/eventlistesi.png" width="100%">

---

# Create Event

Administrators can add new events by entering

- Event Title
- Event Image
- Event Date
- Event City

The information is sent directly to the API and stored in SQL Server.

<img src="https://raw.githubusercontent.com/adenyabasak/EventTicket/master/images/eventekle.png" width="100%">

---
