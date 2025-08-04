# React Kickstart Template

A modern React 19 template featuring the latest tools and best practices for building fast, scalable web applications.

## 🚀 Features

- **React 19** - Latest React with improved performance and new features
- **Rsbuild** - Fast Rust-based build tool with zero config
- **TanStack Router** - Type-safe routing with automatic code splitting
- **shadcn/ui** - Beautiful, accessible UI components built with Radix UI
- **Tailwind CSS** - Utility-first CSS framework with CSS variables
- **TypeScript** - Full type safety throughout the application
- **Bun** - Fast package manager and runtime

## 🛠️ Tech Stack

- **Build Tool**: [Rsbuild](https://rsbuild.rs) - Fast Rust-based bundler
- **Framework**: [React 19](https://react.dev)
- **Routing**: [TanStack Router](https://tanstack.com/router)
- **UI Components**: [shadcn/ui](https://ui.shadcn.com) with [Radix UI](https://radix-ui.com)
- **Styling**: [Tailwind CSS](https://tailwindcss.com) v4
- **Icons**: [Lucide React](https://lucide.dev)
- **Package Manager**: [Bun](https://bun.sh)
- **Language**: [TypeScript](https://typescriptlang.org)

## 📁 Project Structure

```text
├── components/
│   └── ui/              # shadcn/ui components
├── lib/
│   └── utils.ts         # Utility functions
├── src/
│   ├── routes/          # TanStack Router pages
│   │   ├── __root.tsx   # Root layout
│   │   ├── index.tsx    # Home page
│   │   └── about.tsx    # About page
│   ├── App.tsx          # Main app component
│   ├── App.css          # Global styles
│   └── index.tsx        # App entry point
├── components.json      # shadcn/ui configuration
├── rsbuild.config.ts    # Rsbuild configuration
└── package.json
```

## 🚀 Quick Start

### Prerequisites

- [Bun](https://bun.sh) (recommended) or Node.js 18+

### Installation

1. **Clone or use this template**

   ```bash
   git clone <repository-url>
   cd react-kickstart
   ```

2. **Install dependencies**

   ```bash
   bun install
   ```

3. **Start development server**

   ```bash
   bun dev
   ```

   The app will be available at [http://localhost:3000](http://localhost:3000)

### Build for Production

```bash
# Build the application
bun build

# Preview the production build
bun preview
```

## 🎨 Adding UI Components

This template uses shadcn/ui for components. Add new components using:

```bash
bunx shadcn@latest add button
bunx shadcn@latest add card
bunx shadcn@latest add dialog
# ... and many more
```

All components are configured to work with the "New York" style and include:

- Tailwind CSS variables for theming
- TypeScript support
- Lucide React icons
- Proper path aliases (`@/components`, `@/lib`, etc.)

## 🛣️ Routing

This template uses TanStack Router with:

- **File-based routing** - Routes are automatically generated from the `src/routes/` directory
- **Type safety** - Full TypeScript support for routes and navigation
- **Code splitting** - Automatic code splitting for optimal performance
- **Dev tools** - Built-in development tools for debugging routes

### Adding New Routes

Create new route files in `src/routes/`:

```typescript
// src/routes/contact.tsx
import { createFileRoute } from '@tanstack/react-router'

export const Route = createFileRoute('/contact')({
  component: ContactComponent,
})

function ContactComponent() {
  return <div>Contact Page</div>
}
```

## 🎯 What's Included

- ✅ React 19 with latest features
- ✅ TypeScript configuration
- ✅ Tailwind CSS v4 with CSS variables
- ✅ shadcn/ui component system
- ✅ TanStack Router with type safety
- ✅ Path aliases for clean imports
- ✅ ESLint and Prettier ready
- ✅ Development tools and debugging
- ✅ Production-ready build configuration

## 📚 Learn More

Explore the documentation for the tools used in this template:

- [React Documentation](https://react.dev) - Learn about React 19 features
- [Rsbuild Documentation](https://rsbuild.rs) - Explore Rsbuild features and APIs
- [TanStack Router](https://tanstack.com/router) - Type-safe routing guide
- [shadcn/ui](https://ui.shadcn.com) - Component library documentation
- [Tailwind CSS](https://tailwindcss.com/docs) - Utility-first CSS framework

## 🤝 Contributing

This is a template repository. Feel free to:

- Fork and customize for your needs
- Report issues or suggest improvements
- Submit pull requests for enhancements

## 📄 License

This project is open source and available under the [MIT License](LICENSE).
