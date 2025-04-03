# **G-Scores**

This project is a **full-stack application** built with a **React Vite** frontend and a **NestJS** backend. The backend is containerized using **Docker** for easier deployment.

## 🚀 **Features**

- **Frontend**: React + Vite for fast development and optimized builds.
- **Backend**: NestJS with a modular and scalable architecture.
- **Database**: PostgreSQL (configured in Docker).
- **RESTful API** integration between frontend and backend.

## 📥 **Installation**

### **Clone the Repository**

```bash
git clone https://github.com/QuocDuy03/g-scores.git
cd g-scores
```

### **Frontend Setup**

```bash
# Navigate to the frontend directory
cd frontend

# Install dependencies
npm install

# Copy the environment configuration
cp .env.example .env

# Start the development server
npm run dev
```

### **Backend Setup**

```bash
# Navigate to the backend directory
cd backend

# Copy the environment configuration
cp .env.example .env

# Start the development server
docker-compose up --build
```

## **Import Data from CSV File to Database**

```bash
# Check container ID
docker ps

# Run migrations
docker exec -it <container_id> npm run typeorm:run-migrations

# Run seeds
docker exec -it <container_id> npm run seed
```

## **Folder Structure**

```plaintext
/frontend   # React Vite frontend
/backend    # NestJS backend
```

## **Demo**
https://g-scores-frontend-coral.vercel.app/
