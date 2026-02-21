# Maxi Web Components

<div align="center">
  <img src="public/assets/logo.png" alt="Maxi Web Components Logo" width="300" />
</div>

<div align="center">
  <h3>Angular Components Library</h3>
  <p>A comprehensive collection of reusable UI components for Angular applications</p>
  
  ![Angular](https://img.shields.io/badge/Angular-19.2.0-red?style=flat-square&logo=angular)
  ![TypeScript](https://img.shields.io/badge/TypeScript-5.7.2-blue?style=flat-square&logo=typescript)
  ![License](https://img.shields.io/badge/License-Private-orange?style=flat-square)
</div>

---

## 📋 Table of Contents

- [Overview](#overview)
- [Features](#features)
- [Installation](#installation)
- [Getting Started](#getting-started)
- [Components](#components)
- [Compatibility](#compatibility)
- [Development](#development)
- [Contributing](#contributing)

## 🚀 Overview

**Maxi Angular Components** is a comprehensive Angular components library designed to provide developers with a complete set of modern, accessible, and customizable UI components. Built specifically for Angular applications, this library offers a consistent design system and seamless integration with Angular's ecosystem.

### Key Highlights

- **Modern Design**: Clean, contemporary UI components following current design trends
- **Angular Native**: Built specifically for Angular with full TypeScript support
- **Accessibility First**: WCAG compliant components with proper ARIA attributes
- **Customizable**: Extensive theming and styling options
- **Performance Optimized**: Lightweight and efficient components
- **Type Safe**: Full TypeScript support with comprehensive type definitions

## ✨ Features

- 🎨 **27+ Components** covering all major UI patterns
- 📱 **Responsive Design** - Mobile-first approach
- ♿ **Accessibility** - WCAG 2.1 AA compliant
- 🎯 **TypeScript** - Full type safety and IntelliSense support
- 🎨 **Theming** - Customizable color schemes and styling
- 📦 **Tree Shaking** - Import only what you need
- 🔧 **Angular CLI** - Seamless integration with Angular tooling

## 📦 Installation

```bash
npm install maxi-angular-components
```

### Peer Dependencies

Make sure you have the required peer dependencies installed:

```bash
npm install @angular/common @angular/core @angular/forms
```

## 🚀 Getting Started

### 1. Import the Module

```typescript
import { NgModule } from "@angular/core";
import { MaxiComponentsModule } from "maxi-angular-components";

@NgModule({
  imports: [MaxiComponentsModule],
  // ... other module configuration
})
export class AppModule {}
```

### 2. Use Components

```html
<!-- Input Field -->
<maxi-input-field [placeholder]="'Enter your name'" [required]="true"> </maxi-input-field>

<!-- Button -->
<maxi-button [variant]="'primary'" [size]="'medium'" (click)="onSubmit()"> Submit </maxi-button>

<!-- Card -->
<maxi-card [title]="'Sample Card'">
  <p>Your content here</p>
</maxi-card>

<!-- Accordion -->
<maxi-accordion [data]="accordionData" [multiple]="true" (tabChange)="handleTabChange($event)"> </maxi-accordion>

<!-- Cascade Menu -->
<maxi-cascade-menu [data]="menuData" [trigger]="'click'"> </maxi-cascade-menu>
```

## 🧩 Components

### Input Components

- **Input Field** - Text input with validation and styling options
- **Input Number** - Numeric input with increment/decrement controls
- **Input Switch** - Toggle switch for boolean values
- **Radio** - Radio button for single selection
- **Checkbox** - Checkbox for multiple selections
- **Autocomplete** - Input with suggestions and filtering
- **Dropdown** - Select dropdown with search functionality
- **Multi Select** - Multiple selection dropdown with tags
- **Calendar** - Date picker with calendar interface
- **InputOTP** - One-Time Password verification
- **ControlNumber**: Numeric control input for managing numeric values
- **Knob**: Circular dial control for selecting numeric values
- **Input Password**: Password input with strength indicator and mask toggling
- **Text Editor**: Rich text editor with formatting toolbar

### Navigation Components

- **Tabs** - Tabbed interface for content organization
- **Sidebar** - Collapsible navigation sidebar
- **Paginator** - Pagination controls for data navigation
- **Cascade Menu** - Hierarchical dropdown menu with nested navigation, icons, and actions
- **Menubar** - Horizontal navigation bar with dropdown menus and submenus
- **Breadcrumb**: Navigation breadcrumb trail showing current page location
- **Steps**: Step-by-step navigation component - Click on each step to navigate
- **Popover**: Contextual popup component

### Action Components

- **Button** - Interactive buttons with multiple variants and icons
- **Chips** - Small tags for labels and selections
- **Select Button**: Button-based selection component

### Display Components

- **Card** - Content container with header, body, and footer
- **Badge** - Small status indicators and labels
- **Fieldset**: Grouped form fields with collapsible legend for organizing related inputs
- **Timeline** - Vertical timeline for events and progress
- **Table** - Advanced table with sorting, filtering, and pagination
- **Accordion** - Collapsible content sections with expand/collapse functionality and custom headers
- **Carousel** - Interactive carousel for displaying multiple items with navigation
- **Meter Group**: Visualize categorized data in a segmented bar
- **Image**: Advanced image component with preview mode

### Feedback Components

- **Notification** - Toast notifications for user feedback
- **Tooltip** - Hover tooltips for additional information
- **Dialog** - Modal dialogs for forms and confirmations
- **Message**: Contextual messages for displaying different types of feedback with multiple variants

### State Components

- **Preload** - Loading overlay for page transitions
- **Skeleton** - Placeholder content while loading
- **Spinner** - Animated loading spinner
- **ProgressBar**: Progress indicator for showing completion status or loading state

## 🔧 Compatibility

| Angular Version | Library Version | Status       |
| --------------- | --------------- | ------------ |
| 18.x            | 4.0.12+         | ✅ Supported |
| 19.x            | 4.0.12+         | ✅ Supported |
| 20.x            | 4.0.12+         | ✅ Supported |

### Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)

## 🛠 Development

### Prerequisites

- Node.js 18+
- Angular CLI 19+
- npm or yarn

### Setup

1. Clone the repository:

```bash
git clone <repository-url>
cd maxi-angular-components-test
```

2. Install dependencies:

```bash
npm install
```

3. Start the development server:

```bash
npm start
```

4. Open your browser and navigate to `http://localhost:4200`

### Available Scripts

- `npm start` - Start development server
- `npm run build` - Build the project for production
- `npm run watch` - Build and watch for changes
- `npm test` - Run unit tests

### Project Structure

```
src/
├── app/
│   ├── components/
│   │   └── maxi/           # Component implementations
│   │       ├── button/
│   │       ├── input-field/
│   │       ├── card/
│   │       └── ...
│   ├── app.component.html  # Main demo page
│   └── app.component.ts    # App component
├── public/
│   └── assets/             # Static assets
└── styles.css              # Global styles
```

## 🤝 Contributing

We welcome contributions to improve Maxi Web Components! Here's how you can help:

1. **Fork** the repository
2. **Create** a feature branch (`git checkout -b feature/amazing-feature`)
3. **Commit** your changes (`git commit -m 'Add some amazing feature'`)
4. **Push** to the branch (`git push origin feature/amazing-feature`)
5. **Open** a Pull Request

### Development Guidelines

- Follow Angular style guide
- Write comprehensive tests
- Update documentation
- Ensure accessibility compliance
- Maintain backward compatibility

## 📄 License

This project is private and proprietary. All rights reserved.

## 📞 Support

For support, questions, or feature requests, please contact our maxi development team.

---

<div align="center">
  <p>Built with ❤️ by the Maxi Team</p>
  <p>© 2025 Maxi Web Components. All rights reserved.</p>
</div>
