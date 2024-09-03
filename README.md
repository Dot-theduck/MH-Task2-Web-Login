# Simple Web Application with Login and Homepage

## Description

This is a simple web application that consists of a login page and a homepage. The login page requires the user to enter their name, date of birth, and password. The application calculates the user's age based on their date of birth and validates it against specific criteria. If the age is between 18 and 50, the name and password are sent to a Node.js (Express) server for authentication. If the authentication is successful, the user is redirected to a homepage displaying their name and age.

## Features

- **Age Calculation:** Determines the user's age from the date of birth input.
- **Age Validation:** Ensures the user is between 18 and 50 years old. If not, an error message is displayed, and the authentication process is halted.
- **Server-Side Authentication:** The user's name and password are authenticated using hardcoded values on a Node.js (Express) server written in TypeScript.
- **Homepage:** Upon successful login, the user is redirected to a homepage where their name and age are displayed.

## Technologies Used

- **Frontend:** HTML, CSS, JavaScript
- **Backend:** Node.js, Express, TypeScript

## Setup Instructions

### Prerequisites

- Node.js (version 14 or higher)
- npm (version 6 or higher)

### Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com/your-username/simple-web-app.git
   cd simple-web-app
   ```

2. **Install the dependencies:**
   ```bash
   npm install
   ```

3. **Run the development server:**
   ```bash
   npm run dev
   ```

### Usage

1. **Open the application:**
   - Navigate to `http://localhost:3000` in your web browser.

2. **Login:**
   - Enter your name, date of birth, and password.
   - If your age is between 18 and 50, the name and password will be authenticated by the server.
   - Upon successful authentication, you will be redirected to the homepage.

3. **Homepage:**
   - The homepage will display your name and age if the login was successful.

### File Structure

```
simple-web-app/
├── src/
│   ├── index.ts           # Entry point for the Node.js server
│   ├── app.ts             # Express application setup
│   ├── routes/
│   │   └── auth.ts        # Authentication route
│   └── views/
│       ├── login.html     # Login page
│       └── homepage.html  # Homepage
├── public/
│   └── styles.css         # Basic CSS for the application
├── package.json           # Project metadata and dependencies
└── tsconfig.json          # TypeScript configuration
```

### Authentication Logic

The authentication is handled server-side in the `auth.ts` file. The server checks the submitted name and password against hardcoded values. If they match, the server sends a success response, and the user is redirected to the homepage.

### Age Calculation and Validation

The age is calculated client-side using JavaScript by subtracting the user's date of birth from the current date. If the age is not within the valid range (18-50), an error message is displayed, and the login credentials are not sent to the server.

### Customization

- **Change Hardcoded Credentials:**
  - You can modify the hardcoded credentials in the `auth.ts` file to suit your needs.

- **Styling:**
  - Update the `styles.css` file in the `public/` directory to customize the look and feel of the application.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Contact

For any inquiries, please contact [your-email@example.com](mailto:your-email@example.com).

---

This `README.md` provides a comprehensive overview of the project, including setup instructions, features, and file structure. You can adjust the details as needed to match your specific project.
