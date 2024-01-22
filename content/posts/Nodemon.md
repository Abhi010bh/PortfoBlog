+++
title = 'Nodemon'
date = 2023-12-18T00:13:30+05:30
draft = true
+++

## Setting up Nodemon in a Node.js Application

### Installation

1. **Installation:**
   - Use npm (Node Package Manager) to install Nodemon globally or locally within your project:

     ```bash
     # Install Nodemon globally (recommended for convenience)
     npm install -g nodemon

     # Or install Nodemon locally within your project (for project-specific use)
     npm install nodemon --save-dev
     ```

### Usage

2. **Usage:**
   - Once installed, you can start your Node.js server using Nodemon. Instead of `node server.js`, you'll use `nodemon server.js` to monitor for file changes and restart the server automatically.

     ```bash
     nodemon server.js
     ```

### Configuration (Optional)

3. **Configuration:**
   - Create a `nodemon.json` file in your project's root directory for custom configuration settings. This file allows you to define specific configurations for Nodemon, such as watching specific directories, ignoring certain files, setting delay before restart, etc.

     Example `nodemon.json`:

     ```json
     {
       "verbose": true,
       "watch": ["src", "lib"],
       "ignore": ["*.test.js", "node_modules"],
       "delay": "1000",
       "execMap": {
         "js": "node --inspect"
       }
     }
     ```

### Integration with `package.json` Scripts (Optional but Recommended)

4. **Integration with package.json:**
   - In your `package.json` file, you can create custom scripts that use Nodemon for starting your server. This simplifies the command and ensures consistency across your team or project.

     Example `package.json` scripts:

     ```json
     {
       "scripts": {
         "start": "nodemon server.js",
         "dev": "nodemon --watch src server.js"
       }
     }
     ```

     - Running `npm start` or `npm run dev` (as per the example above) executes the associated Nodemon command specified in the scripts.

This setup allows Nodemon to watch for changes in your Node.js application files (e.g., `.js`, `.json`, `.html`, etc.) and automatically restart the server whenever it detects modifications, providing a smoother development experience. Adjust the configurations and commands according to your specific project needs.
