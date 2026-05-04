# Docker Setup & Usage Guide

This guide explains how to set up the fullStackFiverr project using Docker. The project is divided into three main repositories:
1. **Root (Main) Repository**: Orchestrates the services using Docker Compose.
2. **API Repository**: The backend service.
3. **Client Repository**: The frontend service.

---

## 🛠️ Step 1: Clone the Repositories

To get started, you need to collect all three repositories into a single workspace.

1. **Create a root folder:**
   ```bash
   mkdir fullStackFiverr
   cd fullStackFiverr
   ```

2. **Clone the Root repository (this one):**
   ```bash
   git clone https://github.com/ozandmrcn/fullStackFiverr.git .
   ```

3. **Clone the API and Client sub-repositories:**
   ```bash
   git clone https://github.com/ozandmrcn/fullStackFiver-backend.git api
   git clone https://github.com/ozandmrcn/fullStackFiver-frontend.git client
   ```

**Final Directory Structure:**
```text
fullStackFiverr/
├── api/                # Backend code
│   ├── Dockerfile
│   └── ...
├── client/             # Frontend code
│   ├── Dockerfile
│   └── ...
├── docker-compose.yml  # Docker orchestration
├── README.md           # Project overview
└── .env                # Environment variables (Optional)
```

---

## 🚀 Step 2: Running with Docker Compose

Once your files are organized as shown above, you can start the entire stack with a single command.

### 📋 Prerequisites
- **Docker Desktop** installed and running.

### ⚡ Quick Start
Run the following command in the root `fullStackFiverr` folder:
```bash
docker-compose up --build
```

This will:
1. Build the **API** image.
2. Build the **Client** image.
3. Pull the latest **MongoDB** image.
4. Start all containers and link them together.

---

## 🌐 Accessing the Services

Once the containers are running, you can access the following:

| Service | URL | Description |
| :--- | :--- | :--- |
| **Frontend** | [http://localhost](http://localhost) | The React application. |
| **Backend API** | [http://localhost:4000](http://localhost:4000) | RESTful API endpoints. |
| **MongoDB** | `mongodb://localhost:50000` | Database (External access port). |

---

## ⚙️ Environment Variables

The `docker-compose.yml` file is configured to use default values, but you can override them by creating a `.env` file in the root directory.

**Root `.env` Template:**
```env
# Backend Configuration
JWT_SECRET=your_custom_secret
JWT_EXPIRES=1209600
CLOUD_NAME=your_cloudinary_name
CLOUD_API_KEY=your_cloudinary_key
CLOUD_SECRET=your_cloudinary_secret

# Database Configuration
MONGO_URI=mongodb://mongodb:27017/fiverr
```

---

## 🧹 Useful Commands

| Command | Action |
| :--- | :--- |
| `docker-compose down` | Stop and remove all containers. |
| `docker-compose logs -f` | View live logs from all services. |
| `docker-compose restart api` | Restart the backend service only. |
| `docker system prune -a` | Clean up unused Docker images/containers. |
