# Color Selector Application

This project is a simple yet dynamic color selector application built with **React** and styled using **Tailwind CSS**. The app allows users to change the background color of the screen with a single click, using buttons styled and placed in a flexible, responsive layout.

## Features

- **Interactive Color Change**: A user-friendly interface that lets users change the background color of the screen by selecting one of several preset color buttons.
- **Responsive Layout**: Built with Tailwind CSS to ensure the UI is flexible and responsive across various screen sizes.
- **Dynamic Styling**: Each button is dynamically styled to match the color it represents, offering a visual preview of the selected color on the button itself.
- **Accessible and Intuitive Design**: Buttons are centrally positioned and easy to interact with, providing a smooth user experience.

## Project Structure

The main components of the application are as follows:

- **App.jsx**: Contains the primary `App` component where the color state is managed and buttons are rendered for each color option.
- **main.jsx**: Serves as the root file, rendering the `App` component within `StrictMode` for improved error handling and warnings.
- **App.css** and **index.css**: Style sheets with custom Tailwind CSS classes to enhance the design.

## Installation and Setup

1. Clone the repository:
   ```bash
   git clone https://github.com/junaidshaik2600/color-selector-app.git
   ```

2. Navigate to the project directory:
   ```bash
   cd BgChanger
   ```

3. Install dependencies:
   ```bash
   npm install
   ```

4. Start the development server:
   ```bash
   npm start
   ```

Your application will run on `http://localhost:3000` by default..

## How It Works

The main logic is centered in `App.jsx`, where we define a `color` state variable using the `useState` hook to manage the background color. Each button has an `onClick` event that updates the `color` state with the respective color value, changing the background color of the entire screen..

Each color button is styled with Tailwind CSS classes to give it a unique look and shadow effect, providing a clear and polished appearance to users...

---

This project serves as a great foundation for learning about React state management and Tailwind CSS styling.
