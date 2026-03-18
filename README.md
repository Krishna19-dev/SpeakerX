# SpeakerX – Project Context & Documentation

## 1. Project Overview

SpeakerX is a modern web-based platform that connects event organizers with speakers. It works as a marketplace where organizers can discover, compare, and book speakers based on their requirements such as topic, budget, and availability.

Designed as a clean, minimal, and scalable startup product similar to Stripe, Notion, or Linear.

---

## 2. Core Objective

- Simplify speaker discovery
- Provide transparent pricing
- Enable direct communication
- Allow seamless booking

---

## 3. Target Users

### Event Organizers
- College students organizing events
- Corporate teams
- Workshop hosts

### Speakers
- Motivational speakers
- Tech speakers
- Industry experts
- Student speakers

---

## 4. Key Functional Modules

### 4.1 Authentication Module
- Users can sign up/login
- Role-based system: **Organizer** | **Speaker**

### 4.2 Speaker Module
- Create/edit profile: Name, Bio, Topics, Pricing, Experience, Profile image
- Set availability

### 4.3 Organizer Module
- Search, filter, and view speaker profiles
- Send booking requests

### 4.4 Search & Filter System
- Filter by: Topic, Price range, Rating, Availability

### 4.5 Booking System
- Organizer sends request → Speaker accepts/rejects
- Status: `Pending` / `Accepted` / `Rejected`

### 4.6 Chat System
- Direct messaging between organizer and speaker

### 4.7 Rating & Review System
- Organizers rate speakers after events

---

## 5. Pages & Navigation

| Page | Description |
|------|-------------|
| Home | Navbar, Hero, Featured Speakers, Categories |
| Explore Speakers | Grid of cards with filters |
| Speaker Profile | Full details + Book Now button |
| Login / Signup | Auth pages |
| About | Platform explanation & How It Works |

---

## 6. Technical Architecture

| Layer | Stack |
|-------|-------|
| Frontend (initial) | HTML, CSS, JavaScript |
| Frontend (future) | React + Tailwind |
| Backend | Node.js + Express |
| Database | MongoDB |

---

## 7. Data Models

### User
```json
{ "id", "name", "email", "password", "role": "speaker | organizer" }
```

### Speaker Profile
```json
{ "userId", "bio", "topics", "price", "rating", "availability" }
```

### Booking
```json
{ "organizerId", "speakerId", "eventDetails", "status": "pending | accepted | rejected" }
```

---

## 8. UI/UX Guidelines

- Minimal and modern design
- Black & white monochrome theme
- Inter font, clean typography
- Card-based, fully responsive layout

---

## 9. Future Scope

- Payment integration
- AI speaker recommendations
- Verified badges & featured listings
- Mobile app

---

## 10. Development Priority (MVP First)

1. Backend APIs (Auth + Speakers + Bookings)
2. Frontend pages (HTML/CSS)
3. API integration
4. Auth flow
5. UI polish
