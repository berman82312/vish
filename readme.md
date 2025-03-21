# Laravel Project

Welcome to the **Vish** Project! Follow the instructions below to set up and start developing.

## Prerequisites

Make sure you have the following installed on your machine:
- PHP >= 7.3
- Composer
- Node.js & npm
- MySQL or any other supported database

## Installation

1. **Check your environment:**
    ```bash
    php --version
    node --version
    composer --version
    ```

2. **Install dependencies:**
    ```bash
    composer install
    npm install
    ```

3. **Copy the `.env.example` file to `.env`:**
    ```bash
    cp .env.example .env
    ```

4. **Generate an application key:**
    ```bash
    php artisan key:generate
    ```

5. **Configure your database:**
    The default database is Sqlite. Change the db config if you are using other database.

    Open the `.env` file and update the following lines with your database credentials:
    ```
    DB_CONNECTION=mysql
    DB_HOST=127.0.0.1
    DB_PORT=3306
    DB_DATABASE=your_database
    DB_USERNAME=your_username
    DB_PASSWORD=your_password
    ```

6. **Run the database migrations:**
    ```bash
    php artisan migrate
    ```

7. **(Optional) Seed the database:**
    ```bash
    php artisan db:seed
    ```

## Development

1. **Start the local development server:**
    ```bash
    php artisan serve
    ```

2. **Compile the assets:**
    ```bash
    npm run dev
    ```

You can now access the project at `http://localhost:8000`.

### If your are using Herd

1. **Start the Herd services:**
    ```bash
    herd start
    ```

2. **Serving from project directory:**
    ```bash
    cd <path/to/your/project>
    herd open
    ```

## Additional Commands

- **Run tests:**
  ```bash
  php artisan test
  ```

- **Compile assets for production:**
  ```bash
  npm run production
  ```

## Contributing

Feel free to submit issues or pull requests. For major changes, please open an issue first to discuss what you would like to change.

## License

This project is licensed under the MIT License.