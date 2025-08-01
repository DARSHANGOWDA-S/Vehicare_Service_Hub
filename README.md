# 🚗 Vehicare Service Hub (Blazor + Web API)

**Vehicare_Service_Hub** is an all-in-one platform for vehicle service booking, maintenance tracking, and admin-customer interaction. Built using **Blazor Server**, **ASP.NET Core Web API**, and **Bootstrap**, it provides a modern UI and efficient backend to manage your service center operations smoothly.

---

## ✨ Features

- 📅 Book vehicle services online
- 🔍 Track service and maintenance history
- 👨‍🔧 Admin dashboard to manage services
- 📬 Notifications and status updates
- 🧾 Service records stored in SQL database
- 🌐 Responsive UI using Bootstrap

---

## 🛠️ Tech Stack

- **Frontend:** Blazor Server (.NET 6+)
- **Backend:** ASP.NET Core Web API
- **UI Framework:** Bootstrap
- **Database:** SQL Server + Entity Framework Core
- **IDE:** Visual Studio 2022+ / Visual Studio Code
- **Tools:** Git, EF CLI, Postman

---

## 📁 Project Structure

Vehicare_Service_Hub/
│
├── BlazorServer.CarService.sln # Solution file
├── Program.cs # Entry point
├── App.razor / _Imports.razor # Main app files
├── appsettings.json # Configuration file
├── ApiServices/ # Service layer for APIs
│ └── BookingFolder/ # Booking logic
│ ├── IBookingRepository.cs
│ └── BookingRepository.cs
├── Models/ # Data models
├── Pages/ # Razor pages (UI)
└── wwwroot/ # Static assets (CSS, JS)

yaml
Copy
Edit

---

## ▶️ How to Run This Project

### 🔧 Prerequisites

- [.NET 6 SDK or later](https://dotnet.microsoft.com/download)
- SQL Server or LocalDB installed
- Visual Studio 2022+ or VS Code
- Git installed

---

### 📦 Setup Steps

#### 1. Clone the Repository

```bash
git clone https://github.com/your-username/Vehicare_Service_Hub.git
cd Vehicare_Service_Hub
2. Open the Solution
Launch BlazorServer.CarService.sln using Visual Studio.

3. Configure Database
Open appsettings.json or appsettings.Development.json

Edit the ConnectionStrings like below:

json
Copy
Edit
"ConnectionStrings": {
  "DefaultConnection": "Server=(localdb)\\MSSQLLocalDB;Database=VehicareDB;Trusted_Connection=True;"
}
You may use your own server or instance name.

4. Apply EF Core Migrations
If the project uses Entity Framework for database migration:

bash
Copy
Edit
dotnet ef database update
You can also use the Package Manager Console in Visual Studio:

powershell
Copy
Edit
Update-Database
5. Run the Application
Press F5 or click Run in Visual Studio.

The app will start on https://localhost:5001 or http://localhost:5000.

🌐 API Testing (Optional)
You can use Postman or any HTTP client to test the API endpoints.

Base URL (default):

bash
Copy
Edit
https://localhost:5001/api/
Some sample endpoints:

GET /api/bookings

POST /api/bookings

GET /api/bookings/{id}

🤝 Contributing
Pull requests are welcome.
If you want to add features, feel free to fork this repo and contribute.

📫 Contact
Created with 💙 by Darshan S
📧 Email: darshangowda4618.com
🌐 LinkedIn:www.linkedin.com/in/darshan-s-777332337

⭐ If you found this useful, star this repository to support the project!

