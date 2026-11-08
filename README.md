# Student Management Dashboard

A simple student-record dashboard with an Express API, a SQLite database, and a vanilla JavaScript frontend.

## Requirements

- Node.js and npm

## Run locally

```sh
npm install
npm start
```

Open [http://localhost:3000](http://localhost:3000). The app creates `students.db` in the project directory on first run. Set `PORT` to change the listening port, or set `DATABASE_PATH` to choose another SQLite database file.

## GitHub and deployment

The source is hosted at [StudentDB on GitHub](https://github.com/bruhndoomgoof/StudentDB). Clone it with:

```sh
git clone https://github.com/bruhndoomgoof/StudentDB.git
cd StudentDB
```

Do not commit `students.db`, `node_modules`, or real student information.

GitHub Pages only hosts static files; it cannot run this app's Express API or SQLite database. To make the working application accessible online, deploy it to a Node.js host and configure persistent storage for the SQLite file using `DATABASE_PATH`. Many hosts use temporary filesystems, so data may otherwise be lost when the service restarts or redeploys.

**Privacy:** This is a demonstration app and has no authentication or access controls. Do not deploy it with real student records or use it to store personal information on a public service.
