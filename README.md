# Resume-and-CV-Management-CMS


# Route Description for Resume and CV Management CMS

## 🏠 1. Home Page
**Route:** `/`  
➡️ **GET**: Displays the landing page of the app. Users can see options to **Login** or **Register**.

## 🧑‍💼 2. User Authentication
- **Register:**  
  **Route:** `/register`  
  ➡️ **GET**: Displays the registration form for new users to create an account.  
  ➡️ **POST**: Submits registration data (username, email, password) to the backend for account creation.

- **Login:**  
  **Route:** `/login`  
  ➡️ **GET**: Displays the login form for existing users.  
  ➡️ **POST**: Submits login credentials (email, password) to authenticate the user.

- **Logout:**  
  **Route:** `/logout`  
  ➡️ **GET**: Logs out the current user and clears session data.

## 📄 3. Dashboard (User Profile)
**Route:** `/dashboard`  
➡️ **GET**: Displays the user dashboard with options to view, create, edit, or delete resumes and CVs.

## 📝 4. Create New Resume
**Route:** `/resumes/new`  
➡️ **GET**: Displays the form for creating a new resume.  
➡️ **POST**: Submits the new resume data (name, education, experience, skills, etc.) to the backend to be saved in the database.

## 📂 5. View All Resumes
**Route:** `/resumes`  
➡️ **GET**: Displays a list of all resumes stored by the user. Each resume includes options to **View**, **Edit**, **Delete**, or **Download**.

## 📋 6. View Single Resume
**Route:** `/resumes/:id`  
➡️ **GET**: Displays a detailed view of a specific resume based on the unique `id`. The user can view the entire resume information.

## ✏️ 7. Edit Resume
**Route:** `/resumes/:id/edit`  
➡️ **GET**: Displays a form pre-filled with the selected resume’s data for editing.  
➡️ **PUT**: Submits the updated resume data to the backend and updates the resume in the database.

## 🗑️ 8. Delete Resume
**Route:** `/resumes/:id/delete`  
➡️ **DELETE**: Deletes a specific resume based on the unique `id` from the database.

## 📝 9. Upload Resume (PDF/DOCX)
**Route:** `/resumes/upload`  
➡️ **GET**: Displays a file upload option for the user to upload a resume file (PDF, DOCX).  
➡️ **POST**: Handles the file upload (using `multer` middleware for handling file uploads), saves the resume data, and associates it with the user's account.

## 📥 10. Download Resume
**Route:** `/resumes/:id/download`  
➡️ **GET**: Provides a **download link** to the user for downloading the resume as a file (PDF or DOCX).

## 🧑‍💼 11. User Profile
**Route:** `/profile`  
➡️ **GET**: Displays the user’s profile information, including their name, email, and other personal details.

# 🚀 Summary Table of Routes:

| **Route**                     | **Method** | **Description**                                |
|:------------------------------|:-----------|:----------------------------------------------|
| `/`                            | **GET**    | Displays the homepage (Login/Register).       |
| `/register`                    | **GET**    | Displays the registration form.               |
| `/register`                    | **POST**   | Submits registration data (name, email, etc.).|
| `/login`                       | **GET**    | Displays the login form.                      |
| `/login`                       | **POST**   | Submits login credentials (email, password).  |
| `/logout`                      | **GET**    | Logs out the user and clears session data.    |
| `/dashboard`                   | **GET**    | Displays user’s dashboard with resume options.|
| `/resumes/new`                 | **GET**    | Displays form to create a new resume.         |
| `/resumes/new`                 | **POST**   | Submits new resume data to the backend.       |
| `/resumes`                     | **GET**    | Displays list of all resumes for the user.    |
| `/resumes/:id`                 | **GET**    | Displays a specific resume based on `id`.     |
| `/resumes/:id/edit`            | **GET**    | Displays the form to edit an existing resume. |
| `/resumes/:id/edit`            | **PUT**    | Submits updated resume data to the backend.   |
| `/resumes/:id/delete`          | **DELETE** | Deletes a specific resume based on `id`.      |
| `/resumes/upload`              | **GET**    | Displays the resume upload form.              |
| `/resumes/upload`              | **POST**   | Handles resume file upload (PDF/DOCX).        |
| `/resumes/:id/download`        | **GET**    | Provides a download link for the resume.      |
| `/profile`                     | **GET**    | Displays user profile information.            |

