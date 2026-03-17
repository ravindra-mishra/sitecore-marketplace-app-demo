# Sitecore Marketplace Apps – Demo Series

This repository accompanies a blog series that walks through building a **Sitecore Marketplace App** using a modern full-stack approach.

The goal of this series is to move beyond theory and demonstrate how Marketplace apps can be designed, built, and integrated into Sitecore XM Cloud using real-world patterns.

## Blog Series

- Part 0: Overview – Why Marketplace Apps Matter  
  https://ravindra-mishra.github.io/blogs/sitecore-marketplace-apps-overview-why-they-matter

- Part 1: Fullstack Setup with Next.js & shadcn  
  https://ravindra-mishra.github.io/blogs/sitecore-marketplace-app-nextjs-shadcn-fullstack-guide-part-1

- Part 2: Implementation & Extension Points  
  https://ravindra-mishra.github.io/blogs/sitecore-marketplace-app-nextjs-shadcn-fullstack-guide-part-2

## Context

Sitecore Marketplace apps are independent web applications that integrate into Sitecore Cloud via defined extension points. They allow teams to extend XM Cloud capabilities without modifying the core platform.

This repository demonstrates how to:

- Build a full-stack Marketplace app
- Integrate with Sitecore using the Marketplace SDK
- Use extension points like panels, widgets, and standalone apps
- Structure a scalable and production-ready implementation

## Architecture Overview

The demo follows a full-stack architecture:

- Frontend: Next.js (React-based UI)
- UI Components: shadcn/ui
- Backend: Node.js (API routes / server-side logic)
- Authentication: Auth0 (Sitecore Cloud integration)
- Integration Layer: Sitecore Marketplace SDK

Marketplace apps typically:

- Run on independent infrastructure
- Communicate with Sitecore via SDK APIs
- Render inside Sitecore via iframe-based extension points

## Extension Points Covered

This project demonstrates how to plug into different Sitecore contexts:

- Standalone App (Cloud Portal)
- Fullscreen App (XM Cloud navigation)
- Page Builder Context Panel
- Custom Field Integration
- Dashboard Widget

## Key Features

- Full-stack Marketplace app setup
- SDK-based communication with Sitecore
- Modular and reusable component structure
- Example integrations (client + server side)
- Authentication-ready setup

## Project Structure

/app            # Next.js app (routes, pages, layouts)
/components     # Reusable UI components (shadcn)
/lib            # Utilities and helpers
/pages/api      # Backend API routes
/services       # Sitecore SDK integrations
/styles         # Global styles

## Getting Started

### Prerequisites

- Node.js (>= 18)
- Sitecore XM Cloud environment
- Marketplace App registration (Developer Portal)
- Auth0 configuration (for secure access)

### Installation

git clone https://github.com/ravindra-mishra/sitecore-marketplace-app-demo
cd https://github.com/ravindra-mishra/sitecore-marketplace-app-demo
npm install

### Run locally

npm run dev

## Configuration

You will need to configure:

- Sitecore Marketplace App credentials
- Auth0 client details
- Environment variables

Example:

SITECORE_CLIENT_ID=
SITECORE_CLIENT_SECRET=
AUTH0_DOMAIN=
AUTH0_CLIENT_ID=

## What This Demo Focuses On

- Real integration patterns (not mock-only examples)
- Full-stack flows (UI + API + Sitecore interaction)
- Developer experience and maintainability
- Practical extension scenarios

## When to Use This Approach

- You need custom UI inside Sitecore XM Cloud
- You are integrating external systems (CRM, AI, analytics)
- You want to automate editorial workflows
- You are building reusable tools across projects

## Contributing

This repository is primarily for demonstration purposes, but suggestions and improvements are welcome.

## License

MIT License

## Author

Ravindra Mishra  
Senior Sitecore Developer & Full Stack Engineer

## Notes

This repository is part of a learning series. It evolves alongside the blog posts and may include incremental improvements over time.
