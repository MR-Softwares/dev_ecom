MERN Ecommerce
Description
An ecommerce store built with MERN stack, and utilizes third party API's. This ecommerce store enable three main different flows or implementations:

Buyers browse the store categories, products and brands
Sellers or Merchants manage their own brand component
Admins manage and control the entire store components
Features:
Node provides the backend environment for this application
Express middleware is used to handle requests, routes
Mongoose schemas to model the application data
React for displaying UI components
Redux to manage application's state
Redux Thunk middleware to handle asynchronous redux actions
Demo
This application is deployed on Vercel Please check it out 😄 here.

See admin dashboard demo

Docker Guide
To run this project locally you can use docker compose provided in the repository. Here is a guide on how to run this project locally using docker compose.

Clone the repository

git clone https://github.com/mohamedsamara/mern-ecommerce.git
Edit the dockercompose.yml file and update the the values for MONGO_URI and JWT_SECRET

Database Seed
The seed command will create an admin user in the database
The email and password are passed with the command as arguments
Like below command, replace brackets with email and password.
For more information, see code here
npm run seed:db [email-***@****.com] [password-******] // This is just an example.
Install
npm install in the project root will install dependencies in both client and server. See package.json

Some basic Git commands are:

git clone https://github.com/mohamedsamara/mern-ecommerce.git
cd project
npm install
ENV
Create .env file for both client and server. See examples:

Frontend ENV

Backend ENV

Vercel Deployment
Both frontend and backend are deployed on Vercel from the same repository. When deploying on Vercel, make sure to specifiy the root directory as client and server when importing the repository. See client vercel.json and server vercel.json.

Start development
npm run dev
Languages & tools
Node

Express

Mongoose

React

Webpack

Code Formatter
Add a .vscode directory
Create a file settings.json inside .vscode
Install Prettier - Code formatter in VSCode
Add the following snippet:
    {
      "editor.formatOnSave": true,
      "prettier.singleQuote": true,
      "prettier.arrowParens": "avoid",
      "prettier.jsxSingleQuote": true,
      "prettier.trailingComma": "none",
      "javascript.preferences.quoteStyle": "single",
    }
