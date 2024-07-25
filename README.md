# 🚑 EMRI Web App

This is a web application designed to assist doctors in managing the treatment of several patients belonging to the 25 ambulances allotted to them using data such as patient vitals, accessing medical documents, and communicating with Emergency Medical Technicians (EMTs) for critical cases.

The application is built using **React** for the frontend and **Node.js** with **GraphQL** for the backend, and it uses **Amazon S3** for file storage.

## 🌟 Features

- **🩺 View Vitals**: View vitals of patients assigned to the doctor.
- **📄 Document Query**: Search for medicines or procedures from uploaded medical documents.
- **💬 Live Chat**: Communicate with EMT assistants of the ambulances regarding critical cases.
- **📁 Document Management**: Admins can upload, edit, view, and delete documents.

## 🛠️ Setup Instructions

### Backend Setup

1. 📂 Navigate to the code directory.
2. 🖥️ Open a terminal and run `npm i`.
3. ✏️ Modify `server.js`:
   - Change the MongoDB connection string from `process.env.MONGO_URI` to `'mongodb+srv://dass39:dass39@emri.vubkrrz.mongodb.net/?retryWrites=true&w=majority'`.
4. 🚀 Start the servers by running `npm run dev`.

### Frontend Setup

1. 📂 Navigate to the `code/client` directory.
2. 🖥️ Open a terminal and run `npm i`.
3. 🚀 Start the frontend server by running `npm run start`.
4. 🌐 Access the application at `http://localhost:3000`.

### Live Chat Setup for EMT in an Ambulance

1. 📂 Navigate to the `emt dummy` directory.
2. 🖥️ Open a terminal and run `npm i`.
3. 🚀 Start the chat server by running `npm run start`.
4. 🌐 Access the dummy EMT chat at `http://localhost:3001`.

## 🔐 For Login

### For Doctors:
- **Email**: `doctor1@gmail.com`
- **Password**: `doctor1` (similarly for `doctor2`, `doctor3`, and so on)

### For Admin:
- **Email**: `admin1@gmail.com`
- **Password**: `admin1` (similarly for `admin2`, `admin3`, and so on)

## 🚀 Usage

1. 🌐 Navigate to `/` to access the login page.
2. 📝 For Signup, go to `/signup`.
3. Once logged in, you can:
   - 🩺 View patient vitals
   - 📄 Search medical documents
   - 💬 Chat with EMTs (if logged in as a doctor)
   - 📁 Manage documents (if logged in as an admin)

## 🔗 Supported Links

- `/`: Login page
- `/signup`: Signup page
- `/passwordreset`: Password reset page
- `/home`: Dashboard for doctors and admins
- `/profile`: Profile page for doctor or admin after login

## 📂 Interaction with Amazon S3 Storage

### In S3 Bucket:
- **📄 Documents**: `EMRI_audio_files/DASS_39/Document_query/`
- **💬 Chat Files**: `EMRI_audio_files/DASS_39/Message_files/`

### API Endpoints:

- **📤 Upload a file**: `POST http://localhost:5002/upload_files` (Field name: `image`)
- **📤 Upload a document**: `POST http://localhost:5002/upload_documents` (Field name: `image`)
- **📥 Fetch all files**: `GET http://localhost:5002/get_files`
- **📥 Fetch all documents**: `GET http://localhost:5002/get_documents`
- **🗑️ Delete all files**: `DELETE http://localhost:5002/delete_files`
- **🗑️ Delete all documents**: `DELETE http://localhost:5002/delete_documents`
- **🗑️ Delete a specific file**: `DELETE http://localhost:5002/delete_file/filename` (Replace `filename` with the actual filename)
- **🗑️ Delete a specific document**: `DELETE http://localhost:5002/delete_document/filename` (Replace `filename` with the actual filename)

Please note that multiple file uploads are commented out in the codebase, allowing only single-file uploads.

## ⚠️ Note

Ensure that the port used is 3000 for the client and 3001 for the EMT chat. Modify the CORS origin URL if necessary.

## 📄 Documentation

To view the code documentation, [click here](#).

## 🤝 How to Contribute

If you'd like to contribute to this project, please follow these steps:

1. 🍴 Fork the repository.
2. 🌿 Create a new branch: `git checkout -b feature/new-feature`.
3. ✏️ Make your changes and commit them: `git commit -m 'Add new feature'`.
4. 🚀 Push to the branch: `git push origin feature/new-feature`.
5. 🔄 Submit a pull request.

## ✨ Authors

- **Mayank Mittal**
- **Shivam Mittal**
- **Manan Garg**
- **Bassam Adnan**
- **Uday Bindal**
