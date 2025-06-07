# YouTube Music Clone - SaaS Style

This project is a concept for a music streaming web application. It features a modern, professional SaaS-style landing page with an embedded "YouTube Music Clone" tool. The entire front-end is built using only vanilla HTML, CSS, and JavaScript, contained within a single `index.html` file. The backend is a minimal Node.js server using Express to serve the application.

## ✨ Features

- **Modern SaaS Landing Page**: A beautiful, responsive design with sections for features, pricing, FAQs, and more.
- **Dark Mode Theme**: Easy on the eyes with red gradient accents.
- **Embedded Music Player**:
  - **Live Search**: Filter through a list of suggested videos in real-time.
  - **YouTube Iframe Player**: Plays selected videos using YouTube's official player.
  - **Player Controls**: Buttons for Play, Pause, and Fullscreen.
  - **Favorites System**: Add/remove favorite songs, which are saved to your browser's `localStorage`.
- **Fully Responsive**: Looks great on desktops, tablets, and mobile devices.
- **Zero Dependencies**: The front-end uses no external libraries like jQuery or Bootstrap.
- **Ad Placeholders**: Demonstrates potential locations for ad banners.

## 🛠️ Tech Stack

- **Backend**: Node.js, Express.js
- **Frontend**: Vanilla HTML5, CSS3, JavaScript (ES6+)
- **No external libraries or frameworks** on the front end.

## 🚀 How to Get It Working

Follow these steps to run the application on your local machine.

### Prerequisites

You must have [Node.js](https://nodejs.org/) installed on your computer, which includes `npm` (Node Package Manager).

### Setup and Installation

1.  **Download the files**:
    Save the `server.js`, `index.html`, and `README.md` files into a new project folder.

2.  **Navigate to the project directory**:
    Open your terminal or command prompt and change into the folder you just created.
    ```bash
    cd path/to/your-project-folder
    ```

3.  **Initialize npm and install dependencies**:
    This command creates a `package.json` file and installs Express, the only dependency needed for the server.
    ```bash
    npm init -y
    npm install express
    ```

4.  **Start the server**:
    Run the following command to start the Node.js server.
    ```bash
    node server.js
    ```

5.  **View the application**:
    You should see a message in your terminal: `Server is running on http://localhost:3000`. Open your web browser and navigate to this URL to use the app.

## ⚙️ How It Works

-   **`server.js`**: This file sets up a very basic web server using Express. Its sole purpose is to listen for requests on port 3000 and serve the `index.html` file to anyone who visits the root URL (`/`).

-   **`index.html`**: This is a single-file application containing three parts:
    -   **HTML**: The `<head>` and `<body>` sections structure the entire webpage, from the navigation bar and hero section to the embedded app and footer.
    -   **CSS**: All styling is located within the `<style>` tags in the `<head>`. It uses modern CSS features like Custom Properties (for theming), Flexbox, and Grid for layout, along with `@media` queries to ensure the site is responsive.
    -   **JavaScript**: All interactivity is handled by the code inside the `<script>` tag at the bottom of the `<body>`. It listens for user actions (like typing in the search bar or clicking buttons), dynamically updates the page content, controls the YouTube video player, and uses the browser's `localStorage` API to save and retrieve the user's list of favorite songs.
