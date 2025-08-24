# 3D Print Management System

## Overview

This is a full-stack 3D printing management application built with React (frontend) and Express.js (backend). The system helps users manage multiple 3D printers, track print jobs, organize projects, and monitor print queues. It supports both FDM and Resin printer types with real-time status tracking and queue management capabilities.

## User Preferences

Preferred communication style: Simple, everyday language.

## System Architecture

### Frontend Architecture
- **Framework**: React 18 with TypeScript for type safety
- **Routing**: Wouter for lightweight client-side routing
- **State Management**: TanStack Query for server state management and caching
- **UI Framework**: Shadcn/ui components built on Radix UI primitives
- **Styling**: Tailwind CSS with CSS variables for theming
- **Form Handling**: React Hook Form with Zod validation
- **Build Tool**: Vite for fast development and optimized builds

### Backend Architecture
- **Runtime**: Node.js with Express.js web framework
- **Database**: PostgreSQL with Drizzle ORM for type-safe database operations
- **Validation**: Zod schemas shared between frontend and backend
- **Session Management**: Express sessions with PostgreSQL session store
- **Development**: In-memory storage fallback for development/testing

### Data Models
The system manages three core entities:
- **Printers**: Physical 3D printers with status tracking (idle, printing, heating, paused, error)
- **Projects**: Organizational containers for related print jobs
- **Prints**: Individual print jobs with progress tracking, queue management, and printer assignment

### Key Features
- **Multi-Printer Support**: Handles both FDM and Resin printer types
- **Queue Management**: Automatic and manual print job queuing with priority ordering
- **Progress Tracking**: Real-time monitoring of print progress, layer counts, and time estimates
- **Project Organization**: Grouping related prints into projects for better organization
- **Status Management**: Comprehensive status tracking for both printers and print jobs

### Development Patterns
- **Shared Schema**: Common TypeScript types and Zod schemas between client and server
- **API-First Design**: RESTful API with consistent error handling and logging
- **Component Architecture**: Modular React components with clear separation of concerns
- **Type Safety**: Full TypeScript coverage with strict type checking

## External Dependencies

### Database
- **PostgreSQL**: Primary database for production data persistence
- **Neon Database**: Serverless PostgreSQL hosting service
- **Drizzle ORM**: Type-safe database toolkit with migrations support

### UI Components
- **Radix UI**: Accessible component primitives for complex UI interactions
- **Shadcn/ui**: Pre-built component library with consistent design system
- **Lucide React**: Icon library for consistent iconography

### Development Tools
- **Vite**: Build tool with hot module replacement and fast development server
- **TSX**: TypeScript execution environment for server-side development
- **ESBuild**: Fast JavaScript bundler for production builds

### External Services
- **Replit Integration**: Development environment with runtime error overlay and cartographer support
- **Google Fonts**: Typography with Inter font family for modern appearance

### Session Management
- **connect-pg-simple**: PostgreSQL session store for persistent user sessions
- **Express Session**: Server-side session management middleware