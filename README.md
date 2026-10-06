# VeraTechLabs Client Project Management Platform

## Overview

The VeraTechLabs Client Project Management Platform is a full-stack web application designed to help organizations manage clients, projects, team assignments, and project progress from a centralized platform.

The system includes authentication, role-based permissions, project tracking, dashboard analytics, and secure APIs integrated with MongoDB.

---

## Features

### Authentication

- User Login
- JWT Authentication
- Protected Routes
- Protected APIs
- Session Management

Only authenticated users can access the platform.

---

## Role-Based Access Control (RBAC)

The platform supports multiple user roles.

### Admin

Administrators can:

- Create Clients
- Update Clients
- Delete Clients
- Create Projects
- Assign Clients
- Assign Team Members
- Update Project Information
- Delete Projects
- View Dashboard Analytics

### Team Member

Team Members can:

- View Assigned Projects
- View Dashboard
- Update Project Status

Team Members cannot:

- Create Projects
- Delete Projects
- Manage Clients

---

## Client Management

Administrators can:

- Add new clients
- View all clients
- Update client information
- Delete clients

Client information includes:

- Company Name
- Contact Person
- Email Address
- Phone Number

---

## Project Management

Administrators can:

- Create Projects
- Update Projects
- Delete Projects
- Assign Clients
- Assign Team Members

Each project contains:

- Project Name
- Project Description
- Project Status
- Assigned Client
- Assigned Team Members

---

## Project Status Tracking

Projects can use the following statuses:

- Not Started
- In Progress
- Completed
- On Hold

Authorized users can update project statuses.

---

## Project Dashboard

The dashboard provides:

### Statistics

- Total Projects
- Active Projects
- Completed Projects
- On Hold Projects

### Project Overview

Displays:

- Project Name
- Description
- Status
- Assigned Client
- Team Members

---

## Technologies Used

### Frontend

- React.js
- React Router DOM
- CSS3
- Fetch API

### Backend

- Node.js
- Express.js
- JWT Authentication
- Role-Based Authorization

### Database

- MongoDB
- Mongoose

---

## Database Structure

### User

```json
{
  "name": "John Doe",
  "email": "john@email.com",
  "password": "encrypted",
  "role": "admin"
}
```

### Client

```json
{
  "companyName": "Microsoft",
  "contactPerson": "John Smith",
  "email": "john@microsoft.com",
  "phone": "123456789"
}
```

### Project

```json
{
  "projectName": "CRM Platform",
  "description": "Internal CRM System",
  "status": "In Progress",
  "client": "clientId",
  "assignedMembers": ["userId"]
}
```

---

## API Endpoints

### Authentication

```http
POST /api/auth/register
POST /api/auth/login
```

### Clients

```http
GET    /api/clients
POST   /api/clients
PUT    /api/clients/:id
DELETE /api/clients/:id
```

### Projects

```http
GET    /api/projects
POST   /api/projects
PUT    /api/projects/:id
DELETE /api/projects/:id
```

### Users

```http
GET /api/user
```

---

## Project Workflow

Create Client

↓

Create Project

↓

Assign Client

↓

Assign Team Members

↓

Track Project Status

↓

Monitor Dashboard

---

## Security Features

- JWT Authentication
- Protected Frontend Pages
- Protected Backend APIs
- Role-Based Access Control
- Permission Verification Middleware
- Secure User Roles

---

## Dashboard Features

The dashboard provides real-time project monitoring:

### KPI Cards

- Total Projects
- Active Projects
- Completed Projects
- On Hold Projects

### Project Cards

Each project displays:

- Project Name
- Description
- Status
- Client
- Team Member Count

---

## Requirements Covered

### Authentication

✅ User Login

✅ Private Routes

✅ Secure APIs

---

### Role-Based Permissions

✅ Admin Role

✅ Team Member Role

✅ Authorization Rules

---

### Project Management

✅ Create Projects

✅ Update Projects

✅ Delete Projects

✅ Assign Clients

✅ Assign Team Members

---

### Project Status

✅ Not Started

✅ In Progress

✅ Completed

✅ On Hold

---

### Dashboard

✅ Project Statistics

✅ Project Monitoring

✅ Organized Data Display

---

### API

✅ GET

✅ POST

✅ PUT

✅ DELETE

✅ Authorization

---

### Database

✅ MongoDB Integration

✅ Users Collection

✅ Clients Collection

✅ Projects Collection

✅ Entity Relationships

---

## Future Improvements

- Project Deadlines
- Task Management
- Project Comments
- Notifications
- File Attachments
- Advanced Search & Filtering
- Project Reports
- Team Performance Analytics

---

## Author

Mays Ben Youssef

VeraTechLabs Full-Stack Platform
