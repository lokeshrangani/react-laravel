# About
1. Login/Register
2. Create Event and recurring scheduled events for next 90 days.
```sh
   Name
   Description
   Start time
   End Time
   Day of the week
```
3. For Example: On 22nd July 2022 (friday), if a user is creating an event with following properties  
```sh
   Name - Event A
   Description - Discuss ABC
   Start time - 13:00
   End Time - 14:00
   Day of the week - Mon
```
4. Based on the above params, this will create schedules for next 90 days on every next-monday's dates at the event's start and end time. 

# 🔗 Links
Please Look at [Request](https://github.com/lokeshrangani/event-calendar/blob/master/request.txt) for API 

# Tech Stack
**Client:** React, Redux, Bootstrap CSS, React big calendar

**Server:** Laravel

# Installation

1. Clone the repo
   ```sh
   git clone https://github.com/lokeshrangani/event-calendar.git
   ```
2. Goto react-app folder 
   ```sh
   cd react-app
   ```
3. Install NPM packages
   ```sh
   npm install
   ```
4. Goto laravel folder 
   ```sh
   cd.. && cd laravel
   ```
5. Install Composer dependencies
   ```sh
   composer install
   ```
6. Generate Application Key
    ```sh
    php artisan key:generate
    ```
7. Generate JWT Secret
    ```sh
    php artisan jwt:secret
    ```
8. Create DB and make connection in .env
    ```sh
      DB_CONNECTION=mysql
      DB_HOST=HOST
      DB_PORT=PORT
      DB_DATABASE=DB_NAME
      DB_USERNAME=DB_USER
      DB_PASSWORD=DB_PASSWORD
    ```
9. Run Migration
    ```sh
    php artisan migrate
    ```
10. Create .env file and Set API End point in react .env
    ```sh
    REACT_APP_API_URL=PATH_TO_LARAVEL_PROJECT eg.http://localhost/event-calendar/laravel
    ```
11. Run React
    ```sh
    npm start
    ```
