
## 🐳 Install Docker & Docker Compose

Update your system and install Docker:

```bash
sudo apt update
sudo apt install docker.io -y
sudo apt install docker-compose-v2 -y
```

Verify Docker installation:

```bash
docker ps
```

Fix Docker permission issue (so you don’t need `sudo` every time):

```bash
sudo  usermod -aG  docker  $USER
```

---

## 🚀 Run the Application

### 1️⃣ Clone the repository

```bash
git clone <REPOSITORY_URL>
cd <PROJECT_DIRECTORY>
```

---

### 2️⃣ Setup environment files

Copy the sample environment files:

```bash
cp backend/.env-sample backend/.env
cp frontend/.env-sample frontend/.env
```

---

### 3️⃣ Update Frontend `.env`

Edit the frontend environment file:

```bash
nano frontend/.env
```

Update the API URL:

```env
REACT_APP_API_BASE_URL=http://<your_public_ip_or_domain>
```

👉 Example:

```env
REACT_APP_API_BASE_URL=http://192.168.1.100
```

---

### 4️⃣ Build and start containers

Run the application using Docker Compose:

```bash
docker compose up -d --build
```

---

## ✅ Done!

Your application is now running using Docker containers 🎉
Check running containers:

```bash
docker ps
```

---
 **Access the Application:**

   Open your favorite browser and visit [http://your_public_ip or domain_name). Enjoy exploring the MERN stack application!

   <img width="1064" height="517" alt="image" src="https://github.com/user-attachments/assets/fdb0710f-0a27-4ee0-a352-dc61f3aabacc" />


