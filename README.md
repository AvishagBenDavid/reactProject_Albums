# Patient Monitoring System

> **Development Status:** This project is a work in progress. Some implementation details may require further refinement and testing.

## Overview

The Patient Monitoring System is a web-based application designed to help hospital nurses view patient monitor data and receive real-time monitoring updates.

The system combines a React frontend, a Node.js backend, and a dedicated monitoring server to support communication between its different components.

The project demonstrates the integration of frontend and backend technologies, REST APIs, and real-time communication using WebSockets.

## System Architecture

The system consists of three main components:

1. **Frontend Client** – A React application that provides the user interface for viewing patient information and monitoring data.
2. **Backend Server** – A Node.js and Express server responsible for handling API requests and managing application data.
3. **Monitoring Server** – A dedicated server that uses WebSockets to deliver real-time monitoring updates to the frontend.

## Technologies

- React
- JavaScript
- Node.js
- Express.js
- WebSockets
- REST API
- HTML
- CSS

## Repositories

The project is divided into three repositories:

- **Client – React Frontend:**  
  [client_react_finalProject](https://github.com/shugi-star/client_react_finalProject)

- **Main Backend Server:**  
  [server_react_finalProject](https://github.com/shugi-star/server_react_finalProject)

- **Real-Time Monitoring Server:**  
  [monitor_demo_react](https://github.com/shugi-star/monitor_demo_react)

## Running the Project Locally

### Prerequisites

- Node.js and npm installed.
- All three repositories cloned to your computer.

### 1. Start the Backend Server

Open a terminal in the backend project directory and run:

```bash
npm install
npm start
```

The backend is configured to use port `3001` by default.

### 2. Start the Monitoring Server

Open a separate terminal in the monitoring server project directory and run:

```bash
npm install
node server.js
```

The monitoring server uses port `3002` and provides the following WebSocket endpoint:

```text
ws://localhost:3002/ws/monitorsRealtime
```

### 3. Start the Frontend

Open another terminal in the frontend project directory and run:

```bash
npm install
npm start
```

The frontend is typically available at:

```text
http://localhost:3000
```

## Additional Notes

- Start the backend and monitoring servers before using the frontend.
- The frontend and monitoring server are configured to communicate with local services.
- Full build and runtime verification have not yet been completed.
- This project is intended as a software demonstration and has not been validated for clinical use.
