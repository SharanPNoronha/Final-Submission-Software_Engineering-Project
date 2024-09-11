### AN INTELLIGENT HOTEL BOOKING SYSTEM

This is a room booking system designed to allow users to book hotel rooms, and for admins to manage bookings, rooms, staff, and payments. It features functionalities such as user authentication, room booking, payment processing, and an admin dashboard for managing the entire system.

---

#### Features:

1. **User Registration and Login**:
   - Users can register and log in to book rooms.
   - Encrypted passwords using 'bcrypt'.
   - Admins can also log in via a dedicated dashboard.

2. **Room Booking**:
   - Users can browse available rooms, check prices, and make bookings.
   - Users can view their booking history and cancel bookings (if applicable).
   - Admins can manage bookings from the dashboard.

3. **Payment**:
   - The system includes a simulated payment gateway.
   - Users input their card details (validated for correct format) to confirm bookings.

4. **Admin Dashboard**:
   - Admins can manage users, rooms, bookings, payments, and staff from a centralized admin dashboard.
   - Admins can view booking statuses, approve/cancel bookings, and monitor payments.

5. **Staff Management**:
   - Admins can manage staff details, such as name, position, salary, and contact details.

6. **Encrypted Passwords**:
   - User passwords are stored securely in the database using the 'bcrypt' encryption algorithm for added security.

7. **Payment Processing**:
   - Payments are logged in the system with a placeholder payment gateway (manual entry) for future processing.


-----


#### Installation Directions:


1. **Download Required Software:**
	- [XAMPP](https://www.apachefriends.org/download.html) (or any other PHP and MySQL/MariaDB development environment)
		Please download it in D drive.( If you want to download in C drive. Change the path for images under : tulip_garden-> admin -> rooms.php -> 'C:/xampp/htdocs/tulip_garden/admin/images/'   )
	
	- [Visual Studio Code](https://code.visualstudio.com/download) (or any other code editor of your choice)

2. **Download or Clone** the project from the repository.
   **Extract the Hotel Zip Folder:**
   - Extract the contents of the provided "hotel.zip" folder.

3. **Setting up the Database**:
   - Import the SQL file 'source_code/room_booking_system.sql' into MySQL using phpMyAdmin or MySQL Workbench or MySQL/MariaDB.
   - The database contains the necessary tables ('users', 'rooms', 'bookings', 'payments', 'admins', 'staff'), and some sample data, including encrypted passwords.

4. **Running the Application**:
   - Setup/Move the project files in your local server directory (e.g., XAMPP 'htdocs' Directory):
   	-Navigate to the 'D:/Xampp/htdocs' directory on your computer.
   	- Move the extracted "tulip_garden" folder into the `htdocs` directory.

5. **Start Xampp Server:**
   - Launch the Xampp control panel and start the Apache server & Mysql Server.


6. **Import Database:**
   - Open your web browser and go to http://localhost/phpmyadmin/.
   - Create a new database named "tulip_garden".
   - Inside your project directory "D:\Xampp\htdocs\tulip_garden" folder, locate the "tulip_garden.sql" SQL file.
   - Now in browser: phpMyAdmin, navigate to the "tulip_garden" database and go to the "Import" section.
   - Choose the "tulip_garden.sql" file from "D:\Xampp\htdocs\tulip_garden" folder and click the "Import" button to import the database structure.

7. **Access the Website:**
   - After successfully importing the database, Open your favorite web browser and navigate to 'http://localhost/your_project_directoryname' (Eg: http://localhost/tulip_garden)
   - This will take you to the Intelligent Hotel Room booking System website.


8. **Admin and User Login**:
   - Admin Login:
     - **Email**: 'admin@tulipgarden.com'
       **Password**: 'admin`
	or
       email 'sharanP@tulipgarden.com'
       **Password**: 'admin'

   - User Login:
     - **Email**: 'sharan_user@outlook.com'
     - **Password**: 'sharan123'
      or
 	noronhaShar@icloud.com
	noronha

9. **Functionalities**:
   - Users can browse rooms, make bookings, and confirm them through a simulated payment gateway.
   - Admins can manage rooms, bookings, users, staff, and payments from the dashboard.

---

#### Admin Features:
- **View Dashboard**: Admins can access a dashboard showing the latest bookings, room details, and staff information.
- **Manage Rooms**: Add, edit, or delete rooms. Each room has details such as price per night, description, and images.
- **Manage Users**: View and manage user accounts.
- **Manage Bookings**: Approve, cancel, or view details of bookings made by users.
- **Manage Payments**: View details of payments made through the system.

#### User Features:
- **Browse Rooms**: Users can view available rooms, with details about the room type, price, and occupancy.
- **Book Rooms**: Users can select check-in and check-out dates and confirm bookings.
- **Payment**: Users can confirm bookings by entering card details in the simulated payment gateway.
- **Manage Bookings**: Users can view, cancel, or pay for pending bookings.

---

#### Future Improvements:
- **Integration with real payment gateways**: Currently, payments are simulated. This can be replaced with a real-world gateway such as Stripe or PayPal.
- **Social Media Login**: Adding OAuth for login via Google or Facebook.
- **Advanced Reporting**: Generate detailed reports for admins on room occupancy, total payments, etc.

#### Dependencies:
- PHP 7.4 or higher
- MySQL 5.7 or higher
- Apache Server (XAMPP, WAMP, etc.)
