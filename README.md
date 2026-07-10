# SyncScript - Code Collaboration Platform

<div align="center">
  <a href="YOUR_DEPLOYMENT_URL">
    
  </a>
</div>

<br />

<div align="center">
  <a href="https://github.com/YOUR_GITHUB_USERNAME/SyncScript/actions/workflows/playwright.yml"><img src="https://github.com/YOUR_GITHUB_USERNAME/SyncScript/actions/workflows/playwright.yml/badge.svg"></a>
  <a href="https://github.com/YOUR_GITHUB_USERNAME/SyncScript/actions/workflows/jest.yml"><img src="https://github.com/YOUR_GITHUB_USERNAME/SyncScript/actions/workflows/jest.yml/badge.svg"></a>
</div>
<div align="center">
  <a href="https://github.com/YOUR_GITHUB_USERNAME/SyncScript/issues"><img src="https://img.shields.io/github/issues/YOUR_GITHUB_USERNAME/SyncScript.svg?style=flat" /></a>
</div>

<br />

**SyncScript is an online code collaboration platform that enables real-time coding, cursor sharing, live UI preview, and video communication with integrated Git support—no sign-up required.**

**✨ Try now at [YOUR_DEPLOYMENT_URL](YOUR_DEPLOYMENT_URL)**

For detailed usage instructions and feature documentation, please see the **[User Manual](manual.md)**.

## Features

- **Real-time Collaboration** - Code together in real-time with cursor sharing, highlighting, and follow mode
- **Shared Terminal** - Execute code and see results together with over 80 supported languages
- **Live Preview** - Preview UI changes instantly with loaded libraries like Tailwind CSS, and more
- **GitHub Integrated** - Save your work and open files from your repositories
- **Shared Notepad** - Take notes together in real-time with rich text and markdown support
- **Video & Voice** - Communicate with your team using video and voice chat

## Table of Contents

- [SyncScript - Code Collaboration Platform](#syncscript---code-collaboration-platform)
  - [Features](#features)
  - [Table of Contents](#table-of-contents)
  - [Project Structure](#project-structure)
  - [Prerequisites](#prerequisites)
  - [Getting Started](#getting-started)
  - [Development](#development)
  - [Test](#test)
    - [Frontend Test](#frontend-test)
    - [Backend Test](#backend-test)
  - [Build](#build)
  - [Deployment](#deployment)
  - [Scripts](#scripts)
  - [Tech Stack](#tech-stack)
  - [Coding Style](#coding-style)
  - [Contributing](#contributing)
  - [User Manual](#user-manual)
  - [License](#license)

## Project Structure

The project is organized as a [monorepo](https://en.wikipedia.org/wiki/Monorepo) using [Turborepo](https://turbo.build/repo/docs):

```txt
SyncScript
├── apps/                   # Application packages
│   ├── client/             # Frontend Next.js application
│   │   ├── public/         # Static assets
│   │   ├── src/            # Source code
│   │   │   ├── app/        # Next.js app router pages and API routes
│   │   │   ├── components/ # React components
│   │   │   ├── hooks/      # Custom React hooks
│   │   │   └── lib/        # Utility functions and services
│   │   └── tests/          # Frontend tests (Playwright)
│   └── server/             # Backend Socket.IO server
│       ├── src/            # Source code
│       │   ├── service/    # Backend services
│       │   └── utils/      # Utility functions
│       └── tests/          # Backend tests (Jest)
├── docs/                   # Documentation assets
├── packages/               # Shared packages
│   └── types/              # Shared TypeScript types and interfaces
├── scripts/                # Build and maintenance scripts
├── package.json            # Root package.json
└── pnpm-workspace.yaml     # PNPM workspace configuration
