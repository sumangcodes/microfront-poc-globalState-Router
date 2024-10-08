# microfront-poc-globalState-Router



---

### **Microfrontend POC Using Single-SPA and Webpack Module Federation**

This repository demonstrates a **Proof of Concept (POC)** for building microfrontend applications using **single-spa** and **Webpack Module Federation**. It features multiple React-based microfrontends integrated into a shell application. The project also showcases routing between microfrontends, state sharing using React Context, and inter-microfrontend communication using an event bus with RxJS.

#### Features:
- **Microfrontend Architecture**: Each microfrontend is built independently and can be deployed separately.
- **Single-SPA Framework**: Used for integrating multiple microfrontends into a single application shell.
- **Webpack Module Federation**: Enables dynamic loading of microfrontends and sharing of modules across apps.
- **Routing**: Each microfrontend has its own internal routing logic, while the shell app manages top-level routing.
- **State Sharing**: Global state management is implemented using React Context, with the ability to share data between microfrontends.
- **Event Bus**: Microfrontends communicate via a lightweight event bus using RxJS for decoupled communication.

#### Folder Structure:
- **shell-app/**: The main application shell that hosts and integrates microfrontends.
- **app1/**: First microfrontend that is loaded dynamically.
- **app2/**: Second microfrontend, following the same structure as `app1`.

#### How to Run:
1. Clone the repository.
2. Navigate into each app folder (`shell-app`, `app1`, `app2`), install dependencies, and start each app:
   ```bash
   cd shell-app
   npm install
   npm start
   ```
   Follow the same steps for `app1` and `app2`.
   
3. Access the shell app at `http://localhost:3000`. Each microfrontend runs on different ports and can be accessed through the shell app.

#### Technologies:
- **React**: For building the UI components.
- **single-spa**: For microfrontend orchestration.
- **Webpack Module Federation**: For dynamic loading of microfrontends.
- **RxJS**: For event-driven communication between microfrontends.
- **React Router**: For routing within microfrontends.

---

This description will give a clear overview of the project and guide users on how to run it.
