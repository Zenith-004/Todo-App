# Simple To-Do App

Welcome to the **Simple To-Do App**! This web app allows you to manage your tasks effortlessly, with a focus on simplicity and functionality.

## 📝 Features

- **Create** tasks: Easily add new tasks to your to-do list.
- **Update** tasks: Modify your existing tasks with just a click.
- **Delete** tasks: Remove tasks you no longer need.
- **Authentication**: Basic security with HTTP Basic Authentication.
- **Real-time Rendering**: Instant updates to the task list without reloading the page.

## 🚀 Getting Started

### Prerequisites

- Node.js installed on your machine
- MongoDB Atlas or a local MongoDB instance

### Installation

1. **Clone the repository**:
   ```bash
   git clone https://github.com/Zenith-004/Todo-App.git
   cd simple-todo-app
   ```

2. **Install dependencies**:
   ```bash
   npm install
   ```

3. **Configure MongoDB**:
   - Ensure you have a MongoDB database set up. Replace the MongoDB connection string in the code with your own connection string.

4. **Run the app**:
   ```bash
   node index.js
   ```

5. **Visit your app**:
   Open your browser and go to [http://localhost:3000](http://localhost:3000).

### Deployment

The app is deployed at [https://todo-app-d1k4.onrender.com](https://todo-app-d1k4.onrender.com).

> **Note**: The server may take a moment to start up when you first visit the link. Please be patient if the page does not load immediately.

You can follow similar steps to deploy your own version on a hosting service like Render, Vercel, or Heroku.

## 🛠️ Code Overview

Here's a quick breakdown of the code structure:

### `index.js`

This is the main server file that:

- Initializes the Express app.
- Connects to MongoDB.
- Defines routes for handling CRUD operations.
- Protects the app with basic HTTP authentication.

### Key Functions

- **`passwordProtected`**: Middleware to protect routes with HTTP Basic Authentication.
- **`app.get("/")`**: Serves the main HTML page with the task list.
- **`app.post("/create-item")`**: Adds a new task to the database.
- **`app.post("/update-item")`**: Updates an existing task.
- **`app.post("/delete-item")`**: Deletes a task.

### Client-side Code

The HTML served contains embedded JavaScript to handle the UI and AJAX requests:

- **Create**: Adds new tasks without refreshing the page.
- **Update**: Allows inline editing of tasks.
- **Delete**: Removes tasks with confirmation.

### Authentication

- The app uses Basic Authentication (`Basic realm="Simple Todo App"`).
- Username and password are `learn`.

### **`browser.js`**

Handles the client-side rendering and interactivity, including creating, updating, and deleting tasks.

## 📄 License

This project is licensed under the MIT License. Feel free to use, modify, and distribute it as you wish.

## 💡 Fun Facts

- 🚀 The app is minimalistic and focuses on functionality.
- 🧙‍♂️ The authentication might be basic, but it gives a retro vibe!
- 💬 Task management has never been this straightforward!

## 🤝 Contributing

If you have suggestions or improvements, feel free to open an issue or submit a pull request.

---

Enjoy your productive journey with the Simple To-Do App! Happy tasking! 🎉

---

### P.S.

Remember, **with great power comes great responsibility**—or in this case, with a simple to-do app comes a beautifully organized life! 😉

