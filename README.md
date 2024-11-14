
# SLIM (Site Learning Information Management)

## Description

Schools often face difficulties in effectively managing student, teacher, and school activity administration. Academic data, schedules, attendance, and reports are often managed manually, which is time-consuming and prone to errors.

**Solution:**
Building an Integrated School Management Website that can be used by students, teachers, and administration to manage various academic and non-academic aspects online.

## Features

- **Student Dashboard:** Displays grades, attendance, class schedules, and assignments.
- **Teacher Dashboard:** Manages schedules, assigns tasks, and inputs grades.
- **Online Attendance System:** Attendance is taken electronically and can be accessed by parents in real-time.
- **Financial Management:** Features for online payment of tuition fees and other administrative fees.
- **School Activity Notifications:** Information about school events, exams, and parent meetings.

## Impact

- More efficient and transparent administrative processes.
- Reduces the burden on teachers in managing grades and assignments.
- Students become more disciplined with a clear attendance and assignment system.

## Prerequisites

Before proceeding, ensure you have:

- PHP >= 8.2 (Recommended: PHP 8.2 or higher)
- Composer (Recommended: Latest version)
- Node.js >= 16.x (for npm)
- MySQL >= 5.7 (or MariaDB)


## Installation

Follow these steps to set up your development environment:

1. **Clone the repository**

   ```bash
   git clone https://github.com/TakanashaTaryu/SLIM.git
   cd SLIM
   ```

2. **Install PHP dependencies using Composer**

   if you didnt have composer installed, [click here](https://getcomposer.org/download/) to download composer and follow installation instruction
   ```bash
   composer install
   ```




3. **Install JavaScript dependencies using npm**

   ```bash
   npm install
   ```

4. **Copy the `.env.example` file to `.env`**

   ```bash
   cp .env.example .env
   ```

5. **Set up the database configuration in the `.env` file**

   Edit the `.env` file and adjust the database configuration according to your environment.

6. **Generate the application key**

   ```bash
   php artisan key:generate
   ```

7. **Migrate and seed the database**

   If applicable, run the migrations and seeders to create tables and populate initial data:

   ```bash
   php artisan migrate:fresh
   php artisan db:seed
   ```

8. **Compile front-end assets**

   ```bash
   npm run build
   npm run dev
   ```

## Usage

Run the Laravel development server:

```bash
php artisan serve
```

Open your browser and navigate to `http://localhost:8000` to view the application.

## Contribution

If you would like to contribute, please follow these steps:

1. Fork this repository.
2. Create a new branch for the feature or fix you wish to add.
3. Commit your changes.
4. Push to your branch and create a Pull Request.

## Note

1. Use ```.blade.php``` files in ```resources/views``` for the overall layout and static pages.

2. Use ```.vue``` files in ```resources/js/pages``` or ```components``` for dynamic, interactive content that Vue manages.

3. Make sure to use ```<script setup>``` for Vue components.
4. Make sure to have running MySQL or SQLite database and configure the ```.env``` file with the correct database.connection details.
5. Run test with ```php artisan test``` if necessary.

## License

This project is licensed under the [MIT License](LICENSE).
"# SLIM2" 
