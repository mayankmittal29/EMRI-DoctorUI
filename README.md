# 🚑 EMRI Web App 💉

- This web application is designed to assist doctors in managing the treatment of patients assigned to them across 25 ambulances. It utilizes patient vitals, medical documents, and live communication with Emergency Medical Technicians (EMTs) for critical cases.

- Built using React for the frontend and Node.js with GraphQL for the backend.

## Features Provided 🌟

1. **View Vitals:** View vitals of patients assigned to the doctor.
2. **Document Query:** Search for medicines or procedures from uploaded medical documents.
3. **Live Chat:** Communicate with EMT assistants regarding critical cases.

## Setup Instructions 🛠️

### Backend Setup:

Navigate to the **code** directory.

Open a terminal and run `npm i`.

Modify server.js:

Start the server by running `nodemon server.js`.

### Frontend Setup:

Navigate to the client directory.

Open a terminal and run `npm i`.

Start the frontend server by running `npm run start`.

Access the application at [http://localhost:3000](http://localhost:3000).

### Live Chat Setup:

Navigate to the emt dummy 2 directory.

Open a terminal and run `npm i`.

Start the chat server by running `npm run start`.

Access the dummy EMT chat at [http://localhost:3001](http://localhost:3001).

## Default Login (for Development) 🔐

- **Username:** admin
- **Password:** admin

## Usage 🖥️

- Navigate to `/` to access the login page.
- For Signup, go to `/signup`.
- For development, you may directly navigate to `/home`.
- Once logged in, you'll be able to view patient vitals, search medical documents, and chat with EMTs.

## Supported Links 🌐

- `/`: Login page.
- `/signup`: Signup Page.
- `/passwordreset`: To reset password.
- `/forgotpassword`: To enter Email to reset password after forgetting the real one.
- `/forgotresetpassword`: Opens after clicking on link sent on Email to reset password.
- `/home`: Dashboard for doctors.
- `/emt-dummy-2`: Chat interface for dummy EMT.

## Note 📝

- Ensure that the port used is 3000 for the client and 3001 for the EMT chat. Modify CORS origin URL if necessary.

## How to Contribute 🌱

If you'd like to contribute to this project, please follow these steps:
1. Fork the repository.
2. Create a new branch: `git checkout -b feature/new-feature`.
3. Make your changes and commit them: `git commit -m 'Add new feature'`.
4. Push to the branch: `git push origin feature/new-feature`.
5. Submit a pull request.

## Authors 🧑‍💻

- [Shivam Mittal](https://github.com/mittalshivam2709)
- [Manan Garg](https://github.com/manangarg21)
- [Mayank Mittal](https://github.com/mayankmittal29)
- [Bassam Adnan](https://github.com/bassamadnan)
- [Uday Bindal](https://github.com/udaybindal01)
