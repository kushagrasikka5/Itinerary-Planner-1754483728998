# ð§³ Itinerary Planner - Smart Tour Recommendation System

A modern Java web application that recommends personalized tour packages based on user preferences. Built using **Vaadin Flow**, **Spring Boot**, and **MongoDB**.

---

## ð Features

- ð User Authentication (Login / Logout)
- ð¯ Personalized Tour Recommendations
- ð Trip Type Filtering (Adventure, Relaxation, Cultural, etc.)
- ð Preference Management (budget, dates, accommodation, food)
- ð¦ Dynamic Package Display using Vaadin Cards
- ð± Responsive UI built entirely in Java (Vaadin Flow)
- ð Admin/Custom control over tour packages via MongoDB

---

## ð§° Tech Stack

| Layer        | Technology             |
|--------------|------------------------|
| UI           | Vaadin Flow (Java-based UI framework) |
| Backend      | Spring Boot (REST-ready) |
| Database     | MongoDB (NoSQL) using Spring Data |
| Styling      | Custom CSS with CSS Variables |
| Authentication | Custom AuthService |
| Build Tool   | Maven |
| Language     | Java 17+ |

---

## ð Project Structure

```
src/
âââ main/
â   âââ java/
â   â   âââ org.vaadin.example/
â   â   â   âââ model/               # Data models (UserPreferences, TourPackage)
â   â   â   âââ repositories/        # MongoDB Repositories
â   â   â   âââ service/             # Filtering & Auth Services
â   â   â   âââ layout/              # MainLayout (Sidebar, Navigation)
â   â   â   âââ views/               # UI Views (Dashboard, Preferences, etc.)
â   âââ resources/
â       âââ application.properties   # MongoDB config
```

---

## âï¸ Getting Started

### 1. Clone the Repository
```bash
git clone https://github.com/your-username/itinerary-planner.git
cd itinerary-planner
```

### 2. Configure MongoDB
Set your MongoDB URI in `application.properties`:
```properties
spring.data.mongodb.uri=mongodb://localhost:27017/itinerary_planner
```

### 3. Run the App
Use your IDE or terminal:
```bash
./mvnw spring-boot:run
```

Access the app at:  
ð `http://localhost:8080`

---

## ð§ª Test Data

- Tour packages and preferences can be seeded via MongoDB Compass or CLI.
- Sample package structure:
```json
{
  "packageId": "goa_adventure_3d_15k",
  "destination": "Goa",
  "budgetRange": [10000, 15000],
  "tripType": "Adventure",
  "tripDuration": 3,
  "accommodation": {
    "type": "Resort",
    "budgetAllocation": 5000,
    "ratings": [3, 4],
    "amenities": ["WiFi", "Breakfast"]
  }
}
```

---

## â¨ Future Enhancements

- ð Google Maps Integration for destinations
- ð§  AI-powered smart recommendations
- ð Custom Itinerary Planner
