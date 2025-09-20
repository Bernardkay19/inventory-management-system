Inventory Management System
A simple, clean, and modern web-based inventory management system built with HTML, Tailwind CSS, and Google Firebase. This application allows users to track items, manage stock levels, categorize products, and view daily sales reports in real-time.

Features
Real-time Database: All data is stored and synced in real-time using Firestore, ensuring your inventory is always up-to-date.

Item Management: Easily add, sell, and delete inventory items.

Categorization: Group items by category for better organization and filtering.

Stock Tracking: At-a-glance view of total items, out-of-stock items, and low-stock warnings.

Sales Reporting: Automatically generates a report of all sales made during the current day, including total revenue and transaction count.

Responsive UI: The interface is designed to be accessible and easy to use on both desktop and mobile devices.

Technologies Used
Frontend: HTML, Tailwind CSS, Vanilla JavaScript

Backend & Database: Google Firebase (Firestore and Authentication)

Deployment: GitHub Pages

How to Set Up and Run This Project
To run this project on your own, you will need to set up your own Google Firebase project, as the data backend is not public.

Clone the Repository:

git clone [https://github.com/your-username/your-repository-name.git](https://github.com/your-username/your-repository-name.git)

Create a Firebase Project:

Go to the Firebase Console.

Click "Add project" and follow the setup steps.

Once your project is created, click the web icon (</>) to add a web app to your project.

Give it a nickname and Firebase will provide you with a firebaseConfig object. Copy this object.

Set up Firestore Database:

In your Firebase project console, go to the "Firestore Database" section.

Click "Create database" and start in test mode for initial setup. (You can configure security rules later).

Update the index.html file:

Open the index.html file.

Find the <script type="module"> section at the bottom.

You will need to replace the placeholder variables with your own Firebase configuration. Delete these lines:

const appId = typeof **app_id !== 'undefined' ? **app_id : 'default-inventory-app';
let firebaseConfig;
try {
firebaseConfig = typeof **firebase_config !== 'undefined' ? JSON.parse(**firebase_config) : null;
} catch (e) {
// ... error handling
}

And replace them with the firebaseConfig object you copied from your Firebase project, like this:

// Replace with your own Firebase configuration
const firebaseConfig = {
apiKey: "AIza....",
authDomain: "your-project-id.firebaseapp.com",
projectId: "your-project-id",
storageBucket: "your-project-id.appspot.com",
messagingSenderId: "...",
appId: "..."
};

const app = initializeApp(firebaseConfig);
// ... the rest of the script continues

Note: The appId variable also needs to be removed or replaced with your actual App ID if you use it elsewhere. In this project, it's used to construct the database path, so you can hardcode a unique name or use your project ID.

Open in Browser:

You can now open the index.html file directly in your web browser to see the application running with your own database.

License
This project is licensed under the MIT License. See the LICENSE file for details.
