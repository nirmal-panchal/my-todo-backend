# **To-Do App Backend**

A robust and scalable **To-Do App Backend** built with **Node.js**, **Express**, **TypeScript**, and **MongoDB**. This backend provides a RESTful API for managing tasks, including features like task creation, updating, deletion, and fetching tasks.

---

## **Features**

- 🛠️ **RESTful API**: Provides endpoints for CRUD operations on tasks.
- 📦 **TypeScript**: Ensures type safety and improves code maintainability.
- 💾 **MongoDB**: A NoSQL database for storing task data.
- 🔒 **Error Handling**: Comprehensive error and response management.
- 🚀 **Scalable**: Built with modular architecture for scalability and maintainability.

---

## **Tech Stack**

### **Core Technologies**
- **[Node.js](https://nodejs.org/)**: JavaScript runtime for building the server.
- **[Express](https://expressjs.com/)**: Minimal and flexible web application framework.
- **[TypeScript](https://www.typescriptlang.org/)**: Enhances code reliability with static typing.
- **[MongoDB](https://www.mongodb.com/)**: NoSQL database for fast and efficient data management.

### **Utilities**
- **[dotenv](https://github.com/motdotla/dotenv)**: Manages environment variables securely.
- **[Mongoose](https://mongoosejs.com/)**: Elegant MongoDB object modeling for Node.js.

---

## **Getting Started**

Follow the steps below to set up the backend locally.

### **Prerequisites**
Ensure you have the following installed:
- [Node.js](https://nodejs.org/) (v18 or higher)
- [MongoDB](https://www.mongodb.com/)
- [npm](https://www.npmjs.com/) or [yarn](https://yarnpkg.com/)

### **Installation**

1. **Clone the Repository**
   ```bash
   git clone https://github.com/your-username/todo-backend.git
   cd todo-backend
   ```

2. **Install Dependencies**
   ```bash
   npm install
   ```

3. **Set Up Environment Variables**
   Create a `.env` file in the root directory and add the following:
   ```env
   PORT=5000
   MONGO_URI=mongodb://localhost:27017/todoapp
   ```

4. **Run the Development Server**
   ```bash
   npm run dev
   ```

5. **API Documentation**
   Access the API via `http://localhost:5000/api/tasks`.

---

## **Project Structure**

```plaintext
todo-backend/
├── src/
│   ├── app.ts          # Entry point of the app
│   ├── routes/         # API routes
│   │   └── taskRoutes.ts
│   ├── controllers/    # Route handlers
│   │   └── taskController.ts
│   ├── models/         # Mongoose models
│   │   └── taskModel.ts
├── .env                # Environment variables
├── tsconfig.json       # TypeScript configuration
├── package.json        # Project dependencies and scripts
└── README.md           # Documentation
```

---

## **Scripts**

- `npm run dev`: Start the server in development mode with **nodemon**.
- `npm run build`: Compile TypeScript into JavaScript.
- `npm start`: Start the server in production mode.
- `npm run lint`: Run ESLint to check for code issues.

---

## **API Endpoints**

### **Base URL**
```
http://localhost:5000/api/tasks
```

### **Endpoints**
| Method | Endpoint       | Description                | Payload                 |
|--------|----------------|----------------------------|-------------------------|
| GET    | `/`            | Fetch all tasks           | -                       |
| POST   | `/`            | Create a new task         | `{ title: string }`     |
| PUT    | `/:id`         | Update a task             | `{ title, completed }`  |
| DELETE | `/:id`         | Delete a task             | -                       |

---

## **Development Highlights**

1. **TypeScript Integration**  
   - Strongly typed code for fewer bugs and better readability.

2. **Error Handling**  
   - Centralized middleware for clean and consistent error responses.

3. **Database Integration**  
   - Used Mongoose for schema modeling and seamless interaction with MongoDB.

4. **RESTful Design**  
   - Follows REST principles for easy integration with frontend or other services.

---

## **Contributing**

Contributions are welcome! To contribute:

1. Fork the repository.
2. Create a new branch.
   ```bash
   git checkout -b feature-name
   ```
3. Commit your changes.
   ```bash
   git commit -m "Add feature-name"
   ```
4. Push to your branch and open a pull request.

---

## **License**

This project is licensed under the [MIT License](LICENSE).

---

## **Acknowledgments**

- [Node.js Documentation](https://nodejs.org/en/docs/)
- [Express Documentation](https://expressjs.com/en/4x/api.html)
- [TypeScript Documentation](https://www.typescriptlang.org/docs/)
- [Mongoose Documentation](https://mongoosejs.com/docs/)

---

Feel free to update this with actual links (e.g., GitHub repository URL) and any specific details unique to your project!
