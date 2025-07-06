# Operon Portal - A Firebase Studio Project

This is a Next.js application built with Firebase Studio, designed to be an operational portal for a company. It includes features for managing work orders, job cards, and production files, all integrated with Google Cloud's Firebase services.

## Getting Started

The application is ready to run. To get started, explore the different sections available in the dashboard.

-   `src/app/page.tsx`: The landing page.
-   `src/app/dashboard`: The main operational dashboard and its sub-pages.
-   `src/ai`: Contains Genkit AI flows (if any are added).

## Required Environment Variables

To connect the application to your Firebase project, you need to set up a service account and create an environment variable.

### How to get your `FIREBASE_SERVICE_ACCOUNT_KEY`

1.  **Open the Firebase Console:**
    Navigate to [https://console.firebase.google.com/](https://console.firebase.google.com/).

2.  **Select Your Project:**
    Choose the Firebase project you are working with.

3.  **Go to Project Settings:**
    Click on the gear icon (⚙️) next to "Project Overview" in the left-hand sidebar, and then select "Project settings".

4.  **Navigate to the "Service accounts" Tab:**
    In the Project settings page, click on the "Service accounts" tab.

5.  **Generate a New Private Key:**
    Click the **"Generate new private key"** button. A confirmation dialog will appear. Click **"Generate key"**. This will download a JSON file to your computer.

6.  **Copy the JSON Content:**
    Open the downloaded JSON file with a text editor. Copy the *entire contents* of the file.

7.  **Create the Environment Variable:**
    In your development environment (or your hosting provider's configuration), create a new environment variable named `FIREBASE_SERVICE_ACCOUNT_KEY`.

8.  **Set the Environment Variable Value:**
    Paste the entire JSON content you copied as the value for the `FIREBASE_SERVICE_ACCOUNT_KEY`. The value should be a single-line string, so make sure to remove any line breaks if you copy it from a formatted view.

    Example of the final value (all in one line):
    `{"type": "service_account", "project_id": "...", ...}`

Your application will now be able to securely authenticate with your Firebase project and use services like Firestore.
