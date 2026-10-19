# Personal Expense Tracker

A simple, user-friendly mobile app for recording and monitoring daily expenses, built with **C#** and **.NET MAUI**.

"D:\University_Projects\Third year projects\Mobile application development\expense_tracker_thumbnail.png"

---

## Overview

Personal Expense Tracker lets users record their everyday spending, categorise it, review past transactions, and see their total expenditure at a glance. The project deliberately keeps a small, manageable scope to demonstrate the fundamentals of mobile application development without unnecessary complexity.

## Aim

To build a simple, functional mobile app that helps users keep track of their personal spending through basic expense recording, categorisation, and spending calculations.

## Features

- Add a new expense
- Enter the expense amount
- Choose a category: **Food**, **Transport**, **Shopping**, **Bills**, or **Other**
- Record the date of the expense
- Add a short description
- View a list of recorded expenses
- Calculate and display total spending
- Delete an existing expense
- Basic input validation (e.g. required and numeric amount, valid category and date)

## App Screens

| Screen | Purpose |
|---|---|
| **Home** | Shows total spending and the number of expenses, with navigation buttons to the other screens. |
| **Add Expense** | Form to enter the amount, category, date, and description, then save the expense. |
| **Expenses** | Lists all recorded expenses and lets the user delete one. |

> UI mockups: see `docs/screens/Expense_Tracker_App_Screens.png`.

## Tech Stack

- **Language:** C#
- **Framework:** .NET MAUI (cross-platform: Android, iOS, Windows, macOS)
- **UI:** XAML with event handling
- **Storage:** Local persistence (e.g. SQLite via `sqlite-net-pcl`, or JSON file)
- **Version control:** Git and GitHub

### Concepts demonstrated

- Object-oriented programming
- User interface design
- Event handling
- Basic data storage and retrieval
- Input validation

## Suggested Project Structure

```
PersonalExpenseTracker/
├── Models/
│   └── Expense.cs              # Id, Amount, Category, Date, Description
├── Services/
│   └── ExpenseService.cs       # Add, delete, list, total (data access)
├── Views/
│   ├── HomePage.xaml(.cs)
│   ├── AddExpensePage.xaml(.cs)
│   └── ExpensesPage.xaml(.cs)
├── Resources/                  # Fonts, images, styles
├── App.xaml
├── AppShell.xaml               # Navigation
└── MauiProgram.cs
```

## Getting Started

### Prerequisites

- [.NET SDK](https://dotnet.microsoft.com/download) (version matching your MAUI workload)
- Visual Studio 2022 or later with the **.NET Multi-platform App UI development** workload (or VS Code with the .NET MAUI extension)
- An Android emulator, iOS simulator, or physical device

### Run

```bash
git clone https://github.com/<your-username>/PersonalExpenseTracker.git
cd PersonalExpenseTracker
dotnet restore
dotnet build -t:Run -f net8.0-android
```

Or open the solution in Visual Studio, pick a target device, and press **F5**.

## Scope

The first version covers only the essential features above. The following are intentionally **out of scope**: user authentication, online payments, maps, real-time services, and cloud infrastructure.

## Roadmap

- [ ] Weekly and monthly spending summaries
- [ ] Charts showing spending by category
- [ ] Search and filter
- [ ] Budget limits and spending alerts
- [ ] Export expenses to CSV
- [ ] Cloud-based data storage

## Why This Project

It is simple enough to implement quickly, yet covers key C# and mobile development concepts, leaving time for other learning areas such as data engineering.

## Author

Your Name, `rsah75159@gmail.com`

## License

Add a license of your choice (e.g. MIT).
