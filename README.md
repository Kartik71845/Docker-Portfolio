# Docker Portfolio Website 🌐

This is my personal portfolio website that I decided to containerize with **Docker**.  
Instead of just serving a plain `index.html`, I wanted to learn how static websites can be hosted inside a container using **Nginx**.  

---

## Why I Built This 💡
- To practice Docker basics with a real project  
- To understand how Nginx serves static content  
- To prepare this repo for CI/CD with **Jenkins** later  

---

## How It Works ⚙️
- The project uses the official **nginx:alpine** image as the base  
- My `index.html` file is copied into the Nginx default web directory  
- Once the container is running, the website is instantly available on port **8080**  

---

## Run It Locally 🚀
If you want to try it out:  

```bash
# Build the Docker image
docker build -t portfolio-site .

# Run the container
docker run -d -p 8080:80 portfolio-site
