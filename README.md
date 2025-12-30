# 🎧 EchoReviews — Music Album Review Platform

🌐 **Website:** [echoreviews.site](https://echoreviews.site)

EchoReviews is a web-based platform that allows users to explore, review, and manage their favorite music albums.  
Built with **Spring Boot**, it combines an intuitive design with a solid architecture that makes it easy for music lovers to share opinions and discover new artists.

---

## 🚀 Main Features

### 👤 User Management
- User registration and authentication system.  
- Customizable user profiles.  
- Support for **admin** and **regular user** roles.  
- Secure session management.  
- User banning and suspicious activity flagging system.  
- Password hashing for secure storage.  
- **HttpOnly cookies** to prevent XSS attacks.  
- **User-Agent validation** to prevent session hijacking.  

### 💿 Album Management
- Comprehensive album catalog with detailed information:
  - Title  
  - Artist(s)  
  - Genre  
  - Release year  
  - Cover art  
  - Description  
  - Tracklist  
  - Streaming links (Spotify, Apple Music, Tidal)
- Dynamic search with multiple parameters.  
- Support for **multiple artists per album**.  
- Image upload capability for album covers.  
- Admin panel for managing artists and albums.  

### ❤️ Favorites System
- Mark albums as favorites.  
- Personal favorites collection for each user.  
- Easy to add/remove and stored persistently in the database.  

### 📝 Review System
- Write and publish album reviews.  
- Rating system for albums.  
- Comment functionality on reviews.  
- Rich text editing with **Markdown (EasyMDE)**.  
- **HTML sanitization** for safe content rendering.  
- Review moderation and content risk assessment.  

---

## ⚙️ Technical Implementation

### 🧩 Backend
- Built using **Spring Boot** framework.  
- **RESTful API** architecture.  
- **Service-Oriented Architecture (SOA)** pattern.  
- **DTO pattern** for data transfer.  
- **Query-by-example** for dynamic searching.  
- JPA repositories for entity mapping.  

### 🗄️ Data Storage
Database tables include:
- `users`
- `albums`
- `artists`
- `reviews`
- `user_favorites`

---

## 🔐 Security
- Session-based authentication.  
- Role-based access control.  
- Input validation and sanitization.  
- **CSRF protection**.  
- **Content Security Policy (CSP)** headers.  
- **OWASP HTML Sanitizer** for user-generated content.  
- Session invalidation on logout.  

---

## 🧭 How to Use EchoReviews

### 🪪 User Registration
1. Navigate to the registration page.  
2. Fill in your username, email, and password.  
3. Submit the registration form.  
4. Use the visibility toggle to show/hide your password securely.

### 🎶 Browsing Albums
1. Explore the full album catalog on the home page.  
2. Filter by artist, genre, or year.  
3. Use the dynamic search bar to find specific albums.  
4. Click on an album for detailed information.

### ⭐ Managing Favorites
1. Click the ❤️ icon to add an album to your favorites.  
2. Access your favorites from your profile page.  
3. Remove albums from favorites with one click.  
4. Changes are saved automatically in real-time.

### 🖊️ Writing Reviews
1. Go to an album’s detail page.  
2. Click on **"Write Review"**.  
3. Use the Markdown editor for rich text formatting.  
4. Enter your review text and rating.  
5. Submit your review for publication (sanitized before rendering).  

---

## 🧱 Project Structure
```
project-grupo-5/
├── src/
│   ├── main/
│   │   ├── java/
│   │   │   └── com/echoreviews/
│   │   │       ├── config/
│   │   │       ├── controller/
│   │   │       │   ├── api/
│   │   │       ├── dto/
│   │   │       ├── mapper/
│   │   │       ├── model/
│   │   │       ├── repository/
│   │   │       ├── security/
│   │   │       ├── service/
│   │   │       ├── util/
│   │   │       └── EchoReviewsApplication.java
│   │   └── resources/
│   │       ├── static/
│   │       │   ├── css/
│   │       │   └── images/
│   │       ├── templates/
│   │       │   ├── album/
│   │       │   ├── artist/
│   │       │   ├── auth/
│   │       │   ├── fragments/
│   │       │   ├── review/
│   │       │   ├── reviews/
│   │       │   ├── user/
│   │       │   └── error.html
│   │       └── application.properties
├── pom.xml
└── README.md
```

---

## 👥 Contributors
- **darkxvortex**  
- **paaul19**  
- **Mntt05**  
- **noegomezz**
```
