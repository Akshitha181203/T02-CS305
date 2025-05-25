# CauseCraft

**CauseCraft** is a web-based platform that empowers Non-Governmental Organizations (NGOs) to create, host, and manage their websites effortlessly. With customizable templates, intuitive task management, volunteer coordination, and secure hosting, CauseCraft streamlines online presence for NGOs, enabling them to showcase their mission, engage volunteers, and attract donors.

---

## Table of Contents

1. [Features](#features)  
2. [Technology Stack](#technology-stack)  
3. [Installation](#installation)  
   - [Prerequisites](#prerequisites)  
   - [Backend Setup](#backend-setup)  
   - [Frontend Setup](#frontend-setup)  
   - [Database & Cloud Storage](#database--cloud-storage)  
4. [Project Structure](#project-structure)  
5. [Usage](#usage)  
6. [Acknowledgements](#acknowledgements)

---

## Features

- **User Authentication & Authorization**: Secure registration, login, and role-based access (executives, volunteers, administrators).  
- **Template Customization**: Browse, preview, and customize website templates with content, layout, colors, fonts, and image uploads.  
- **Hosting Services**: One-click deployment of customized NGO websites with reliable hosting.  
- **Task Management**: Executives can create tasks, assign volunteers, set deadlines, and track progress.  
- **Volunteer Coordination**: Volunteers indicate availability, accept tasks, and communicate with executives.  
- **User Profiles**: Manage personal information, skills, interests, and profile pictures.  
- **Image Management**: Upload, update, and delete images used in templates and profiles.

---

## Technology Stack

- **Frontend**: React.js  
- **Backend**: Node.js, Express.js  
- **Database**: MongoDB  
- **Cloud Storage**: (e.g., AWS S3, Google Cloud Storage)  
- **Authentication**: JWT or OAuth2

---

## Installation

### Prerequisites

- Node.js (v14+)  
- npm or yarn  
- MongoDB (local or cloud)  
- Cloud storage account (e.g., AWS S3) and credentials

### Backend Setup

1. Navigate to the backend directory:  
   ```bash
   cd server
   ```
2. Install dependencies:
   ```bash
   npm install
   # or
   yarn install
   ```
3. Create a ```.env``` file in ```backend/``` with the following (update values accordingly):
   ```text
   PORT=4000
   MONGO_URI=<your-mongodb-connection-string>
   JWT_SECRET=<your-jwt-secret>
   CLOUD_STORAGE_BUCKET=<your-bucket-name>
   CLOUD_PROVIDER=<aws|gcp>
   CLOUD_ACCESS_KEY_ID=<access-key-id>
   CLOUD_SECRET_ACCESS_KEY=<secret-access-key>
   ```
4. Start the backend server:
   ```bash
   npm run dev
   # or
   yarn dev
   ```
   
### Frontend Setup

1. Navigate to the frontend directory:  
   ```bash
   cd client
   ```
2. Install dependencies:
   ``` bash
   npm clean install
   # or
   yarn clean install
   ```
3. Create a ```.env``` file in ```client/``` with the following:
   ```text
   REACT_APP_API_URL=http://localhost:4000/api
   ```
4. Start the frontend server:
   ```bash
   npm start
   # or
   yarn start
   ```
### Database & Cloud Storage

- Ensure MongoDB is running and accessible via the connection string in your `.env`.  
- Configure your cloud storage bucket to accept file uploads and update the backend environment variables accordingly.

---
  

### Project Structure
```text
├── server/                # Express.js server
│   ├── controllers/        # Route handlers
│   ├── models/             # Mongoose schemas
│   ├── routes/             # API endpoints
│   ├── services/           # Business logic & integrations
│   ├── utils/              # Utility functions
│   ├── .env                # Environment variables
│   └── server.js           # Entry point

├── client/               # React.js client
│   ├── public/
│   ├── src/
│   │   ├── components/     # Reusable UI components
│   │   ├── pages/          # Route-based components
│   │   ├── services/       # API calls
│   │   └── App.js
│   └── .env

├── srs/                    # Software Requirement Specification document
│   └── SRS_CauseCraft.pdf  # Detailed requirements

└── README.md               # Project overview & setup
```
### Usage

1. Register a new account or log in with existing credentials.  
2. Select or customize a website template.  
3. Upload images and content as needed.  
4. Deploy your website with a single click.  
5. Create and assign tasks to volunteers via the dashboard.  
6. Monitor task progress and manage user roles through the admin panel.  

---

### Acknowledgements

- **Supervisor**: Dr. SP Abhinandan (IIT Ropar)  
- **Contributors**:  
  - Dasaraju Karthik Nandan  
  - Divyankar Shah  
  - Doodh Nath Tiwari  
  - Gattu Pavithran Goud  
  - Kola Sai Datta  
  - Nitesh Kumar  
  - Chaitanya Pedapudi  
  - Akshitha Peguda  
  - Shaik Darakshinda  
  - Yashaswini Vajja  
  - Vudem Rishik Vardhan Reddy  
