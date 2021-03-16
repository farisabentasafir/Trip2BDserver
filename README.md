# This is the Repository of TourPlanner server application

## To Run this on the local machine just follow the steps

### 1. First Clone the Repository to your local machine. It's recomended to clone the repo in your local htdocs folder.

   * To clone the repo run the following command: `git clone repo_link`.

### 2. Change the directory with to project directory with `cd`.

### 3. Install Composer Dependencies.
    * Run the following command to install composer dependencies.
`composer install`

### 4. Create copy of .env file.

`.env` files are not generally committed to source control for security reasons. But there is a `.env.example` which is a template of the .env file that the project expects us to have. So we will make a copy of the `.env.example` file and create a `.env` file that we can start to fill out to do things like database configurations and so on.

`cp .env.example .env`

### 5. Generate App encryption key.
     * Run the following command to generate key.
`php artisan key:generate`

### 6. Create an Empty Database.
Create an empty database with xampp control panel. 
Give the database name:
`tour_planner_db`
Now Add the db info in your .env file of the project.

### 7. Migrate the database.
To migrate the database run the following command.
`php artisan migrate`

### Database Schema : 

![](db_backup/tour_planner_db_schema2.PNG)