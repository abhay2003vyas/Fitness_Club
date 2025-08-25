# Overview

This is a professional responsive website for "धर्मवीर छत्रपती संभाजीराजे फिटनेस क्लब", a gym and fitness center. The application is a full-stack web application built with React for the frontend and Express.js for the backend, featuring modern UI design with animations, membership management, contact forms, and comprehensive gym information including services, pricing, equipment, and team details.

# User Preferences

Preferred communication style: Simple, everyday language.

# System Architecture

## Frontend Architecture

**Framework & Libraries**: React 18 with TypeScript, using Vite as the build tool and development server. The frontend follows a component-based architecture with modern React patterns.

**UI Framework**: Built with shadcn/ui components and Radix UI primitives, providing accessible and customizable UI components. Tailwind CSS is used for styling with a custom color scheme featuring orange (#FF6B35), black (#1A1A1A), and white as primary theme colors.

**State Management**: Uses TanStack Query (React Query) for server state management, data fetching, and caching. Local component state is managed with React hooks.

**Routing**: Implemented with Wouter for client-side routing, providing a lightweight routing solution.

**Animations**: Framer Motion is integrated for smooth animations and transitions throughout the website.

**Form Handling**: React Hook Form with Zod validation for type-safe form management and validation.

**Typography**: Uses Google Fonts including Poppins, Inter, and Noto Sans Devanagari to support both English and Devanagari text.

## Backend Architecture

**Server Framework**: Express.js with TypeScript, providing RESTful API endpoints for contact forms and membership management.

**Development Setup**: Uses tsx for TypeScript execution in development and esbuild for production builds. The server includes middleware for JSON parsing, URL encoding, and request logging.

**API Structure**: Clean separation of concerns with routes defined in separate modules. Includes error handling middleware and request/response logging for debugging.

**Validation**: Server-side validation using Zod schemas shared between frontend and backend for type consistency.

## Data Storage Solutions

**Database ORM**: Drizzle ORM for type-safe database operations with PostgreSQL dialect configuration.

**Database Provider**: Configured for Neon Database using serverless PostgreSQL with connection pooling.

**Schema Design**: Three main entities:
- Users table for authentication (username, password)
- Contacts table for contact form submissions (personal details, interests, messages)
- Memberships table for membership applications (personal details, plan selection, pricing)

**Development Storage**: In-memory storage implementation for development and testing, with the ability to switch to database storage in production.

**Migration System**: Drizzle Kit for database migrations and schema management.

## External Dependencies

**Database Service**: Neon Database - Serverless PostgreSQL database service
**CDN Services**: 
- Google Fonts for typography
- Font Awesome for icons
- Unsplash for placeholder images

**Development Tools**:
- Replit integration for development environment
- Vite plugins for development enhancement
- TypeScript for type safety across the stack

**UI Component Libraries**:
- Radix UI primitives for accessible components
- shadcn/ui for pre-built component library
- Embla Carousel for image galleries
- Framer Motion for animations

**Utility Libraries**:
- clsx and tailwind-merge for conditional styling
- date-fns for date manipulation
- nanoid for unique ID generation
- class-variance-authority for component variants

The application architecture supports both development and production environments with proper build processes, static file serving, and environment-specific configurations.