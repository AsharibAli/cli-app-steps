### **Calculator Practice**

This project is a **Command Line Interface (CLI) calculator** implemented in **TypeScript**, utilizing the `inquirer` library for handling user input. Follow the steps below to set up and run the project.

#### **Prerequisites**

- Node.js installed on your system
- Basic understanding of TypeScript and npm

#### **Steps to Set Up the Project**

1. **Initialize a New npm Project**
   - Run the following command to create a new npm project:
     ```
     npm init -y
     ```

2. **Generate a TypeScript Configuration File**
   - Initialize TypeScript in your project:
     ```
     tsc --init
     ```

3. **Install the Inquirer Library**
   - Add `inquirer` to your project for collecting user input:
     ```
     npm i inquirer
     ```

4. **Install Types for Inquirer**
   - Since we are using TypeScript, install the types for `inquirer`:
     ```
     npm i --save-dev @types/inquirer
     ```

5. **Configure TypeScript (tsconfig.json)**
   - Edit your `tsconfig.json` to include the following configurations:
     ```json
     {
       "compilerOptions": {
         "target": "ES2022",
         "module": "NodeNext",
         "moduleResolution": "NodeNext"
       }
     }
     ```

6. **Update package.json Configuration**
   - Modify these lines of code in your `package.json`:
     ```json
     {
      "name": "@your-npm-usernmae/calculator", 
       "main": "index.js",
       "type": "module",
       "publishConfig": {
        "access": "public"
      },
       "bin": {
        "calculator": "./index.js"
      },
     }
     ```

7. **Implement the CLI Calculator**
   - Start your calculator code in `index.ts`. At the top of this file, include the shebang:
  ```
   #! /usr/bin/env node
  ```

1. **Compile TypeScript to JavaScript**
   - Compile your TypeScript file (`index.ts`) to JavaScript using:
     ```
     tsc
     ```

2. **Run Your Project**
   - Execute your CLI calculator with:
     ```
     node index.js
     ```

#### **Publishing Your Project on npm**

To make your CLI calculator accessible to others, follow these steps to publish your project on npm:

1. **Log in to npm**
   - If you haven't already, you will need to create an npm account [npmjs.com](npmjs.com). Once you have your account set up, log in to npm from your command line:
     ```
     npm login
     ```
   - Enter your username, password, and email address as prompted.

2. **Publish Your Package**
   - Publish your package to npm, ensuring it is available publicly:
     ```
     npm publish
     ```

#### **Conclusion**

By following these steps, you will have set up a simple yet functional CLI calculator using TypeScript and the inquirer library. This project not only demonstrates basic usage of TypeScript and npm but also introduces handling user inputs in a CLI environment.
