# React + Vite

# React Project Setup with Vite: README Guide

## Overview
This README guide provides detailed instructions for setting up a React project using Vite, including Hot Module Replacement (HMR) and ESLint rules. Follow the steps below to create your project and run it using `npm run dev`.

## Prerequisites
- Node.js and npm installed on your machine ([Download Node.js](https://nodejs.org/))

## Getting Started

1. **Create a New React Project:**
    - Open your terminal and navigate to the desired directory.
    - Run the following commands:
        ```bash
        npx create-vite@latest my-react-project --template react
        cd my-react-project
        ```

2. **Install Dependencies:**
    - Install project dependencies using npm:
        ```bash
        npm install
        ```

3. **Run the Development Server:**
    - Start the development server with HMR:
        ```bash
        npm run dev
        ```
    - Your app will be available at `http://localhost:3000`.

4. **ESLint Configuration:**
    - Vite comes with built-in ESLint support.
    - Customize ESLint rules by creating an `.eslintrc.js` file in your project root.
    - Example `.eslintrc.js`:
        ```javascript
        module.exports = {
            extends: ['plugin:react/recommended', 'plugin:prettier/recommended'],
            rules: {
                // Add your custom rules here
            },
        };
        ```

5. **Project Structure:**
    - Your project structure will look like this:
        ```
        my-react-project/
        ├── node_modules/
        ├── public/
        ├── src/
        │   ├── main.js
        │   ├── App.jsx
        │   └── ...
        ├── .eslintrc.js
        ├── package.json
        └── ...
        ```

6. **Customize Your App:**
    - Edit `src/App.jsx` to create your React components.
    - Add styles, images, and other assets as needed.

## Available Scripts

- `npm run dev`: Starts the development server with HMR.
- `npm run build`: Builds your app for production.
- `npm run serve`: Serves the production build locally.

## Additional Resources

- [Vite Documentation](https://vitejs.dev/)
- [React Documentation](https://reactjs.org/)

Feel free to customize your project further and enjoy building with Vite and React! 🚀
Currently, two official plugins are available:

- [@vitejs/plugin-react](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react/README.md) uses [Babel](https://babeljs.io/) for Fast Refresh
- [@vitejs/plugin-react-swc](https://github.com/vitejs/vite-plugin-react-swc) uses [SWC](https://swc.rs/) for Fast Refresh
