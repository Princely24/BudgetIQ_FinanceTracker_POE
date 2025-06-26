# BudgetIQ - Smart Personal Finance Manager_POE

<p align="center">
  <img src="app/src/main/res/mipmap-xxxhdpi/ic_launcher_round.png" alt="BudgetIQ Logo" width="120"/>
</p>

BudgetIQ is a modern Android application designed to help users manage their personal finances effectively. Built with Jetpack Compose, Room, Hilt, and MVVM, it offers a seamless and intuitive experience for tracking expenses, setting budgets, and achieving financial goals.

---

## Features

- **User Authentication**: Secure login and registration system.
- **Expense Tracking**: Add, view, and manage expenses with category assignment and receipt capture.
- **Category Management**: Organize expenses with customizable categories and view recent categories.
- **Budget Goals**: Set monthly budget goals per category and track your progress visually.
- **Achievements & Badges**: Earn badges for financial milestones (e.g., Consistency, Frugal spending).
- **Analytics & Insights**:
  - Visual bar and pie charts for spending by category.
  - Time period selector (week, month, year) for dynamic analytics.
  - Dashboard with summaries, top categories, and recent expenses.
- **Material Design 3**: Modern, responsive UI with dynamic theming.
- **Receipt Management**: Capture and store receipt images using CameraX.
- **Data Persistence**: All data is stored locally using Room.

---

## Screenshots

---

## Tech Stack

- **UI Framework**: Jetpack Compose
- **Architecture**: MVVM (Model-View-ViewModel)
- **Dependency Injection**: Hilt
- **Database**: Room
- **Concurrency**: Kotlin Coroutines & Flow
- **Navigation**: Jetpack Navigation Compose
- **Image Loading**: Coil
- **Camera**: CameraX
- **Design System**: Material Design 3

---

## Architecture Overview

The app follows Clean Architecture principles and is organized into the following layers:

- **UI Layer**: Compose UI screens, reusable components, and ViewModels.
- **Data Layer**: Room entities, DAOs, and repositories for expenses, categories, users, badges, and budget goals.
- **Dependency Injection**: All repositories and data sources are injected using Hilt.
- **Navigation**: Centralized navigation using Jetpack Compose Navigation.

### Main Packages

- `ui/screens/` - All main screens (Home, AddExpense, BudgetGoals, Achievements, Categories, etc.)
- `ui/components/` - Reusable Compose UI components.
- `ui/viewmodels/` - ViewModels for each screen, handling state and business logic.
- `data/model/` - Data entities (Expense, Category, BudgetGoal, Badge, User).
- `data/dao/` - Room DAOs for database access.
- `data/repository/` - Repositories abstracting data access.
- `di/` - Hilt modules for dependency injection.
- `util/` - Utility classes and converters.

---

## Key Features in Detail

### 1. Dashboard & Analytics
- **Dynamic Bar and Pie Charts**: Visualize spending by category.
- **Time Period Selector**: Filter analytics by week, month, or year.
- **Budget Progress**: See your total and per-category budget progress with color cues.
- **Recent Expenses & Categories**: Quick overview of your latest activity.

### 2. Budget Goals
- Set minimum and maximum budget goals per category.
- Visual progress bars for each goal.
- Edit and manage goals easily.

### 3. Achievements & Badges
- **Consistency Badge**: Awarded for logging expenses 7 days in a row.
- **Frugal Badge**: Awarded for spending less than 80% of your monthly budget.
- All badges are persistent and shown on the dashboard and Achievements screen.

### 4. Categories
- Add, edit, and delete custom categories.
- Recent categories are highlighted for quick access.

### 5. Expense Management
- Add expenses with amount, description, category, date, and optional receipt photo.
- View, edit, and delete expenses.
- Filter and analyze expenses by time period.

---

## Prerequisites

- Android Studio Hedgehog | 2023.1.1 or newer
- Minimum SDK: 24
- Target SDK: 34
- Kotlin version: 1.9.0 or newer

---

## Getting Started

1. **Clone the repository:**
   ```bash
   git clone https://github.com/yourusername/BudgetIQ.git
   ```

2. **Open the project in Android Studio**

3. **Sync the project with Gradle files**

4. **Run the app** on an emulator or physical device

---

## Building

To build the app, you can use Android Studio or run the following command:

```bash
./gradlew assembleDebug
```

For release build:
```bash
./gradlew assembleRelease
```

---

## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

---

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details

---

## Acknowledgments

- Material Design 3 for the modern UI components
- Android Jetpack libraries
- All contributors who help improve BudgetIQ

---

## Contact

Princely Makhwara (ST10263265) - [LinkedIn](https://www.linkedin.com/in/princely-makhwara-096285197)  
Aime Ndumuhire (ST10255663) - [LinkedIn](https://www.linkedin.com/in/aime-ishimwe-675557272/)  
Fortunate Majere (ST10231459) - [LinkedIn](https://za.linkedin.com/in/fortunate-majere-205933289)  
Sabelo Sibiya (ST10327016) - [LinkedIn](https://za.linkedin.com/in/sabelo-sibiya-712935289)  
Enrique Arendse (10302006) - [LinkedIn](https://www.linkedin.com/in/enrique-arendse-033700231?utm_source=share&utm_campaign=share_via&utm_content=profile&utm_medium=android_app)

Project Link: [https://github.com/yourusername/BudgetIQ](https://github.com/yourusername/BudgetIQ)
