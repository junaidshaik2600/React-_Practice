# Tailwind Card Component Demo

This project is a simple React application demonstrating the use of Tailwind CSS to create styled user profile cards. The application displays profile cards with a background image, a title, and a description for each user.

## Project Structure

The project is structured as follows:

- **`App.jsx`**: The main component that renders a heading and a list of user profile cards.
- **`Card.jsx`**: A functional component in the `components` folder responsible for rendering an individual profile card.
- **`main.jsx`**: The entry point of the application that mounts the `App` component to the DOM.

### Technologies Used

- **React**: A JavaScript library for building user interfaces.
- **Tailwind CSS**: A utility-first CSS framework for styling the components.

## Code Overview

### `App.jsx`

The `App` component renders the main content of the application, including the heading and two `Card` components with sample usernames.

```javascript
import "./App.css";
import Card from "./components/card";

function App() {
  return (
    <>
      <h1 className="bg-green-400 p-5 rounded-xl mb-5">Tailwind test</h1>
      <Card userName="junaid1" />
      <Card userName="junaid2" />
    </>
  );
}

export default App;
```

### `Card.jsx`

The `Card` component is a reusable UI component that accepts a `userName` prop and renders a user profile card. It includes an image, a name, and placeholder text for the description. The component uses Tailwind CSS classes for styling.

```javascript
function Card({ userName }) {
  console.log(userName);

  return (
    <div className="relative h-[400px] w-[300px] rounded-md">
      <img
        src="https://images.unsplash.com/photo-1546961329-78bef0414d7c?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxzZWFyY2h8MTB8fHVzZXJ8ZW58MHx8MHx8&auto=format&fit=crop&w=800&q=60"
        alt="User Avatar"
        className="z-0 h-full w-full rounded-md object-cover"
      />
      <div className="absolute inset-0 bg-gradient-to-t from-gray-900 to-transparent"></div>
      <div className="absolute bottom-4 left-4 text-left">
        <h1 className="text-lg font-semibold text-white">{userName}</h1>
        <p className="mt-2 text-sm text-gray-300">
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Excepturi, debitis?
        </p>
        <button className="mt-2 inline-flex cursor-pointer items-center text-sm font-semibold text-black">
          View Profile →
        </button>
      </div>
    </div>
  );
}

export default Card;
```

### `main.jsx`

The `main.jsx` file is the entry point that renders the `App` component into the root of the DOM using React's `createRoot` API.

```javascript
import { StrictMode } from 'react';
import { createRoot } from 'react-dom/client';
import './index.css';
import App from './App.jsx';

createRoot(document.getElementById('root')).render(
  <StrictMode>
    <App />
  </StrictMode>
);
```

## Getting Started

1. Clone the repository and navigate to the project folder.
2. Run `npm install` to install dependencies.
3. Start the development server with `npm start`.

## Customization

- **User Profiles**: Update the `userName` prop in `App.jsx` to display different usernames.
- **Styling**: Modify Tailwind CSS classes in `Card.jsx` to change the card appearance.

## License

This project is open-source and freely available for use and modification.
