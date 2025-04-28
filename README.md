# Resume-and-CV-Management-CMS

Route | Method | Description
/ | GET | Displays the homepage (Login/Register).
/register | GET | Displays the registration form.
/register | POST | Submits registration data (name, email, etc.).
/login | GET | Displays the login form.
/login | POST | Submits login credentials (email, password).
/logout | GET | Logs out the user and clears session data.
/dashboard | GET | Displays user’s dashboard with resume options.
/resumes/new | GET | Displays form to create a new resume.
/resumes/new | POST | Submits new resume data to the backend.
/resumes | GET | Displays list of all resumes for the user.
/resumes/:id | GET | Displays a specific resume based on id.
/resumes/:id/edit | GET | Displays the form to edit an existing resume.
/resumes/:id/edit | PUT | Submits updated resume data to the backend.
/resumes/:id/delete | DELETE | Deletes a specific resume based on id.
/resumes/upload | GET | Displays the resume upload form.
/resumes/upload | POST | Handles resume file upload (PDF/DOCX).
/resumes/:id/download | GET | Provides a download link for the resume.
/profile | GET | Displays user profile information.
