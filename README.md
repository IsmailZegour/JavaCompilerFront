Java Online Compiler - Frontend
Description
Java Online Compiler is a modern web application that provides a seamless interface for writing, compiling, and executing Java code directly in your browser. Built with Angular, the frontend features a sleek and intuitive design powered by Monaco Editor for a superior coding experience.

This project communicates with a backend API to handle code compilation and execution, making it a perfect tool for developers, students, and anyone learning Java.

Features
Integrated Code Editor: Monaco Editor for syntax highlighting and error detection.
Real-Time Code Execution: Compile and execute Java code instantly.
Result Display: View execution output in a dedicated result pane.
Responsive Design: Works seamlessly across devices and screen sizes.
Prerequisites
Node.js (v16 or later)
Angular CLI (v15 or later)
Installation and Setup
Clone the repository:



git clone https://github.com/your-username/java-online-compiler-frontend.git
cd java-online-compiler-frontend
Install dependencies:



npm install
Start the development server:



ng serve
Open your browser and navigate to:

arduino

http://localhost:4200
How to Use
Write your Java code in the integrated editor.
Click the Run Code button to send your code to the backend for compilation and execution.
View the output in the result pane below the editor.
API Integration
The frontend interacts with the backend API hosted at http://localhost:8080. Below is an example of the API request and response:

POST /compile
Request Body:
json

{
  "code": "public class Main { public static void main(String[] args) { System.out.println(\"Hello, World!\"); }}"
}
Response:
json

{
  "output": "Hello, World!"
}
Project Structure


src/
├── app/
│   ├── code-editor/       # Component for code writing and execution
│   ├── shared/            # Shared utilities and services
│   └── assets/            # Static assets
├── environments/          # Environment-specific configurations
Technologies Used
Angular: Framework for building the frontend.
Monaco Editor: Rich code editor with syntax highlighting.
RxJS: Reactive programming library for managing asynchronous data streams.
Known Issues
Ensure the backend server is running and properly configured for CORS to avoid connection issues.
Contributions
Contributions are welcome! To contribute:

Fork the repository.
Create a feature branch.
Submit a pull request with detailed changes.
License
This project is licensed under the MIT License. See the LICENSE file for details.

Start coding Java in your browser with Java Online Compiler today! 🚀
