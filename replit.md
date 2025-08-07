# Gradify - Career Development Platform

## Overview

Gradify is a comprehensive career development platform built as a full-stack web application that helps users advance their careers through AI-powered tools and community features. The platform provides resume building, interview preparation, professional branding, research tools, and virtual study communities. It follows a modern "Your Career, Curated" approach with a focus on personalized career advancement.

## User Preferences

Preferred communication style: Simple, everyday language.

## System Architecture

### Frontend Architecture
- **React 18** with TypeScript for the user interface
- **Vite** for build tooling and development server
- **Wouter** for client-side routing instead of React Router
- **TanStack Query v5** for server state management and caching
- **React Hook Form** with Zod validation for form handling
- **shadcn/ui** component library with Radix UI primitives
- **Tailwind CSS** for styling with custom design system implementation

### Backend Architecture
- **Express.js** server with TypeScript
- **RESTful API** design with organized route structure
- **Modular service layer** with storage abstraction pattern
- **Error handling middleware** with standardized error responses
- **Request/response logging** for API monitoring
- **Session-based authentication** with PostgreSQL session store

### Authentication & Authorization
- **Replit Auth** integration using OpenID Connect
- **Passport.js** strategy for authentication flow
- **Session-based authentication** with secure cookie configuration
- **Route protection middleware** for authenticated endpoints
- **User profile management** with automatic user creation on first login

### Database Design
- **PostgreSQL** as the primary database
- **Drizzle ORM** for database interactions and migrations
- **Neon Database** as the PostgreSQL provider (@neondatabase/serverless)
- **Comprehensive schema** covering users, profiles, resumes, career tools, study rooms, and activities
- **UUID-based primary keys** for better scalability
- **Proper foreign key relationships** with cascade delete for data integrity

### UI/UX Design System
- **"Gradify" branded design system** with neumorphic styling
- **Custom color palette**: Soft Blue primary (#A7C7E7), Mint Green accent (#AEE6D8), Light Beige background (#FDF7F2)
- **Inter font family** for consistent typography
- **Rounded corners (2xl)** and soft shadows throughout
- **Mobile-first responsive design** with desktop and tablet breakpoints
- **Accessible component patterns** using Radix UI primitives

### Application Structure
- **Feature-based page organization**: Dashboard, Career Tools, Research, Branding, Community, Profile
- **Shared component library** with reusable UI components
- **Layout components** including responsive sidebar and mobile navigation
- **Modular hook system** for authentication and UI state management

### Development & Deployment
- **ESM module system** throughout the codebase
- **TypeScript strict mode** for type safety
- **Vite development server** with hot module replacement
- **Build process** that bundles both client and server
- **Replit-specific integrations** for development environment

## External Dependencies

### Database & Storage
- **Neon Database** - Serverless PostgreSQL hosting
- **Drizzle ORM** - Type-safe database toolkit
- **connect-pg-simple** - PostgreSQL session store for Express sessions

### Authentication
- **Replit Auth** - OpenID Connect authentication provider
- **Passport.js** - Authentication middleware
- **openid-client** - OpenID Connect client implementation

### UI Framework & Styling
- **Radix UI** - Comprehensive primitive component library
- **Tailwind CSS** - Utility-first CSS framework
- **Lucide Icons** - Icon library for consistent iconography
- **Google Fonts (Inter)** - Typography via CDN

### State Management & Data Fetching
- **TanStack Query** - Server state management and caching
- **React Hook Form** - Form state and validation
- **Zod** - Runtime type validation and schema definition

### Development Tools
- **Vite** - Build tool and development server
- **TypeScript** - Static type checking
- **ESBuild** - Fast JavaScript bundler for production builds
- **PostCSS & Autoprefixer** - CSS processing pipeline