# BudgetWise – Smart Personal Finance Manager

## Run locally
1. Open this folder in VS Code.
2. Open the terminal in the folder containing `package.json`.
3. Run `npm install`.
4. Run `npm run dev`.
5. Open the local URL shown by Vite.

## Sign-in and registration
- Demo sign-in: `demo@budgetwise.app`
- Demo password: `budgetwise123`
- New users can select Register, enter their name, email and password, and create a temporary demo account.
- Accounts and app data are stored only in React state. They reset after refreshing the page.

This is a frontend review prototype. It does not connect to a backend, database, or real authentication service. Do not use real or sensitive passwords.


## Login and registration storage

- Registration checks whether the email is already registered.
- A successful registration displays a confirmation message and opens the dashboard.
- Login checks the saved email and password and displays a success message.
- User records are saved in browser `localStorage` under `budgetwise_users`.
- The signed-in session is saved under `budgetwise_session`, so the user stays signed in after refreshing.
- Logout clears the saved session but does not delete the registered account.

**Security note:** This is a frontend learning prototype. Passwords stored in localStorage are not secure. Do not use real or reused passwords. A real application needs server-side authentication and secure password hashing.
