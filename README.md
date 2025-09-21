Inventory Management System (Local Version)
A simple, clean, and modern web-based inventory management system built entirely with HTML, Tailwind CSS, and vanilla JavaScript. This application allows users to track items, manage stock levels, categorize products, and view daily sales reports directly in their browser.

Note: This version of the application is completely self-contained. All data is stored in your browser's memory and will reset when you refresh the page.

Features
No Setup Required: Just open the index.html file in a browser to start using it.

Item Management: Easily add, sell, and delete inventory items.

Categorization: Group items by category for better organization and a clearer view of your stock.

Stock Tracking: At-a-glance summary cards show total items, out-of-stock items, and the number of categories.

Sales Reporting: Automatically generates a report of all sales made during the current day, including total revenue and transaction count.

Responsive UI: The interface is designed to be accessible and easy to use on both desktop and mobile devices.

Technologies Used
Frontend: HTML, Tailwind CSS (via CDN), Vanilla JavaScript

How to Use
Download: Save the index.html file to your computer.

Open: Right-click the file and choose "Open with" your favorite web browser (like Chrome, Firefox, or Edge).

That's it! The application is ready to use.

How It Works
This project uses JavaScript arrays to manage the inventory and sales data. Here’s a brief look at the core data structures:

inventory array: Stores a list of item objects. Each object contains an id, name, category, quantity, and price.

sales array: Stores a record of each sale, including the item details, quantity sold, total price, and a timestamp.

All operations (adding, selling, deleting) directly modify these arrays. The UI is then re-rendered to reflect the latest state of the data.

License
This project is licensed under the MIT License.
