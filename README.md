URL Shortener and Logging Web Application
This is a responsive, modern web application built with React that allows users to shorten URLs, view statistics, handle redirections via shortcodes, and log structured events to an evaluation server. The project follows a modular and scalable design, using functional components and a clean CSS-based interface.

Features
URL Shortening – Convert long URLs into concise, shareable shortcodes.

Statistics View – Access and review data related to shortened URLs.

Redirection Support – Automatically handle navigation from shortcodes to target URLs.

Custom Logging – Send structured logs with stack, severity, and context to an external service.

Responsive UI – Works across devices with a polished, professional design.

Unit Testing – Basic test coverage using @testing-library/react.

Project Structure
pgsql
Copy
Edit
├── public/
│   └── logo.svg
├── src/
│   ├── components/
│   │   ├── RedirectHandler.js
│   │   └── LogButton.js
│   ├── pages/
│   │   ├── UrlShortenerPage.js
│   │   └── UrlStatsPage.js
│   ├── App.js
│   ├── App.css
│   ├── index.js
│   ├── index.css
│   ├── log.js
│   ├── reportWebVitals.js
│   ├── setupTests.js
│   └── App.test.js
Prerequisites
Before you begin, ensure you have the following installed:

Node.js (v14 or higher)

npm or yarn

Installation
Clone the repository and install dependencies:

bash
Copy
Edit
git clone https://github.com/your-username/url-shortener-app.git
cd url-shortener-app
npm install
Or with yarn:

bash
Copy
Edit
yarn install
Running the Application
Start the development server with:

bash
Copy
Edit
npm start
Or:

bash
Copy
Edit
yarn start
The app will be available at http://localhost:3000.

Testing
Run tests using:

bash
Copy
Edit
npm test
Or:

bash
Copy
Edit
yarn test
This will execute tests defined in App.test.js using @testing-library/react.

Logging Service Integration
This application includes a utility (log.js) to send logs to an external evaluation service.

Usage
js
Copy
Edit
log("frontend", "info", "component", "Shortened URL successfully", "<your_token>");
Parameters
stack: "frontend" or "backend"

level: One of "debug", "info", "warn", "error", "fatal"

logPackage: Logical context, e.g., "component", "hook", "utils"

message: Descriptive log message

token: Bearer token for authentication

Logs are sent via HTTP POST to http://20.244.56.144/evaluation-service/logs.

Styling and UI
Gradient-based backgrounds for a modern aesthetic

Animated SVG logo support

Responsive typography and layout

Accessible buttons and interactive elements

Uses both App.css and index.css for scoped and global styles
