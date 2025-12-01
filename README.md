# EchoReviews - Music Album Review Platform
> [!NOTE]
> You can visit our web in: [echoreviews.site](https://echoreviews.site)
## Overview
EchoReviews is a web-based platform that allows users to explore, review, and manage their favorite music albums. Built with Spring Boot, this application provides a robust and user-friendly interface for music enthusiasts to share their thoughts and discover new music.

## Features
### User Management
- User registration and authentication system
- User profiles with customizable information
- Admin and regular user role support
- Session management for secure access
- User banning system for content moderation
- High-risk user flagging for suspicious activity
- Password hashing for secure storage
- HttpOnly cookies to prevent XSS attacks
- User-agent validation to prevent session hijacking
### Album Management
- Comprehensive album catalog with detailed information
- Album details including:
  - Title
  - Artist
  - Genre
  - Release Year
  - Cover Art
  - Description
  - Tracklist
  - Streaming Platform Links (Spotify, Apple Music, Tidal)
- Dynamic search with multiple parameters (artist, release date)
- Support for multiple artists per album
- Image upload capability for album covers
- Admin panel for managing artists and albums
### Favorites System
- Users can mark albums as favorites
- Personal favorite album collection for each user
- Easy management of favorite albums
- Database persistence of user preferences
### Review System
- Users can write and publish album reviews
- Rating system for albums
- Comment functionality on reviews
- Rich text editing with markdown support (EasyMDE)
- HTML sanitization for secure content rendering
- Review moderation by administrators
- Risk assessment for review content 
### Technical Implementation
#### Backend
- Built with Spring Boot framework
- RESTful API architecture
- Service-oriented architecture pattern
- DTO pattern for data transfer
- Query-by-example for dynamic searching
- Entity mapping with repositories
### Data Storage
- Database integration for persistent storage
- Database tables for:
  - Users
  - Albums
  - Artists
  - Reviews
  - User favorites
### Security
- Session-based authentication
- Role-based access control
- Input validation and sanitization
- CSRF protection
- Content security policy headers
- OWASP HTML Sanitizer for user-generated content
- Session invalidation on logout
### Usage
#### User Registration
1. Navigate to the registration page 
2. Fill in required information (username, email, password)
2. Submit the registration form
3. Secure password toggle for visibility control
#### Browsing Albums
1. View the complete album catalog on the home page
2. Use filters to sort by artist, genre, or year
3. Dynamic search functionality for finding specific albums
4. Click on individual albums for detailed information
#### Managing Favorites
1. Click the heart icon on any album to add it to favorites
2. Access your favorite albums through your user profile
3. Remove albums from favorites with a single click
4. Real-time updates in the database
#### Writing Reviews
1. Navigate to an album's detail page
2. Click on "Write Review"
3. Use the markdown editor for rich text formatting
4. Enter your review text and rating
5. Submit the review for publication after sanitization
---
## Project Structure
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

## Contributors
- darkxvortex
- paaul19
- M0ntoto
- noegomezz
