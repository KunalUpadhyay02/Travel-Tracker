# Travel Tracker

The **Travel Tracker** is a web application that allows users to track and manage the countries they've visited. It utilizes a PostgreSQL database to store country information and displays the visited countries on a user-friendly interface.

## Features
- Display a list of visited countries along with the total count.
- Add a new country to the list by entering the country name.
- Integrated with PostgreSQL to store and retrieve country data.

## Prerequisites
To run this project, ensure you have the following installed:
- [Node.js](https://nodejs.org/) (v14+)
- [PostgreSQL](https://www.postgresql.org/) (v12+)
- [Nodemon](https://nodemon.io/) (for automatic server restarting, optional)

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/username/travel-tracker.git
   cd travel-tracker

2. Install dependencies:
   ```bash
    npm install  
   ```
3. Create a .env file in the root directory and add the following database configuration:
    ```bash
    DB_USER=your_database_user
    DB_HOST=localhost
    DB_NAME=your_database_name
    DB_PASSWORD=your_database_password
    DB_PORT=5432
4. Set up the PostgreSQL database:

- Create a PostgreSQL database and populate it with two tables:
    - countries: stores country names and their corresponding codes.
    - visited_countries: stores the country codes of visited countries.
 

- Example SQL schema:

```bash
  CREATE TABLE countries (
      country_name VARCHAR(100),
      country_code VARCHAR(10)
  );

  CREATE TABLE visited_countries (
      country_code VARCHAR(10)
  );
```
## Running the Project
1. Start the server:

```bash
nodemon index.js
```
2. Access the app in your browser:
```bash
http://localhost:3000
```
## Technologies Used
- Backend: Node.js, Express.js
- Database: PostgreSQL
- Frontend: HTML, CSS (served via static files)
- Templating Engine: EJS

## License
This project is licensed under the MIT License.

Feel free to customize or extend the Travel Tracker app!
