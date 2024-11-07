# Pet App Project

Welcome to the **Pet App Project**! This application is a modern web-based reimagining of the classic Tamagotchi-style game, allowing users to interact with and care for a virtual pet. The project showcases a full-stack web application, with separate frontend and backend components working in harmony.

## Table of Contents

- [Project Overview](#project-overview)
- [Features](#features)
- [Tech Stack](#tech-stack)
- [Project Structure](#project-structure)
- [Setup Instructions](#setup-instructions)
- [Frontend](#frontend)
- [Backend](#backend)
- [Demo](#demo)

## Project Overview

The Pet App allows users to:

- Interact with a virtual pet by feeding, playing, and cleaning it.
- Monitor the pet's health, hunger, and happiness in real-time.
- Authenticate and securely manage user sessions with JWT.
- Engage in mini-games, like the Memory Game, that impact pet stats such as happiness.
  
The backend updates the pet’s state every few minutes, and the frontend fetches data periodically to provide real-time updates.

## Features

### Core Functionality

- **Pet Lifecycle**: Tracks and updates pet hunger, health, happiness, and cleanliness.
- **Authentication**: Users can securely log in to manage their pet.
- **Mini-games**: Includes a Memory Game that influences the pet's happiness when completed successfully.
- **Pet Dashboard**: Displays the pet’s current status and real-time feedback on its needs (e.g., hunger, happiness).
- **Tamagochi UI Elements**: Real-time indicators for pet health and status, and console-like interactive elements.

### Tech Stack

- **Frontend**: React with Axios for API requests
- **Backend**: Node.js, Express, MongoDB, JWT authentication
- **Deployment**: Vercel for both frontend and backend

## Project Structure

```plaintext
pet-app-main/
├── pet-app-backend/    # Backend API with Express and MongoDB
│   ├── README.md       # Instructions specific to backend setup and API
├── pet-app-frontend/   # Frontend React application
│   ├── README.md       # Instructions specific to frontend setup
├── README.md           # This file
```

Each directory (pet-app-backend and pet-app-frontend) is a separate GitHub repository linked as a submodule.

## Setup Instructions

### Prerequisites

- Node.js (v14+)
- MongoDB (local or cloud instance)
- Vercel CLI (optional, for deployment)
- Git

#### 1. Clone the Repository

Clone this main repository, which includes both frontend and backend as submodules:

```bash
git clone --recurse-submodules <https://github.com/auan369/pet-app-main.git>
```

Navigate to the main directory:

```bash
cd pet-app-main
```

#### 2. Install Dependencies

##### Backend Dependencies

Navigate to the backend directory and install dependencies:

```bash
cd pet-app-backend
npm install
```

Create a .env file in the backend folder and add your environment variables as shown in the backend's README.

#### Frontend Dependencies

Navigate to the frontend directory and install dependencies:

```bash
cd ../pet-app-frontend
npm install
```

### 3. Run Locally

#### Start Backend Server

From the backend folder:

```bash
npm start
```

#### Start Frontend Server

From the frontend folder:

```bash
npm start
```

Your app should now be running on localhost:3000 (frontend) and localhost:4000 (backend).

## Frontend

The frontend is a React app that provides the user interface and communicates with the backend API. For more details, see the [Frontend README](./pet-app-frontend/README.md).

## Backend

The backend is an Express.js server that handles user authentication, pet data management, and periodic updates to the pet’s state. For more details, see the [Backend README](./pet-app-backend/README.md).

## Demo

A live demo of the app is available here:

[Frontend (User Interface)](https://pet-app-frontend-drab.vercel.app/)
[Backend (API)](https://pet-app-backend-gamma.vercel.app/)
