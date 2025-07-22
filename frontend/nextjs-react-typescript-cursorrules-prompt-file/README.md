# Sinova Cursor Rules - Next.js React TypeScript Development Guidelines

## Overview

This repository contains Sinova's official development guidelines and best practices for building modern web applications using Next.js, React, and TypeScript. These rules ensure consistency, maintainability, and high performance across all Sinova's projects.

## Technologies

Our tech stack includes:

- Next.js 15 App Router with Partial Prerendering
- React
- TypeScript
- Vite
- Shadcn UI
- Radix UI
- Tailwind
- Turbopack (Development)

## Key Principles

- Functional and declarative programming
- Type safety with TypeScript
- Server-first approach with Next.js
- Measurable code quality standards:
  - Component size limits
  - Nesting depth restrictions
  - Props count limitations
- Consistent naming conventions
- Comprehensive error handling
- Performance optimization with Partial Prerendering
- Feature-based code organization
- Modern UI/UX practices
- Enhanced static optimization

## Guidelines Structure

The repository contains specialized guidelines for:

- Error handling and validation
- JavaScript/TypeScript coding style
- Next.js 15 conventions and best practices
- Server actions implementation with built-in features
- React/Next.js component architecture
- General development principles

## Benefits for Sinova Teams

- Consistent code quality across projects
- Improved development velocity with Turbopack
- Reduced technical debt
- Better collaboration between teams
- Enhanced maintainability
- Optimized performance with Partial Prerendering
- Robust error handling
- Type-safe development

## Implementation

Our guidelines are implemented through:

- `.cursorrules` - Core development rules and principles
- Specialized MDC files for specific aspects
- Integration with modern development tools
- Comprehensive documentation
- Next.js 15's enhanced development features

## Getting Started

1. Clone this repository
2. Review the `.cursorrules` file for core principles
3. Follow specific guidelines in the MDC files
4. Enable Turbopack for development
5. Implement these practices in your Sinova projects

## Best Practices

- Use Server Components by default
- Keep components focused and measurable:
  - Maximum 100 lines per component
  - Maximum 3 levels of nesting
  - Maximum 8 props per component
  - Required documentation for shared components
- Follow naming conventions:
  - PascalCase for React component files (.tsx)
  - kebab-case for utility files and directories
  - camelCase for utility functions
  - PascalCase for React component functions
- Implement comprehensive error handling:
  - Use try/catch for async operations
  - Use type guards for type narrowing
  - Use optional chaining and nullish coalescing
  - Implement error boundaries for components
- Leverage Next.js 15's built-in Server Actions
- Follow proper directory structure:
  - /app/actions/ for app-wide actions
  - /app/(features)/[feature]/ for feature code
  - Group related components and utilities
- Use Zod for form validation
- Optimize for Core Web Vitals (including INP)
- Follow proper TypeScript practices
- Use Partial Prerendering for optimal performance
- Leverage server-only packages

## Documentation

For detailed implementation guidelines, refer to:

- [Next.js 15 Documentation](https://nextjs.org/docs)
- [React Documentation](https://react.dev)
- [TypeScript Documentation](https://www.typescriptlang.org/docs)
- Internal Sinova documentation

## Contributing

We encourage all Sinova developers to contribute to these guidelines. Please follow our contribution process:

1. Review existing guidelines
2. Propose improvements
3. Discuss with the team
4. Submit updates

## Support

For questions or clarifications about these guidelines, please reach out to the Sinova development team.
