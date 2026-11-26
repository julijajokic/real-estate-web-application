
# Installation and Setup

## backend setup (laravel)

Open a terminal and navigate to the backend folder

Install PHP dependencies:

```bash
composer install
```

Create the environment configuration file:

```bash
cp .env.example .env
```

Generate the application key:

```bash
php artisan key:generate
```

Configure your database connection in the `.env` file:

```env
DB_DATABASE=your_database_name
DB_USERNAME=your_database_username
DB_PASSWORD=your_database_password
```

Create the database in MySQL before running the migrations.

Run database migrations:

```bash
php artisan migrate
```

Start the Laravel development server:

```bash
php artisan serve
```

The backend will be available at:

`http://127.0.0.1:8000`

## frontend setup (react)

Open a **new terminal** and navigate to the frontend folder

Install React dependencies:

```bash
npm install
```

Start the React development server:

```bash
npm start
```

The frontend will be available at:

`http://localhost:3000`

## running the application

Both development servers must be running simultaneously:

- laravel backend: `http://127.0.0.1:8000`
- react frontend: `http://localhost:3000`

Open the frontend address in your browser to access the application
