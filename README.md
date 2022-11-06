~Description
Create a simple app where admins can create interviews by selecting participants, interview start time and end time

~Basic Requirements
1 An interview creation page where the admin can create an interview by selecting participants, start time and end time. Backend should throw error with proper error message if: 
  a. Any of the participants is not available during the scheduled time (i.e, has another interview scheduled)
  b. No of participants is less than 2
2. An interviews list page where admin can see all the upcoming interviews.
3. Note: No need to add a page to create Users/Participants. Create them directly in the database


~Instructions to run the project

1 Clone this repository.
2 Run `npm install`
3 Login to MySQL using your root user.
4 Execute the following MySQL Queries:
  4.1 `CREATE USER 'username'@'localhost' IDENTIFIED WITH mysql_native_password BY 'password';`
  4.2 `GRANT ALL PRIVILEGES ON DB_NAME.* TO 'username'@'localhost';`
  4.3 `FLUSH PRIVILEGES;`
  4.4 `exit`
5 Rename the following files:
  * .env.example --> .env
  * ormconfig.json.example --> ormconfig.json
6 Give `username`, `password` and `database` (DB_NAME) info in **ormconfig.json** for typeorm to properly connect to the Database.
7 Provide `NODE_ENV` (dev/prod), `PORT`, `EMAIL`, `PASSWORD` in **.env** file
8 Execute `npm start`.
