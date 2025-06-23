# Guide-to-Test-Generation-of-Cursor
This is just technical document file to guide playwright project using playwright

# Initialize new project with specific folder structure

*# Playwright Test Automation Framework Initialization

*## Project Initialization Instructions

I need you to help me set up a comprehensive Playwright test automation framework with TypeScript and Page Object Model pattern for the Dwara Source to Pay (STP) Application. Please follow these steps:

Base URL: https://dev.app.dwara.one/

1. Create a new Playwright project with the following structure:

   ```
   ├── tests/
   │   ├── e2e/                 # Test files organized by feature
   │   ├── fixtures/            # Test data and mocks
   │   ├── pages/               # Page Object Model classes
   │   └── utils/               # Utility functions and helpers
   ├── playwright.config.ts     # Playwright configuration
   ├── auth.config.ts           # Authentication configuration
   ├── package.json             # Project dependencies and scripts
   ├── tsconfig.json            # TypeScript configuration
   ├── .gitignore               # Git ignore files
   └── README.md                # Project documentation
   ```

2. Set up the following dependencies:

   - Playwright (latest version)
   - TypeScript
   - @playwright/test package
   - Any required libraries for reporting and visual comparison

3. Create TypeScript configuration (tsconfig.json) with appropriate settings for Playwright.

4. Set up the Playwright configuration (playwright.config.ts) with:

   - Base URL configuration for the target application
   - Browser settings (Chromium, Firefox, WebKit)
   - Viewport settings
   - Screenshot and video settings
   - Test timeout configurations

5. Create a .env file to securely store credentials:

   ```
   VALID_USER=standard_user
   INVALID_USER=locked_out_user
   PASSWORD=secret_sauce
   ```

6. Ensure .env file is added to .gitignore to prevent sensitive credentials from being committed to version control:

   ```
   # Add to .gitignore
   .env
   ```

7. Create a base Page Object class (BasePage.ts) with common methods:

   - Navigation
   - Element interaction (click, fill, etc.)
   - Verification methods
   - Waiting and assertion helpers

8. Configure the package.json with necessary scripts:
   - Run tests in headless mode
   - Run tests with UI mode
   - Run tests with specific browsers
   - Generate and view HTML reports

After initialization, I'll provide test scenarios that you'll implement using the Page Object Model pattern.
