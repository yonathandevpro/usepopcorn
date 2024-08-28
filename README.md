### Project Overview

**Project Name:** UsePopcorn

This project is a dynamic React web application that allows users to search for movies, view detailed information about them, rate them, and manage a list of movies they've watched. The project leverages several custom hooks and components to enhance user experience, manage state, and integrate with external APIs.

### Table of Contents
- [Installation](#installation)
- [Features](#features)
- [File Structure](#file-structure)
- [Usage](#usage)
- [Components](#components)
- [Hooks](#hooks)
- [Configuration](#configuration)
- [Contributing](#contributing)
- [License](#license)

### Installation

1. Clone the repository:
    ```bash
    git clone https://github.com/yonathandevpro/usepopcorn.git
    ```
2. Navigate to the project directory:
    ```bash
    cd usepopcorn
    ```
3. Install the dependencies:
    ```bash
    npm install
    ```
4. Start the development server:
    ```bash
    npm run dev
    ```
   The app will be running at `http://localhost:5173/`.

### Features

#### 1. **Movie Search and Display**
   - **Search Bar Integration:** Users can search for movies by typing in a query. The app automatically fetches and displays movie results from an external API based on the search query.
   - **Loading and Error Handling:** The app manages loading states while fetching data and gracefully handles any errors that occur during API requests.
   - **Dynamic Movie List:** Movies matching the search query are dynamically displayed in a list. Users can click on a movie to view more details.

#### 2. **Movie Details and Management**
   - **Movie Details View:** When a user selects a movie, detailed information about the movie, such as the plot, genre, and ratings, is displayed. This view also provides options for user interaction.
   - **Watched Movies Management:** Users can add movies to their "watched" list, where the app tracks movies the user has already seen. This list is persistent, thanks to local storage integration.
   - **Remove from Watched List:** Users can remove movies from their watched list, allowing them to manage their movie collection effectively.

#### 3. **Custom Star Rating System**
   - **StarRating Component:** The app includes a custom, reusable `StarRating` component that allows users to rate movies. The component is highly configurable, with options for setting maximum rating values, color, and initial rating.
   - **Dynamic Feedback:** The star rating component provides immediate feedback to users, displaying the selected rating alongside the movie details.

#### 4. **State Management and Persistence**
   - **useLocalStorageState Hook:** This custom hook is used to persist state in the browser's local storage. It ensures that the list of watched movies is saved across sessions, providing a seamless user experience.
   - **useMovies Hook:** This hook abstracts the logic for fetching movies from the API and manages the associated states, including loading and error handling.

#### 5. **Keyboard Shortcuts**
   - **useKey Hook:** The app includes a custom hook for handling keyboard shortcuts, making the user interface more interactive and accessible. For instance, certain actions can be triggered by pressing specific keys.

### File Structure

```plaintext
usepopcorn/
│
├── public/
│   └── vite.svg
│
├── src/
│   ├── App.jsx
│   ├── App-v1.jsx
│   ├── App-v2.jsx
│   ├── StarRating.jsx
│   ├── index.css
│   ├── main.jsx
│   ├── useKey.jsx
│   ├── useLocalStorageState.js
│   └── useMovies.js
│
├── .eslintrc.cjs
├── .gitignore
├── index.html
├── package-lock.json
├── package.json
├── README.md
└── vite.config.js
```

### Usage

The main application logic is contained within `App.jsx`. Different versions of the app (`App-v1.jsx` and `App-v2.jsx`) are also included for reference or experimental purposes.

To use the project:

1. Ensure you have Node.js installed.
2. Follow the installation steps mentioned above.
3. Start the development server.
4. Open your browser and navigate to `http://localhost:5173/`.

### Components

- **App.jsx:** The main application component that ties together all other components and manages the application's state.
- **StarRating.jsx:** A reusable star rating component that allows users to rate movies.
- **App-v1.jsx & App-v2.jsx:** Experimental versions of the main app component, providing alternative layouts or functionality.

### Hooks

- **useLocalStorageState.js:** Manages state with local storage persistence, allowing for state to be saved across browser sessions.
- **useMovies.js:** Handles fetching and managing movie data from an API, including managing loading and error states.
- **useKey.jsx:** Manages keyboard events within the app, allowing for interactive shortcuts.

### Configuration

- **vite.config.js:** Configuration file for Vite, a fast build tool that serves the development server and builds the app.
- **.eslintrc.cjs:** ESLint configuration file for code quality and consistency.
- **package.json:** Lists dependencies and scripts for running, building, and testing the app.

### Contributing

Contributions are welcome! If you would like to contribute, please fork the repository and submit a pull request. 
Email me `yonathanber@icloud.com` for more info.

### License

This project is licensed under the MIT License. 

