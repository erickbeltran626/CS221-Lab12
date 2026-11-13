# CS208 Full Stack Lab Project

- Name: Erick Beltran
- GitHub: https://github.com/erickbeltran626/CS221-Lab12.git
- Term: Fall 2026

## Project Descripton

For my CS208 full-stack project, I worked with the provided starter code to make a simple To-Do List application. The application lets users create tasks, edit them, mark them as completed, and delete them. It uses Node.js and Express to handle the backend and MariaDB to store the tasks. I also made some changes to prevent users from submitting empty tasks and updated the CSS to give the website a cleaner look with a light blue and white color scheme to look business adjacent.

## Install the Database

To set up the database, run the `install_db.sh` script. This installs MariaDB and starts the database server. You only need to do this once per Codespace.

```bash
./setup_scripts/install_db.sh
```

During setup, choose `n` for unix_socket authentication and `Y` to change the root password. Set the password to `12345` and answer `Y` to the remaining questions.

## Create the Database Tables

Run the following command to create the database tables:

```bash
sudo mysql -u root -p < ./setup_scripts/create_demo_table.sql
```

Enter the database password when asked.

## Install Dependencies

Install the dependencies using npm:

```bash
npm install
```

## Run the Application

Start the application by running:

```bash
npm start
```

## Access the Application

In GitHub Codespaces, forward port 3000 and open it in your browser to access the application.

From there, you can add new tasks, edit existing ones, mark tasks as completed, or delete them. All of the tasks are stored in the database, so they will still be there when you refresh the page.