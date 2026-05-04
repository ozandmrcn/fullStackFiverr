# fullStackFiverr

Welcome to the **fullStackFiverr** project! This is a complete, full-stack Fiverr clone application built with modern technologies and a focus on scalability, performance, and user experience. The project is fully containerized using **Docker** for easy deployment and development.

## <img src="https://raw.githubusercontent.com/Tarikul-Islam-Anik/Animated-Fluent-Emojis/master/Emojis/Activities/Bullseye.png" alt="Bullseye" width="25" height="25" /> Project Structure

The project is divided into two main parts:

- **[api](https://github.com/ozandmrcn/fullStackFiver-backend):** The backend RESTful API built with Node.js, Express, and MongoDB.
- **[client](https://github.com/ozandmrcn/fullStackFiver-frontend):** The frontend web application built with React, Vite, and TailwindCSS.

## <img src="https://raw.githubusercontent.com/Tarikul-Islam-Anik/Animated-Fluent-Emojis/master/Emojis/Travel%20and%20places/Rocket.png" alt="Rocket" width="25" height="25" /> Docker Setup & Installation

This project is fully containerized. To get everything up and running in a single command, follow these steps:

### 📋 Prerequisites
- [Docker Desktop](https://www.docker.com/products/docker-desktop/) installed on your machine.

### 🚀 Quick Start
1. **Clone the repository:**
   ```bash
   git clone https://github.com/ozandmrcn/fullStackFiverr.git
   cd fullStackFiverr
   ```

2. **Build and start services:**
   ```bash
   docker-compose up --build
   ```

3. **Access the application:**
   - **Frontend:** [http://localhost](http://localhost)
   - **Backend API:** [http://localhost:4000](http://localhost:4000)
   - **MongoDB:** `mongodb://localhost:50000` (External access port)

## <img src="https://raw.githubusercontent.com/Tarikul-Islam-Anik/Animated-Fluent-Emojis/master/Emojis/Objects/Hammer%20and%20Wrench.png" alt="Hammer and Wrench" width="25" height="25" /> Useful Docker Commands

| Command | Description |
| :--- | :--- |
| `docker-compose up -d` | Start services in detached mode (background). |
| `docker-compose down` | Stop and remove all containers. |
| `docker-compose logs -f` | View live logs from all services. |
| `docker-compose restart api` | Restart only the API service. |

## <img src="https://raw.githubusercontent.com/Tarikul-Islam-Anik/Animated-Fluent-Emojis/master/Emojis/Objects/Desktop%20Computer.png" alt="Desktop Computer" width="25" height="25" /> Environment Setup

Both `api` and `client` require their own `.env` files for local (non-docker) development. Follow the templates below:

### 🔌 Backend API (`/api/.env`)
Create a `.env` file in the `api` directory with the following variables:
```env
PORT=4000
NODE_ENV=development
MONGO_URI=mongodb+srv://<username>:<password>@cluster.mongodb.net/fiverr
JWT_SECRET=your_super_secret_key_here
JWT_EXPIRES=1209600
CLOUD_NAME=your_cloud_name
CLOUD_API_KEY=your_api_key
CLOUD_SECRET=your_api_secret
CROSS_ORIGIN=http://localhost:5173
```

### 💻 Frontend Client (`/client/.env`)
Create a `.env` file in the `client` directory with the following variable:
```env
VITE_API_URL=http://localhost:4000/api/
```

> [!TIP]
> For more detailed configuration options, please refer to the individual [API Guide](./api/README.md) and [Client Guide](./client/README.md).


## 📁 Key Features

- **End-to-End Type Safety:** Fully implemented with TypeScript.
- **Image Cloud Hosting:** Integrated with Cloudinary for media management.
- **Modern UI/UX:** Styled with TailwindCSS v4 and animated components.
- **Containerization:** Ready for production with Docker Compose.

## 📧 Contact

For any questions or feedback, feel free to contact:  
**Ozan Demircan** – ozandmrcn47@gmail.com
