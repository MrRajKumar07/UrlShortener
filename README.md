# 🔗 URL Shortener

A simple and efficient **URL Shortener** built with **Java**.  
It takes a long URL and generates a short, unique link for easier sharing and management.

---

## ✨ Features
- Shorten long URLs into unique short links  
- Redirect short links to original URLs  
- Lightweight and fast  
- Clean, minimal Java implementation  

---

## 🛠️ Tech Stack
- **Java** (Core logic)  
- **Maven** (Build tool, dependency management)  

---

## 📂 Folder Structure
```
UrlShortener/
├── src/
│   ├── main/java/
│   │   └── com/demo/urlshortener/
│   │       ├── UrlShortenerApplication.java   # Main entry point
│   │       ├── controller/                   # Handles URL shortening & redirection
│   │       ├── service/                      # Core logic for generating & mapping URLs
│   │       └── repository/                   # In-memory or DB persistence
│   └── resources/
│       └── application.properties            # Configurations
├── pom.xml                                   # Maven build file
└── README.md
```
---

## 🚀 Getting Started

### Prerequisites
- Java 17+
- Maven 3.6+

### Setup & Run
```bash
# Clone the repo
git clone https://github.com/MrRajKumar07/UrlShortener.git
cd UrlShortener

# Build and run
mvn clean install
mvn spring-boot:run
```

### Usage

- Once running (default: http://localhost:8080):
- POST /shorten → Provide a long URL, get a short one back
- GET /{shortCode} → Redirects to the original long URL
