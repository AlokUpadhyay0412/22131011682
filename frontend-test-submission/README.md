
# React URL Shortener Application

This is a production-grade, frontend-only URL Shortener web application built using React and Material UI.

## Features

- Shorten up to 5 URLs concurrently
- Custom shortcodes with uniqueness validation
- Optional expiry support (defaults to 30 minutes)
- Click analytics (frontend-mocked)
- Redirect from short URL to original target
- Integrated logging middleware for all major actions

## Tech Stack

- React (with Hooks)
- Material UI for components and styling
- React Router for routing
- JavaScript (ES6+)
- Custom Logging via token-based API

## Project Structure

```
├── public/
│   └── logo.svg                 # Application logo
├── src/
│   ├── components/
│   │   ├── RedirectHandler.js   # Handles automatic redirection
│   │   └── LogButton.js         # Triggers logging via API
│   ├── pages/
│   │   ├── UrlShortenerPage.js  # Home page for shortening URLs
│   │   └── UrlStatsPage.js      # Displays analytics/stats (mocked)
│   ├── App.js                   # Main application router
│   ├── App.css                  # Application-specific styles
│   ├── index.js                 # Application entry point
│   ├── index.css                # Global styles and theming
│   ├── log.js                   # Logging utility for sending logs
│   ├── reportWebVitals.js       # Performance metrics hook
│   ├── setupTests.js            # Jest test environment setup
│   └── App.test.js              # Unit test for root component
```
