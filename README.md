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
   - Modify your `package.json` to recognize TypeScript modules by adding `"type": "module"` right after the `"main"` property:
     ```json
     {
       "main": "index.js",
       "type": "module"
     }
     ```

7. **Implement the CLI Calculator**
   - Write your calculator logic in `index.ts`.

8. **Compile TypeScript to JavaScript**
   - Compile your TypeScript file (`index.ts`) to JavaScript using:
     ```
     tsc index.ts
     ```

9. **Run Your Project**
   - Execute your CLI calculator with:
     ```
     node index.js
     ```

#### **Conclusion**

By following these steps, you will have set up a simple yet functional CLI calculator using TypeScript and the inquirer library. This project not only demonstrates basic usage of TypeScript and npm but also introduces handling user inputs in a CLI environment.