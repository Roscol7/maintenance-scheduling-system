# Maintenance Scheduling System

## Description
Enterprise-level maintenance scheduling system built with ASP.NET Core Web API and SQL Server.  
Allows organizations to plan, manage, and reserve maintenance of technological assets while respecting business rules, schedules, and department allocations.

## Features
- Role-based authentication using SQL column (`UserType`) for roles: Admin, Technician, Employee
- Calendar-based scheduling using **FullCalendar**
- Time slot reservations in 3 fixed blocks: 9–11 AM, 11–1 PM, 1–3 PM
- Maximum of 1 equipment per time slot (3 per day)
- Considers business days and holidays
- Maintenance cancellation (reservations cannot be deleted)
- Equipment assignment and status management

## Tech Stack
- ASP.NET Core Web API
- Entity Framework Core
- SQL Server (with seed/demo data)
- Bootstrap
- FullCalendar
- JavaScript for frontend interactions

## Architecture
**Clean Architecture**:
- `Domain`: Entities and business logic
- `Application`: Services, DTOs, and use cases
- `Infrastructure`: Database context, repositories
- `API`: Controllers, authentication, and routing

## Screenshots
<img width="940" height="423" alt="image" src="https://github.com/user-attachments/assets/52bd1115-2b54-4b0a-a4e7-1127b8710f7a" />
<img width="940" height="449" alt="image" src="https://github.com/user-attachments/assets/db0281a7-3b4a-45f2-86a1-c24975573d7c" />
<img width="940" height="451" alt="image" src="https://github.com/user-attachments/assets/e40eda05-42e8-4631-b9d4-48cb660c0a7c" />
<img width="940" height="416" alt="image" src="https://github.com/user-attachments/assets/6dbb9954-cb27-44cb-a24f-12c74b3990cc" />
<img width="723" height="512" alt="image" src="https://github.com/user-attachments/assets/a6960f95-d303-4153-ac25-03dae982e588" />
<img width="784" height="650" alt="image" src="https://github.com/user-attachments/assets/f338e553-f253-41da-a39a-bcb63ddebc27" />
<img width="940" height="486" alt="image" src="https://github.com/user-attachments/assets/5fc15166-5559-43c8-8d88-459621b6a7c9" />
<img width="940" height="642" alt="image" src="https://github.com/user-attachments/assets/df1755a4-2273-46fe-bc45-5093cfd826d7" />
<img width="940" height="478" alt="image" src="https://github.com/user-attachments/assets/5ac72a61-70c4-40a8-bc90-207826efaefc" />


## How to Run
1. Clone repository
2. Update connection string in `appsettings.json`
3. Restore NuGet packages
4. Apply migrations or run `database.sql` to seed database
5. Start API project (Visual Studio or `dotnet run`)
6. Open browser and navigate to `https://localhost:5001` (or configured port)
