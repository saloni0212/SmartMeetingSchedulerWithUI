# 🗓️ MeetingSchedulerWithUI

A smart ASP.NET MVC web application for managing and scheduling meetings efficiently, developed during my internship at **Fendahl Technology, Nagpur**.

![License](https://img.shields.io/badge/license-MIT-green)
![Platform](https://img.shields.io/badge/platform-Windows-lightgrey)
![Tech](https://img.shields.io/badge/tech-stack-blue)

## 📌 About the Project

The **MeetingSchedulerWithUI** is a web-based meeting scheduler built with ASP.NET MVC (.NET Framework 4.8) and C#. It provides an intuitive interface for creating, viewing, editing, and deleting meetings and helps users find **free time slots** between 9:00 AM to 5:00 PM by dynamically analyzing existing meetings.

This application is ideal for academic or organizational environments where managing time effectively is crucial.

## 🔧 Tech Stack
---------------------------------------------------
| Component      | Technology / Tool              |
|----------------|--------------------------------|
| Framework      | ASP.NET MVC (.NET Framework)   |
| Language       | C#                             |
| ORM            | Entity Framework 6             |
| Database       | SQL Server (LocalDB)           |
| Frontend       | Razor, HTML, CSS, Bootstrap 4  |
| IDE            | Visual Studio 2019             |
---------------------------------------------------

## ✨ Features

- 📝 Full CRUD operations for meetings
- ⏰ Dynamic free slot calculation
- 💾 Persistent storage via SQL Server
- 📱 Responsive UI with Bootstrap
- 🔧 Easily extendable for:
  - Multi-user authentication
  - Calendar integrations
  - Email notifications

## 📸 Screenshots
Uploaded in the Screenshots folder.

## 📁 Project Structure

---------------------------------------------------
|                 |    MeetingSchedulerWithUI     |
|-----------------|-------------------------------|
| Controllers     | MeetingsController.cs         |
|                 |                               |
| Models          | Meeting.cs                    | 
|                 | MeetingContext.cs             |
|                 |                               |
| Views/Meetings  | Index.cshtml                  |
|                 | Create.cshtml                 |
|                 | Edit.cshtml                   |
|                 | Delete.cshtml                 |
|                 | Details.cshtml                |
|                 | FreeSlots.cshtml              |
--------------------------------------------------


## 🚀 How to Run

1. Clone this repo:  
   ```bash
   git clone https://github.com/your-username/MeetingSchedulerWithUI.git

2. Open the solution in Visual Studio 2019

3. Restore NuGet packages

4. Run the application using IIS Express (F5)


## 🧠 Algorithm - Free Slot Calculation

Define working hours (9 AM – 5 PM)

Fetch all meetings for a selected date

Sort meetings by start time

Check gaps between:

Start of workday and first meeting

End of one meeting and start of next

End of last meeting and end of workday

Return gaps as available time slots
Make sure SQL Server LocalDB is installed and running.
