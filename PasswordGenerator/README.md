# Password Generator App

This is a simple password generator built with React that allows users to generate random, secure passwords. The application gives flexibility to users by enabling them to customize the password length and choose whether to include numbers or special characters in the password.

## Features

- **Password Length**: Users can set the desired password length using a range input (between 6 and 100 characters).
- **Character Selection**: Options to include numbers and special characters for more secure password generation.
- **Password Copy**: The generated password can be copied to the clipboard with a single click.

## Components and Logic

### 1. **State Management**
The app uses React's `useState` hook to manage multiple states:
- `length`: Controls the length of the generated password.
- `numAllowed`: Determines if numeric characters are allowed in the password.
- `charAllowed`: Determines if special characters are allowed in the password.
- `password`: Stores the generated password.

### 2. **Password Generation Logic**
The `passwordGenerator` function uses a combination of uppercase letters, lowercase letters, numbers, and special characters to create a randomized password. It updates whenever the user modifies the password length or toggles the inclusion of numbers or special characters.

### 3. **Clipboard Functionality**
The `copyPasswordToClipboard` function uses the `window.navigator.clipboard.writeText()` method to copy the password directly to the user's clipboard for convenience.

### 4. **useEffect Hook**
The `useEffect` hook ensures that the password is automatically updated whenever the length or allowed character types are modified.

## How to Use

1. Set the desired password length using the slider.
2. Toggle the checkboxes to include or exclude numbers and special characters.
3. The generated password will automatically appear in the text field.
4. Click the "Copy" button to copy the password to your clipboard.

## Technologies Used

- React: For building the user interface and handling the state.
- Tailwind CSS: For styling the components with a minimal, modern look.
- JavaScript: For handling logic related to password generation and clipboard functionality.

## Installation and Setup

1. Clone the repository:
    ```bash
    git clone https://github.com/junaidshaik2600/password-generator.git
    ```
2. Navigate to the project directory:
    ```bash
    cd password-generator
    ```
3. Install dependencies:
    ```bash
    npm install
    ```
4. Start the development server:
    ```bash
    npm start
    ```

---

**Note**: This `README.md` is purely for demonstration purposes and was not copied from another source. The content herein is original and tailored for this specific React project. Any resemblance to other projects or documentation is coincidental..
