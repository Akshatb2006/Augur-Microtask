# Microtask 0 — GrimoireLab Installation and Setup 🚀

This microtask involves installing and configuring **GrimoireLab**, a CHAOSS project used for software development analytics. Below is a detailed walkthrough of the setup process, challenges I encountered, and how I resolved them.

---

## ✅ Steps Followed

### 📥 1. Clone the GrimoireLab Repository

I started by cloning the official GrimoireLab repository:

```
git clone https://github.com/chaoss/grimoirelab.git
cd grimoirelab
```

---

### 🔍 2. Locate docker-compose.yml
To find the docker-compose.yml file, I ran:

bash
Copy
Edit
```
find . -name "docker-compose.yml"
```
Output:

```bash
./docker-compose/docker-compose.yml
./tests/docker-compose.yml
```
I then navigated to the main docker-compose/ directory.

```
cd docker-compose
```

---

### 🐳 3. Start GrimoireLab Using Docker Compose
To launch all the GrimoireLab services, I ran:
```
docker-compose up -d
```
This pulled all required Docker images (like mordred, elasticsearch, kibiter, etc.) and started the containers.

---

### ✅ 4. Check Running Containers
To ensure all services were up and running, I checked the container status:
```
docker ps
```
I verified that key containers like mariadb, mordred, redis, kibiter, and nginx were healthy and running.

---

### 🌐 5. Access the Kibiter Dashboard
After everything was running, I opened Kibiter in the browser at:

arduino
```
http://localhost:5601
```
This confirmed that the GrimoireLab UI was successfully set up.

---

### ⚠️ Challenges Faced and Solutions
1. Obsolete Version Warning in docker-compose.yml
   Issue: pgsql the attribute `version` is obsolete, it will be ignored, please remove it to avoid potential confusion

   Solution: It’s just a warning and doesn’t break anything. I ignored it, and the services ran fine.

2. Kibiter not accessible immediately
   Issue:It took some time after docker-compose up -d for Kibiter to be fully operational.

   Solution: Waited 1–2 minutes. Then accessed at: http://localhost:5601

3. Pulling Images Was Slow
   Issue: Some Docker images (e.g., elasticsearch, mordred) took time to download.

   Solution: I waited patiently and ensured a stable internet connection. Once downloaded, containers ran smoothly.

   ---

### 📂 Folder Structure
Here’s how my microtask repo looks:

arduino
microtask-0/
├── README.md
├── clone.png
├── find-docker-compose.png
├── docker-up.png
├── docker-ps.png
└── kibiter.png

---

### 📸 Screenshots
Screenshots for every step are stored in the assets/ folder:

clone.png – Git clone of the repo

find-docker-compose.png – Output of find command

docker-up.png – Docker images being pulled

docker-ps.png – Verifying running containers

kibiter.png – Kibiter dashboard UI

---

### 🙌 Outcome
GrimoireLab is now fully set up and running on my local machine. I can access the Kibiter dashboard and will proceed with data exploration and visualization in upcoming microtasks.

---

### 🔗 Useful References
📘 GrimoireLab Tutorial

🐙 GrimoireLab GitHub

📚 CHAOSS Documentation
