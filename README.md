# DESIGN AND IMPLEMENTATION OF A BLOCKCHAIN POWERED HEALTHCARE RECORD MANAGEMENT SYSTEM.

<hr/>

## Overview

<hr>
<p>A blockchain record management system for smart contracts for identity management and ownership verification using <b>HyperLedger Platform</b>.</p>

<hr/>

### Project Structure

```
├── README.md
├── LICENSE
│
├── smart-contracts                     # Contains the smart contracts
│   ├── healthcare-record.sol
│   └── identity-management.sol
│
├── backend
│   ├── package.json
│   ├── package-lock.json
│   ├── node_modules# Contains the backend server
│   ├── routes                              # Express Routes
│   ├── auth.routes.ts
│   ├── user.routes.ts
│   └── index.ts
│   ├── config                              # Configuration files
│   │   ├── env.ts
│   │   ├── .env.development.local
│   │   ├── env.example.local
│   │   └── .env.production.local
│   ├── controller                          # Server logic
│   │   ├── auth.controller.ts
│   │    ├── user.controller.ts
│   │    └── index.ts
│   ├── database                            # Database related files
│   │    └── mongodb.ts  
│   ├── middleware                          # Middleware files
│   │   ├── auth.middleware.ts
│   │   ├── error.middleware.ts
│   │   └── index.ts
│   ├── models                              # Model files
│   │   ├── user.model.ts
│   │   └── index.ts
│   ├── others                          # Contains other files
│   │   ├── social-login.ts
│   │   └── index.ts
│   └── index.ts                            # Entry point
│
├── frontend                            # Contains the frontend server
│   ├── public
│   ├── src
│   │   ├── components
│   │   ├── pages
│   │   ├── App.tsx
│   │   ├── index.tsx
│   │   └── react-app-env.d.ts
│   ├── .gitignore
│   ├── package.json
│   ├── package-lock.json
│   └── tsconfig.json
└── .gitignore
```

### Getting Started.

Before you begin, ensure you have the following installed on your system:
<li>Node.js</li>
<li>MongoDB</li>
<li>Bun runtime</li>
<li>A text-editor or an IDE</li>
<li>Typescript</li>
<li>An API testing tool like HTTPie, Postman or Aqua</li>

### Installation

1. Clone the repository

```bash
  git clone https://github.com/121-praise/Blockchain-RMS.git
```

2. Install all necessary packages

```bash
  bun install
```

3. Start the nodemon server

```bash
   nodemon index.ts
 ```

4. Create a branch
5. copy the .env.example.local and update it with your environment variables into the .env.development.local file
6. Make changes
7. Push to GitHub
8. Open a Pull Request

### Commit Rules

We follow conventional commit messages, without which you would not be able to make a commit. Here's a quick overview:

<li>fix: A bug fix.</li>

    Example: fix: correct typo in user model

<li>feat: A new feature for the user.</li>

    Example: feat: add user authentication module

<li>docs: Documentation changes.</li>

    Example: docs: update README with setup instructions

<li>refactor: Code changes that neither fix a bug nor add a feature.</li>

    Example: refactor: simplify user service logic

<li>chore: Changes to the build process or auxiliary tools, or changes that do not directly impact the codebase.</li>

    Example: chore: update dependencie