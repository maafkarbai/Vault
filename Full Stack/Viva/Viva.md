# Git Characteristics (Viva)

## 1. What is Node.js?
Node.js is a runtime environment that allows you to run JavaScript on the server side. It is built on Google Chrome’s V8 JavaScript engine and is used to build scalable network applications.

## 2. Full Form of CDN
CDN stands for **Content Delivery Network**. It is a distributed network of servers that delivers web content to users based on their geographical location, optimizing speed and performance.

## 3. What Architecture is FETCH/REST API?
FETCH and REST APIs follow the **client-server architecture**. The client makes requests to the server (e.g., using HTTP methods like GET or POST), and the server responds with the requested data.

## 4. What are Node Modules?
Node modules are reusable blocks of code in Node.js. They can be:
- **Built-in modules** (e.g., fs, http) provided by Node.js.
- **Custom modules** created by developers.
- **Third-party modules** like Express, available via npm (Node Package Manager).

## 5. What Does `git status` Do?
`git status` shows the current state of your Git repository, including:
- Changes staged for commit.
- Changes not yet staged.
- Untracked files. 
	- 

## 6. Full Form of API
API stands for **Application Programming Interface**. It defines a set of rules for how software components interact with each other.

## 7. What Type of Stack Involves Frontend and Backend?
A **Full Stack** involves both frontend and backend development. Examples include:
- **MERN** (MongoDB, Express, React, Node.js)
- **MEVN** (MongoDB, Express, Vue, Node.js)

## 8. Can API Be Only in JSON Format?
No, APIs can return data in various formats like:
- JSON (most common for REST APIs)
- XML
- HTML
- Plain text, etc.

## 9. What Do PUT, GET, & POST Do?
- **GET**: Retrieve data from the server.
- **POST**: Send new data to the server.
- **PUT**: Update existing data on the server.

## 10. What Does Git Do?
Git is a **version control system** that tracks changes to code, enabling collaboration, version history, and management of multiple branches in a project.

## 11. How Does Frontend Connect With Backend in Vue.js?
The frontend (Vue.js) connects with the backend using:
- **HTTP Requests**: Made with libraries like `axios` or the `fetch` API.
- **REST APIs**: The backend exposes endpoints that the frontend calls to interact with the database.

## 12. What is a Promise?
A **Promise** is an object in JavaScript used for asynchronous operations.
- `.then`: Used to handle the result of a successful promise.
- `.catch`: Handles errors in a promise.

## 13. Difference Between Methods & Computed Properties
- **Methods**: Functions that are called explicitly and run every time.
- **Computed Properties**: Cached functions that recalculate only when their dependencies change.

## 14. What is Data Binding?
Data binding is a feature in Vue.js that allows automatic synchronization between the model (data) and the view (UI). Examples:
- **One-way binding**: Updates data in the UI (`v-bind`).
- **Two-way binding**: Syncs data between UI and model (`v-model`).

## 15. Types of Node Modules
1. **Built-in**: Modules like `fs`, `http`, `path`.
2. **Custom**: Modules created by developers.
3. **Third-party**: Modules from npm, like `express`.

## 16. What are CORS Headers and Full Form?
CORS stands for **Cross-Origin Resource Sharing**.
CORS headers control which resources can be shared between different origins (domains). Common headers include:
- `Access-Control-Allow-Origin`
- `Access-Control-Allow-Methods`
- `Access-Control-Allow-Headers`

## 17. What is Express and its Role in the Backend with MongoDB?
Express is a **Node.js framework** used to create server-side applications.
- It handles routes, middleware, and HTTP requests/responses.
- When used with MongoDB, Express serves as the intermediary to process user requests and interact with the database.

## 18. What is a Wildcard?
In programming, a **wildcard** is a symbol used to represent any character(s).
For example, in routing, `*` can match any path.

## 19. How Does Add-to-Cart Work in a Vue Application?
4. **User Interaction**: The user clicks “Add to Cart.”
5. **Trigger**: An event (e.g., `@click="addToCart(item)"`) is triggered.
6. **Directive**: Vue uses `v-model` or `v-bind` to update the cart array.
7. **State Update**: The item is added to the cart in the Vuex store or local data.
8. **UI Update**: The cart UI re-renders based on the updated state.

## 20. What Are Vue Directives?
Vue directives are special attributes in templates that bind DOM elements to data. Examples:
- `v-bind`: Dynamically bind attributes.
- `v-model`: Two-way data binding.
- `v-if/v-else`: Conditional rendering.
- `v-for`: Looping through items.
- `v-on`: Event handling.

## 21. Explain Search with Autocomplete
9. Create search **indexes** in MongoDB and set up **autocomplete**.
10. Set up a **GET route** to get the user's search query.
11. Use **aggregate**, which is a pipeline to utilize the **Atlas search index**.

## 22. What Approach Does GitHub Use?
GitHub uses a **snapshot-based approach**.

## 23. Why is MongoDB a Good Database Choice for JSON Data?
Because MongoDB is **schema-less**, allowing for flexible data storage.

## 24. What Are Static Files?
Static files are files that **do not change** for each user and are sent to the browser **as they are** from the server.

## 25. Why Do We Serve Static Files Using Middleware?
By default, Express.js **does not know** how to handle static files and will return a **404 error**. Middleware is used to serve static files properly.

## 26. What is cURL?
cURL (**Client URL**) is a command-line tool used to **transfer data** to and from a server.

## 27. What is Render?
Render is a **cloud platform** designed to deploy and manage web applications, APIs, static sites, and databases.

## 28. What is Middleware?
Middleware is a **function or module** that handles **requests (req)** and **responses (res)** in an application.

## 29. What is Mounting in Vue.js?
Mounting refers to **attaching Vue components** to the **DOM**.

## 30. What are the 3 stages in GIT?
 ### Working Directory
- The **Working Directory** is the area where files are checked out and modified. It represents the current state of your project, containing all the files and folders you are actively working on. Changes made in the working directory are untracked until they are staged.

 ### Staging Area
- The **Staging Area** (also called the **Index**) is an intermediate space where changes are prepared before committing. When you use `git add`, the modified or newly created files are added to the staging area. This allows you to selectively commit changes while keeping other modifications separate.

 ### .Git Directory
- The **.git Directory** is a hidden folder inside a Git repository that stores all metadata and history related to version control. It contains essential components such as commit history, branches, configuration settings, and objects necessary to track changes. This directory is what makes a folder a Git repository.

