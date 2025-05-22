# CodePass

CodePass is a secure password manager that allows you to store and manage your credentials safely. This project is part of the Code initiative.

## Repository Structure

The repository is organized as follows:

- **src/**: Contains the main source code of the application
- **test/**: Contains application tests
  - **models/**: Tests for data models
    - `PasswordItems.test.js`: Tests for password items class
    - `User.test.js`: Tests for user class
  - **services/**: Tests for services
    - `UsersManager.test.js`: User management tests
    - `PasswordManager.test.js`: Password management tests
    - `CodePass.test.js`: Main service tests

- **public/**: Contains publicly accessible files
- **.husky/**: Configuration for git hooks
- **.github/**: Templates and configurations for GitHub

## Features

CodePass offers the following features:

- **User Management**
  - Registration with username, email, password, and master password
  - Login and logout
  - User data updates
  - Account deletion

- **Password Management**
  - Secure password storage
  - Add, edit, and delete credentials
  - Organization by website
  - Custom descriptions

## Data Models

### PasswordItems
- Email
- Password
- Website
- Description
- Unique ID (generated using UUID)

### User
- Username
- Email
- Password (encrypted)
- Master Password (encrypted)
- Unique ID
- List of password items

## Services

### UsersManager
Manages all user-related operations:
- Registration and authentication
- Session management
- User data updates
- Input validation

### PasswordManager
Manages all password-related operations:
- Adding and removing credentials
- Updating information
- Secure organization

### CodePass
Main service that integrates UsersManager and PasswordManager.

## Technical Requirements

- Node.js
- bcrypt for encryption
- UUID for unique ID generation
- Validator for input validation

## Getting Started

1. Clone this repository
2. Install dependencies with `npm install`
3. Start the application with `npm start`

## User Interface

The application includes a user interface with:
- Login/registration page
- Dashboard for password management
- Functionality for adding and editing credentials

## Security

- Passwords are encrypted with bcrypt
- Use of master password for additional protection
- Input validation to prevent attacks

---

*This project is part of the Code initiative.*