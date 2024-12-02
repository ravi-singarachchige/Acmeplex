# Acmeplex Movie Theater Ticket Reservation App


## Objectives
The goal of this project is to create a movie ticket registration system, where users can both buy and cancel tickets.


## Project Structure

![dir tree](images/structure.png)

+ [`config`](config) - contains the config files containing important settings for the project to work

+ [`lib`](lib) - contains the JARs used by the project

+ [`src`](src) - contains all the source code as `.java` files


## How to run

1. Clone the repository to your local machine.

2. Start the MySQL server on your local machine. 

3. Open the file [config/db_details.properties](config/db_details.properties) and enter your Db server details. For `db.user` and `db.password`, enter your DB user login details. Please use a user that has all the CRUD access, like `root`.

3. Connect to your MySQL server using an user used in step 3.

4. Run [this](ENSF480_Project_Database.sql) script on the MySQL server. This script will create a schema **ENSF480PROJECT**, create all necessary tables, and load them with some dummy data.

5. To compile the source code, run the below command
   ```bash
   $ javac -cp ".;lib/*" -sourcepath "src" -d "bin" src/movieTicketSystem/*java src/movieTicketSystem/controller/*java src/movieTicketSystem/model/*java src/movieTicketSystem/view/*java
   ```

6. To run the source code, run the below command
   ```bash
   $ java -cp ".;lib/*;bin" movieTicketSystem.movieApp
   ```

