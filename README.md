# fullStackFiverr

Welcome to the **fullStackFiverr** project! This is a complete, full-stack Fiverr clone application built with modern technologies and a focus on scalability, performance, and user experience. The project is fully containerized using **Docker** for easy deployment and development.

## <img src="https://raw.githubusercontent.com/Tarikul-Islam-Anik/Animated-Fluent-Emojis/master/Emojis/Activities/Bullseye.png" alt="Bullseye" width="25" height="25" /> Project Structure

The project is divided into two main parts:

- **[api](https://github.com/ozandmrcn/fullStackFiver-backend):** The backend RESTful API built with Node.js, Express, and MongoDB.
- **[client](https://github.com/ozandmrcn/fullStackFiver-frontend):** The frontend web application built with React, Vite, and TailwindCSS.

## <img src="https://raw.githubusercontent.com/Tarikul-Islam-Anik/Animated-Fluent-Emojis/master/Emojis/Travel%20and%20places/Rocket.png" alt="Rocket" width="25" height="25" /> Docker Setup & Installation

This project is fully containerized. For a step-by-step guide on how to organize the repositories and run them, please refer to the **[Docker Setup & Usage Guide](./DOCKER_GUIDE.md)**.

### 🚀 Quick Start

1. **Organize Folders:** Ensure `api` and `client` folders are present in the root directory.
2. **Build and start services:**
   ```bash
   docker-compose up --build
   ```
3. **Access the application:**
   - **Frontend:** [http://localhost](http://localhost)
   - **Backend API:** [http://localhost:4000](http://localhost:4000)

## <img src="https://raw.githubusercontent.com/Tarikul-Islam-Anik/Animated-Fluent-Emojis/master/Emojis/Objects/Hammer%20and%20Wrench.png" alt="Hammer and Wrench" width="25" height="25" /> Useful Docker Commands

| Command                      | Description                                   |
| :--------------------------- | :-------------------------------------------- |
| `docker-compose up -d`       | Start services in detached mode (background). |
| `docker-compose down`        | Stop and remove all containers.               |
| `docker-compose logs -f`     | View live logs from all services.             |
| `docker-compose restart api` | Restart only the API service.                 |

## <img src="https://raw.githubusercontent.com/Tarikul-Islam-Anik/Animated-Fluent-Emojis/master/Emojis/Objects/Desktop%20Computer.png" alt="Desktop Computer" width="25" height="25" /> Environment Setup

Both `api` and `client` services are pre-configured in `docker-compose.yml`. For custom configurations, you can use `.env` files:

> [!TIP]
> For more detailed configuration options, please refer to the individual [API Guide](https://github.com/ozandmrcn/fullStackFiver-backend/blob/main/README.md) and [Client Guide](https://github.com/ozandmrcn/fullStackFiver-frontend/blob/main/README.md).

## <img src="https://raw.githubusercontent.com/Tarikul-Islam-Anik/Animated-Fluent-Emojis/master/Emojis/Objects/File%20Folder.png" alt="File Folder" width="25" height="25" /> Key Features

- **End-to-End Type Safety:** Fully implemented with TypeScript.
- **Image Cloud Hosting:** Integrated with Cloudinary for media management.
- **Modern UI/UX:** Styled with TailwindCSS v4 and animated components.
- **Containerization:** Ready for production with Docker Compose.

## <img src="https://raw.githubusercontent.com/Tarikul-Islam-Anik/Animated-Fluent-Emojis/master/Emojis/Objects/E-Mail.png" alt="E-Mail" width="25" height="25" /> Contact

For any questions or feedback, feel free to contact:  
**Ozan Demircan** – [ozandmrcn47@gmail.com](mailto:ozandmrcn47@gmail.com)
