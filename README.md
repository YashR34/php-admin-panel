# PHP Admin Panel Template

This is a PHP admin panel template built using PHP, HTML, Bootstrap, CSS, and JavaScript. The template provides a responsive and customizable admin panel for managing various aspects of a web application.

## Features

- Responsive Design using Bootstrap
- User Authentication
- Dashboard with Key Metrics
- CRUD Operations for Data Management
- Modular and Scalable Code Structure

## Technologies Used

- PHP
- HTML
- Bootstrap
- CSS
- JavaScript

## Getting Started

### Prerequisites

- XAMPP or any other PHP development environment
- Git

### Installation

1. Clone the repository:
    ```sh
    git clone https://github.com/YashR34/admin_p.git
    cd php_admin_panel_template
    ```

2. Move the project files to your XAMPP htdocs directory:
    ```sh
    mv php_admin_panel_template /path/to/xampp/htdocs/admin_panel
    ```

3. Create a database in MySQL:
    - Open phpMyAdmin (http://localhost/phpmyadmin)
    - Create a new database named `admin_panel`

4. Import the `admin_panel.sql` file into the `admin_panel` database:
    - In phpMyAdmin, select the `admin_panel` database
    - Go to the Import tab
    - Choose the `admin_panel.sql` file from the project directory
    - Click Go

5. Update the database configuration in `config.php` file:
    ```php
    <?php
    $servername = "localhost";
    $username = "root";
    $password = "";
    $dbname = "admin_panel";

    // Create connection
    $conn = new mysqli($servername, $username, $password, $dbname);

    // Check connection
    if ($conn->connect_error) {
        die("Connection failed: " . $conn->connect_error);
    }
    ?>
    ```

6. Make sure to create an `uploads` folder inside the `assets` directory for storing uploaded files:
    ```sh
    mkdir -p assets/uploads
    ```

7. Start XAMPP and ensure Apache and MySQL are running.

8. Access the admin panel by navigating to:
    ```
    http://localhost/admin_panel
    ```

## Usage

- Login with the default admin credentials:
    ```
    Username: admin
    Password: admin123
    ```
- Customize the dashboard and manage your web application through the admin panel.
- Implement additional modules and features as needed.

## Contributing

1. Fork the repository.
2. Create your feature branch:
    ```sh
    git checkout -b feature/your-feature
    ```
3. Commit your changes:
    ```sh
    git commit -m 'Add some feature'
    ```
4. Push to the branch:
    ```sh
    git push origin feature/your-feature
    ```
5. Open a pull request.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Contact

For any questions or feedback, please contact [YashR34](https://github.com/YashR34).
