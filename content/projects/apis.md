---
title: "A Revised Collection of APIs"
date: 2024-01-15
draft: false
description: "RESTful APIs built with Laravel"
---

# Student Management API

A comprehensive REST API group for miscellaneous tasks.

## Features
- Complete CRUD operations 
- Data validation and error handling  
- MySQL database with Eloquent ORM
- RESTful API design principles
- Comprehensive API documentation

## Technology Stack
- **Backend**: Laravel 10, PHP 8.2
- **Database**: MySQL 8.0
- **Testing**: Postman, PHPUnit

## Example API Endpoint (see docs for more)

### Students Management
| Method | Endpoint             | Description               |
|--------|----------------------|---------------------------|
| GET    | `/api/art`           | Retrieve all artworks     |
| GET    | `/api/art/{id}`      | Retrieve specific artwork |
| POST   | `/api/art`           | Create new artwork        |
| PUT    | `/api/art/{id}`      | Update artwork            |
| DELETE | `/api/art/{id}`      | Delete artwork            |

## Example Usage

### Create an artwork
```bash
curl -X POST http://localhost:8000/api/art \
  -H "Content-Type: application/json" \
  -d '{
    "name": "The Mona Lisa",
    "size": "100",
    "artist": "Leonardo Da Vinci",
  }'
```

### Response

```json
{
  "success": true,
  "message": "Art created successfully",
  "data": {
    "id": 1,
    "name": "The Mona Lisa",
    "size": "100",
    "artist": "Leonardo Da Vinci",
    "created_at": "2024-01-15T10:30:00.000Z",
    "updated_at": "2024-01-15T10:30:00.000Z"
  }
}
```

## Quick Start with script

```bash
# Clone the repository
git clone https://github.com/yourusername/project2.git
cd project2

# Start with Script
sudo bash run.sh

# The APIs can be started with "composer run apis"
```

## Link

- **GitHub Repository**: [github.com/interestingpoint/project2](https://github.com/interestingpoint/project2.git)