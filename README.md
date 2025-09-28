# 🥘 Recipe & Meal Planner App

![Node.js](https://img.shields.io/badge/node-%3E=18.x-brightgreen?logo=node.js&logoColor=white)  
![TypeScript](https://img.shields.io/badge/typescript-5.x-blue?logo=typescript&logoColor=white)  
![Next.js](https://img.shields.io/badge/next.js-14-black?logo=nextdotjs&logoColor=white)  
![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)   
![Last Commit](https://img.shields.io/github/last-commit/hibrahi000/meal_planner)  
![Build Status](https://img.shields.io/badge/build-passing-brightgreen)

A full-stack web application that helps users create, manage, and plan meals efficiently.  
Built with **Next.js**, **Node.js**, **TypeScript**, **GraphQL**, and **Hive** for schema monitoring.  
Future expansion includes **OpenAI integration** for smart meal plan suggestions.

---

## ✨ Features

- 👤 **User Accounts** – Signup, login, and manage personal profiles
- 📚 **Recipe Management** – Add, update, and delete recipes with ingredients
- 🗓️ **Meal Planning** – Create meal plans and organize recipes by day/week
- 🔒 **Authentication** – Secure login with JWT
- 📊 **GraphQL Hive Integration** – Schema registry & usage monitoring
- 🤖 **AI-Powered Suggestions (Future)** – Personalized meal plans using OpenAI

---

## 🏗️ Tech Stack

- **Frontend**: Next.js (React + TypeScript)
- **Backend**: Node.js, Express, Apollo GraphQL
- **Database**: MongoDB with Mongoose (or Postgres + Prisma if preferred)
- **Auth**: JWT-based authentication
- **Monitoring**: GraphQL Hive
- **Deployment**: Vercel (Frontend) + Render/Heroku (Backend) + MongoDB Atlas

---

## 📂 Project Structure

```
src/
├── app/ # Next.js app router pages and layouts
├── components/ # Reusable React UI components
├── lib/ # Frontend utilities (API client, auth helpers, etc.)
├── server/ # Backend (Express + Apollo GraphQL + Hive integration)
├── styles/ # Global styles and CSS
├── types/ # Shared TypeScript types (GraphQL, domain models, etc.)
└── config/ # Environment configs and constants
```

---

## 🖥️ System Architecture

```
         ┌──────────────────────┐
         │      Frontend        │
         │   Next.js (React)    │
         └─────────┬────────────┘
                   │
                   ▼
         ┌──────────────────────┐
         │      Backend         │
         │ Express + Apollo GQL │
         └─────────┬────────────┘
                   │
     ┌─────────────┼─────────────┐
     ▼             ▼             ▼
┌──────────┐ ┌───────────┐ ┌─────────────┐
│ Database │ │   Hive     │ │   Auth/JWT  │
│ MongoDB  │ │ Monitoring │ │  Validation │
└──────────┘ └───────────┘ └─────────────┘
```

---

## 🚀 Getting Started

### 1️⃣ Clone the repo

```bash
git clone https://github.com/hibrahi000/meal_planner.git
cd recipe-meal-planner
```

### 2️⃣ Install dependencies

```bash
npm install
```

### 3️⃣ Run the backend (GraphQL API)

```bash
cd src/server
npm run dev
```

### 4️⃣ Run the frontend (Next.js)

```bash
cd src/app
npm run dev
```

### 5️⃣ Open in browser

```
http://localhost:3000
```

---

## 📊 GraphQL Hive Integration

This project uses [GraphQL Hive](https://the-guild.dev/graphql/hive) to monitor schema changes and query usage.  
To set it up, add your **HIVE_API_TOKEN** to your `.env` file:

```bash
HIVE_API_TOKEN=your_token_here
```

---

## 📦 Example Recipe (XML Format)

```xml
<?xml version="1.0" encoding="UTF-8"?>
<recipe>
  <id>101</id>
  <title>Grilled Chicken Salad</title>
  <description>A healthy grilled chicken salad with avocado and lemon dressing.</description>
  <ingredients>
    <ingredient quantity="2" unit="pieces">Chicken Breast</ingredient>
    <ingredient quantity="1" unit="cup">Mixed Greens</ingredient>
    <ingredient quantity="1" unit="piece">Avocado</ingredient>
    <ingredient quantity="2" unit="tbsp">Olive Oil</ingredient>
    <ingredient quantity="1" unit="tbsp">Lemon Juice</ingredient>
  </ingredients>
  <steps>
    <step>Marinate chicken with olive oil, salt, and pepper.</step>
    <step>Grill chicken for 6–8 minutes per side until cooked.</step>
    <step>Slice avocado and mix with greens.</step>
    <step>Top salad with grilled chicken and drizzle lemon dressing.</step>
  </steps>
  <metadata>
    <prepTime>15 minutes</prepTime>
    <cookTime>20 minutes</cookTime>
    <servings>2</servings>
    <author>Hashmat Ibrahimi</author>
  </metadata>
</recipe>
```

---

## 🔮 Roadmap

- [x] Initial project setup (Next.js + Node.js + GraphQL)
- [ ] Recipe CRUD operations
- [ ] Meal planner system
- [ ] Authentication & authorization
- [ ] GraphQL Hive monitoring
- [ ] OpenAI-powered meal suggestions

---

## 📜 License

This project is licensed under the **MIT License**.

---

## 👨‍💻 Author

Built with ❤️ by **[Hashmat Ibrahimi](https://github.com/hibrahi000)**
