# Cromwell-test

## 🖥️ Installation

1. Fork the project
2. Clone 
3. Navigate to the project directory `cd cromwell-test`.
* the server code is in the root directory
4. Install dependencies for the node server code: 
```bash
npm install
```
the above will install the dependencies of the Node project

- rename .env.temp to .env
- setup values for - MONGO_URL, JWT_SECRET, JWT_LIFETIME

5. Install dependencies for the Client side (REACT):
`cd client`.
```bash
npm install
```

6. Once both Client and server dependencies are installed:
to start the node server
 `cd cromwell-test` 
```bash
npm start
```

to start the client:
 `cd client` 
```bash
npm start
```

### Features
----
#### Existing Features:
This  MERN project consists of:
1. Accounts/Registration:

* Registration: a user can register for an account, upon successful registration a user gets redirected to login page
* Login / logout: a user can easily login with their registered details and gets redirected to their profile page


2. Site Navigation: is consistent and responsive across the site it allows the user to do the following:

* User login / register
* Access to user profile (available to authenticated users)
* logout (available to authenticated users)
* Home page

3. Server side:
* User data is validated and only if valid gets added to the system
* Custom error handling and appropriate response sent to the user
* JWT gets created and attached to the response cookie upon successful login
* Authentication middleware added to get user route, resource is only returned if the use is successfully authenticated with valid token
* bcrypt used for password harsh

4. Client:
* User input is validated with real time validation and appropriate feedback to is provided to the user
* Redux toolkit is used for state management

5. Pages
* Landing page
* Login Page
* Register Page
* Home (Profile) available to authenticated users

6. Testing is provided using react testing library, Jest and Mock Service Worker to mock API communication

7. Security packages added:
* [express-mongo-sanitize](https://www.npmjs.com/package/express-mongo-sanitize)
  Sanitizes user-supplied data to prevent MongoDB Operator Injection.
* [helmet](https://www.npmjs.com/package/helmet)
  Helmet helps you secure your Express apps by setting various HTTP headers.
* [xss-clean](https://www.npmjs.com/package/xss-clean)
  Node.js Connect middleware to sanitize user input coming from POST body, GET queries, and url params.
