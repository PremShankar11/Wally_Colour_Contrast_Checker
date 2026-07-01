# Wally Color Contrast Checker

A professional web application designed to help developers and designers ensure their color combinations meet Web Content Accessibility Guidelines (WCAG 2.1 & 2.2) standards. This tool calculates contrast ratios in real-time and provides intelligent color suggestions to meet accessibility compliance levels.

## Description

The Wally Color Contrast Checker is a client-side application that operates entirely in your browser with no data transmission to external servers. It enables you to test color combinations for accessibility compliance, validate whether foreground and background colors meet AA (4.5:1) or AAA (7.0:1) contrast ratios, and discover alternative color options that satisfy accessibility requirements.

The application features an intelligent color suggestion engine that generates diverse, visually distinct alternatives across the color spectrum rather than offering repetitive variations. Whether you are designing user interfaces, developing websites, or ensuring your digital products are accessible to everyone, this tool provides immediate feedback and practical solutions.

## Technology Stack

The application is built with modern, production-ready technologies:

- **Framework:** Next.js 16.2.9 - React framework for building performant web applications
- **Runtime:** React 19.2.4 - Latest React version for optimized component rendering
- **Color Processing:** Colord 2.9.3 - Lightweight library for color manipulation and conversion
- **Styling:** Tailwind CSS 4 - Utility-first CSS framework for rapid UI development
- **Build Tools:** Node.js-based build pipeline with integrated ESLint for code quality
- **Deployment:** Optimized for modern hosting platforms and production environments

## Features

The application provides a comprehensive suite of accessibility testing and suggestion capabilities:

- Real-time contrast ratio calculation between foreground and background colors
- WCAG AA and AAA compliance validation with clear pass/fail indicators
- Intelligent color suggestion engine that samples across the hue spectrum to provide diverse alternatives
- Interactive AA/AAA filtering to enforce strict accessibility thresholds
- Target ratio sliders to prioritize color suggestions closest to your desired contrast level
- Graceful handling of edge cases where no compliant colors exist mathematically
- Color picker interface with visual feedback through pencil icon badges
- One-click copy functionality for hex color codes with confirmation tooltips
- Responsive design that adapts to all screen sizes and devices
- Completely client-side processing with no server dependencies or data transmission

## Accessibility First Design

The Wally Color Contrast Checker is built with accessibility at its core, ensuring the tool itself meets the highest accessibility standards.

**Keyboard Navigation:**
- All interactive elements are fully accessible via keyboard
- Lightness sliders support standard keyboard controls: Arrow Up/Down for single-step adjustments, Page Up/Page Down for larger increments, Home/End to jump to minimum/maximum values
- Color pickers, buttons, and input fields are all navigable through Tab and Shift+Tab
- Focus indicators provide clear visual feedback for keyboard users

**Screen Reader Support:**
- The page title "Contrast Ratio Checker" and header are semantically marked for screen reader announcement
- Main sections including "Color Inputs" region are labeled with proper ARIA attributes
- All form inputs have descriptive labels: "Foreground Color Picker", "Background Color Hex Code", "Foreground Lightness", "Background Lightness"
- Copy buttons include clear action labels for assistive technology
- A live ARIA region continuously announces contrast ratio updates and WCAG compliance results in real-time
- Color swatches are interactive elements properly labeled for assistive technologies
- Button actions like "Swap Colors" and "Reset" are clearly announced

**Real-time Feedback:**
- Live updates to contrast ratios are automatically announced to screen readers
- WCAG compliance status (Pass/Fail) for Normal Text, Large Text, and UI Components is dynamically communicated
- Visual feedback is accompanied by ARIA live regions to ensure all users receive information simultaneously

By combining keyboard accessibility, screen reader support, and semantic HTML structure, the application ensures that users relying on assistive technologies have equal access to all features and information.

## Getting Started

### Prerequisites

Ensure you have the following software installed on your system:

- Node.js (version 18 or higher)
- npm (Node Package Manager, installed with Node.js)

### Installation

Clone the repository to your local machine:

```bash
git clone <repository-url>
cd Wally_Color_Contrast_Checker
```

Install project dependencies:

```bash
npm install
```

### Running the Application

Start the development server:

```bash
npm run dev
```

Open your browser and navigate to `http://localhost:3000` to access the application. The page will automatically refresh as you make changes to the source code during development.

### Building for Production

Create an optimized production build:

```bash
npm run build
```

Start the production server:

```bash
npm start
```

### Linting and Code Quality

Run the linter to check code quality and identify potential issues:

```bash
npm run lint
```

## How to Use

Using the Wally Color Contrast Checker is straightforward:

1. Select a background color using the interactive color picker
2. Select a foreground color (text color) using the color picker
3. View the calculated contrast ratio and WCAG compliance status
4. Check whether your color combination passes AA or AAA standards
5. Review the suggested alternatives panel for compliant color options
6. Use the AA/AAA toggle to filter suggestions by compliance level
7. Adjust the target ratio slider to prioritize colors closest to your desired contrast
8. Click any suggested color to preview it or copy the hex code with the copy button
9. Scroll through results on mobile devices to access all interface elements

## Contributing

We welcome contributions from the community. To contribute to this project:

1. Fork the repository on GitHub
2. Create a new branch for your feature or bug fix:
   ```bash
   git checkout -b feature/your-feature-name
   ```
3. Make your changes following the project's coding standards
4. Test your changes thoroughly with the development server
5. Run the linter to ensure code quality:
   ```bash
   npm run lint
   ```
6. Commit your changes with clear, descriptive messages:
   ```bash
   git commit -m "Add detailed description of your changes"
   ```
7. Push your branch to your fork:
   ```bash
   git push origin feature/your-feature-name
   ```
8. Open a pull request on the main repository with a detailed description of your changes

When submitting contributions, please ensure your code:
- Follows React and Next.js best practices
- Maintains the existing code style and structure
- Includes appropriate comments for complex logic
- Works correctly across different screen sizes and devices
- Preserves the accessibility-first approach of the application

## License

This project is open source and available under the terms specified in the LICENSE file. Please review the LICENSE file for complete details on usage and distribution.

## Accessibility

The Wally Color Contrast Checker itself is built with accessibility in mind. If you encounter any accessibility barriers while using the application, please open an issue to let us know how we can improve the experience for all users.
